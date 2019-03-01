---
title: Microsoft Azure PowerShell Az 1.0.0 の破壊的変更
description: この移行ガイドには、Az バージョン 1 リリースの Azure PowerShell で行われた破壊的変更が記載されています。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/14/2018
ms.openlocfilehash: be3e19dc4b689adbc63b933dd9f3454122d5344a
ms.sourcegitcommit: 5630030c5cfa9828c3c024b69de59248263ef17f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "56837369"
---
# <a name="migration-guide-for-az-100"></a><span data-ttu-id="2865e-103">Az 1.0.0 の移行ガイド</span><span class="sxs-lookup"><span data-stu-id="2865e-103">Migration Guide for Az 1.0.0</span></span>

<span data-ttu-id="2865e-104">このドキュメントでは、AzureRM の 6.x バージョンと Az バージョン 1.0.0 の間での変更点について説明します。</span><span class="sxs-lookup"><span data-stu-id="2865e-104">This document describes the changes between the 6.x versions of AzureRM and Az version 1.0.0.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="2865e-105">目次</span><span class="sxs-lookup"><span data-stu-id="2865e-105">Table of Contents</span></span>
- [<span data-ttu-id="2865e-106">重大な変更 - 全般</span><span class="sxs-lookup"><span data-stu-id="2865e-106">General breaking changes</span></span>](#general-breaking-changes)
  - [<span data-ttu-id="2865e-107">コマンドレットの名詞プレフィックスの変更</span><span class="sxs-lookup"><span data-stu-id="2865e-107">Cmdlet Noun Prefix Changes</span></span>](#cmdlet-noun-prefix-changes)
  - [<span data-ttu-id="2865e-108">モジュール名の変更</span><span class="sxs-lookup"><span data-stu-id="2865e-108">Module name changes</span></span>](#module-name-changes)
  - [<span data-ttu-id="2865e-109">削除されたモジュール</span><span class="sxs-lookup"><span data-stu-id="2865e-109">Removed modules</span></span>](#removed-modules)
  - [<span data-ttu-id="2865e-110">Windows PowerShell 5.1 と .NET 4.7.2</span><span class="sxs-lookup"><span data-stu-id="2865e-110">Windows PowerShell 5.1 and .NET 4.7.2</span></span>](#windows-powershell-51-and-net-472)
  - [<span data-ttu-id="2865e-111">PSCredential を使用したユーザー ログインの一時的な削除</span><span class="sxs-lookup"><span data-stu-id="2865e-111">Temporary removal of User login using PSCredential</span></span>](#temporary-removal-of-user-login-using-pscredential)
  - [<span data-ttu-id="2865e-112">Web ブラウザー プロンプトの代わりにデバイス コード ログインを既定で使用</span><span class="sxs-lookup"><span data-stu-id="2865e-112">Default Device Code login instead of Web Browser prompt</span></span>](#temporary-default-device-code-login-instead-of-web-browser-prompt)
- [<span data-ttu-id="2865e-113">モジュールの破壊的変更</span><span class="sxs-lookup"><span data-stu-id="2865e-113">Module breaking changes</span></span>](#module-breaking-changes)
  - [<span data-ttu-id="2865e-114">Az.ApiManagement (以前の AzureRM.ApiManagement)</span><span class="sxs-lookup"><span data-stu-id="2865e-114">Az.ApiManagement (previously AzureRM.ApiManagement)</span></span>](#azapimanagement-previously-azurermapimanagement)
  - [<span data-ttu-id="2865e-115">Az.Billing (以前の AzureRM.Billing、AzureRM.Consumption、および AzureRM.UsageAggregates)</span><span class="sxs-lookup"><span data-stu-id="2865e-115">Az.Billing (previously AzureRM.Billing, AzureRM.Consumption, and AzureRM.UsageAggregates)</span></span>](#azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates)
  - [<span data-ttu-id="2865e-116">Az.CognitiveServices (以前の AzureRM.CognitiveServices)</span><span class="sxs-lookup"><span data-stu-id="2865e-116">Az.CognitiveServices (previously AzureRM.CognitiveServices)</span></span>](#azcognitiveservices-previously-azurermcognitiveservices)
  - [<span data-ttu-id="2865e-117">Az.Compute (以前の AzureRM.Compute)</span><span class="sxs-lookup"><span data-stu-id="2865e-117">Az.Compute (previously AzureRM.Compute)</span></span>](#azcompute-previously-azurermcompute)
  - [<span data-ttu-id="2865e-118">Az.DataFactory (以前の AzureRM.DataFactories および AzureRM.DataFactoryV2)</span><span class="sxs-lookup"><span data-stu-id="2865e-118">Az.DataFactory (previously AzureRM.DataFactories and AzureRM.DataFactoryV2)</span></span>](#azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2)
  - [<span data-ttu-id="2865e-119">Az.DataLakeAnalytics (以前の AzureRM.DataLakeAnalytics)</span><span class="sxs-lookup"><span data-stu-id="2865e-119">Az.DataLakeAnalytics (previously AzureRM.DataLakeAnalytics)</span></span>](#azdatalakeanalytics-previously-azurermdatalakeanalytics)
  - [<span data-ttu-id="2865e-120">Az.DataLakeStore (以前の AzureRM.DataLakeStore)</span><span class="sxs-lookup"><span data-stu-id="2865e-120">Az.DataLakeStore (previously AzureRM.DataLakeStore)</span></span>](#azdatalakestore-previously-azurermdatalakestore)
  - [<span data-ttu-id="2865e-121">Az.KeyVault (以前の AzureRM.KeyVault)</span><span class="sxs-lookup"><span data-stu-id="2865e-121">Az.KeyVault (previously AzureRM.KeyVault)</span></span>](#azkeyvault-previously-azurermkeyvault)
  - [<span data-ttu-id="2865e-122">Az.Media (以前の AzureRM.Media)</span><span class="sxs-lookup"><span data-stu-id="2865e-122">Az.Media (previously AzureRM.Media)</span></span>](#azmedia-previously-azurermmedia)
  - [<span data-ttu-id="2865e-123">Az.Monitor (以前の AzureRM.Insights)</span><span class="sxs-lookup"><span data-stu-id="2865e-123">Az.Monitor (previously AzureRM.Insights)</span></span>](#azmonitor-previously-azurerminsights)
  - [<span data-ttu-id="2865e-124">Az.Network (以前の AzureRM.Network)</span><span class="sxs-lookup"><span data-stu-id="2865e-124">Az.Network (previously AzureRM.Network)</span></span>](#aznetwork-previously-azurermnetwork)
  - [<span data-ttu-id="2865e-125">Az.OperationalInsights (以前の AzureRM.OperationalInsights)</span><span class="sxs-lookup"><span data-stu-id="2865e-125">Az.OperationalInsights (previously AzureRM.OperationalInsights)</span></span>](#azoperationalinsights-previously-azurermoperationalinsights)
  - [<span data-ttu-id="2865e-126">Az.RecoveryServices (以前の AzureRM.RecoveryServices、AzureRM.RecoveryServices.Backup、および AzureRM.RecoveryServices.SiteRecovery)</span><span class="sxs-lookup"><span data-stu-id="2865e-126">Az.RecoveryServices (previously AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, and AzureRM.RecoveryServices.SiteRecovery)</span></span>](#azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery)
  - [<span data-ttu-id="2865e-127">Az.Resources (以前の AzureRM.Resources)</span><span class="sxs-lookup"><span data-stu-id="2865e-127">Az.Resources (previously AzureRM.Resources)</span></span>](#azresources-previously-azurermresources)
  - [<span data-ttu-id="2865e-128">Az.ServiceFabric (以前の AzureRM.ServiceFabric)</span><span class="sxs-lookup"><span data-stu-id="2865e-128">Az.ServiceFabric (previously AzureRM.ServiceFabric)</span></span>](#azservicefabric-previously-azurermservicefabric)
  - [<span data-ttu-id="2865e-129">Az.Sql (以前の AzureRM.Sql)</span><span class="sxs-lookup"><span data-stu-id="2865e-129">Az.Sql (previously AzureRM.Sql)</span></span>](#azsql-previously-azurermsql)
  - [<span data-ttu-id="2865e-130">Az.Storage (以前の Azure.Storage and AzureRM.Storage)</span><span class="sxs-lookup"><span data-stu-id="2865e-130">Az.Storage (previously Azure.Storage and AzureRM.Storage)</span></span>](#azstorage-previously-azurestorage-and-azurermstorage)
  - [<span data-ttu-id="2865e-131">Az.Websites (以前の AzureRM.Websites)</span><span class="sxs-lookup"><span data-stu-id="2865e-131">Az.Websites (previously AzureRM.Websites)</span></span>](#azwebsites-previously-azurermwebsites)

## <a name="general-breaking-changes"></a><span data-ttu-id="2865e-132">重大な変更 - 全般</span><span class="sxs-lookup"><span data-stu-id="2865e-132">General breaking changes</span></span>
### <a name="cmdlet-noun-prefix-changes"></a><span data-ttu-id="2865e-133">コマンドレットの名詞プレフィックスの変更</span><span class="sxs-lookup"><span data-stu-id="2865e-133">Cmdlet Noun Prefix Changes</span></span>
<span data-ttu-id="2865e-134">AzureRM では、コマンドレットの名詞プレフィックスとして "AzureRM" または "Azure" が使用されていました。</span><span class="sxs-lookup"><span data-stu-id="2865e-134">In AzureRM, cmdlets used either 'AzureRM' or 'Azure' as a noun prefix.</span></span>  <span data-ttu-id="2865e-135">Az ではコマンドレット名が簡略化され、正規化されています。そのため、すべてのコマンドレットでコマンドレット名詞プレフィックスとして "Az" が使用されます。</span><span class="sxs-lookup"><span data-stu-id="2865e-135">Az simplifies and normalizes cmndlet names, so that all cmdlets use 'Az' as their cmdlet noun prefix.</span></span> <span data-ttu-id="2865e-136">例: </span><span class="sxs-lookup"><span data-stu-id="2865e-136">For example:</span></span>
```powershell
Get-AzureRMVM
Get-AzureKeyVaultSecret
```

<span data-ttu-id="2865e-137">次のように変更されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-137">Have changed to</span></span>
```powershell
Get-AzVM
Get-AzKeyVaultSecret
```

<span data-ttu-id="2865e-138">これらの新しいコマンドレット名に簡単に移行できるように、Az では ```Enable-AzureRmAlias``` と ```Disable-AzureRmAlias``` の 2 つの新しいコマンドレットが導入されています。</span><span class="sxs-lookup"><span data-stu-id="2865e-138">To make the transition to these new cmdlet names simpler, Az introduces two new cmdlets, ```Enable-AzureRmAlias``` and ```Disable-AzureRmAlias```.</span></span>  <span data-ttu-id="2865e-139">```Enable-AzureRmAlias``` は、AzureRM の古いコマンドレット名から新しい Az コマンドレット名に対するエイリアスを作成します。</span><span class="sxs-lookup"><span data-stu-id="2865e-139">```Enable-AzureRmAlias``` creates aliases from the older cmdlet names in AzureRM to the newer Az cmdlet names.</span></span>  <span data-ttu-id="2865e-140">このコマンドレットでは、現在のセッションでエイリアスを作成することも、ユーザー プロファイルまたはマシン プロファイルを変更してすべてのセッションでエイリアスを作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="2865e-140">The cmdlet allows creating aliases in the current session, or across all sessions by changing your user or machine profile.</span></span> 

<span data-ttu-id="2865e-141">たとえば、AzureRM の次のスクリプトがあるとします。</span><span class="sxs-lookup"><span data-stu-id="2865e-141">For example, the following script in AzureRM:</span></span>
```powershell
#Requires -Modules AzureRM.Storage
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="2865e-142">```Enable-AzureRmAlias``` を使用すると、最小限の変更で実行できます。</span><span class="sxs-lookup"><span data-stu-id="2865e-142">Could be run with minimal changes using ```Enable-AzureRmAlias```:</span></span>
```powershell
#Requires -Modules Az.Storage
Enable-AzureRmAlias
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="2865e-143">```Enable-AzureRmAlias -Scope CurrentUser``` を実行すると、現在のユーザーが開くすべての PowerShell セッションでエイリアスが有効になるため、このコマンドレットの実行後は、次のようなスクリプトを変更する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="2865e-143">Running ```Enable-AzureRmAlias -Scope CurrentUser``` will enable the aliases for all powershell sessions you open, so that after executing this cmdlet, a script like this would not need to be changed at all:</span></span>
```powershell
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="2865e-144">エイリアス コマンドレットの使用方法の詳細については、PowerShell プロンプトから ```Get-Help -Online Enable-AzureRmAlias``` を実行してください。</span><span class="sxs-lookup"><span data-stu-id="2865e-144">For complete details on the usage of the alias cmdlets, execute ```Get-Help -Online Enable-AzureRmAlias``` from the powershell prompt.</span></span>

<span data-ttu-id="2865e-145">```Disable-AzureRmAlias``` は、```Enable-AzureRmAlias``` によって作成された AzureRM コマンドレットのエイリアスを削除します。</span><span class="sxs-lookup"><span data-stu-id="2865e-145">```Disable-AzureRmAlias``` removes AzureRM cmdlet aliases created by ```Enable-AzureRmAlias```.</span></span>  <span data-ttu-id="2865e-146">詳細については、PowerShell プロンプトから ```Get-Help -Online Disable-AzureRmAlias``` を実行してください。</span><span class="sxs-lookup"><span data-stu-id="2865e-146">For complete details, execute ```Get-Help -Online Disable-AzureRmAlias``` from the powershell prompt.</span></span>

### <a name="module-name-changes"></a><span data-ttu-id="2865e-147">モジュール名の変更</span><span class="sxs-lookup"><span data-stu-id="2865e-147">Module Name Changes</span></span>
- <span data-ttu-id="2865e-148">次のモジュールを除き、モジュール名が `AzureRM.*` から `Az.*` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-148">The module names have changed from `AzureRM.*` to `Az.*`, except for the following modules:</span></span>
```
AzureRM.Profile                       -> Az.Accounts
Azure.AnalysisServices                -> Az.AnalysisServices
AzureRM.Consumption                   -> Az.Billing
AzureRM.UsageAggregates               -> Az.Billing
AzureRM.DataFactories                 -> Az.DataFactory
AzureRM.DataFactoryV2                 -> Az.DataFactory
AzureRM.MachineLearningCompute        -> Az.MachineLearning
AzureRM.Insights                      -> Az.Monitor
AzureRM.RecoveryServices.Backup       -> Az.RecoveryServices
AzureRM.RecoveryServices.SiteRecovery -> Az.RecoveryServices
AzureRM.Tags                          -> Az.Resources
Azure.Storage                         -> Az.Storage
```

<span data-ttu-id="2865e-149">モジュール名が変更されたので、```#Requires``` または ```Import-Module``` を使用して特定のモジュールを読み込むスクリプトは、新しいモジュールを代わりに使用するように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-149">The changes in module names mean that any script that uses ```#Requires``` or ```Import-Module``` to load specific modules will need to be changed to use the new module instead.</span></span>

#### <a name="migrating-requires-statements"></a><span data-ttu-id="2865e-150">#Requires ステートメントの移行</span><span class="sxs-lookup"><span data-stu-id="2865e-150">Migrating #Requires Statements</span></span>
<span data-ttu-id="2865e-151">#Requires を使用して AzureRM モジュールへの依存関係を宣言しているスクリプトは、新しいモジュール名を使用するように更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-151">Scripts that use #Requires to declare a dependency on AzureRM modules should be updated to use the new module names</span></span>
```powershell
#Requires -Module AzureRM.Compute
```

<span data-ttu-id="2865e-152">次のように変更します。</span><span class="sxs-lookup"><span data-stu-id="2865e-152">Should be changed to</span></span>
```powershell
#Requires -Module Az.Compute
```

#### <a name="migrating-import-module-statements"></a><span data-ttu-id="2865e-153">Import-Module ステートメントの移行</span><span class="sxs-lookup"><span data-stu-id="2865e-153">Migrating Import-Module Statements</span></span>
<span data-ttu-id="2865e-154">```Import-Module``` を使用して AzureRM モジュールを読み込むスクリプトは、新しいモジュール名を反映するように更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-154">Scripts that use ```Import-Module``` to load AzureRM modules will need to be updated to reflect the new module names.</span></span>
```powershell
Import-Module -Name AzureRM.Compute
```

<span data-ttu-id="2865e-155">次のように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-155">Should be changed to</span></span>
```powershell
Import-Module -Name Az.Compute
```

### <a name="migrating-fully-qualified-cmdlet-invocations"></a><span data-ttu-id="2865e-156">完全修飾コマンドレットの呼び出しの移行</span><span class="sxs-lookup"><span data-stu-id="2865e-156">Migrating Fully-Qualified Cmdlet Invocations</span></span>
<span data-ttu-id="2865e-157">次のように、モジュール修飾コマンドレットの呼び出しを使用するスクリプトは</span><span class="sxs-lookup"><span data-stu-id="2865e-157">Scripts that use module-qualified cmdlet invocations, like</span></span>
```powershell
AzureRM.Compute\Get-AzureRmVM
```

<span data-ttu-id="2865e-158">新しいモジュール名とコマンドレット名を使用するように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-158">Should be changed to use the new module and cmdlet names</span></span>
```powershell
Az.Compute\Get-AzVM
```

### <a name="migrating-module-manifest-dependencies"></a><span data-ttu-id="2865e-159">モジュール マニフェスト依存関係の移行</span><span class="sxs-lookup"><span data-stu-id="2865e-159">Migrating Module Manifest Dependencies</span></span>
<span data-ttu-id="2865e-160">モジュール マニフェスト (.psd1) ファイルを使用して AzureRM モジュールへの依存関係を表すモジュールは、"RequiredModules" セクションのモジュール名を更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-160">Modules that express dependencies on AzureRM modules through a module manifest (.psd1) file will need to updated the module names in their 'RequiredModules' section</span></span>

```powershell
RequiredModules = @(@{ModuleName="AzureRM.Profile"; ModuleVersion="5.8.2"})
```

<span data-ttu-id="2865e-161">次のように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-161">Should be changed to</span></span>

```powershell
RequiredModules = @(@{ModuleName="Az.Profile"; ModuleVersion="1.0.0"})
```

### <a name="removed-modules"></a><span data-ttu-id="2865e-162">削除されたモジュール</span><span class="sxs-lookup"><span data-stu-id="2865e-162">Removed modules</span></span>
- `AzureRM.Backup`
- `AzureRM.Compute.ManagedService`
- `AzureRM.Scheduler`

<span data-ttu-id="2865e-163">これらのサービス用のツールは積極的にサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="2865e-163">The tooling for these services are no longer actively supported.</span></span>  <span data-ttu-id="2865e-164">都合がつき次第、代替サービスに移行することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="2865e-164">Customers are encouraged to move to alternative services as soon as it is convenient.</span></span>

### <a name="windows-powershell-51-and-net-472"></a><span data-ttu-id="2865e-165">Windows PowerShell 5.1 と .NET 4.7.2</span><span class="sxs-lookup"><span data-stu-id="2865e-165">Windows PowerShell 5.1 and .NET 4.7.2</span></span>
- <span data-ttu-id="2865e-166">Windows PowerShell 5.1 で Az を使用するには、.NET 4.7.2 をインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-166">Using Az with Windows PowerShell 5.1 requires the installation of .NET 4.7.2.</span></span> <span data-ttu-id="2865e-167">ただし、PowerShell Core で Az を使用する場合、.NET 4.7.2 は不要です。</span><span class="sxs-lookup"><span data-stu-id="2865e-167">However, using Az with PowerShell Core does not require .NET 4.7.2.</span></span> 

### <a name="temporary-removal-of-user-login-using-pscredential"></a><span data-ttu-id="2865e-168">PSCredential を使用したユーザー ログインの一時的な削除</span><span class="sxs-lookup"><span data-stu-id="2865e-168">Temporary removal of User login using PSCredential</span></span>
- <span data-ttu-id="2865e-169">.NET Standard の認証フローの変更により、PSCredential を使用したユーザー ログインが一時的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="2865e-169">Due to changes in the authentication flow for .NET Standard, we are temporarily removing user login via PSCredential.</span></span> <span data-ttu-id="2865e-170">この機能は、Windows PowerShell 5.1 の 2019/1/15 リリースで再導入されます。</span><span class="sxs-lookup"><span data-stu-id="2865e-170">This capability will be re-introduced in the 1/15/2019 release for Windows PowerShell 5.1.</span></span> <span data-ttu-id="2865e-171">詳細については、[こちらの問題](https://github.com/Azure/azure-powershell/issues/7430)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2865e-171">This is duscussed in detail in [this issue.](https://github.com/Azure/azure-powershell/issues/7430)</span></span>

### <a name="default-device-code-login-instead-of-web-browser-prompt"></a><span data-ttu-id="2865e-172">Web ブラウザー プロンプトの代わりにデバイス コード ログインを既定で使用</span><span class="sxs-lookup"><span data-stu-id="2865e-172">Default Device Code login instead of Web Browser prompt</span></span>
- <span data-ttu-id="2865e-173">.NET Standard の認証フローの変更により、対話型ログイン時の既定のログイン フローとしてデバイス ログインが使用されます。</span><span class="sxs-lookup"><span data-stu-id="2865e-173">Due to changes in the authentication flow for .NET Standard, we are using device login as the default login flow during interactive login.</span></span> <span data-ttu-id="2865e-174">Web ブラウザー ベースのログインは、Windows PowerShell 5.1 の 2019/1/15 リリースで既定のログインとして再導入されます。</span><span class="sxs-lookup"><span data-stu-id="2865e-174">Web browser based login will be re-introduced for Windows PowerShell 5.1 as the default in the 1/15/2019 release.</span></span> <span data-ttu-id="2865e-175">その時点で、ユーザーは Switch パラメーターを使用してデバイス ログインを選択できるようになります。</span><span class="sxs-lookup"><span data-stu-id="2865e-175">At that time, users will be able to choose device login using a Switch parameter.</span></span>

## <a name="module-breaking-changes"></a><span data-ttu-id="2865e-176">モジュールの破壊的変更</span><span class="sxs-lookup"><span data-stu-id="2865e-176">Module breaking changes</span></span>

### <a name="azapimanagement-previously-azurermapimanagement"></a><span data-ttu-id="2865e-177">Az.ApiManagement (以前の AzureRM.ApiManagement)</span><span class="sxs-lookup"><span data-stu-id="2865e-177">Az.ApiManagement (previously AzureRM.ApiManagement)</span></span>
- <span data-ttu-id="2865e-178">次のコマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-178">Removing the following cmdlets:</span></span>
  - <span data-ttu-id="2865e-179">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="2865e-179">New-AzureRmApiManagementHostnameConfiguration</span></span>
  - <span data-ttu-id="2865e-180">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="2865e-180">Set-AzureRmApiManagementHostnames</span></span>
  - <span data-ttu-id="2865e-181">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="2865e-181">Update-AzureRmApiManagementDeployment</span></span>
  - <span data-ttu-id="2865e-182">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="2865e-182">Import-AzureRmApiManagementHostnameCertificate</span></span>
  - <span data-ttu-id="2865e-183">代わりに、**Set-AzApiManagement** コマンドレットを使用して、これらのプロパティを設定します</span><span class="sxs-lookup"><span data-stu-id="2865e-183">Use **Set-AzApiManagement** cmdlet to set these properites instead</span></span>
- <span data-ttu-id="2865e-184">次のプロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-184">Following properties were removed</span></span>
  - <span data-ttu-id="2865e-185">`PsApiManagementContext` から、`PsApiManagementHostnameConfiguration` 型の `PortalHostnameConfiguration`、`ProxyHostnameConfiguration`、`ManagementHostnameConfiguration`、`ScmHostnameConfiguration` の各プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-185">Removed property `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration` and `ScmHostnameConfiguration` of type `PsApiManagementHostnameConfiguration` from `PsApiManagementContext`.</span></span> <span data-ttu-id="2865e-186">代わりに、`PsApiManagementCustomHostNameConfiguration` 型の `PortalCustomHostnameConfiguration`、`ProxyCustomHostnameConfiguration`、`ManagementCustomHostnameConfiguration`、`ScmCustomHostnameConfiguration` を使用します。</span><span class="sxs-lookup"><span data-stu-id="2865e-186">Instead use `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration` and `ScmCustomHostnameConfiguration` of type `PsApiManagementCustomHostNameConfiguration`.</span></span>
  - <span data-ttu-id="2865e-187">PsApiManagementContext から `StaticIPs` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-187">Removed property `StaticIPs` from PsApiManagementContext.</span></span> <span data-ttu-id="2865e-188">このプロパティは、`PublicIPAddresses` と `PrivateIPAddresses` に分割されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-188">The property has been split into `PublicIPAddresses` and `PrivateIPAddresses`.</span></span>
  - <span data-ttu-id="2865e-189">New-AzureApiManagementVirtualNetwork コマンドレットから、必須の `Location` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-189">Removed required property `Location` from New-AzureApiManagementVirtualNetwork cmdlet.</span></span>

### <a name="azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates"></a><span data-ttu-id="2865e-190">Az.Billing (以前の AzureRM.Billing、AzureRM.Consumption、および AzureRM.UsageAggregates)</span><span class="sxs-lookup"><span data-stu-id="2865e-190">Az.Billing (previously AzureRM.Billing, AzureRM.Consumption, and AzureRM.UsageAggregates)</span></span>
- <span data-ttu-id="2865e-191">`Get-AzConsumptionUsageDetail` コマンドレットから、`InvoiceName` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-191">The `InvoiceName` parameter was removed from the `Get-AzConsumptionUsageDetail` cmdlet.</span></span>  <span data-ttu-id="2865e-192">スクリプトでは、請求書に他の ID パラメーターを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-192">Scripts will need to use other identity parameters for the invoice.</span></span>

### <a name="azcognitiveservices-previously-azurermcognitiveservices"></a><span data-ttu-id="2865e-193">Az.CognitiveServices (以前の AzureRM.CognitiveServices)</span><span class="sxs-lookup"><span data-stu-id="2865e-193">Az.CognitiveServices (previously AzureRM.CognitiveServices)</span></span>
- <span data-ttu-id="2865e-194">`Get-AzCognitiveServicesAccountSkus` コマンドレットから、`GetSkusWithAccountParamSetName` パラメーター セットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-194">Removed `GetSkusWithAccountParamSetName` parameter set from `Get-AzCognitiveServicesAccountSkus` cmdlet.</span></span>  <span data-ttu-id="2865e-195">ResourceGroupName とアカウント名を使用するのではなく、アカウントの種類と場所で SKU を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-195">You must get Skus by Account Type and Location, instead of using ResourceGroupName and Account Name.</span></span>

### <a name="azcompute-previously-azurermcompute"></a><span data-ttu-id="2865e-196">Az.Compute (以前の AzureRM.Compute)</span><span class="sxs-lookup"><span data-stu-id="2865e-196">Az.Compute (previously AzureRM.Compute)</span></span>
- <span data-ttu-id="2865e-197">`PSVirtualMachine` および `PSVirtualMachineScaleSet` オブジェクトの `Identity` プロパティから `IdentityIds` が削除されました。スクリプトでは、このフィールドの値を使用して処理を決定することはできなくなりました。</span><span class="sxs-lookup"><span data-stu-id="2865e-197">`IdentityIds` are removed from `Identity` property in `PSVirtualMachine` and `PSVirtualMachineScaleSet` objects Scripts should no longer use the value of this field to make processing decisions.</span></span>
- <span data-ttu-id="2865e-198">`PSVirtualMachineScaleSetVM` オブジェクトの `InstanceView` プロパティの型が、`VirtualMachineInstanceView` から `VirtualMachineScaleSetVMInstanceView` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-198">The type of `InstanceView` property of `PSVirtualMachineScaleSetVM` object is changed from `VirtualMachineInstanceView` to `VirtualMachineScaleSetVMInstanceView`</span></span>
- <span data-ttu-id="2865e-199">`UpgradePolicy` プロパティから、`AutoOSUpgradePolicy` および `AutomaticOSUpgrade` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-199">`AutoOSUpgradePolicy` and `AutomaticOSUpgrade` properties are removed from `UpgradePolicy` property</span></span>
- <span data-ttu-id="2865e-200">`PSSnapshotUpdate` オブジェクトの `Sku` プロパティの型が、`DiskSku` から `SnapshotSku` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-200">The type of `Sku` property in `PSSnapshotUpdate` object is changed from `DiskSku` to `SnapshotSku`</span></span>
- <span data-ttu-id="2865e-201">`Add-AzVMDataDisk` コマンドレットから、`VmScaleSetVMParameterSet` が削除されました。スケールセット VM にデータ ディスクを個別に追加することはできなくなりました。</span><span class="sxs-lookup"><span data-stu-id="2865e-201">`VmScaleSetVMParameterSet` is removed from `Add-AzVMDataDisk` cmdlet, you cna no longer add a data disk individually to a ScaleSet VM.</span></span>

### <a name="azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2"></a><span data-ttu-id="2865e-202">Az.DataFactory (以前の AzureRM.DataFactories および AzureRM.DataFactoryV2)</span><span class="sxs-lookup"><span data-stu-id="2865e-202">Az.DataFactory (previously AzureRM.DataFactories and AzureRM.DataFactoryV2)</span></span>
- <span data-ttu-id="2865e-203">`New-AzDataFactoryEncryptValue` コマンドレットで `GatewayName` パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="2865e-203">The `GatewayName` parameter has become mandatory in the `New-AzDataFactoryEncryptValue` cmdlet</span></span>
- <span data-ttu-id="2865e-204">`New-AzDataFactoryGatewayKey` コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-204">Removed `New-AzDataFactoryGatewayKey` cmdlet</span></span>
- <span data-ttu-id="2865e-205">`Get-AzDataFactoryV2ActivityRun` コマンドレットから、`LinkedServiceName` パラメーターが削除されました。スクリプトでは、このフィールドの値を使用して処理を決定することはできなくなりました。</span><span class="sxs-lookup"><span data-stu-id="2865e-205">Removed `LinkedServiceName` parameter from `Get-AzDataFactoryV2ActivityRun` cmdlet Scripts should no longer use the value of this field to make processing decisions.</span></span>

### <a name="azdatalakeanalytics-previously-azurermdatalakeanalytics"></a><span data-ttu-id="2865e-206">Az.DataLakeAnalytics (以前の AzureRM.DataLakeAnalytics)</span><span class="sxs-lookup"><span data-stu-id="2865e-206">Az.DataLakeAnalytics (previously AzureRM.DataLakeAnalytics)</span></span>
- <span data-ttu-id="2865e-207">非推奨の `New-AzDataLakeAnalyticsCatalogSecret`、`Remove-AzDataLakeAnalyticsCatalogSecret`、`Set-AzDataLakeAnalyticsCatalogSecret` の各コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-207">Removed deprecated cmdlets: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret`, and `Set-AzDataLakeAnalyticsCatalogSecret`</span></span>

### <a name="azdatalakestore-previously-azurermdatalakestore"></a><span data-ttu-id="2865e-208">Az.DataLakeStore (以前の AzureRM.DataLakeStore)</span><span class="sxs-lookup"><span data-stu-id="2865e-208">Az.DataLakeStore (previously AzureRM.DataLakeStore)</span></span>
- <span data-ttu-id="2865e-209">次のコマンドレットの `Encoding` パラメーターの型が、`FileSystemCmdletProviderEncoding` から `System.Text.Encoding` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-209">The following cmdlets have had the `Encoding` parameter changed from the type `FileSystemCmdletProviderEncoding` to `System.Text.Encoding`.</span></span> <span data-ttu-id="2865e-210">この変更により、エンコード値 `String` と `Oem` が削除されます。</span><span class="sxs-lookup"><span data-stu-id="2865e-210">This change removes the encoding values `String` and `Oem`.</span></span> <span data-ttu-id="2865e-211">以前からの他のエンコード値はすべて残ります。</span><span class="sxs-lookup"><span data-stu-id="2865e-211">All the other prior encoding values remain.</span></span>
  - <span data-ttu-id="2865e-212">New-AzureRmDataLakeStoreItem</span><span class="sxs-lookup"><span data-stu-id="2865e-212">New-AzureRmDataLakeStoreItem</span></span>
  - <span data-ttu-id="2865e-213">Add-AzureRmDataLakeStoreItemContent</span><span class="sxs-lookup"><span data-stu-id="2865e-213">Add-AzureRmDataLakeStoreItemContent</span></span>
  - <span data-ttu-id="2865e-214">Get-AzureRmDataLakeStoreItemContent</span><span class="sxs-lookup"><span data-stu-id="2865e-214">Get-AzureRmDataLakeStoreItemContent</span></span>
- <span data-ttu-id="2865e-215">`New-AzDataLakeStoreAccount` および `Set-AzDataLakeStoreAccount` コマンドレットから、非推奨の `Tags` プロパティのエイリアスが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-215">Removed deprecated `Tags` property alias from `New-AzDataLakeStoreAccount` and `Set-AzDataLakeStoreAccount` cmdlets</span></span>

  <span data-ttu-id="2865e-216">次のコマンドレットを使用するスクリプトは</span><span class="sxs-lookup"><span data-stu-id="2865e-216">Scripts using</span></span>
  ```powershell
  New-AzureRMDataLakeStoreAccount -Tags @{TagName="TagValue"}
  ```

  <span data-ttu-id="2865e-217">次のように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-217">Should be changed to</span></span>
  ```powershell
  New-AzDataLakeStoreAccount -Tag @{TagName="TagValue"}
  ```

- <span data-ttu-id="2865e-218">```PSDataLakeStoreAccountBasic``` オブジェクトから、非推奨の ```Identity```、```EncryptionState```、```EncrypotionProvisioningState```、```EncryptionConfig```、```FirewallState```、```FirewallRules```、```VirtualNetworkRules```、```TrustedIdProviderState```、```TrustedIdProviders```、```DefaultGroup```、```NewTier```、```CurrentTier```、```FirewallAllowAzureIps``` の各プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-218">Removed deprecated properties ```Identity```, ```EncryptionState```, ```EncrypotionProvisioningState```, ```EncryptionConfig```, ```FirewallState```, ```FirewallRules```, ```VirtualNetworkRules```, ```TrustedIdProviderState```, ```TrustedIdProviders```, ```DefaultGroup```, ```NewTier```, ```CurrentTier```, ```FirewallAllowAzureIps``` from ```PSDataLakeStoreAccountBasic``` object.</span></span>  <span data-ttu-id="2865e-219">```Get-AzDataLakeStoreAccount``` から返された ```PSDatalakeStoreAccount``` を使用するスクリプトでは、これらのプロパティを参照しないでください。</span><span class="sxs-lookup"><span data-stu-id="2865e-219">Any script that uses the ```PSDatalakeStoreAccount``` returned from ```Get-AzDataLakeStoreAccount``` should not reference these properties.</span></span>

### <a name="azkeyvault-previously-azurermkeyvault"></a><span data-ttu-id="2865e-220">Az.KeyVault (以前の AzureRM.KeyVault)</span><span class="sxs-lookup"><span data-stu-id="2865e-220">Az.KeyVault (previously AzureRM.KeyVault)</span></span>
- <span data-ttu-id="2865e-221">`PSKeyVaultKeyAttributes`、`PSKeyVaultKeyIdentityItem`、`PSKeyVaultSecretAttributes` の各オブジェクトから、`PurgeDisabled` プロパティが削除されました。スクリプトでは、```PurgeDisabled``` プロパティを参照して処理を決定することはできなくなりました。</span><span class="sxs-lookup"><span data-stu-id="2865e-221">The `PurgeDisabled` property was removed from the `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem`, and `PSKeyVaultSecretAttributes` objects Scripts shoudl no longer reference the ```PurgeDisabled``` property to make processing decisions.</span></span>

### <a name="azmedia-previously-azurermmedia"></a><span data-ttu-id="2865e-222">Az.Media (以前の AzureRM.Media)</span><span class="sxs-lookup"><span data-stu-id="2865e-222">Az.Media (previously AzureRM.Media)</span></span>
- <span data-ttu-id="2865e-223">`New-AzMediaService` コマンドレットから、非推奨の `Tags` プロパティのエイリアスが削除されました。次のコマンドレットを使用するスクリプトは</span><span class="sxs-lookup"><span data-stu-id="2865e-223">Remove deprecated `Tags` property alias from `New-AzMediaService` cmdlet Scripts using</span></span>
  ```powershell
  New-AzureRMMediaService -Tags @{TagName="TagValue"}
  ```

  <span data-ttu-id="2865e-224">次のように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-224">Should be changed to</span></span>
  ```powershell
  New-AzMMediaService -Tag @{TagName="TagValue"}
  ```
### <a name="azmonitor-previously-azurerminsights"></a><span data-ttu-id="2865e-225">Az.Monitor (以前の AzureRM.Insights)</span><span class="sxs-lookup"><span data-stu-id="2865e-225">Az.Monitor (previously AzureRM.Insights)</span></span>
- <span data-ttu-id="2865e-226">単数形のパラメーター名を優先して、`Set-AzDiagnosticSetting` コマンドレットから複数形のパラメーター名 `Categories` と `Timegrains` が削除されました。次のコマンドレットを使用するスクリプトは</span><span class="sxs-lookup"><span data-stu-id="2865e-226">Removed plural names `Categories` and `Timegrains` parameter in favor of singular parameter names from `Set-AzDiagnosticSetting` cmdlet Scripts using</span></span>
  ```powershell
  Set-AzureRmDiagnosticSetting -Timegrains PT1M -Categories Category1, Category2
  ```

  <span data-ttu-id="2865e-227">次のように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-227">Should be changed to</span></span>
  ```powershell
  Set-AzDiagnosticSetting -Timegrain PT1M -Category Category1, Category2
  ```
### <a name="aznetwork-previously-azurermnetwork"></a><span data-ttu-id="2865e-228">Az.Network (以前の AzureRM.Network)</span><span class="sxs-lookup"><span data-stu-id="2865e-228">Az.Network (previously AzureRM.Network)</span></span>
- <span data-ttu-id="2865e-229">`Get-AzServiceEndpointPolicyDefinition` コマンドレットから、非推奨の `ResourceId` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-229">Removed deprecated `ResourceId` parameter from `Get-AzServiceEndpointPolicyDefinition` cmdlet</span></span>
- <span data-ttu-id="2865e-230">`PSVirtualNetwork` オブジェクトから、非推奨の `EnableVmProtection` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-230">Removed deprecated `EnableVmProtection` property from `PSVirtualNetwork` object</span></span>
- <span data-ttu-id="2865e-231">非推奨の `Set-AzVirtualNetworkGatewayVpnClientConfig` コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-231">Removed deprecated `Set-AzVirtualNetworkGatewayVpnClientConfig` cmdlet</span></span>
  
<span data-ttu-id="2865e-232">スクリプトでは、これらのフィールドの値に基づいて処理を決定することはできなくなりました。</span><span class="sxs-lookup"><span data-stu-id="2865e-232">Scripts shoudl no longer make processing decisions based on the values fo these fields.</span></span>

### <a name="azoperationalinsights-previously-azurermoperationalinsights"></a><span data-ttu-id="2865e-233">Az.OperationalInsights (以前の AzureRM.OperationalInsights)</span><span class="sxs-lookup"><span data-stu-id="2865e-233">Az.OperationalInsights (previously AzureRM.OperationalInsights)</span></span>
- <span data-ttu-id="2865e-234">`Get-AzOperationalInsightsDataSource` の既定のパラメーター セットが削除され、`ByWorkspaceNameByKind` が既定のパラメーター セットになりました。</span><span class="sxs-lookup"><span data-stu-id="2865e-234">Default parameter set for `Get-AzOperationalInsightsDataSource` is removed, and `ByWorkspaceNameByKind` has become the default parameter set</span></span>

  <span data-ttu-id="2865e-235">次のコマンドレットを使用してデータ ソースのリストを表示するスクリプトは</span><span class="sxs-lookup"><span data-stu-id="2865e-235">Scripts that listed data sources using</span></span>
  ```powershell
  Get-AzureRmOperationalInsightsDataSource
  ```

  <span data-ttu-id="2865e-236">種類 (Kind) を指定するように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-236">Should be changed to specify a Kind</span></span>
  ```powershell
  Get-AzOperationalInsightsDataSource -Kind AzureActivityLog
  ```

### <a name="azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery"></a><span data-ttu-id="2865e-237">Az.RecoveryServices (以前の AzureRM.RecoveryServices、AzureRM.RecoveryServices.Backup、および AzureRM.RecoveryServices.SiteRecovery)</span><span class="sxs-lookup"><span data-stu-id="2865e-237">Az.RecoveryServices (previously AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, and AzureRM.RecoveryServices.SiteRecovery)</span></span>
- <span data-ttu-id="2865e-238">`New/Set-AzRecoveryServicesAsrPolicy` コマンドレットから、`Encryption` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-238">Removed `Encryption` parameter from `New/Set-AzRecoveryServicesAsrPolicy` cmdlet</span></span>
- <span data-ttu-id="2865e-239">`Restore-AzRecoveryServicesBackupItem` コマンドレットでのマネージド ディスクの復元に `TargetStorageAccountName` パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="2865e-239">`TargetStorageAccountName` parameter is now mandatory for managed disk restores in `Restore-AzRecoveryServicesBackupItem` cmdlet</span></span>
- <span data-ttu-id="2865e-240">`Restore-AzRecoveryServicesBackupItem` コマンドレットの `StorageAccountName` および `StorageAccountResourceGroupName` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-240">Removed `StorageAccountName` and `StorageAccountResourceGroupName` parameters in `Restore-AzRecoveryServicesBackupItem` cmdlet</span></span>
- <span data-ttu-id="2865e-241">`Get-AzRecoveryServicesBackupContainer` コマンドレットの `Name` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-241">Removed `Name`parameter in `Get-AzRecoveryServicesBackupContainer` cmdlet</span></span>

### <a name="azresources-previously-azurermresources"></a><span data-ttu-id="2865e-242">Az.Resources (以前の AzureRM.Resources)</span><span class="sxs-lookup"><span data-stu-id="2865e-242">Az.Resources (previously AzureRM.Resources)</span></span>
- <span data-ttu-id="2865e-243">`New/Set-AzPolicyAssignment` コマンドレットから、`Sku` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-243">Removed `Sku` parameter from `New/Set-AzPolicyAssignment` cmdlet</span></span>
- <span data-ttu-id="2865e-244">`New-AzADServicePrincipal` および `New-AzADSpCredential` コマンドレットから、`Password` パラメーターが削除されました。パスワードは自動的に生成されます。次のようにパスワードを指定しているスクリプトは</span><span class="sxs-lookup"><span data-stu-id="2865e-244">Removed `Password` parameter from `New-AzADServicePrincipal` and `New-AzADSpCredential` cmdlet Passwords are automatically generated, scripts that provided the password:</span></span>
  ```powershell
  New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476 -Password $secPassword
  ```

  <span data-ttu-id="2865e-245">出力からパスワードを取得するように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2865e-245">Should be changed to retriedve the password from the output:</span></span>
  ```powershell
  $credential = New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476
  $secPassword = $credential.Secret
  ```

### <a name="azservicefabric-previously-azurermservicefabric"></a><span data-ttu-id="2865e-246">Az.ServiceFabric (以前の AzureRM.ServiceFabric)</span><span class="sxs-lookup"><span data-stu-id="2865e-246">Az.ServiceFabric (previously AzureRM.ServiceFabric)</span></span>
- <span data-ttu-id="2865e-247">コマンドレットの次の戻り値の型が変更されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-247">The following cmdlet return types have been changed:</span></span>
  - <span data-ttu-id="2865e-248">`ApplicationHealthPolicy` 型の `SerivceTypeHealthPolicies` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-248">The property `SerivceTypeHealthPolicies` of type `ApplicationHealthPolicy` has been removed.</span></span>
  - <span data-ttu-id="2865e-249">`ClusterUpgradeDeltaHealthPolicy` 型の `ApplicationHealthPolicies` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-249">The property `ApplicationHealthPolicies` of type `ClusterUpgradeDeltaHealthPolicy` has been removed.</span></span>
  - <span data-ttu-id="2865e-250">`ClusterUpgradePolicy` 型の `OverrideUserUpgradePolicy` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-250">The property `OverrideUserUpgradePolicy` of type `ClusterUpgradePolicy` has been removed.</span></span>
  - <span data-ttu-id="2865e-251">これらの変更は、次のコマンドレットに影響します。</span><span class="sxs-lookup"><span data-stu-id="2865e-251">These changes affect the following cmdlets:</span></span>
    - <span data-ttu-id="2865e-252">Add-AzServiceFabricClientCertificate</span><span class="sxs-lookup"><span data-stu-id="2865e-252">Add-AzServiceFabricClientCertificate</span></span>
    - <span data-ttu-id="2865e-253">Add-AzServiceFabricClusterCertificate</span><span class="sxs-lookup"><span data-stu-id="2865e-253">Add-AzServiceFabricClusterCertificate</span></span>
    - <span data-ttu-id="2865e-254">Add-AzServiceFabricNode</span><span class="sxs-lookup"><span data-stu-id="2865e-254">Add-AzServiceFabricNode</span></span>
    - <span data-ttu-id="2865e-255">Add-AzServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="2865e-255">Add-AzServiceFabricNodeType</span></span>
    - <span data-ttu-id="2865e-256">Get-AzServiceFabricCluster</span><span class="sxs-lookup"><span data-stu-id="2865e-256">Get-AzServiceFabricCluster</span></span>
    - <span data-ttu-id="2865e-257">Remove-AzServiceFabricClientCertificate</span><span class="sxs-lookup"><span data-stu-id="2865e-257">Remove-AzServiceFabricClientCertificate</span></span>
    - <span data-ttu-id="2865e-258">Remove-AzServiceFabricClusterCertificate</span><span class="sxs-lookup"><span data-stu-id="2865e-258">Remove-AzServiceFabricClusterCertificate</span></span>
    - <span data-ttu-id="2865e-259">Remove-AzServiceFabricNode</span><span class="sxs-lookup"><span data-stu-id="2865e-259">Remove-AzServiceFabricNode</span></span>
    - <span data-ttu-id="2865e-260">Remove-AzServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="2865e-260">Remove-AzServiceFabricNodeType</span></span>
    - <span data-ttu-id="2865e-261">Remove-AzServiceFabricSetting</span><span class="sxs-lookup"><span data-stu-id="2865e-261">Remove-AzServiceFabricSetting</span></span>
    - <span data-ttu-id="2865e-262">Set-AzServiceFabricSetting</span><span class="sxs-lookup"><span data-stu-id="2865e-262">Set-AzServiceFabricSetting</span></span>
    - <span data-ttu-id="2865e-263">Set-AzServiceFabricUpgradeType</span><span class="sxs-lookup"><span data-stu-id="2865e-263">Set-AzServiceFabricUpgradeType</span></span>
    - <span data-ttu-id="2865e-264">Update-AzServiceFabricDurability</span><span class="sxs-lookup"><span data-stu-id="2865e-264">Update-AzServiceFabricDurability</span></span>
    - <span data-ttu-id="2865e-265">Update-AzServiceFabricReliability</span><span class="sxs-lookup"><span data-stu-id="2865e-265">Update-AzServiceFabricReliability</span></span>

### <a name="azsql-previously-azurermsql"></a><span data-ttu-id="2865e-266">Az.Sql (以前の AzureRM.Sql)</span><span class="sxs-lookup"><span data-stu-id="2865e-266">Az.Sql (previously AzureRM.Sql)</span></span>
- <span data-ttu-id="2865e-267">`Set-AzSqlDatabaseBackupLongTermRetentionPolicy` コマンドレットから、`State` および `ResourceId` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-267">Removed `State` and `ResourceId` parameters from `Set-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet</span></span>
- <span data-ttu-id="2865e-268">非推奨の `Get/Set-AzSqlServerBackupLongTermRetentionVault`、`Get/Start/Stop-AzSqlServerUpgrade`、`Get/Set-AzSqlDatabaseAuditingPolicy`、`Get/Set-AzSqlServerAuditingPolicy`、`Remove-AzSqlDatabaseAuditing`、`Remove-AzSqlServerAuditing` の各コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-268">Removed deprecated cmdlets: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing`, `Remove-AzSqlServerAuditing`</span></span>
- <span data-ttu-id="2865e-269">`Get-AzSqlDatabaseBackupLongTermRetentionPolicy` コマンドレットから、非推奨の `Current` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-269">Removed deprecated parameter `Current` from `Get-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet</span></span>
- <span data-ttu-id="2865e-270">`Get-AzSqlServerServiceObjective` コマンドレットから、非推奨の `DatabaseName` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-270">Removed deprecated parameter `DatabaseName` from `Get-AzSqlServerServiceObjective` cmdlet</span></span>
- <span data-ttu-id="2865e-271">`Set-AzSqlDatabaseDataMaskingPolicy` コマンドレットから、非推奨の `PrivilegedLogin` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-271">Removed deprecated parameter `PrivilegedLogin` from `Set-AzSqlDatabaseDataMaskingPolicy` cmdlet</span></span>

### <a name="azstorage-previously-azurestorage-and-azurermstorage"></a><span data-ttu-id="2865e-272">Az.Storage (以前の Azure.Storage and AzureRM.Storage)</span><span class="sxs-lookup"><span data-stu-id="2865e-272">Az.Storage (previously Azure.Storage and AzureRM.Storage)</span></span>
- <span data-ttu-id="2865e-273">ストレージ アカウント名のみを使用した Oauth ストレージ コンテキストの作成をサポートするために、既定のパラメーター セットが `OAuthParameterSet` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-273">To support creating an Oauth storage context with only the storage account name, the default parameter set has been changed to `OAuthParameterSet`</span></span>
  - <span data-ttu-id="2865e-274">例: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`</span><span class="sxs-lookup"><span data-stu-id="2865e-274">Example: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`</span></span>
- <span data-ttu-id="2865e-275">`Get-AzStorageUsage` コマンドレットで `Location` パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="2865e-275">The `Location` parameter has become mandatory in the `Get-AzStorageUsage` cmdlet</span></span>
- <span data-ttu-id="2865e-276">Storage API のメソッドで、同期 API 呼び出しの代わりに、タスク ベースの非同期パターン (TAP) が使用されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2865e-276">The Storage API methods now use the Task-based Asynchronous Pattern (TAP), instead of synchronous API calls.</span></span>
#### <a name="1-blob-snapshot"></a><span data-ttu-id="2865e-277">1.BLOB スナップショット</span><span class="sxs-lookup"><span data-stu-id="2865e-277">1. Blob Snapshot</span></span>
##### <a name="before"></a><span data-ttu-id="2865e-278">変更前:</span><span class="sxs-lookup"><span data-stu-id="2865e-278">Before:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$b.ICloudBlob.Snapshot()
```

##### <a name="after"></a><span data-ttu-id="2865e-279">変更後:</span><span class="sxs-lookup"><span data-stu-id="2865e-279">After:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$task = $b.ICloudBlob.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="2-share-snapshot"></a><span data-ttu-id="2865e-280">2.スナップショットの共有</span><span class="sxs-lookup"><span data-stu-id="2865e-280">2. Share Snapshot</span></span>
##### <a name="before"></a><span data-ttu-id="2865e-281">変更前:</span><span class="sxs-lookup"><span data-stu-id="2865e-281">Before:</span></span>
```powershell
$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$snapshot = $Share.Snapshot()
```
#####  <a name="after"></a><span data-ttu-id="2865e-282">変更後:</span><span class="sxs-lookup"><span data-stu-id="2865e-282">After:</span></span>
```powershell

$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$task = $Share.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="3-undelete-a-soft-delete-blob"></a><span data-ttu-id="2865e-283">手順 3.BLOB の論理的な削除の取り消し</span><span class="sxs-lookup"><span data-stu-id="2865e-283">3. Undelete a soft delete blob</span></span>
##### <a name="before"></a><span data-ttu-id="2865e-284">変更前:</span><span class="sxs-lookup"><span data-stu-id="2865e-284">Before:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$b.ICloudBlob.Undelete()
```
##### <a name="after"></a><span data-ttu-id="2865e-285">変更後:</span><span class="sxs-lookup"><span data-stu-id="2865e-285">After:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$task = $b.ICloudBlob.UndeleteAsync()
$task.Wait()
```

#### <a name="4-set-blob-tier"></a><span data-ttu-id="2865e-286">4.BLOB 層の設定</span><span class="sxs-lookup"><span data-stu-id="2865e-286">4. Set Blob Tier</span></span>
##### <a name="before"></a><span data-ttu-id="2865e-287">変更前:</span><span class="sxs-lookup"><span data-stu-id="2865e-287">Before:</span></span>
```powershell
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$blockBlob.ICloudBlob.SetStandardBlobTier("hot")

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$pageBlob.ICloudBlob.SetPremiumBlobTier("P4")
```

##### <a name="after"></a><span data-ttu-id="2865e-288">変更後:</span><span class="sxs-lookup"><span data-stu-id="2865e-288">After:</span></span>
```powershell
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$task = $blockBlob.ICloudBlob.SetStandardBlobTierAsync("hot")
$task.Wait()

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$task = $pageBlob.ICloudBlob.SetPremiumBlobTierAsync("P4")
$task.Wait()
```

### <a name="azwebsites-previously-azurermwebsites"></a><span data-ttu-id="2865e-289">Az.Websites (以前の AzureRM.Websites)</span><span class="sxs-lookup"><span data-stu-id="2865e-289">Az.Websites (previously AzureRM.Websites)</span></span>
- <span data-ttu-id="2865e-290">`PSAppServicePlan`、`PSCertificate`、`PSCloningInfo`、`PSSite` の各オブジェクトから非推奨のプロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2865e-290">Removed deprecated properties from the `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo`, and `PSSite` objects</span></span>
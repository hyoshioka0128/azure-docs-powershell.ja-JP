---
title: Azure PowerShell の使用に関するページ
description: ''
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: get-started-article
ms.date: 01/14/2019
ms.openlocfilehash: 0c3b749cb2ac7f11dacafca76b65944f523f727d
ms.sourcegitcommit: 0356a4694f77eda40eec8c3759b9bb7f28979eb6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/18/2019
ms.locfileid: "67193211"
---
# <a name="get-started-with-azure-powershell"></a><span data-ttu-id="da742-102">Azure PowerShell の使用に関するページ</span><span class="sxs-lookup"><span data-stu-id="da742-102">Get started with Azure PowerShell</span></span>

<span data-ttu-id="da742-103">Azure PowerShell は、コマンド ラインから Azure リソースを管理できるように設計されています。</span><span class="sxs-lookup"><span data-stu-id="da742-103">Azure PowerShell is designed for managing and administering Azure resources from the command line.</span></span> <span data-ttu-id="da742-104">Azure Resource Manager モデルを使用する自動化ツールをビルドする場合に Azure PowerShell を使用します。</span><span class="sxs-lookup"><span data-stu-id="da742-104">Use Azure PowerShell when you want to build automated tools that use the Azure Resource Manager model.</span></span>
<span data-ttu-id="da742-105">[Azure Cloud Shell](/azure/cloud-shell/overview) を使ってブラウザーで試してみるか、ローカル コンピューターにインストールします。</span><span class="sxs-lookup"><span data-stu-id="da742-105">Try it out in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or install on your local machine.</span></span>

<span data-ttu-id="da742-106">この記事では、Azure PowerShell の基本的な使い方と、主要な概念について説明します。</span><span class="sxs-lookup"><span data-stu-id="da742-106">This article helps you get started with Azure PowerShell and teaches the core concepts behind it.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="da742-107">Azure Cloud Shell でのインストールまたは実行</span><span class="sxs-lookup"><span data-stu-id="da742-107">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="da742-108">Azure PowerShell の使用を開始する最も簡単な方法として、Azure Cloud Shell 環境でこれを試してみます。</span><span class="sxs-lookup"><span data-stu-id="da742-108">The easiest way to get started with Azure PowerShell is by trying it out in an Azure Cloud Shell environment.</span></span>
<span data-ttu-id="da742-109">Cloud Shell を起動して実行する方法については、「[Azure Cloud Shell の PowerShell のクイックスタート](/azure/cloud-shell/quickstart-powershell)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="da742-109">To get up and running with Cloud Shell, see [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
<span data-ttu-id="da742-110">Cloud Shell では Linux コンテナー上で PowerShell 6 が実行されるため、Windows 固有の機能は利用できません。</span><span class="sxs-lookup"><span data-stu-id="da742-110">Cloud Shell runs PowerShell 6 on a Linux container, so Windows-specific functionality isn't available.</span></span>

<span data-ttu-id="da742-111">Azure PowerShell をローカル コンピューターにインストールする準備ができたら、「[Install the Azure PowerShell module (Azure PowerShell モジュールのインストール)](install-az-ps.md)」の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="da742-111">When you're ready to install Azure PowerShell on your local machine, follow the instructions in [Install the Azure PowerShell module](install-az-ps.md).</span></span>

## <a name="sign-in-to-azure"></a><span data-ttu-id="da742-112">Azure へのサインイン</span><span class="sxs-lookup"><span data-stu-id="da742-112">Sign in to Azure</span></span>

<span data-ttu-id="da742-113">`Connect-AzAccount` コマンドレットを使って対話形式でサインインします。</span><span class="sxs-lookup"><span data-stu-id="da742-113">Sign in interactively with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="da742-114">Cloud Shell を使用する場合は、次の手順をスキップします。Azure Cloud Shell セッションは、Cloud Shell セッションを起動した環境、サブスクリプション、およびテナント用に既に認証されています。</span><span class="sxs-lookup"><span data-stu-id="da742-114">Skip this step if you use Cloud Shell: Your Azure Cloud Shell session is already authenticated for the environment, subscription, and tenant that launched the Cloud Shell session.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="da742-115">米国以外のリージョンの場合、`-Environment` パラメーターを使ってサインインします。</span><span class="sxs-lookup"><span data-stu-id="da742-115">If you're in a non-US region, use the `-Environment` parameter to sign in.</span></span> <span data-ttu-id="da742-116">[Get AzEnvironment](/powershell/module/Az.Accounts/Get-AzEnvironment) コマンドレットを使って、リージョンの環境の名前を取得します。</span><span class="sxs-lookup"><span data-stu-id="da742-116">Get the name of the environment for your region by using the [Get-AzEnvironment](/powershell/module/Az.Accounts/Get-AzEnvironment) cmdlet.</span></span> <span data-ttu-id="da742-117">たとえば、Azure China 21Vianet にサインインするには、以下を使用します。</span><span class="sxs-lookup"><span data-stu-id="da742-117">For example, to sign in to Azure China 21Vianet:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="da742-118">使用するトークンを取得します https://microsoft.com/devicelogin します。</span><span class="sxs-lookup"><span data-stu-id="da742-118">You'll get a token to use on https://microsoft.com/devicelogin.</span></span> <span data-ttu-id="da742-119">お使いのブラウザーでこのページを開いてトークンを入力し、Azure アカウントの資格情報でサインインし、Azure PowerShell を承認します。</span><span class="sxs-lookup"><span data-stu-id="da742-119">Open this page in your browser and enter the token, then sign in with your Azure account credentials and authorize Azure PowerShell.</span></span> 

<span data-ttu-id="da742-120">サインインすると、どの Azure サブスクリプションがアクティブになっているかを示す情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="da742-120">After signing in, you'll see information indicating which of your Azure subscriptions is active.</span></span> <span data-ttu-id="da742-121">アカウントに複数の Azure サブスクリプションがあり、別のサブスクリプションを選択する場合は、使用可能なサブスクリプションを [Get-AzSubscription](/powershell/module/az.accounts/get-azsubscription) コマンドレットで取得し、サブスクリプション ID を指定して [Set-AzContext](/powershell/module/az.accounts/set-azcontext) コマンドレットを実行します。</span><span class="sxs-lookup"><span data-stu-id="da742-121">If you have multiple Azure subscriptions in your account and want to select a different one, get your available subscriptions with [Get-AzSubscription](/powershell/module/az.accounts/get-azsubscription) and use the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet with your subscription ID.</span></span>
<span data-ttu-id="da742-122">Azure PowerShell による Azure サブスクリプションの管理の詳細については、「[複数の Azure サブスクリプションの使用](manage-subscriptions-azureps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da742-122">For more information about managing your Azure subscriptions in Azure PowerShell, see [Use multiple Azure subscriptions](manage-subscriptions-azureps.md).</span></span>

<span data-ttu-id="da742-123">サインインしたら、Azure PowerShell コマンドレットを使ってサブスクリプションのリソースにアクセスし、管理できます。</span><span class="sxs-lookup"><span data-stu-id="da742-123">Once signed in, use the Azure PowerShell cmdlets to access and manage resources in your subscription.</span></span> <span data-ttu-id="da742-124">サインイン プロセスと、認証方法の詳細については、「[Sign in with Azure PowerShell (Azure PowerShell を使用してサインインする)](authenticate-azureps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da742-124">To learn more about the sign-in process and authentication methods, see [Sign in with Azure PowerShell](authenticate-azureps.md).</span></span>

## <a name="find-commands"></a><span data-ttu-id="da742-125">コマンドを見つける</span><span class="sxs-lookup"><span data-stu-id="da742-125">Find commands</span></span>

<span data-ttu-id="da742-126">Azure PowerShell コマンドレットは、PowerShell の標準的な名前付け規則 (`VERB-NOUN`) に従っています。</span><span class="sxs-lookup"><span data-stu-id="da742-126">Azure PowerShell cmdlets follow a standard naming convention for PowerShell, `VERB-NOUN`.</span></span> <span data-ttu-id="da742-127">動詞はアクションを説明し (例: `Create`、`Get`、`Set`、`Delete`)、名詞はリソースの種類を説明します (例: `AzVM`、`AzKeyVaultCertificate`、`AzFirewall`、`AzVirtualNetworkGateway`)。</span><span class="sxs-lookup"><span data-stu-id="da742-127">The verb describes the action (examples include `Create`, `Get`, `Set`, `Delete`) and the noun describes the resource type (examples include `AzVM`, `AzKeyVaultCertificate`, `AzFirewall`, `AzVirtualNetworkGateway`).</span></span> <span data-ttu-id="da742-128">Azure PowerShell では名詞は常にプレフィックス `Az` で始まります。</span><span class="sxs-lookup"><span data-stu-id="da742-128">Nouns in Azure PowerShell always start with the prefix `Az`.</span></span> <span data-ttu-id="da742-129">標準的な動詞の完全な一覧については、「[Approved verbs for PowerShell Command (PowerShell コマンドの承認された動詞)](/powershell/developer/cmdlet/approved-verbs-for-windows-powershell-commands)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da742-129">For the full list of standard verbs, see [Approved verbs for PowerShell Commands](/powershell/developer/cmdlet/approved-verbs-for-windows-powershell-commands).</span></span>

<span data-ttu-id="da742-130">使用できる名詞、動詞、および Azure PowerShell モジュールを知ることは、[Get-Command](/powershell/module/microsoft.powershell.core/get-command) コマンドレットを使ったコマンドの検索に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="da742-130">Knowing the nouns, verbs, and the Azure PowerShell modules available help you find commands with the [Get-Command](/powershell/module/microsoft.powershell.core/get-command) cmdlet.</span></span> <span data-ttu-id="da742-131">たとえば、動詞 `Get` を使用したすべての VM 関連のコマンドを見つけるには、以下を使用します。</span><span class="sxs-lookup"><span data-stu-id="da742-131">For example, to find all VM-related commands that use the `Get` verb:</span></span>

```powershell-interactive
Get-Command -Verb Get -Noun AzVM* -Module Az.Compute
```

<span data-ttu-id="da742-132">一般的なコマンドを簡単に見つけられるように、この表にはリソースの種類、対応する Azure PowerShell モジュール、および `Get-Command` と共に使用する名詞プレフィックスが示されています。</span><span class="sxs-lookup"><span data-stu-id="da742-132">To help you find common commands, this table lists the resource type, corresponding Azure PowerShell module, and noun prefix to use with `Get-Command`:</span></span>

| <span data-ttu-id="da742-133">リソースの種類</span><span class="sxs-lookup"><span data-stu-id="da742-133">Resource type</span></span> | <span data-ttu-id="da742-134">Azure PowerShell モジュール</span><span class="sxs-lookup"><span data-stu-id="da742-134">Azure PowerShell module</span></span> | <span data-ttu-id="da742-135">名詞プレフィックス</span><span class="sxs-lookup"><span data-stu-id="da742-135">Noun prefix</span></span> |
|---------------|-------------------------|----------------|
| [<span data-ttu-id="da742-136">リソース グループ</span><span class="sxs-lookup"><span data-stu-id="da742-136">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="da742-137">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="da742-137">Az.Resources</span></span>](/powershell/module/az.resources#resources) | `AzResourceGroup` |
| [<span data-ttu-id="da742-138">仮想マシン</span><span class="sxs-lookup"><span data-stu-id="da742-138">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="da742-139">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="da742-139">Az.Compute</span></span>](/powershell/module/az.compute#virtual_machines) | `AzVM` |
| [<span data-ttu-id="da742-140">ストレージ アカウント</span><span class="sxs-lookup"><span data-stu-id="da742-140">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="da742-141">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="da742-141">Az.Storage</span></span>](/powershell/module/az.storage/) | `AzStorageAccount` |
| [<span data-ttu-id="da742-142">Key Vault</span><span class="sxs-lookup"><span data-stu-id="da742-142">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="da742-143">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="da742-143">Az.KeyVault</span></span>](/powershell/module/az.keyvault) | `AzKeyVault` |
| [<span data-ttu-id="da742-144">Web アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da742-144">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="da742-145">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="da742-145">Az.Websites</span></span>](/powershell/module/az.websites) | `AzWebApp` |
| [<span data-ttu-id="da742-146">SQL データベース</span><span class="sxs-lookup"><span data-stu-id="da742-146">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="da742-147">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="da742-147">Az.Sql</span></span>](/powershell/module/az.sql) | `AzSqlDatabase` |

<span data-ttu-id="da742-148">Azure PowerShell のモジュールの完全な一覧については、GitHub でホストされている [Azure PowerShell モジュールの一覧](https://github.com/Azure/azure-powershell/blob/master/documentation/azure-powershell-modules.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="da742-148">For a full list of the modules in Azure PowerShell, see the [Azure PowerShell modules list](https://github.com/Azure/azure-powershell/blob/master/documentation/azure-powershell-modules.md) hosted on GitHub.</span></span>

## <a name="learn-azure-powershell-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="da742-149">クイックスタートとチュートリアルを利用して Azure PowerShell の基本について学習する</span><span class="sxs-lookup"><span data-stu-id="da742-149">Learn Azure PowerShell basics with quickstarts and tutorials</span></span>

<span data-ttu-id="da742-150">Azure PowerShell の使用を開始するには、仮想マシンの設定方法、またはそれらにクエリを実行する方法を説明した詳細なチュートリアルをお試しください。</span><span class="sxs-lookup"><span data-stu-id="da742-150">To get started with Azure PowerShell, try an in-depth tutorial for setting up virtual machines and learning how to query them.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="da742-151">Azure PowerShell を使用した仮想マシンの作成</span><span class="sxs-lookup"><span data-stu-id="da742-151">Create virtual machines with Azure PowerShell</span></span>](azureps-vm-tutorial.yml)

<span data-ttu-id="da742-152">その他の一般的な Azure サービス用の Azure PowerShell クイックスタートもあります。</span><span class="sxs-lookup"><span data-stu-id="da742-152">There are also Azure PowerShell quickstarts for other popular Azure services:</span></span>

* [<span data-ttu-id="da742-153">ストレージ アカウントの作成</span><span class="sxs-lookup"><span data-stu-id="da742-153">Create a storage account</span></span>](/azure/storage/common/storage-quickstart-create-account?tabs=azure-powershell)
* [<span data-ttu-id="da742-154">Azure Blob Storage との間でのオブジェクトの転送に関するページ</span><span class="sxs-lookup"><span data-stu-id="da742-154">Transfer objects to/from Azure Blob storage</span></span>](/azure/storage/blobs/storage-quickstart-blobs-powershell)
* [<span data-ttu-id="da742-155">Azure Key Vault からのシークレットの作成と取得に関するページ</span><span class="sxs-lookup"><span data-stu-id="da742-155">Create and retrieve secrets from Azure Key Vault</span></span>](/azure/key-vault/quick-create-powershell)
* [<span data-ttu-id="da742-156">Azure SQL データベースとファイアウォールの作成に関するページ</span><span class="sxs-lookup"><span data-stu-id="da742-156">Create an Azure SQL database and firewall</span></span>](/azure/sql-database/scripts/sql-database-create-and-configure-database-powershell)
* [<span data-ttu-id="da742-157">Azure Container Instances でのコンテナーの実行に関するページ</span><span class="sxs-lookup"><span data-stu-id="da742-157">Run a container in Azure Container Instances</span></span>](/azure/container-instances/container-instances-quickstart-powershell)
* [<span data-ttu-id="da742-158">仮想マシン スケール セット (VMSS) の作成に関するページ</span><span class="sxs-lookup"><span data-stu-id="da742-158">Create a Virtual Machine Scale Set (VMSS)</span></span>](/azure/virtual-machine-scale-sets/quick-create-powershell)
* [<span data-ttu-id="da742-159">Standard ロード バランサ―の作成に関するページ</span><span class="sxs-lookup"><span data-stu-id="da742-159">Create a standard load balancer</span></span>](/azure/load-balancer/quickstart-create-standard-load-balancer-powershell)

## <a name="next-steps"></a><span data-ttu-id="da742-160">次の手順</span><span class="sxs-lookup"><span data-stu-id="da742-160">Next steps</span></span>

* [<span data-ttu-id="da742-161">Azure PowerShell を使用してサインインする</span><span class="sxs-lookup"><span data-stu-id="da742-161">Sign in with Azure PowerShell</span></span>](authenticate-azureps.md)
* [<span data-ttu-id="da742-162">Azure PowerShell による Azure サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="da742-162">Manage Azure subscriptions with Azure PowerShell</span></span>](manage-subscriptions-azureps.md)
* [<span data-ttu-id="da742-163">Azure PowerShell でサービス プリンシパルを作成する</span><span class="sxs-lookup"><span data-stu-id="da742-163">Create service principals with Azure PowerShell</span></span>](create-azure-service-principal-azureps.md)
* <span data-ttu-id="da742-164">コミュニティに質問する:</span><span class="sxs-lookup"><span data-stu-id="da742-164">Get help from the community:</span></span>
  * [<span data-ttu-id="da742-165">MSDN の Azure フォーラム</span><span class="sxs-lookup"><span data-stu-id="da742-165">Azure forum on MSDN</span></span>](http://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [<span data-ttu-id="da742-166">Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="da742-166">Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkId=320213)
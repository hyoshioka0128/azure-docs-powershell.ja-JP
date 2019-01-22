---
title: Azure PowerShell の使用に関するページ
description: ''
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: get-started-article
ms.date: 01/14/2019
ms.openlocfilehash: 483e74d7d047562b1c170c3767495161b9c5eb2f
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/16/2019
ms.locfileid: "54342001"
---
# <a name="get-started-with-azure-powershell"></a><span data-ttu-id="737ff-102">Azure PowerShell の使用に関するページ</span><span class="sxs-lookup"><span data-stu-id="737ff-102">Get started with Azure PowerShell</span></span>

<span data-ttu-id="737ff-103">Azure PowerShell は、コマンド ラインから Azure リソースを管理できるように設計されています。</span><span class="sxs-lookup"><span data-stu-id="737ff-103">Azure PowerShell is designed for managing and administering Azure resources from the command line.</span></span> <span data-ttu-id="737ff-104">Azure Resource Manager モデルを使用する自動化ツールをビルドする場合に Azure PowerShell を使用します。</span><span class="sxs-lookup"><span data-stu-id="737ff-104">Use Azure PowerShell when you want to build automated tools that use the Azure Resource Manager model.</span></span>
<span data-ttu-id="737ff-105">[Azure Cloud Shell](/azure/cloud-shell/overview) を使ってブラウザーで試してみるか、ローカル コンピューターにインストールします。</span><span class="sxs-lookup"><span data-stu-id="737ff-105">Try it out in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or install on your local machine.</span></span>

<span data-ttu-id="737ff-106">この記事では、Azure PowerShell の基本的な使い方と、主要な概念について説明します。</span><span class="sxs-lookup"><span data-stu-id="737ff-106">This article helps you get started with Azure PowerShell and teaches the core concepts behind it.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="737ff-107">Azure Cloud Shell でのインストールまたは実行</span><span class="sxs-lookup"><span data-stu-id="737ff-107">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="737ff-108">Azure PowerShell の使用を開始する最も簡単な方法として、Azure Cloud Shell 環境でこれを試してみます。</span><span class="sxs-lookup"><span data-stu-id="737ff-108">The easiest way to get started with Azure PowerShell is by trying it out in an Azure Cloud Shell environment.</span></span>
<span data-ttu-id="737ff-109">Cloud Shell を起動して実行する方法については、「[Azure Cloud Shell の PowerShell のクイックスタート](/azure/cloud-shell/quickstart-powershell)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="737ff-109">To get up and running with Cloud Shell, see [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
<span data-ttu-id="737ff-110">Cloud Shell では Linux コンテナー上で PowerShell 6 が実行されるため、Windows 固有の機能は利用できません。</span><span class="sxs-lookup"><span data-stu-id="737ff-110">Cloud Shell runs PowerShell 6 on a Linux container, so Windows-specific functionality isn't available.</span></span>

<span data-ttu-id="737ff-111">Azure PowerShell をローカル コンピューターにインストールする準備ができたら、「[Install the Azure PowerShell module (Azure PowerShell モジュールのインストール)](install-az-ps.md)」の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="737ff-111">When you're ready to install Azure PowerShell on your local machine, follow the instructions in [Install the Azure PowerShell module](install-az-ps.md).</span></span>

## <a name="sign-in-to-azure"></a><span data-ttu-id="737ff-112">Azure へのサインイン</span><span class="sxs-lookup"><span data-stu-id="737ff-112">Sign in to Azure</span></span>

<span data-ttu-id="737ff-113">`Connect-AzAccount` コマンドレットを使って対話形式でサインインします。</span><span class="sxs-lookup"><span data-stu-id="737ff-113">Sign in interactively with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="737ff-114">Cloud Shell を使用する場合は、次の手順をスキップします。Azure Cloud Shell セッションは、Cloud Shell セッションを起動した環境、サブスクリプション、およびテナント用に既に認証されています。</span><span class="sxs-lookup"><span data-stu-id="737ff-114">Skip this step if you use Cloud Shell: Your Auzre Cloud Shell session is already authenticated for the environment, subscription, and tenant that launched the Cloud Shell session.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="737ff-115">米国以外のリージョンの場合、`-Environment` パラメーターを使ってサインインします。</span><span class="sxs-lookup"><span data-stu-id="737ff-115">If you're in a non-US region, use the `-Environment` parameter to sign in.</span></span> <span data-ttu-id="737ff-116">[Get AzEnvironment](/powershell/module/Az.Accounts/Get-AzEnvironment) コマンドレットを使って、リージョンの環境の名前を取得します。</span><span class="sxs-lookup"><span data-stu-id="737ff-116">Get the name of the environment for your region by using the [Get-AzEnvironment](/powershell/module/Az.Accounts/Get-AzEnvironment) cmdlet.</span></span> <span data-ttu-id="737ff-117">たとえば、Azure China 21Vianet にサインインするには、以下を使用します。</span><span class="sxs-lookup"><span data-stu-id="737ff-117">For example, to sign in to Azure China 21Vianet:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="737ff-118">https://microsoft.com/devicelogin で使用するトークンを取得します。</span><span class="sxs-lookup"><span data-stu-id="737ff-118">You'll get a token to use on https://microsoft.com/devicelogin.</span></span> <span data-ttu-id="737ff-119">お使いのブラウザーでこのページを開いてトークンを入力し、Azure アカウントの資格情報でサインインし、Azure PowerShell を承認します。</span><span class="sxs-lookup"><span data-stu-id="737ff-119">Open this page in your browser and enter the token, then sign in with your Azure account credentials and authorize Azure PowerShell.</span></span> 

<span data-ttu-id="737ff-120">サインインしたら、Azure PowerShell コマンドレットを使ってサブスクリプションのリソースにアクセスし、管理できます。</span><span class="sxs-lookup"><span data-stu-id="737ff-120">Once signed in, use the Azure PowerShell cmdlets to access and manage resources in your subscription.</span></span> <span data-ttu-id="737ff-121">サインイン プロセスと、認証方法の詳細については、「[Sign in with Azure PowerShell (Azure PowerShell を使用してサインインする)](authenticate-azureps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="737ff-121">To learn more about the sign-in process and authentication methods, see [Sign in with Azure PowerShell](authenticate-azureps.md).</span></span>

## <a name="find-commands"></a><span data-ttu-id="737ff-122">コマンドを見つける</span><span class="sxs-lookup"><span data-stu-id="737ff-122">Find commands</span></span>

<span data-ttu-id="737ff-123">Azure PowerShell コマンドレットは、PowerShell の標準的な名前付け規則 (`VERB-NOUN`) に従っています。</span><span class="sxs-lookup"><span data-stu-id="737ff-123">Azure PowerShell cmdlets follow a standard naming convention for PowerShell, `VERB-NOUN`.</span></span> <span data-ttu-id="737ff-124">動詞はアクションを説明し (例: `Create`、`Get`、`Set`、`Delete`)、名詞はリソースの種類を説明します (例: `AzVM`、`AzKeyVaultCertificate`、`AzFirewall`、`AzVirtualNetworkGateway`)。</span><span class="sxs-lookup"><span data-stu-id="737ff-124">The verb describes the action (examples include `Create`, `Get`, `Set`, `Delete`) and the noun describes the resource type (examples include `AzVM`, `AzKeyVaultCertificate`, `AzFirewall`, `AzVirtualNetworkGateway`).</span></span> <span data-ttu-id="737ff-125">Azure PowerShell では名詞は常にプレフィックス `Az` で始まります。</span><span class="sxs-lookup"><span data-stu-id="737ff-125">Nouns in Azure PowerShell always start with the prefix `Az`.</span></span> <span data-ttu-id="737ff-126">標準的な動詞の完全な一覧については、「[Approved verbs for PowerShell Command (PowerShell コマンドの承認された動詞)](/powershell/developer/cmdlet/approved-verbs-for-windows-powershell-commands)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="737ff-126">For the full list of standard verbs, see [Approved verbs for PowerShell Commands](/powershell/developer/cmdlet/approved-verbs-for-windows-powershell-commands).</span></span>

<span data-ttu-id="737ff-127">使用できる名詞、動詞、および Azure PowerShell モジュールを知ることは、[Get-Command](/powershell/module/microsoft.powershell.core/get-command) コマンドレットを使ったコマンドの検索に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="737ff-127">Knowing the nouns, verbs, and the Azure PowerShell modules available help you find commands with the [Get-Command](/powershell/module/microsoft.powershell.core/get-command) cmdlet.</span></span> <span data-ttu-id="737ff-128">たとえば、動詞 `Get` を使用したすべての VM 関連のコマンドを見つけるには、以下を使用します。</span><span class="sxs-lookup"><span data-stu-id="737ff-128">For example, to find all VM-related commands that use the `Get` verb:</span></span>

```powershell-interactive
Get-Command -Verb Get -Noun AzVM* -Module Az.Compute
```

<span data-ttu-id="737ff-129">一般的なコマンドを簡単に見つけられるように、この表にはリソースの種類、対応する Azure PowerShell モジュール、および `Get-Command` と共に使用する名詞プレフィックスが示されています。</span><span class="sxs-lookup"><span data-stu-id="737ff-129">To help you find common commands, this table lists the resource type, corresponding Azure PowerShell module, and noun prefix to use with `Get-Command`:</span></span>

| <span data-ttu-id="737ff-130">リソースの種類</span><span class="sxs-lookup"><span data-stu-id="737ff-130">Resource type</span></span> | <span data-ttu-id="737ff-131">Azure PowerShell モジュール</span><span class="sxs-lookup"><span data-stu-id="737ff-131">Azure PowerShell module</span></span> | <span data-ttu-id="737ff-132">名詞プレフィックス</span><span class="sxs-lookup"><span data-stu-id="737ff-132">Noun prefix</span></span> |
|---------------|-------------------------|----------------|
| [<span data-ttu-id="737ff-133">リソース グループ</span><span class="sxs-lookup"><span data-stu-id="737ff-133">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="737ff-134">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="737ff-134">Az.Resources</span></span>](/powershell/module/az.resources#resources) | `AzResourceGroup` |
| [<span data-ttu-id="737ff-135">仮想マシン</span><span class="sxs-lookup"><span data-stu-id="737ff-135">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="737ff-136">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="737ff-136">Az.Compute</span></span>](/powershell/module/az.compute#virtual_machines) | `AzVM` |
| [<span data-ttu-id="737ff-137">ストレージ アカウント</span><span class="sxs-lookup"><span data-stu-id="737ff-137">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="737ff-138">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="737ff-138">Az.Storage</span></span>](/powershell/module/az.storage/) | `AzStorageAccount` |
| [<span data-ttu-id="737ff-139">Key Vault</span><span class="sxs-lookup"><span data-stu-id="737ff-139">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="737ff-140">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="737ff-140">Az.KeyVault</span></span>](/powershell/module/az.keyvault) | `AzKeyVault` |
| [<span data-ttu-id="737ff-141">Web アプリケーション</span><span class="sxs-lookup"><span data-stu-id="737ff-141">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="737ff-142">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="737ff-142">Az.Websites</span></span>](/powershell/module/az.websites) | `AzWebApp` |
| [<span data-ttu-id="737ff-143">SQL データベース</span><span class="sxs-lookup"><span data-stu-id="737ff-143">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="737ff-144">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="737ff-144">Az.Sql</span></span>](/powershell/module/az.sql) | `AzSqlDatabase` |

<span data-ttu-id="737ff-145">Azure PowerShell のモジュールの完全な一覧については、GitHub でホストされている [Azure PowerShell モジュールの一覧](https://github.com/Azure/azure-powershell/blob/master/documentation/azure-powershell-modules.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="737ff-145">For a full list of the modules in Azure PowerShell, see the [Azure PowerShell modules list](https://github.com/Azure/azure-powershell/blob/master/documentation/azure-powershell-modules.md) hosted on GitHub.</span></span>

## <a name="learn-azure-powershell-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="737ff-146">クイックスタートとチュートリアルを利用して Azure PowerShell の基本について学習する</span><span class="sxs-lookup"><span data-stu-id="737ff-146">Learn Azure PowerShell basics with quickstarts and tutorials</span></span>

<span data-ttu-id="737ff-147">Azure PowerShell の使用を開始するには、仮想マシンの設定方法、またはそれらにクエリを実行する方法を説明した詳細なチュートリアルをお試しください。</span><span class="sxs-lookup"><span data-stu-id="737ff-147">To get started with Azure PowerShell, try an in-depth tutorial for setting up virtual machines and learning how to query them.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="737ff-148">Azure PowerShell を使用した仮想マシンの作成</span><span class="sxs-lookup"><span data-stu-id="737ff-148">Create virtual machines with Azure PowerShell</span></span>](azureps-vm-tutorial.yml)

<span data-ttu-id="737ff-149">その他の一般的な Azure サービス用の Azure PowerShell クイックスタートもあります。</span><span class="sxs-lookup"><span data-stu-id="737ff-149">There are also Azure PowerShell quickstarts for other popular Azure services:</span></span>

* [<span data-ttu-id="737ff-150">ストレージ アカウントの作成</span><span class="sxs-lookup"><span data-stu-id="737ff-150">Create a storage account</span></span>](/azure/storage/common/storage-quickstart-create-account?tabs=azure-powershell)
* [<span data-ttu-id="737ff-151">Azure Blob Storage との間でのオブジェクトの転送に関するページ</span><span class="sxs-lookup"><span data-stu-id="737ff-151">Transfer objects to/from Azure Blob storage</span></span>](/azure/storage/blobs/storage-quickstart-blobs-powershell)
* [<span data-ttu-id="737ff-152">Azure Key Vault からのシークレットの作成と取得に関するページ</span><span class="sxs-lookup"><span data-stu-id="737ff-152">Create and retrieve secrets from Azure Key Vault</span></span>](/azure/key-vault/quick-create-powershell)
* [<span data-ttu-id="737ff-153">Azure SQL データベースとファイアウォールの作成に関するページ</span><span class="sxs-lookup"><span data-stu-id="737ff-153">Create an Azure SQL database and firewall</span></span>](/azure/sql-database/scripts/sql-database-create-and-configure-database-powershell)
* [<span data-ttu-id="737ff-154">Azure Container Instances でのコンテナーの実行に関するページ</span><span class="sxs-lookup"><span data-stu-id="737ff-154">Run a container in Azure Container Instances</span></span>](/azure/container-instances/container-instances-quickstart-powershell)
* [<span data-ttu-id="737ff-155">仮想マシン スケール セット (VMSS) の作成に関するページ</span><span class="sxs-lookup"><span data-stu-id="737ff-155">Create a Virtual Machine Scale Set (VMSS)</span></span>](/azure/virtual-machine-scale-sets/quick-create-powershell)
* [<span data-ttu-id="737ff-156">Standard ロード バランサ―の作成に関するページ</span><span class="sxs-lookup"><span data-stu-id="737ff-156">Create a standard load balancer</span></span>](/azure/load-balancer/quickstart-create-standard-load-balancer-powershell)

## <a name="next-steps"></a><span data-ttu-id="737ff-157">次の手順</span><span class="sxs-lookup"><span data-stu-id="737ff-157">Next steps</span></span>

* [<span data-ttu-id="737ff-158">Azure PowerShell を使用してサインインする</span><span class="sxs-lookup"><span data-stu-id="737ff-158">Sign in with Azure PowerShell</span></span>](authenticate-azureps.md)
* [<span data-ttu-id="737ff-159">Azure PowerShell による Azure サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="737ff-159">Manage Azure subscriptions with Azure PowerShell</span></span>](manage-subscriptions-azureps.md)
* [<span data-ttu-id="737ff-160">Azure PowerShell でサービス プリンシパルを作成する</span><span class="sxs-lookup"><span data-stu-id="737ff-160">Create service principals with Azure PowerShell</span></span>](create-azure-service-principal-azureps.md)
* <span data-ttu-id="737ff-161">コミュニティに質問する:</span><span class="sxs-lookup"><span data-stu-id="737ff-161">Get help from the community:</span></span>
  * [<span data-ttu-id="737ff-162">MSDN の Azure フォーラム</span><span class="sxs-lookup"><span data-stu-id="737ff-162">Azure forum on MSDN</span></span>](http://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [<span data-ttu-id="737ff-163">スタック オーバーフロー</span><span class="sxs-lookup"><span data-stu-id="737ff-163">Stacki Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkId=320213)

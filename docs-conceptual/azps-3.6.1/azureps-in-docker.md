---
title: Docker での Azure PowerShell の使用
description: Docker イメージにプレインストールされている Azure PowerShell の使用方法
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: a5746b71cfc41f7c6283b0e95b0940ca4b594ec7
ms.sourcegitcommit: fb95591c45bb5f12b98e0690938d18f2ec611897
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/15/2020
ms.locfileid: "79402682"
---
# <a name="using-azure-powershell-in-docker"></a><span data-ttu-id="8d59b-103">Docker での Azure PowerShell の使用</span><span class="sxs-lookup"><span data-stu-id="8d59b-103">Using Azure PowerShell in Docker</span></span>

<span data-ttu-id="8d59b-104">Azure PowerShell がプレインストールされた Docker イメージが公開されています。</span><span class="sxs-lookup"><span data-stu-id="8d59b-104">We are publishing Docker images with Azure PowerShell preinstalled.</span></span> <span data-ttu-id="8d59b-105">この記事では、Docker コンテナーで Azure PowerShell の使用を開始する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="8d59b-105">This article shows you how to get started using Azure PowerShell in the Docker container.</span></span>

## <a name="finding-available-images"></a><span data-ttu-id="8d59b-106">使用可能なイメージの検索</span><span class="sxs-lookup"><span data-stu-id="8d59b-106">Finding available images</span></span>

<span data-ttu-id="8d59b-107">リリースされたイメージには、Docker 17.05 以降が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d59b-107">The released images require Docker 17.05 or newer.</span></span> <span data-ttu-id="8d59b-108">また、`sudo` またはローカル管理者権限なしで Docker を実行できる必要もあります。</span><span class="sxs-lookup"><span data-stu-id="8d59b-108">It is also expected that you are able to run Docker without `sudo` or local administrative rights.</span></span> <span data-ttu-id="8d59b-109">`docker` を正しくインストールするには、Docker の公式な[手順][install]に従ってください。</span><span class="sxs-lookup"><span data-stu-id="8d59b-109">Please follow Docker's official [instructions][install] to install `docker` correctly.</span></span>

<span data-ttu-id="8d59b-110">リリースされたコンテナーは、公式の PowerShell コンテナーから構築され、Az モジュールがレイヤーとして追加されています。</span><span class="sxs-lookup"><span data-stu-id="8d59b-110">The released containers are built from the official PowerShell containers, then the Az module added as a layer.</span></span>

<span data-ttu-id="8d59b-111">最新の安定バージョンは以下のとおりです。</span><span class="sxs-lookup"><span data-stu-id="8d59b-111">The latest stable image includes:</span></span>

- <span data-ttu-id="8d59b-112">Ubuntu 18.04</span><span class="sxs-lookup"><span data-stu-id="8d59b-112">Ubuntu 18.04</span></span>
- <span data-ttu-id="8d59b-113">PowerShell バージョン 6.2.4</span><span class="sxs-lookup"><span data-stu-id="8d59b-113">PowerShell version 6.2.4</span></span>
- <span data-ttu-id="8d59b-114">Azure PowerShell の最新の Az モジュール</span><span class="sxs-lookup"><span data-stu-id="8d59b-114">Azure PowerShell most current Az module</span></span>

<span data-ttu-id="8d59b-115">使用可能なイメージの完全な一覧については、[Docker イメージ][az image]に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d59b-115">A full list of available images can be found on our [Docker image][az image] page.</span></span>

## <a name="using-azure-powershell-in-a-container"></a><span data-ttu-id="8d59b-116">コンテナーでの Azure PowerShell の使用</span><span class="sxs-lookup"><span data-stu-id="8d59b-116">Using Azure PowerShell in a container</span></span>

<span data-ttu-id="8d59b-117">次の手順は、イメージをダウンロードし、対話型 PowerShell セッションを開始するのに必要な Docker コマンドを示しています。</span><span class="sxs-lookup"><span data-stu-id="8d59b-117">The following steps show the Docker commands required to download the image and start an interactive PowerShell session.</span></span>

1. <span data-ttu-id="8d59b-118">最新の azure-powershell イメージをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="8d59b-118">Download the latest azure-powershell image.</span></span>

   ```console
   docker pull mcr.microsoft.com/azure-powershell
   ```

1. <span data-ttu-id="8d59b-119">対話モードで azure-powershell コンテナーを実行します。</span><span class="sxs-lookup"><span data-stu-id="8d59b-119">Run the azure-powershell container in interactive mode:</span></span>

   ```console
   docker run -it mcr.microsoft.com/azure-powershell pwsh
   ```

### <a name="run-the-azure-powershell-container-interactively-using-host-authentication"></a><span data-ttu-id="8d59b-120">ホスト認証を使用して対話形式で azure-powershell コンテナーを実行する</span><span class="sxs-lookup"><span data-stu-id="8d59b-120">Run the azure-powershell container interactively using host authentication</span></span>

<span data-ttu-id="8d59b-121">Docker をホストしているシステムに Azure PowerShell が既にインストールされている場合は、Azure 資格情報がキャッシュされている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="8d59b-121">If you have Azure PowerShell already installed on the system hosting Docker, you may have cached Azure credentials.</span></span> <span data-ttu-id="8d59b-122">これらの資格情報を、Docker コンテナー内で実行されている PowerShell セッションで使用できます。</span><span class="sxs-lookup"><span data-stu-id="8d59b-122">These credentials can be used in the PowerShell session running in the Docker container.</span></span>

<span data-ttu-id="8d59b-123">既定では、キャッシュされた資格情報はホスト上の `$HOME/.Azure` ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8d59b-123">By default, the cached credentials are in `$HOME/.Azure` directory on your host.</span></span> <span data-ttu-id="8d59b-124">Docker サービスが資格情報にアクセスするには、この場所へのアクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d59b-124">The Docker service must have access to this location to access the credentials.</span></span> <span data-ttu-id="8d59b-125">次のコマンドは、資格情報のキャッシュがマウントされた状態でコンテナーを起動し、対話形式の PowerShell セッションを開始します。</span><span class="sxs-lookup"><span data-stu-id="8d59b-125">The following command starts the container with the credential cache mounted and starts an interactive PowerShell session.</span></span>

```console
docker run -it -v ~/.Azure/AzureRmContext.json:/root/.Azure/AzureRmContext.json -v ~/.Azure/TokenCache.dat:/root/.Azure/TokenCache.dat mcr.microsoft.com/azure-powershell pwsh
```

### <a name="remove-the-image-when-no-longer-needed"></a><span data-ttu-id="8d59b-126">不要になったイメージを削除する</span><span class="sxs-lookup"><span data-stu-id="8d59b-126">Remove the image when no longer needed</span></span>

<span data-ttu-id="8d59b-127">次のコマンドは、不要になった Docker コンテナーを削除するときに使用します。</span><span class="sxs-lookup"><span data-stu-id="8d59b-127">The following command is used to delete the Docker container when you no longer need it.</span></span>

```console
docker rmi mcr.microsoft.com/azure-powershell
```

## <a name="next-steps"></a><span data-ttu-id="8d59b-128">次のステップ</span><span class="sxs-lookup"><span data-stu-id="8d59b-128">Next steps</span></span>

<span data-ttu-id="8d59b-129">Azure PowerShell のモジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8d59b-129">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span>

<!-- link references -->
[install]: https://docs.docker.com/engine/installation/
[powershell image]: https://hub.docker.com/_/microsoft-powershell
[az image]: https://hub.docker.com/_/microsoft-azure-powershell
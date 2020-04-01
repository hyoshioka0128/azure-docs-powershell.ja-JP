---
title: Docker での Azure PowerShell の使用
description: Docker イメージにプレインストールされている Azure PowerShell の使用方法
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/20/2020
ms.openlocfilehash: b5ad201abcabbdc1a88db241b028d88f05054a14
ms.sourcegitcommit: eeb720e053939a68873ae3973bc81d5826358c9f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/31/2020
ms.locfileid: "80440386"
---
# <a name="using-azure-powershell-in-docker"></a><span data-ttu-id="51a80-103">Docker での Azure PowerShell の使用</span><span class="sxs-lookup"><span data-stu-id="51a80-103">Using Azure PowerShell in Docker</span></span>

<span data-ttu-id="51a80-104">Azure PowerShell がプレインストールされた Docker イメージが公開されています。</span><span class="sxs-lookup"><span data-stu-id="51a80-104">We are publishing Docker images with Azure PowerShell preinstalled.</span></span> <span data-ttu-id="51a80-105">この記事では、Docker コンテナーで Azure PowerShell の使用を開始する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="51a80-105">This article shows you how to get started using Azure PowerShell in the Docker container.</span></span>

## <a name="finding-available-images"></a><span data-ttu-id="51a80-106">使用可能なイメージの検索</span><span class="sxs-lookup"><span data-stu-id="51a80-106">Finding available images</span></span>

<span data-ttu-id="51a80-107">リリースされたイメージには、Docker 17.05 以降が必要です。</span><span class="sxs-lookup"><span data-stu-id="51a80-107">The released images require Docker 17.05 or newer.</span></span> <span data-ttu-id="51a80-108">また、`sudo` またはローカル管理者権限なしで Docker を実行できる必要もあります。</span><span class="sxs-lookup"><span data-stu-id="51a80-108">It is also expected that you are able to run Docker without `sudo` or local administrative rights.</span></span> <span data-ttu-id="51a80-109">`docker` を正しくインストールするには、Docker の公式な[手順][install]に従ってください。</span><span class="sxs-lookup"><span data-stu-id="51a80-109">Please follow Docker's official [instructions][install] to install `docker` correctly.</span></span>

<span data-ttu-id="51a80-110">最新のコンテナー イメージには、最新バージョンの PowerShell と、Az モジュールでサポートされている最新の Azure PowerShell モジュールが含まれています。</span><span class="sxs-lookup"><span data-stu-id="51a80-110">The latest container image contains the latest version of PowerShell and the latest Azure PowerShell modules supported with the Az module.</span></span>

<span data-ttu-id="51a80-111">Az モジュールの新しいリリースごとに、次のオペレーティング システム用のイメージをリリースします。</span><span class="sxs-lookup"><span data-stu-id="51a80-111">For each new release of the Az module we are releasing an image for the following operating systems:</span></span>

- <span data-ttu-id="51a80-112">Ubuntu 18.04 (既定)</span><span class="sxs-lookup"><span data-stu-id="51a80-112">Ubuntu 18.04 (default)</span></span>
- <span data-ttu-id="51a80-113">Debian 9</span><span class="sxs-lookup"><span data-stu-id="51a80-113">Debian 9</span></span>
- <span data-ttu-id="51a80-114">CentOs 7</span><span class="sxs-lookup"><span data-stu-id="51a80-114">CentOs 7</span></span>

<span data-ttu-id="51a80-115">使用可能なイメージの完全な一覧については、[Docker イメージ][az image]に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="51a80-115">A full list of available images can be found on our [Docker image][az image] page.</span></span>

## <a name="using-azure-powershell-in-a-container"></a><span data-ttu-id="51a80-116">コンテナーでの Azure PowerShell の使用</span><span class="sxs-lookup"><span data-stu-id="51a80-116">Using Azure PowerShell in a container</span></span>

<span data-ttu-id="51a80-117">次の手順は、イメージをダウンロードし、対話型 PowerShell セッションを開始するのに必要な Docker コマンドを示しています。</span><span class="sxs-lookup"><span data-stu-id="51a80-117">The following steps show the Docker commands required to download the image and start an interactive PowerShell session.</span></span>

1. <span data-ttu-id="51a80-118">最新の azure-powershell イメージをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="51a80-118">Download the latest azure-powershell image.</span></span>

   ```console
   docker pull mcr.microsoft.com/azure-powershell
   ```

1. <span data-ttu-id="51a80-119">対話モードで azure-powershell コンテナーを実行します。</span><span class="sxs-lookup"><span data-stu-id="51a80-119">Run the azure-powershell container in interactive mode:</span></span>

   ```console
   docker run -it mcr.microsoft.com/azure-powershell pwsh
   ```

<span data-ttu-id="51a80-120">Windows Docker ホストの場合、Windows 上のローカル ドライブを Linux コンテナーと共有できるようにするには、Docker ファイル共有を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="51a80-120">For Windows Docker hosts, you must enable Docker File Sharing to allow local drives on Windows to be shared with Linux containers.</span></span> <span data-ttu-id="51a80-121">詳細については、「[Docker for Windows を使用する][file-sharing]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51a80-121">For more information see [Get started with Docker for Windows][file-sharing].</span></span>

### <a name="run-the-azure-powershell-container-interactively-using-host-authentication"></a><span data-ttu-id="51a80-122">ホスト認証を使用して対話形式で azure-powershell コンテナーを実行する</span><span class="sxs-lookup"><span data-stu-id="51a80-122">Run the azure-powershell container interactively using host authentication</span></span>

<span data-ttu-id="51a80-123">Docker をホストしているシステムに Azure PowerShell が既にインストールされている場合は、Azure 資格情報がキャッシュされている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="51a80-123">If you have Azure PowerShell already installed on the system hosting Docker, you may have cached Azure credentials.</span></span> <span data-ttu-id="51a80-124">これらの資格情報を、Docker コンテナー内で実行されている PowerShell セッションで使用できます。</span><span class="sxs-lookup"><span data-stu-id="51a80-124">These credentials can be used in the PowerShell session running in the Docker container.</span></span>

<span data-ttu-id="51a80-125">既定では、キャッシュされた資格情報はホスト上の `$HOME/.Azure` ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="51a80-125">By default, the cached credentials are in `$HOME/.Azure` directory on your host.</span></span> <span data-ttu-id="51a80-126">Docker サービスが資格情報にアクセスするには、この場所へのアクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="51a80-126">The Docker service must have access to this location to access the credentials.</span></span> <span data-ttu-id="51a80-127">次のコマンドは、資格情報のキャッシュがマウントされた状態でコンテナーを起動し、対話形式の PowerShell セッションを開始します。</span><span class="sxs-lookup"><span data-stu-id="51a80-127">The following command starts the container with the credential cache mounted and starts an interactive PowerShell session.</span></span>

```console
docker run -it -v ~/.Azure/AzureRmContext.json:/root/.Azure/AzureRmContext.json -v ~/.Azure/TokenCache.dat:/root/.Azure/TokenCache.dat mcr.microsoft.com/azure-powershell pwsh
```

### <a name="remove-the-image-when-no-longer-needed"></a><span data-ttu-id="51a80-128">不要になったイメージを削除する</span><span class="sxs-lookup"><span data-stu-id="51a80-128">Remove the image when no longer needed</span></span>

<span data-ttu-id="51a80-129">次のコマンドは、不要になった Docker コンテナーを削除するときに使用します。</span><span class="sxs-lookup"><span data-stu-id="51a80-129">The following command is used to delete the Docker container when you no longer need it.</span></span>

```console
docker rmi mcr.microsoft.com/azure-powershell
```

## <a name="next-steps"></a><span data-ttu-id="51a80-130">次のステップ</span><span class="sxs-lookup"><span data-stu-id="51a80-130">Next steps</span></span>

<span data-ttu-id="51a80-131">Azure PowerShell のモジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="51a80-131">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span>

<!-- link references -->
[install]: https://docs.docker.com/engine/installation/
[powershell image]: https://hub.docker.com/_/microsoft-powershell
[az image]: https://hub.docker.com/_/microsoft-azure-powershell
[file-sharing]: https://docs.docker.com/docker-for-windows/#file-sharing

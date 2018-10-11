---
title: Docker コンテナー内での Azure PowerShell の実行
description: Docker コンテナー内で Azure PowerShell を実行する方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/09/2018
ms.openlocfilehash: 0ed8f50abbcb2aa00192196f19004446dc696b5d
ms.sourcegitcommit: a749eb729f583c9d0dd86141bbd04984d77ae9ab
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/11/2018
ms.locfileid: "48882163"
---
# <a name="run-azure-powershell-in-a-docker-container"></a><span data-ttu-id="dcb33-103">Docker コンテナー内での Azure PowerShell の実行</span><span class="sxs-lookup"><span data-stu-id="dcb33-103">Run Azure PowerShell in a Docker container</span></span>

<span data-ttu-id="dcb33-104">Microsoft では、Azure PowerShell が事前インストールされた Docker イメージを公開しています。</span><span class="sxs-lookup"><span data-stu-id="dcb33-104">Microsoft publishes Docker images with Azure PowerShell pre-installed.</span></span> <span data-ttu-id="dcb33-105">これらのイメージにより、Azure PowerShell を試験的に利用するか、分離環境で Azure PowerShell を実行することができます。</span><span class="sxs-lookup"><span data-stu-id="dcb33-105">These images allow for experimenting with Azure PowerShell or running it in an isolated environment.</span></span> <span data-ttu-id="dcb33-106">PowerShell Core と PowerShell 5 の両方が実行されているイメージがあります。</span><span class="sxs-lookup"><span data-stu-id="dcb33-106">There are images running both PowerShell Core and PowerShell 5.</span></span> 

| <span data-ttu-id="dcb33-107">環境</span><span class="sxs-lookup"><span data-stu-id="dcb33-107">Environment</span></span> | <span data-ttu-id="dcb33-108">Docker イメージ</span><span class="sxs-lookup"><span data-stu-id="dcb33-108">Docker image</span></span> |
|-------------|--------------|
| <span data-ttu-id="dcb33-109">Windows 上の PowerShell</span><span class="sxs-lookup"><span data-stu-id="dcb33-109">PowerShell on Windows</span></span> | [<span data-ttu-id="dcb33-110">azuresdk/azure-powershell</span><span class="sxs-lookup"><span data-stu-id="dcb33-110">azuresdk/azure-powershell</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| <span data-ttu-id="dcb33-111">Windows 上の PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="dcb33-111">PowerShell Core on Windows</span></span> | [<span data-ttu-id="dcb33-112">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="dcb33-112">azuresdk/azure-powershell-core:nanoserver</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| <span data-ttu-id="dcb33-113">Linux 上の PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="dcb33-113">PowerShell Core on Linux</span></span> | [<span data-ttu-id="dcb33-114">azuresdk/azure-powershell-core:latest</span><span class="sxs-lookup"><span data-stu-id="dcb33-114">azuresdk/azure-powershell-core:latest</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

<span data-ttu-id="dcb33-115">これらのコンテナーのいずれかを実行するには、`docker run -it $ImageName` を使用して、対話型ターミナルを取得します。</span><span class="sxs-lookup"><span data-stu-id="dcb33-115">To run any of these containers, use `docker run -it $ImageName` to get an interactive terminal.</span></span> <span data-ttu-id="dcb33-116">たとえば、PowerShell Core で Linux コンテナーを実行するには、次を使用します。</span><span class="sxs-lookup"><span data-stu-id="dcb33-116">For example, to run a Linux container with PowerShell Core:</span></span>

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> <span data-ttu-id="dcb33-117">Docker で Windows コンテナーを実行するには、お使いのホスト OS が Windows でなければなりません。また、Windows コンテナーを実行するように Docker が設定されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dcb33-117">To run a Windows container in Docker, your host OS must be Windows and Docker must be set to run Windows containers.</span></span> <span data-ttu-id="dcb33-118">Docker での Windows 環境と Linux 環境の切り替えについては、[Windows コンテナーと Linux コンテナーの切り替え](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers)に関する Docker のドキュメントをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="dcb33-118">To learn about switching between Windows and Linux environments in Docker, see the Docker documentation [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span></span>

## <a name="use-a-powershell-core-container"></a><span data-ttu-id="dcb33-119">PowerShell Core コンテナーを使用する</span><span class="sxs-lookup"><span data-stu-id="dcb33-119">Use a PowerShell Core container</span></span>

<span data-ttu-id="dcb33-120">PowerShell Core コンテナーには PowerShell Core v6 が付属し、`AzureRM.NetCore` モジュールがプレインストールされています。</span><span class="sxs-lookup"><span data-stu-id="dcb33-120">The PowerShell Core containers come with PowerShell Core v6 and the `AzureRM.NetCore` module pre-installed.</span></span> <span data-ttu-id="dcb33-121">[Import-Module](/powershell/module/microsoft.powershell.core/import-module) コマンドレットを実行し、Azure アカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="dcb33-121">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM.NetCore
Connect-AzureRmAccount
```

## <a name="use-the-windows-container-with-powershell"></a><span data-ttu-id="dcb33-122">PowerShell で Windows コンテナーを使用する</span><span class="sxs-lookup"><span data-stu-id="dcb33-122">Use the Windows container with PowerShell</span></span>

<span data-ttu-id="dcb33-123">Windows コンテナーには、`AzureRM` モジュールがプレインストールされています。</span><span class="sxs-lookup"><span data-stu-id="dcb33-123">The Windows container has the `AzureRM` module pre-installed.</span></span> <span data-ttu-id="dcb33-124">[Import-Module](/powershell/module/microsoft.powershell.core/import-module) コマンドレットを実行し、Azure アカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="dcb33-124">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM
Connect-AzureRmAccount
```

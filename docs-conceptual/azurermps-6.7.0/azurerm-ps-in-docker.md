---
title: Docker コンテナー内での Azure PowerShell の実行
description: Docker コンテナー内で Azure PowerShell を実行する方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: 27ac176d8bd0b142b7740b2ba6793edb500a8af3
ms.sourcegitcommit: 7df99dc139e93a8a4e6d5b1a27968857588d75dd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/16/2018
ms.locfileid: "40106553"
---
# <a name="run-azure-powershell-in-a-docker-container"></a><span data-ttu-id="4f716-103">Docker コンテナー内での Azure PowerShell の実行</span><span class="sxs-lookup"><span data-stu-id="4f716-103">Run Azure PowerShell in a Docker container</span></span>

<span data-ttu-id="4f716-104">ポータブル環境で Azure PowerShell を実行しやすくするために、Microsoft では、Azure PowerShell が事前インストールされた Docker イメージを公開しています。</span><span class="sxs-lookup"><span data-stu-id="4f716-104">To make running Azure PowerShell in portable environments easy, Microsoft publishes Docker images with Azure PowerShell pre-installed.</span></span> <span data-ttu-id="4f716-105">これらのイメージにより、PowerShell Core が実行されている Linux ゲスト、または PowerShell Core か PowerShell 5 のいずれかを含む Windows ゲストが提供されます。</span><span class="sxs-lookup"><span data-stu-id="4f716-105">These images offer a Linux guest running PowerShell Core, or a Windows guest with either PowerShell Core or PowerShell 5.</span></span>

| <span data-ttu-id="4f716-106">環境</span><span class="sxs-lookup"><span data-stu-id="4f716-106">Environment</span></span> | <span data-ttu-id="4f716-107">Docker イメージ</span><span class="sxs-lookup"><span data-stu-id="4f716-107">Docker image</span></span> |
|-------------|--------------|
| <span data-ttu-id="4f716-108">Windows 上の PowerShell</span><span class="sxs-lookup"><span data-stu-id="4f716-108">PowerShell on Windows</span></span> | [<span data-ttu-id="4f716-109">azuresdk/azure-powershell</span><span class="sxs-lookup"><span data-stu-id="4f716-109">azuresdk/azure-powershell</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| <span data-ttu-id="4f716-110">Windows 上の PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="4f716-110">PowerShell Core on Windows</span></span> | [<span data-ttu-id="4f716-111">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="4f716-111">azuresdk/azure-powershell-core:nanoserver</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| <span data-ttu-id="4f716-112">Linux 上の PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="4f716-112">PowerShell Core on Linux</span></span> | [<span data-ttu-id="4f716-113">azuresdk/azure-powershell-core:latest</span><span class="sxs-lookup"><span data-stu-id="4f716-113">azuresdk/azure-powershell-core:latest</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

<span data-ttu-id="4f716-114">これらのコンテナーのいずれかを実行するには、`docker run -it $ImageName` を使用して、対話型ターミナルを取得します。</span><span class="sxs-lookup"><span data-stu-id="4f716-114">To run any of these containers, you use `docker run -it $ImageName` to get an interactive terminal.</span></span> <span data-ttu-id="4f716-115">たとえば、Linux コンテナー上で PowerShell Core を実行するには、次を使用します。</span><span class="sxs-lookup"><span data-stu-id="4f716-115">For example, to run the PowerShell Core on Linux container, use:</span></span>

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> <span data-ttu-id="4f716-116">Docker で Windows コンテナーを実行するには、お使いのホスト OS が Windows でなければなりません。また、Windows コンテナーを実行するように Docker が設定されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4f716-116">To run a Windows container in Docker, your host OS must be Windows and Docker must be set to run Windows containers.</span></span> <span data-ttu-id="4f716-117">Docker での Windows 環境と Linux 環境の切り替えについては、[Windows コンテナーと Linux コンテナーの切り替え](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers)に関する Docker のドキュメントをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4f716-117">To learn about switching between Windows and Linux environments in Docker, see the Docker documentation [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span></span>

## <a name="use-a-powershell-core-container"></a><span data-ttu-id="4f716-118">PowerShell Core コンテナーを使用する</span><span class="sxs-lookup"><span data-stu-id="4f716-118">Use a PowerShell Core container</span></span>

<span data-ttu-id="4f716-119">PowerShell Core コンテナーには PowerShell Core v6 が付属し、`AzureRM.NetCore` モジュールがプレインストールされています。</span><span class="sxs-lookup"><span data-stu-id="4f716-119">The PowerShell Core containers come with PowerShell Core v6 and the `AzureRM.NetCore` module pre-installed.</span></span> <span data-ttu-id="4f716-120">[Import-Module](/powershell/module/microsoft.powershell.core/import-module) コマンドレットを実行し、Azure アカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="4f716-120">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM.NetCore
Connect-AzureRmAccount
```

## <a name="use-the-windows-container-with-powershell"></a><span data-ttu-id="4f716-121">PowerShell で Windows コンテナーを使用する</span><span class="sxs-lookup"><span data-stu-id="4f716-121">Use the Windows container with PowerShell</span></span>

<span data-ttu-id="4f716-122">Windows コンテナーには、`AzureRM` モジュールがプレインストールされています。</span><span class="sxs-lookup"><span data-stu-id="4f716-122">The Windows container has the `AzureRM` module pre-installed.</span></span> <span data-ttu-id="4f716-123">[Import-Module](/powershell/module/microsoft.powershell.core/import-module) コマンドレットを実行し、Azure アカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="4f716-123">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM
Connect-AzureRmAccount
```

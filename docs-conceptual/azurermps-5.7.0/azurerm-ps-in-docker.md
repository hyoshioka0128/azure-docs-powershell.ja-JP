---
title: Docker コンテナー内での Azure PowerShell の実行
description: Docker コンテナー内で Azure PowerShell を実行する方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: 656c58fbb7cafb539736a0083d6aed1f46b7b98d
ms.sourcegitcommit: cb1fd248920d7efca67bd6c738a3b47206df7890
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/13/2018
ms.locfileid: "39024615"
---
# <a name="run-azure-powershell-in-a-docker-container"></a><span data-ttu-id="74c4e-103">Docker コンテナー内での Azure PowerShell の実行</span><span class="sxs-lookup"><span data-stu-id="74c4e-103">Run Azure PowerShell in a Docker container</span></span>

<span data-ttu-id="74c4e-104">Azure PowerShell で事前構成されている一連の Docker イメージがあります。</span><span class="sxs-lookup"><span data-stu-id="74c4e-104">There are a set of Docker images preconfigured with Azure PowerShell.</span></span> <span data-ttu-id="74c4e-105">使用できるコンテナーは 2 種類あります。Windows 上で従来の PowerShell を実行しているコンテナーと、Windows または Linux 上で PowerShell Core を実行しているコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="74c4e-105">Two types of containers are available: Those running traditional PowerShell on Windows, and a container running PowerShell Core on either Windows or Linux.</span></span>

| <span data-ttu-id="74c4e-106">環境</span><span class="sxs-lookup"><span data-stu-id="74c4e-106">Environment</span></span> | <span data-ttu-id="74c4e-107">Docker イメージ</span><span class="sxs-lookup"><span data-stu-id="74c4e-107">Docker image</span></span> |
|-------------|--------------|
| <span data-ttu-id="74c4e-108">Windows 上の PowerShell</span><span class="sxs-lookup"><span data-stu-id="74c4e-108">PowerShell on Windows</span></span> | [<span data-ttu-id="74c4e-109">azuresdk/azure-powershell</span><span class="sxs-lookup"><span data-stu-id="74c4e-109">azuresdk/azure-powershell</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| <span data-ttu-id="74c4e-110">Windows 上の PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="74c4e-110">PowerShell Core on Windows</span></span> | [<span data-ttu-id="74c4e-111">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="74c4e-111">azuresdk/azure-powershell-core:nanoserver</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| <span data-ttu-id="74c4e-112">Linux 上の PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="74c4e-112">PowerShell Core on Linux</span></span> | [<span data-ttu-id="74c4e-113">azuresdk/azure-powershell-core:latest</span><span class="sxs-lookup"><span data-stu-id="74c4e-113">azuresdk/azure-powershell-core:latest</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

<span data-ttu-id="74c4e-114">これらのコンテナーのいずれかを実行するには、`docker run -it $ImageName` を使用して、対話型ターミナルを取得します。</span><span class="sxs-lookup"><span data-stu-id="74c4e-114">To run any of these containers, you use `docker run -it $ImageName` to get an interactive terminal.</span></span> <span data-ttu-id="74c4e-115">たとえば、Linux コンテナー上で PowerShell Core を実行するには、次を使用します。</span><span class="sxs-lookup"><span data-stu-id="74c4e-115">For example, to run the PowerShell Core on Linux container, use:</span></span>

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> <span data-ttu-id="74c4e-116">Docker で Windows コンテナーを実行するには、お使いのホスト OS が Windows でなければなりません。また、Windows コンテナーを実行するように Docker が設定されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="74c4e-116">To run a Windows container in Docker, your host OS must be Windows and Docker must be set to run Windows containers.</span></span> <span data-ttu-id="74c4e-117">Docker での Windows 環境と Linux 環境の切り替えについては、[Windows コンテナーと Linux コンテナーの切り替え](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers)に関する Docker のドキュメントをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="74c4e-117">To learn about switching between Windows and Linux environments in Docker, see the Docker documentation [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span></span>

## <a name="use-a-powershell-core-container"></a><span data-ttu-id="74c4e-118">PowerShell Core コンテナーを使用する</span><span class="sxs-lookup"><span data-stu-id="74c4e-118">Use a PowerShell Core container</span></span>

<span data-ttu-id="74c4e-119">PowerShell Core コンテナーには PowerShell Core v6 が付属し、`AzureRM.NetCore` モジュールがプレインストールされています。</span><span class="sxs-lookup"><span data-stu-id="74c4e-119">The PowerShell Core containers come with PowerShell Core v6 and the `AzureRM.NetCore` module pre-installed.</span></span> <span data-ttu-id="74c4e-120">[Import-Module](/powershell/module/microsoft.powershell.core/import-module) コマンドレットを実行し、Azure アカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="74c4e-120">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM.NetCore
Connect-AzureRmAccount
```

## <a name="use-the-windows-container-with-powershell"></a><span data-ttu-id="74c4e-121">PowerShell で Windows コンテナーを使用する</span><span class="sxs-lookup"><span data-stu-id="74c4e-121">Use the Windows container with PowerShell</span></span>

<span data-ttu-id="74c4e-122">Windows コンテナーには、`AzureRM` モジュールがプレインストールされています。</span><span class="sxs-lookup"><span data-stu-id="74c4e-122">The Windows container has the `AzureRM` module pre-installed.</span></span> <span data-ttu-id="74c4e-123">[Import-Module](/powershell/module/microsoft.powershell.core/import-module) コマンドレットを実行し、Azure アカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="74c4e-123">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM
Connect-AzureRmAccount
```
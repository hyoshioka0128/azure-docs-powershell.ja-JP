---
title: Docker での Azure PowerShell の使用
description: Docker イメージにプレインストールされている Azure PowerShell の使用方法
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/20/2020
ms.openlocfilehash: b5ad201abcabbdc1a88db241b028d88f05054a14
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/05/2020
ms.locfileid: "81445817"
---
# <a name="using-azure-powershell-in-docker"></a>Docker での Azure PowerShell の使用

Azure PowerShell がプレインストールされた Docker イメージが公開されています。 この記事では、Docker コンテナーで Azure PowerShell の使用を開始する方法を説明します。

## <a name="finding-available-images"></a>使用可能なイメージの検索

リリースされたイメージには、Docker 17.05 以降が必要です。 また、`sudo` またはローカル管理者権限なしで Docker を実行できる必要もあります。 [ を正しくインストールするには、Docker の公式な][install]手順`docker`に従ってください。

最新のコンテナー イメージには、最新バージョンの PowerShell と、Az モジュールでサポートされている最新の Azure PowerShell モジュールが含まれています。

Az モジュールの新しいリリースごとに、次のオペレーティング システム用のイメージをリリースします。

- Ubuntu 18.04 (既定)
- Debian 9
- CentOs 7

使用可能なイメージの完全な一覧については、[Docker イメージ][az image]に関するページを参照してください。

## <a name="using-azure-powershell-in-a-container"></a>コンテナーでの Azure PowerShell の使用

次の手順は、イメージをダウンロードし、対話型 PowerShell セッションを開始するのに必要な Docker コマンドを示しています。

1. 最新の azure-powershell イメージをダウンロードします。

   ```console
   docker pull mcr.microsoft.com/azure-powershell
   ```

1. 対話モードで azure-powershell コンテナーを実行します。

   ```console
   docker run -it mcr.microsoft.com/azure-powershell pwsh
   ```

Windows Docker ホストの場合、Windows 上のローカル ドライブを Linux コンテナーと共有できるようにするには、Docker ファイル共有を有効にする必要があります。 詳細については、「[Docker for Windows を使用する][file-sharing]」を参照してください。

### <a name="run-the-azure-powershell-container-interactively-using-host-authentication"></a>ホスト認証を使用して対話形式で azure-powershell コンテナーを実行する

Docker をホストしているシステムに Azure PowerShell が既にインストールされている場合は、Azure 資格情報がキャッシュされている可能性があります。 これらの資格情報を、Docker コンテナー内で実行されている PowerShell セッションで使用できます。

既定では、キャッシュされた資格情報はホスト上の `$HOME/.Azure` ディレクトリにあります。 Docker サービスが資格情報にアクセスするには、この場所へのアクセス権が必要です。 次のコマンドは、資格情報のキャッシュがマウントされた状態でコンテナーを起動し、対話形式の PowerShell セッションを開始します。

```console
docker run -it -v ~/.Azure/AzureRmContext.json:/root/.Azure/AzureRmContext.json -v ~/.Azure/TokenCache.dat:/root/.Azure/TokenCache.dat mcr.microsoft.com/azure-powershell pwsh
```

### <a name="remove-the-image-when-no-longer-needed"></a>不要になったイメージを削除する

次のコマンドは、不要になった Docker コンテナーを削除するときに使用します。

```console
docker rmi mcr.microsoft.com/azure-powershell
```

## <a name="next-steps"></a>次のステップ

Azure PowerShell のモジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。

<!-- link references -->
[install]: https://docs.docker.com/engine/installation/
[powershell image]: https://hub.docker.com/_/microsoft-powershell
[az image]: https://hub.docker.com/_/microsoft-azure-powershell
[file-sharing]: https://docs.docker.com/docker-for-windows/#file-sharing

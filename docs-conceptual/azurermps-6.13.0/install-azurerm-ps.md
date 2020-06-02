---
title: PowerShellGet を使用した Windows への Azure PowerShell のインストール
description: PowerShellGet を使用して Azure PowerShell をインストールする方法
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/16/2018
ms.openlocfilehash: b04d4070e420f2d1e64f233eda6b3e250f8bb68c
ms.sourcegitcommit: 9f5c7d231b069ad501729bf015a829f3fe89bc6a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/28/2020
ms.locfileid: "84122031"
---
# <a name="install-azure-powershell-on-windows-with-powershellget"></a>PowerShellGet を使用した Windows への Azure PowerShell のインストール

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

この記事では、PowerShellGet を使用して、Windows 用 PowerShell 5.x の Azure PowerShell モジュールをインストールする手順について説明します。 Azure PowerShell をインストールするときは、PowerShellGet およびモジュール管理を使用することをお勧めしますが、Web Platform Installer または MSI パッケージを使ってインストールすることもできます。方法については、[その他のインストール方法](other-install.md)に関する記事をご覧ください。

このバージョンの Azure PowerShell では、Azure クラシック デプロイ モデルはサポートされていません。 クラシック デプロイのサポートについては、「[Azure PowerShell Service Management モジュールのインストール](/powershell/azure/servicemanagement/install-azure-ps)」の手順に従ってください。

> [!IMPORTANT]
> AzureRM モジュールは、macOS または Linux ではサポートされません。 これらのプラットフォームで Azure PowerShell コマンドレットを使用するには、[Az モジュールをインストール](/powershell/azure/install-az-ps)します。

## <a name="requirements"></a>必要条件

Azure PowerShell バージョン 6.0 以降、Azure PowerShell では PowerShell バージョン 5.0 が必要です。 お使いのマシンで実行されている PowerShell のバージョンを確認するには、次のコマンドを実行します。

```powershell-interactive
$PSVersionTable.PSVersion
```

バージョンが古い場合は、「[既存の Windows PowerShell をアップグレードする](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell)」をご覧ください。

> [!IMPORTANT]
> このドキュメントで説明するモジュール AzureRM では、.NET Framework を使用します。 そのため、.NET Core を使用する PowerShell 6.0 とは互換性がなくなります。 PowerShell 6.0 を使用している場合は、[macOS および Linux のインストール手順](install-azurermps-maclinux.md)に従います。

## <a name="install-the-azure-powershell-module"></a>Azure PowerShell モジュールのインストール

PowerShell ギャラリーからモジュールをインストールするには、昇格された特権が必要です。 Azure PowerShell をインストールするには、管理者特権のセッションで次のコマンドを実行します。

```azurepowershell-interactive
Install-Module -Name AzureRM -AllowClobber
```

> [!NOTE]
> ご利用の NuGet のバージョンが 2.8.5.201 未満である場合、最新バージョンの NuGet をダウンロードしてインストールするように求められます。

既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。 PSGallery の初回使用時には、次のプロンプトが表示されます。

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

インストールを続行するには、`Yes` または `Yes to All` を選択します。

`AzureRM` モジュールは、Azure PowerShell コマンドレットのロールアップ モジュールです。 これをインストールすると、利用可能な Azure Resource Manager モジュールがすべてダウンロードされ、コマンドレットを使用できるようになります。

## <a name="sign-in"></a>サインイン

Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。

```azurepowershell-interactive
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

> [!NOTE]
> モジュールの自動読み込みを無効にしている場合は、`Import-Module AzureRM` を使用してモジュールを手動でインポートする必要があります。 モジュールが構造化されているため、これには数秒かかることがあります。

新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。 Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。

## <a name="update-the-azure-powershell-module"></a>Azure PowerShell モジュールの更新

Azure PowerShell のインストールを更新するには、[Update-Module](/powershell/module/powershellget/update-module) を実行します。 このコマンドでは、以前のバージョンはアンインストール**されません**。

```powershell-interactive
Update-Module -Name AzureRM
```

古いバージョンの Azure PowerShell をシステムから削除する場合は、「[Uninstall the Azure PowerShell module (Azure PowerShell モジュールのアンインストール)](uninstall-azurerm-ps.md)」をご覧ください。

## <a name="use-multiple-versions-of-azure-powershell"></a>複数のバージョンの Azure PowerShell の使用

複数のバージョンの Azure PowerShell をインストールできます。 複数のバージョンの Azure PowerShell がインストールされているかどうかを確認するには、次のコマンドを使用します。

```azurepowershell-interactive
Get-InstalledModule -Name AzureRM -AllVersions | select Name,Version
```

Azure PowerShell のバージョンを削除するには、「[Azure PowerShell モジュールのアンインストール](uninstall-azurerm-ps.md)」を参照してください。

オンプレミスの Azure Stack リソースを使用する場合、古いバージョンの Windows を実行している場合、または Azure クラシック デプロイ モデルを使用している場合は、複数のバージョンが必要になります。 古いバージョンをインストールするには、インストール時に `-RequiredVersion` 引数を指定します。

```azurepowershell-interactive
# Install version 2.3.0 of Azure PowerShell
Install-Module -Name AzureRM -RequiredVersion 2.3.0
```

Azure PowerShell モジュールの読み込み時には、最新バージョンが既定で読み込まれます。 別のバージョンを読み込むには、`-RequiredVersion` 引数を指定します。

```azurepowershell-interactive
# Load version 2.3.0 of Azure PowerShell
Import-Module -Name AzureRM -RequiredVersion 2.3.0
```

## <a name="provide-feedback"></a>フィードバックの提供

Azure Powershell の使用時にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。 コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/azurerm.profile/send-feedback) コマンドレットを使用します。

## <a name="next-steps"></a>次の手順

Azure PowerShell を使い始める場合、モジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。

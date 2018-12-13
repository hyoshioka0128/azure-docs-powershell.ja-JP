---
title: PowerShellGet を使用して Azure PowerShell "Az" をインストールする
description: PowerShellGet を使用して、Windows、macOS、Linux に Azure PowerShell をインストールする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/26/2018
ms.openlocfilehash: 3d52b18750341f220dc8e10d6bf89796457c5a10
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/13/2018
ms.locfileid: "53216999"
---
# <a name="install-the-azure-powershell-az-module"></a>Azure PowerShell "Az" モジュールのインストール

この記事では、PowerShellGet を使用して Azure PowerShell モジュールをインストールする方法を説明します。 これらの手順は、Windows、macOS、および Linux プラットフォーム上で使用できます。 Az のプレビュー リリースでは、他のインストール方法はサポートされていません。 

## <a name="requirements"></a>必要条件

Azure PowerShell は、Windows 上の PowerShell 5.x、または任意のプラットフォーム上の PowerShell 6.x で動作します。 お使いのマシンで実行されている PowerShell のバージョンを確認するには、次のコマンドを実行します。

```powershell-interactive
$PSVersionTable.PSVersion
```

期限切れのバージョンをお使いの場合や PowerShell をインストールする必要がある場合は、「[PowerShell のさまざまなバージョンのインストール](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6)」を参照してください。 お使いのプラットフォームでのインストール情報については、そのページにリンクがあります。

## <a name="install-the-azure-powershell-module"></a>Azure PowerShell モジュールのインストール

> [!IMPORTANT]
>
> `AzureRM` と `Az` の両方のモジュールを同時にインストールすることができます。 両方のモジュールをインストールした場合は、__別名を有効にしない__でください。
> 別名を有効にすると、`AzureRM` コマンドレットと `Az` コマンドの別名との間に競合が発生して、予期しない動作が起こる可能性があります。
> `Az` モジュールをインストールする前に、`AzureRM` をアンインストールすることをお勧めします。 `AzureRM` のインストールや別名の有効化はいつでもできます。 アンインストールの手順については、[Azure PowerShell モジュール (AzureRM) のアンインストール](uninstall-azurerm-ps.md)に関するページを参照してください。 

グローバル スコープでモジュールをインストールするには、PowerShell ギャラリーからモジュールをインストールするための、昇格された特権が必要です。 Azure PowerShell をインストールするには、管理者特権セッション (Windows の場合は [管理者として実行]、macOS または Linux の場合はスーパーユーザー権限) で、次のコマンドを実行します。

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

管理者特権へのアクセス許可がない場合は、`-Scope` 引数を追加することで、現在のユーザーに対してインストールできます。

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。 PSGallery の初回使用時には、次のプロンプトが表示されます。

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

インストールを続行するには、`Yes` または `Yes to All` を選択します。

`Az` モジュールは、Azure PowerShell コマンドレットのロールアップ モジュールです。 これをインストールすると、利用可能な Azure Resource Manager モジュールがすべてダウンロードされ、コマンドレットを使用できるようになります。

## <a name="sign-in"></a>[サインイン]

Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> モジュールの自動読み込みを無効にしている場合は、`Import-Module Az` を使用してモジュールを手動でインポートする必要があります。 モジュールが構造化されているため、これには数秒かかることがあります。

新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。 Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。

## <a name="update-the-azure-powershell-module"></a>Azure PowerShell モジュールの更新

Azure PowerShell のインストールを更新するには、[Update-Module](/powershell/module/powershellget/update-module) を実行します。 このコマンドでは、以前のバージョンはアンインストール__されません__。

```powershell-interactive
Update-Module -Name Az
```

古いバージョンの Azure PowerShell をシステムから削除する場合は、「[Uninstall the Azure PowerShell module (Azure PowerShell モジュールのアンインストール)](uninstall-azurerm-ps.md)」をご覧ください。

## <a name="use-multiple-versions-of-azure-powershell"></a>複数のバージョンの Azure PowerShell の使用

複数のバージョンの Azure PowerShell をインストールできます。 複数のバージョンの Azure PowerShell がインストールされているかどうかを確認するには、次のコマンドを使用します。

```powershell-interactive
Get-Module -Name Az -List | select Name,Version
```

Azure PowerShell のバージョンを削除するには、「[Azure PowerShell モジュールのアンインストール](uninstall-azurerm-ps.md)」を参照してください。

特定のバージョンの `Az` モジュールを読み込むには、`Install-Module` および `Import-Module` で `-RequiredVersion` 引数を使用します。

```powershell-interactive
Install-Module -Name Az -RequiredVersion 0.4.0
Import-Module -Name Az -RequiredVersion 0.4.0
```

複数のバージョンのモジュールがインストールされている場合は、既定で最新バージョンが読み込まれます。

## <a name="provide-feedback"></a>フィードバックの提供

Azure Powershell の使用時にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。
コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/az.profile/send-feedback) コマンドレットを使用します。

## <a name="next-steps"></a>次の手順

Azure PowerShell を使い始める場合、モジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。

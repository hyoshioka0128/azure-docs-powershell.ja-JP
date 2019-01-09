---
title: Azure PowerShell の概要
description: Azure PowerShell Az モジュールの概要と、インストールして使い始める方法に関する情報。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 10/29/2018
ms.openlocfilehash: 7982e122d49db4d558648231d1ab8bfeed80be2d
ms.sourcegitcommit: 4acddc7026522c4fe39de2c4424917d88ee01b7e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/21/2018
ms.locfileid: "53736462"
---
# <a name="overview-of-azure-powershell"></a>Azure PowerShell の概要

Azure PowerShell には、Azure リソースの管理に [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) モデルを使う一連のコマンドレットが用意されています。 Azure PowerShell では .NET Standard が使用されているので、Windows、macOS、Linux で使用できます。
Azure PowerShell は、Azure Cloud Shell から利用することもできます。

Azure PowerShell は、[Azure Cloud Shell](/azure/cloud-shell/overview) を使用してブラウザーで実行するか、[ローカルにインストール](install-az-ps.md)します。 Azure PowerShell の基礎を学び、Azure を使い始めるには、[概要](get-started-azureps.md)に関する記事をご覧ください。

Azure PowerShell の最新リリースについては、[リリース ノート](release-notes-azureps.md)をご覧ください。

## <a name="about-the-new-az-module"></a>新しい Az モジュールについて

このドキュメントでは、Azure PowerShell の新しい Az モジュールについて説明します。 この新しいモジュールは、.NET Standard で一から作成されています。 .NET Standard の使用により、Azure PowerShell は Windows 上の PowerShell 5.x または任意のプラットフォーム上の PowerShell 6 で実行できます。 PowerShell を使用して Azure を操作するときに、Az モジュールが使用されるようになりました。
AzureRM はバグの修正プログラムを引き続き取得できますが、新機能は追加されなくなります。

コマンド名の変更や、AzureRM のメンテナンス プランなど、新しいモジュールの詳細については、[Azure PowerShell Az モジュールの概要](new-azureps-module-az.md)に関する記事をご覧ください。 新しいモジュールをすぐに使い始める場合は、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関する記事をご覧ください。

[AzureRM のドキュメント](/powershell/azure/azurerm)も利用できます。

> [!IMPORTANT]
>
> 新しいモジュールのコマンドレット名を反映するために、Azure のドキュメントを更新中ですが、記事で AzureRM コマンドが引き続き使用されている場合があります。 Az モジュールをインストールしたら、`Enable-AzureRmAlias` を使用して、AzureRM コマンドレットのエイリアスを有効にすることをお勧めします。 詳細については、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関する記事をご覧ください。

## <a name="common-scenarios"></a>一般的なシナリオ

Azure PowerShell の基本的な使い方については、次のサンプルが参考になります。

* [Linux virtual machines](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [Windows Virtual Machines](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [Web Apps](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [SQL Database](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="learn-powershell-basics"></a>PowerShell の基礎を学ぶ

PowerShell について初めて学ぶ場合は、概要に関するページからご覧ください。

* [PowerShell のインストール](/powershell/scripting/setup/installing-windows-powershell)
* [PowerShell を使用したスクリプト](/powershell/scripting/powershell-scripting)

次のビデオをご覧いただくこともできます。[PowerShell の基礎: (パート 1) PowerShell の概要](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1)。

または、Microsoft Virtual Academy の [PowerShell の概要](https://mva.microsoft.com/liveevents/powershell-jumpstart)に関するクラスにご参加ください。

## <a name="build-your-skills-with-microsoft-learn"></a>Microsoft Learn でスキルを身に付ける

- [PowerShell でスクリプトを使用した Azure タスクの自動化](/learn/modules/automate-azure-tasks-with-powershell/)
- [対話型学習の詳細...](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a>その他の Azure PowerShell モジュール

* [Azure Active Directory](/powershell/azure/active-directory/)
* [Azure Information Protection](/powershell/azure/aip/)
* [Azure Service Fabric](/powershell/azure/service-fabric/)
* [Azure ElasticDB](/powershell/azure/elasticdbjobs/)

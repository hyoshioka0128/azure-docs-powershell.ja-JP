---
title: Azure PowerShell Az モジュールの概要
description: AzureRM モジュールに代わる新しい Azure PowerShell Az モジュールの概要。
ms.date: 12/13/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 10665a72bc7dcae8ecf36b5ef4e2ab285a0e78b7
ms.sourcegitcommit: ae4540a90508db73335a54408dfd6cdf3712a1e9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/18/2019
ms.locfileid: "59364103"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a>新しい Azure PowerShell Az モジュールの概要

2018 年 12 月から、Azure PowerShell Az モジュールが一般公開リリースされました。このモジュールは、Azure の操作を目的とする PowerShell モジュールです。 Az で、コマンドの短縮、安定性の向上、およびクロスプラットフォームのサポートが実現します。 また、機能パリティと、AzureRM からの簡単な移行パスも提供されます。

Az では .NET Standard ライブラリが使用されます。つまり、PowerShell 5 と PowerShell 6 上で実行できます。
PowerShell 6 は Linux、macOS、および Windows 上で実行できるため、Azure PowerShell はすべてのプラットフォームで利用できるようになりました。
.NET Standard を使用すると Azure PowerShell のコード ベースを統合でき、ユーザーへの影響を最小限に抑えることができます。

Az は新しいモジュールであるため、バージョンが 1.0.0 にリセットされます。

## <a name="upgrade-to-az"></a>Az にアップグレードする

すべてのユーザーを新しい Az モジュールにアップグレードすることをお勧めします。 そのためには、次の手順を実行します。

* __推奨__:[Azure PowerShell AzureRM モジュールをアンインストールする](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)
* [Azure PowerShell Az モジュールをインストールする](/powershell/azure/install-az-ps)
* 新しいコマンド セットについて理解を深めながら、`Enable-AzureRMAlias` を使用して AzureRM コマンドレットのエイリアスを互換モードで追加できるようにします。 AzureRM がインストールされていない場合は、別名の有効化__のみ__を行います。

## <a name="migrate-existing-scripts-to-az"></a>Az に既存のスクリプトを移行する

主要な更新プログラムの適用には手間取る可能性があります。 ただし、Az モジュールには、新しい構文への更新に取り組みながら、既存のスクリプトを使用できるようにする互換モードがあります。 AzureRM 互換モードを有効にするには、`Enable-AzureRmAlias` コマンドレットを使用します。 このコマンドレットで、新しい Az コマンドレット名の別名として AzureRM コマンドレット名を定義できます。

新しいコマンドレット名は、覚えやすいように設計されています。 コマンドレット名では `AzureRm` や `Azure` を使用する代わりに、`Az` を使用します。 たとえば、古いコマンド `New-AzureRMVm` は `New-AzVm` になりました。

移行プロセスの詳細については、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。

## <a name="the-future-of-support-for-azurerm"></a>今後の AzureRM のサポート

既存の AzureRM モジュールは、新しいコマンドレットや機能を受け入れなくなります。 ただし、AzureRM は 2020 年 12 月まで引き続き正式に維持され、バグの修正プログラムを取得できます。 Azure の最新のサービスと機能に対応するには、Az モジュールに切り替えてください。

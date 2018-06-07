---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: c57ba563b5a4d4d19944fe8eca2cb4244ee5ed9e
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/06/2018
ms.locfileid: "34819713"
---
# <a name="release-notes"></a>リリース ノート

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

## <a name="version-129"></a>バージョン 1.2.9

このリリースの変更

* AzureRm.AzureStackAdmin モジュール
    + 管理者の Azure Resource Manager とテナントの Azure Resource Manager の分割に対応するために Add-AzureRmResourceProviderRegistration コマンドレットを変更しました。 新しいパラメーター (-ResourceManagerType) を追加しました。
    + 各コマンドレットから -AdminUri、-ApiVersion、-SubscriptionId、-Token の各パラメーターを削除しました。 これらのパラメーターが非推奨となる予定であると、かねてからお伝えしてきましたが、今回でそれらが削除されたことになります。
* AzureStackStorage モジュール
    + コンテナーの移行のシナリオに対応するために新しいコマンドレットを追加しました。
    + 内部コンポーネントと基になる機能を参照するコマンドレットを削除しました。
* AzureRM.BootStrapper
    + バージョン プロファイルを使って Azure PowerShell コマンドレットのバージョンを管理する新しいモジュールを作成しました。
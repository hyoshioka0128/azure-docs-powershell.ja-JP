---
title: Azure PowerShell による Azure サブスクリプションの管理
description: Azure PowerShell による Azure サブスクリプションの管理
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/30/2017
ms.openlocfilehash: e1606ddb02adf1de2cb5496917d61755ac3dad23
ms.sourcegitcommit: 971f19181b2cd68b7845bbebdb22858c06541c8c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/06/2018
ms.locfileid: "43384146"
---
# <a name="manage-multiple-azure-subscriptions"></a>複数の Azure サブスクリプションの管理

Azure を使い始めたばかりの場合、所有しているサブスクリプションは 1 つだけだと思われます。 一方、しばらく前から Azure を使用している場合は、複数の Azure サブスクリプションを作成済みであることも考えられます。 その場合は、特定のサブスクリプションに対してコマンドを実行するように Azure PowerShell を構成することができます。

1. アカウント内のすべてのサブスクリプションの一覧を取得します。

    ```azurepowershell-interactive
    Get-AzureRmSubscription
    ```

    ```output
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Production Subscription
    CurrentStorageAccount :

    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My DevTest Subscription
    CurrentStorageAccount :

    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

2. 既定のサブスクリプションを設定します。

    ```azurepowershell-interactive
    Select-AzureRmSubscription -Subscription "My Demos"
    ```

3. `Get-AzureRmContext` コマンドレットを実行して変更内容を確認します。

    ```azurepowershell-interactive
    Get-AzureRmContext
    ```

    ```output
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

既定のサブスクリプションを設定すると、後続のすべての Azure PowerShell コマンドは、このサブスクリプションに対して実行されます。

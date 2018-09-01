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
ms.sourcegitcommit: dca906e73e943aac207cee23b79915773419c673
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/30/2018
ms.locfileid: "43250356"
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="3e412-103">複数の Azure サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="3e412-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="3e412-104">Azure を使い始めたばかりの場合、所有しているサブスクリプションは 1 つだけだと思われます。</span><span class="sxs-lookup"><span data-stu-id="3e412-104">If you are brand new to Azure, you probably only have a single subscription.</span></span> <span data-ttu-id="3e412-105">一方、しばらく前から Azure を使用している場合は、複数の Azure サブスクリプションを作成済みであることも考えられます。</span><span class="sxs-lookup"><span data-stu-id="3e412-105">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span> <span data-ttu-id="3e412-106">その場合は、特定のサブスクリプションに対してコマンドを実行するように Azure PowerShell を構成することができます。</span><span class="sxs-lookup"><span data-stu-id="3e412-106">You can configure Azure PowerShell to execute commands against a particular subscription.</span></span>

1. <span data-ttu-id="3e412-107">アカウント内のすべてのサブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="3e412-107">Get a list of all subscriptions in your account.</span></span>

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

2. <span data-ttu-id="3e412-108">既定のサブスクリプションを設定します。</span><span class="sxs-lookup"><span data-stu-id="3e412-108">Set the default.</span></span>

    ```azurepowershell-interactive
    Select-AzureRmSubscription -Subscription "My Demos"
    ```

3. <span data-ttu-id="3e412-109">`Get-AzureRmContext` コマンドレットを実行して変更内容を確認します。</span><span class="sxs-lookup"><span data-stu-id="3e412-109">Verify the change by running the `Get-AzureRmContext` cmdlet.</span></span>

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

<span data-ttu-id="3e412-110">既定のサブスクリプションを設定すると、後続のすべての Azure PowerShell コマンドは、このサブスクリプションに対して実行されます。</span><span class="sxs-lookup"><span data-stu-id="3e412-110">Once you set your default subscription, all subsequent Azure PowerShell commands run against this subscription.</span></span>
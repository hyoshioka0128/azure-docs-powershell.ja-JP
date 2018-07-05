---
title: Azure PowerShell による Azure サブスクリプションの管理
description: Azure PowerShell による Azure サブスクリプションの管理
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/30/2017
ms.openlocfilehash: fbd2fe315efbdfb2147218229d51e983e2b61361
ms.sourcegitcommit: de0e60800df1add9f3400166faacca202ef567d9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/03/2018
ms.locfileid: "37406473"
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="d00e6-103">複数の Azure サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="d00e6-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="d00e6-104">Azure を使い始めたばかりの場合、所有しているサブスクリプションは 1 つだけだと思われます。</span><span class="sxs-lookup"><span data-stu-id="d00e6-104">If you are brand new to Azure, you probably only have a single subscription.</span></span> <span data-ttu-id="d00e6-105">一方、しばらく前から Azure を使用している場合は、複数の Azure サブスクリプションを作成済みであることも考えられます。</span><span class="sxs-lookup"><span data-stu-id="d00e6-105">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span> <span data-ttu-id="d00e6-106">その場合は、特定のサブスクリプションに対してコマンドを実行するように Azure PowerShell を構成することができます。</span><span class="sxs-lookup"><span data-stu-id="d00e6-106">You can configure Azure PowerShell to execute commands against a particular subscription.</span></span>

1. <span data-ttu-id="d00e6-107">アカウント内のすべてのサブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="d00e6-107">Get a list of all subscriptions in your account.</span></span>

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

2. <span data-ttu-id="d00e6-108">既定のサブスクリプションを設定します。</span><span class="sxs-lookup"><span data-stu-id="d00e6-108">Set the default.</span></span>

    ```azurepowershell-interactive
    Select-AzureRmSubscription -SubscriptionName "My Demos"
    ```

3. <span data-ttu-id="d00e6-109">`Get-AzureRmContext` コマンドレットを実行して変更内容を確認します。</span><span class="sxs-lookup"><span data-stu-id="d00e6-109">Verify the change by running the `Get-AzureRmContext` cmdlet.</span></span>

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

<span data-ttu-id="d00e6-110">既定のサブスクリプションを設定すると、後続のすべての Azure PowerShell コマンドは、このサブスクリプションに対して実行されます。</span><span class="sxs-lookup"><span data-stu-id="d00e6-110">Once you set your default subscription, all subsequent Azure PowerShell commands run against this subscription.</span></span>

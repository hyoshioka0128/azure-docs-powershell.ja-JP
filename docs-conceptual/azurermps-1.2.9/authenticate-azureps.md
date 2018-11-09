---
title: Azure PowerShell でのログイン
description: Azure PowerShell でのログイン
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: edbf17141cac4ea6e41282c8e1dd07c5b738351c
ms.sourcegitcommit: ac4b53bb42a25aae013a9d8cd9ae98ada9397274
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/08/2018
ms.locfileid: "51274706"
---
# <a name="log-in-with-azure-powershell"></a>Azure PowerShell でのログイン

Azure PowerShell は、複数のログイン方法をサポートしています。 最も簡単に始められるのは、コマンド ラインから対話形式でログインする方法です。

## <a name="interactive-log-in"></a>対話形式でのログイン

1. 「 `Login-AzureRmAccount`」と入力します。 Azure の資格情報の入力を求めるダイアログ ボックスが表示されます。

2. アカウントに関連付けられている電子メール アドレスとパスワードを入力します。 Azure により資格情報が認証および保存され、ウィンドウが閉じます。

## <a name="log-in-with-a-service-principal"></a>サービス プリンシパルによるログイン

サービス プリンシパルは、リソースの操作に使用できる非対話型のアカウントを作成する方法を提供します。 サービス プリンシパルは、Azure Active Directory を使用してルールを適用できるユーザー アカウントに似ています。 サービス プリンシパルに最低限必要なアクセス許可だけを付与することによって、自動化スクリプトをより安全にすることができます。

1. まだサービス プリンシパルがない場合は、サービス プリンシパルを[作成](create-azure-service-principal-azureps.md)します。

2. サービス プリンシパルを使用してログインします。

    ```powershell-interactive
    Login-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
    ```

    テナント ID を取得するには、対話形式でログインし、サブスクリプションから TenantId を取得します。

    ```powershell-interactive
    Get-AzureRmSubscription
    ```

    ```output
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Production Subscription
    CurrentStorageAccount :
    ```

### <a name="log-in-using-managed-identities-for-azure-resources"></a>Azure リソースのマネージド ID を使用してログインする

Azure リソースのマネージドID は、Azure Active Directory の機能です。 サインインにマネージド ID サービス プリンシパルを使用し、その他のリソースにアクセスするためにアプリ専用のアクセス トークンを取得できます。

Azure リソースのマネージド ID の詳細については、「[How to use managed identities for Azure resources on an Azure VM to acquire an access token (Azure VM 上で Azure リソースのマネージド ID を使用してアクセス トークンを取得する方法)](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token)」を参照してください。

## <a name="log-in-to-another-cloud"></a>別のクラウドにログインする

Azure Cloud Services では、さまざまな政府機関から発せられるデータ処理規制に準拠したさまざまな環境を提供します。 Azure アカウントが政府機関のクラウド内にある場合は、サインイン時に環境を指定する必要があります。 たとえば、アカウントが中国のクラウド内にある場合、次のコマンドを使用してサインインします。

```powershell-interactive
Login-AzureRmAccount -EnvironmentName AzureChinaCloud
```

使用可能な環境の一覧を取得するには、次のコマンドを使用します。

```powershell-interactive
Get-AzureRmEnvironment | Select-Object Name
```

```output
Name
----
AzureCloud
AzureChinaCloud
AzureUSGovernment
AzureGermanCloud
```

## <a name="learn-more-about-managing-azure-role-based-access"></a>Azure ロールベース アクセスの管理についての詳細情報

Azure での認証とサブスクリプション管理の詳細については、[アカウント、サブスクリプション、管理者ロールの管理](/azure/active-directory/role-based-access-control-configure)に関するページを参照してください。

ロール管理を目的とした Azure PowerShell のコマンドレット

* [Get-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [Get-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [New-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [New-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [Remove-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [Remove-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [Set-AzureRmRoleDefinition](/powershell/moduel/AzureRM.Resources/Set-AzureRmRoleDefinition)

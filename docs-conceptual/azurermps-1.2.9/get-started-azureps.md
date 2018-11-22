---
title: Azure PowerShell を使ってみる | Microsoft Docs
description: ''
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: get-started-article
ms.date: 11/15/2017
ms.openlocfilehash: 3114f9e9b36dc374f9fb2d402c448cff7fef0aa3
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/22/2018
ms.locfileid: "52258657"
---
# <a name="getting-started-with-azure-powershell"></a>Azure PowerShell を使ってみる

Azure PowerShell は、コマンド ラインから Azure リソースを管理したり、Azure Resource Manager を操作対象とする自動化スクリプトを作成したりできるように設計されています。 これは、[Azure Cloud Shell](/azure/cloud-shell/overview) を使用してブラウザーで使用することも、ローカル コンピューターにインストールして PowerShell セッションで使用することもできます。 この記事では、その基本的な使い方と核となる概念について説明します。

## <a name="connect"></a>接続

最も簡単に始められるのは、[Cloud Shell を起動](/azure/cloud-shell/quickstart)する方法です。

1. Cloud Shell は、Azure Portal の上部のナビゲーションから起動します。

   ![Shell アイコン](~/media/get-started-azureps/shell-icon.png)

2. 使用するサブスクリプションを選択し、ストレージ アカウントを作成します。

   ![ストレージ アカウントの作成](~/media/get-started-azureps/storage-prompt.png)

ストレージが作成されたら、Cloud Shell によってブラウザーで PowerShell セッションが開きます。

![Cloud Shell for PowerShell](~/media/get-started-azureps/cloud-powershell.png)

Azure PowerShell をインストールし、ローカルの PowerShell セッションで使用することもできます。

## <a name="install-azure-powershell"></a>Azure PowerShell をインストールする

初めに最新バージョンの Azure PowerShell がインストールされていることを確認します。 最新リリースについては、[リリース ノート](./release-notes-azureps.md)をご覧ください。

1. [Azure PowerShell をインストールします](install-azurerm-ps.md)。

2. インストールが成功したことを確認するために、コマンド ラインから `Get-Module AzureRM -ListAvailable` を実行します。

## <a name="log-in-to-azure"></a>Azure にログインする

対話操作でサインオンするには:

1. 「 `Login-AzureRmAccount`」と入力します。 Azure の資格情報の入力を求めるダイアログ ボックスが表示されます。 オプション '-EnvironmentName' により、Azure China または Azure Germany にログインできます。

   例: Login-AzureRmAccount -EnvironmentName AzureChinaCloud

2. アカウントに関連付けられている電子メール アドレスとパスワードを入力します。 Azure により資格情報が認証および保存され、ウィンドウが閉じます。

Azure アカウントへのサインイン後、Azure PowerShell のコマンドレットを使って自分のサブスクリプションのリソースにアクセスし、管理することができます。

## <a name="create-a-resource-group"></a>リソース グループの作成

必要な設定がすべて整ったら、Azure PowerShell を使って Azure にリソースを作成してみましょう。

まずリソース グループを作成します。 Azure ではリソース グループを使うことで、複数のリソースを論理上のグループとして 1 つにまとめて管理することができます。 たとえばアプリケーションまたはプロジェクトのリソース グループを作成し、仮想マシンやデータベース、CDN サービスをそこに追加することができます。

"MyResourceGroup" という名前のリソース グループを Azure の westeurope リージョンに作成しましょう。 そのためには次のコマンドを入力します。

```powershell-interactive
New-AzureRmResourceGroup -Name 'myResourceGroup' -Location 'westeurope'
```

```Output
ResourceGroupName : myResourceGroup
Location          : westeurope
ProvisioningState : Succeeded
Tags              :
ResourceId        : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myResourceGroup
```

## <a name="create-a-windows-virtual-machine"></a>Windows 仮想マシンの作成

リソース グループが完成したら、そこに Windows VM を作成します。 新しい VM を作成するには、その他の必要なリソースを最初に作成し、構成に割り当てる必要があります。 その構成を使って VM を作成することができます。

### <a name="create-the-required-network-resources"></a>必要なネットワーク リソースの作成

まず、仮想ネットワークの作成プロセスで使用するサブネット構成を作成する必要があります。 その VM に接続できるように、さらにパブリック IP アドレスも作成します。 そのパブリック アドレスへのアクセスについては、ネットワーク セキュリティ グループを作成してセキュリティを確保します。 最後に、前述のリソースをすべて使って仮想 NIC を作成します。

```powershell-interactive
# Variables for common values
$resourceGroup = "myResourceGroup"
$location = "westeurope"
$vmName = "myWindowsVM"

# Create a subnet configuration
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet1 -AddressPrefix 192.168.1.0/24

# Create a virtual network
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName $resourceGroup -Location $location `
  -Name MYvNET1 -AddressPrefix 192.168.0.0/16 -Subnet $subnetConfig

# Create a public IP address and specify a DNS name
$publicIp = New-AzureRmPublicIpAddress -ResourceGroupName $resourceGroup -Location $location `
  -Name "mypublicdns$(Get-Random)" -AllocationMethod Static -IdleTimeoutInMinutes 4
$publicIp | Select-Object Name,IpAddress

# Create an inbound network security group rule for port 3389
$nsgRuleRDP = New-AzureRmNetworkSecurityRuleConfig -Name myNetworkSecurityGroupRuleRDP  -Protocol Tcp `
  -Direction Inbound -Priority 1000 -SourceAddressPrefix * -SourcePortRange * -DestinationAddressPrefix * `
  -DestinationPortRange 3389 -Access Allow

# Create a network security group
$nsg = New-AzureRmNetworkSecurityGroup -ResourceGroupName $resourceGroup -Location $location `
  -Name myNetworkSecurityGroup1 -SecurityRules $nsgRuleRDP

# Create a virtual network card and associate with public IP address and NSG
$nic = New-AzureRmNetworkInterface -Name myNic1 -ResourceGroupName $resourceGroup -Location $location `
  -SubnetId $vnet.Subnets[0].Id -PublicIpAddressId $publicIp.Id -NetworkSecurityGroupId $nsg.Id
```

### <a name="create-the-virtual-machine"></a>仮想マシンの作成

最初に、OS の一連の資格情報が必要です。

```powershell-interactive
# Create user object
$cred = Get-Credential -Message "Enter a username and password for the virtual machine."
```

これで必要なリソースが揃ったので、VM を作成することができます。 このステップでは、VM 構成オブジェクトを作成し、その構成を使って VM を作成します。

```powershell-interactive
# Create a virtual machine configuration
$vmConfig = New-AzureRmVMConfig -VMName $vmName -VMSize Standard_D1 |
  Set-AzureRmVMOperatingSystem -Windows -ComputerName $vmName -Credential $cred |
  Set-AzureRmVMSourceImage -PublisherName MicrosoftWindowsServer -Offer WindowsServer -Skus 2016-Datacenter -Version latest |
  Add-AzureRmVMNetworkInterface -Id $nic.Id

# Create a virtual machine
New-AzureRmVM -ResourceGroupName $resourceGroup -Location $location -VM $vmConfig
```

VM の作成が完了し、使用する準備ができると、`New-AzureRmVM` コマンドから結果が出力されます。

```Output
RequestId IsSuccessStatusCode StatusCode ReasonPhrase
--------- ------------------- ---------- ------------
                         True         OK OK
```

新しく作成した Windows Server VM のパブリック IP アドレスとリモート デスクトップを使って VM にログオンします。 次のコマンドを実行すると、前述のスクリプトで作成したパブリック IP アドレスが表示されます。

```powershell-interactive
$publicIp | Select-Object Name,IpAddress
```

```Output
Name                  IpAddress
----                  ---------
mypublicdns1400512543 xx.xx.xx.xx
```

Windows ベースのシステムでは、コマンド ラインで mstsc コマンドを使って同じ操作を実行できます。

```powershell-interactive
mstsc /v:xx.xxx.xx.xxx
```

VM を作成したときと同じユーザー名/パスワードの組み合わせを指定してログインしてください。

## <a name="create-a-linux-virtual-machine"></a>Linux 仮想マシンを作成する

新しい Linux VM を作成するには、その他の必要なリソースを最初に作成し、構成に割り当てる必要があります。 その構成を使って VM を作成することができます。 ここでは、前述のリソース グループが既に作成済みであることを前提としています。 また、`id_rsa.pub` という名前の SSH 公開キーがユーザー プロファイルの .ssh ディレクトリに必要です。

### <a name="create-the-required-network-resources"></a>必要なネットワーク リソースの作成

まず、仮想ネットワークの作成プロセスで使用するサブネット構成を作成する必要があります。 その VM に接続できるように、さらにパブリック IP アドレスも作成します。 そのパブリック アドレスへのアクセスについては、ネットワーク セキュリティ グループを作成してセキュリティを確保します。 最後に、前述のリソースをすべて使って仮想 NIC を作成します。

```powershell-interactive
# Variables for common values
$resourceGroup = "myResourceGroup"
$location = "westeurope"
$vmName = "myLinuxVM"

# Definer user name and blank password
$securePassword = ConvertTo-SecureString ' ' -AsPlainText -Force
$cred = New-Object System.Management.Automation.PSCredential ("azureuser", $securePassword)

# Create a subnet configuration
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 192.168.2.0/24

# Create a virtual network
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName $resourceGroup -Location $location `
  -Name MYvNET2 -AddressPrefix 192.168.0.0/16 -Subnet $subnetConfig

# Create a public IP address and specify a DNS name
$publicIp = New-AzureRmPublicIpAddress -ResourceGroupName $resourceGroup -Location $location `
  -Name "mypublicdns$(Get-Random)" -AllocationMethod Static -IdleTimeoutInMinutes 4
$publicIp | Select-Object Name,IpAddress

# Create an inbound network security group rule for port 22
$nsgRuleSSH = New-AzureRmNetworkSecurityRuleConfig -Name myNetworkSecurityGroupRuleSSH  -Protocol Tcp `
  -Direction Inbound -Priority 1000 -SourceAddressPrefix * -SourcePortRange * -DestinationAddressPrefix * `
  -DestinationPortRange 22 -Access Allow

# Create a network security group
$nsg = New-AzureRmNetworkSecurityGroup -ResourceGroupName $resourceGroup -Location $location `
  -Name myNetworkSecurityGroup2 -SecurityRules $nsgRuleSSH

# Create a virtual network card and associate with public IP address and NSG
$nic = New-AzureRmNetworkInterface -Name myNic2 -ResourceGroupName $resourceGroup -Location $location `
  -SubnetId $vnet.Subnets[0].Id -PublicIpAddressId $publicIp.Id -NetworkSecurityGroupId $nsg.Id
```

### <a name="create-the-virtual-machine"></a>仮想マシンの作成

これで必要なリソースが揃ったので、VM を作成することができます。 このステップでは、VM 構成オブジェクトを作成し、その構成を使って VM を作成します。

```powershell-interactive
# Create a virtual machine configuration
$vmConfig = New-AzureRmVMConfig -VMName $vmName -VMSize Standard_D1 |
  Set-AzureRmVMOperatingSystem -Linux -ComputerName $vmName -Credential $cred -DisablePasswordAuthentication |
  Set-AzureRmVMSourceImage -PublisherName Canonical -Offer UbuntuServer -Skus 14.04.2-LTS -Version latest |
  Add-AzureRmVMNetworkInterface -Id $nic.Id

# Configure SSH Keys
$sshPublicKey = Get-Content "$env:USERPROFILE\.ssh\id_rsa.pub"
Add-AzureRmVMSshPublicKey -VM $vmConfig -KeyData $sshPublicKey -Path "/home/azureuser/.ssh/authorized_keys"

# Create a virtual machine
New-AzureRmVM -ResourceGroupName $resourceGroup -Location $location -VM $vmConfig
```

VM が作成されたら、その VM のパブリック IP アドレスを SSH で使用し、新しい Linux VM にログオンすることができます。

```bash
ssh xx.xxx.xxx.xxx
```

```Output
Welcome to Ubuntu 14.04.4 LTS (GNU/Linux 3.19.0-65-generic x86_64)

 * Documentation:  https://help.ubuntu.com/

  System information as of Sun Feb 19 00:32:28 UTC 2017

  System load: 0.31              Memory usage: 3%   Processes:       89
  Usage of /:  39.6% of 1.94GB   Swap usage:   0%   Users logged in: 0

  Graph this data and manage this system at:
    https://landscape.canonical.com/

  Get cloud support with Ubuntu Advantage Cloud Guest:
    http://www.ubuntu.com/business/services/cloud

0 packages can be updated.
0 updates are security updates.



The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

my-login@MyLinuxVM:../../..$
```

## <a name="creating-other-resources-in-azure"></a>その他の Azure リソースを作成する

ここまでは、リソース グループ、Linux VM、Windows Server VM の作成方法を見てきました。 そのほかにも、さまざまな種類の Azure リソースを作成することができます。

たとえば、新しく作成した VM に関連付けるための Azure ネットワーク ロード バランサーを作成するには、次のコマンドを使います。

```powershell-interactive
New-AzureRmLoadBalancer -Name MyLoadBalancer -ResourceGroupName myResourceGroup -Location westeurope
```

また、次のコマンドを使って、インフラストラクチャ用に新しいプライベート仮想ネットワーク (Azure では通常 "VNet" と呼ばれます) を作成することもできます。

```powershell-interactive
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 10.0.0.0/16
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName myResourceGroup -Location westeurope `
  -Name MYvNET3 -AddressPrefix 10.0.0.0/16 -Subnet $subnetConfig
```

Azure と Azure PowerShell の優れている点は、それらを使ってクラウドベースのインフラストラクチャを実現できるだけでなく、管理対象となるプラットフォーム サービスを作成できることです。 その管理されたプラットフォーム サービスにインフラストラクチャを組み合わせることで、さらに強力なソリューションを構築することもできます。

たとえば Azure PowerShell を使って Azure AppService を作成することができます。 Azure AppService は、管理されたプラットフォーム サービスであり、インフラストラクチャには一切気を遣わずに Web アプリをホストできるのが特徴です。 Azure AppService の作成後、次のコマンドを使って AppService 内に 2 つの新しい Azure Web アプリを作成することができます。

```powershell-interactive
# Create an Azure AppService that we can host any number of web apps within
New-AzureRmAppServicePlan -Name MyAppServicePlan -Tier Basic -NumberofWorkers 2 -WorkerSize Small -ResourceGroupName myResourceGroup -Location westeurope

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
New-AzureRmWebApp -Name MyWebApp43432 -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westeurope
New-AzureRmWebApp -Name MyWebApp43433 -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westeurope
```

## <a name="listing-deployed-resources"></a>デプロイされているリソースの一覧表示

Azure 内で実行されているリソースは、`Get-AzureRmResource` コマンドレットを使って一覧表示することができます。 先ほど新しいリソース グループに作成したリソースを表示する例を次に示します。

```powershell-interactive
Get-AzureRmResource |
  Where-Object ResourceGroupName -eq myResourceGroup |
    Select-Object Name,Location,ResourceType
```

```Output
Name                                                  Location   ResourceType
----                                                  --------   ------------
myLinuxVM_OsDisk_1_36ca038791f642ba91270879088c249a   westeurope Microsoft.Compute/disks
myWindowsVM_OsDisk_1_f627e6e2bb454c72897d72e9632adf9a westeurope Microsoft.Compute/disks
myLinuxVM                                             westeurope Microsoft.Compute/virtualMachines
myWindowsVM                                           westeurope Microsoft.Compute/virtualMachines
myWindowsVM/BGInfo                                    westeurope Microsoft.Compute/virtualMachines/extensions
myNic1                                                westeurope Microsoft.Network/networkInterfaces
myNic2                                                westeurope Microsoft.Network/networkInterfaces
myNetworkSecurityGroup1                               westeurope Microsoft.Network/networkSecurityGroups
myNetworkSecurityGroup2                               westeurope Microsoft.Network/networkSecurityGroups
mypublicdns245369171                                  westeurope Microsoft.Network/publicIPAddresses
mypublicdns779537141                                  westeurope Microsoft.Network/publicIPAddresses
MYvNET1                                               westeurope Microsoft.Network/virtualNetworks
MYvNET2                                               westeurope Microsoft.Network/virtualNetworks
micromyresomywi032907510                              westeurope Microsoft.Storage/storageAccounts
```

## <a name="deleting-resources"></a>リソースの削除

Azure アカウントをクリーンアップするために、この例で作成したリソースを削除しましょう。 不要になったリソースは、`Remove-AzureRm*` コマンドレットを使って削除できます。 作成した Windows VM を削除するには、次のコマンドを使います。

```powershell-interactive
Remove-AzureRmVM -Name myWindowsVM -ResourceGroupName myResourceGroup
```

リソースを削除してよいか確認するメッセージが表示されます。

```Output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

多数のリソースを一度に削除することもできます。 たとえば次のコマンドを実行すると、この概要チュートリアルのすべてのサンプルで使ってきたリソース グループ ("MyResourceGroup") が完全に削除されます。 リソース グループだけでなく、そこに含まれるリソースもすべて削除されます。

```powershell-interactive
Remove-AzureRmResourceGroup -Name myResourceGroup
```

```Output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

このコマンドは、完了までに数分かかる場合があります。

## <a name="get-samples"></a>サンプルを入手する

Azure PowerShell の使用方法について詳しくは、[Linux VM](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json)、[Windows VM](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json)、[Web Apps](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json)、[SQL Database](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json) 用の一般的なスクリプトが用意されているので、そちらをご覧ください。

## <a name="next-steps"></a>次の手順

* [Azure PowerShell でのログイン](authenticate-azureps.md)
* [Azure PowerShell による Azure サブスクリプションの管理](manage-subscriptions-azureps.md)
* [Azure PowerShell を使って Azure にサービス プリンシパルを作成する](create-azure-service-principal-azureps.md)
* 以前のリリースからの移行については、リリース ノート ([ https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes](https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes)) を参照してください。
* コミュニティに質問する:
  * [MSDN の Azure フォーラム](http://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [stackoverflow](http://go.microsoft.com/fwlink/?LinkId=320213)

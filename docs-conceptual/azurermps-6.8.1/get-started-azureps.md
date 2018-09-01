---
title: Azure PowerShell の使用に関するページ
description: ''
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: get-started-article
ms.date: 11/15/2017
ms.openlocfilehash: 5354a75e969e084d6457d0566a516705f365476f
ms.sourcegitcommit: dca906e73e943aac207cee23b79915773419c673
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/30/2018
ms.locfileid: "43250450"
---
# <a name="get-started-with-azure-powershell"></a><span data-ttu-id="43608-102">Azure PowerShell の使用に関するページ</span><span class="sxs-lookup"><span data-stu-id="43608-102">Get started with Azure PowerShell</span></span>

<span data-ttu-id="43608-103">Azure PowerShell は、コマンド ラインから Azure リソースを管理したり、Azure Resource Manager を操作対象とする自動化スクリプトを作成したりできるように設計されています。</span><span class="sxs-lookup"><span data-stu-id="43608-103">Azure PowerShell is designed for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="43608-104">これは、[Azure Cloud Shell](/azure/cloud-shell/overview) を使ってブラウザーで使用することも、ローカル コンピューターにインストールすることもできます。</span><span class="sxs-lookup"><span data-stu-id="43608-104">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview) or you install it on your local machine.</span></span> <span data-ttu-id="43608-105">この記事では、Azure PowerShell の基本的な使い方と、主要な概念について説明します。</span><span class="sxs-lookup"><span data-stu-id="43608-105">This article helps get you started with Azure PowerShell and teaches the core concepts behind it.</span></span>

## <a name="install-azure-powershell"></a><span data-ttu-id="43608-106">Azure PowerShell をインストールする</span><span class="sxs-lookup"><span data-stu-id="43608-106">Install Azure PowerShell</span></span>

<span data-ttu-id="43608-107">初めに最新バージョンの Azure PowerShell がインストールされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="43608-107">The first step is to make sure you have the latest version of the Azure PowerShell installed.</span></span> <span data-ttu-id="43608-108">最新リリースについては、[リリース ノート](./release-notes-azureps.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="43608-108">For information about the latest release, see the [release notes](./release-notes-azureps.md).</span></span>

1. <span data-ttu-id="43608-109">[Azure PowerShell をインストールします](install-azurerm-ps.md)。</span><span class="sxs-lookup"><span data-stu-id="43608-109">[Install Azure PowerShell](install-azurerm-ps.md).</span></span>

2. <span data-ttu-id="43608-110">インストールが成功したことを確認するために、コマンド ラインから `Get-Module AzureRM -ListAvailable` を実行します。</span><span class="sxs-lookup"><span data-stu-id="43608-110">To verify the installation was successful, run `Get-Module AzureRM -ListAvailable` from your command line.</span></span>

## <a name="azure-cloud-shell"></a><span data-ttu-id="43608-111">Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="43608-111">Azure Cloud Shell</span></span>

<span data-ttu-id="43608-112">最も簡単に始められるのは、[Cloud Shell を起動](/azure/cloud-shell/quickstart)する方法です。</span><span class="sxs-lookup"><span data-stu-id="43608-112">The simplest way to get started is to [launch Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

1. <span data-ttu-id="43608-113">Cloud Shell は、Azure Portal の上部のナビゲーションから起動します。</span><span class="sxs-lookup"><span data-stu-id="43608-113">Launch Cloud Shell from the top navigation of the Azure portal.</span></span>

   ![Shell アイコン](~/media/get-started-azureps/shell-icon.png)

2. <span data-ttu-id="43608-115">使用するサブスクリプションを選択し、ストレージ アカウントを作成します。</span><span class="sxs-lookup"><span data-stu-id="43608-115">Choose the subscription you want to use and create a storage account.</span></span>

   ![ストレージ アカウントの作成](~/media/get-started-azureps/storage-prompt.png)

<span data-ttu-id="43608-117">ストレージが作成されたら、Cloud Shell によってブラウザーで PowerShell セッションが開きます。</span><span class="sxs-lookup"><span data-stu-id="43608-117">Once your storage has been created, the Cloud Shell will open a PowerShell session in the browser.</span></span>

![Cloud Shell for PowerShell](~/media/get-started-azureps/cloud-powershell.png)

<span data-ttu-id="43608-119">Azure PowerShell をインストールし、ローカルの PowerShell セッションで使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="43608-119">You can also install Azure PowerShell and use it locally in a PowerShell session.</span></span>

## <a name="sign-in-to-azure"></a><span data-ttu-id="43608-120">Azure へのサインイン</span><span class="sxs-lookup"><span data-stu-id="43608-120">Sign in to Azure</span></span>

<span data-ttu-id="43608-121">対話操作でサインオンするには:</span><span class="sxs-lookup"><span data-stu-id="43608-121">Sign on interactively:</span></span>

1. <span data-ttu-id="43608-122">「 `Connect-AzureRmAccount`」と入力します。</span><span class="sxs-lookup"><span data-stu-id="43608-122">Type `Connect-AzureRmAccount`.</span></span> <span data-ttu-id="43608-123">Azure の資格情報の入力を求めるダイアログ ボックスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="43608-123">You will get dialog box asking for your Azure credentials.</span></span> <span data-ttu-id="43608-124">"-Environment" オプションを使用すると、Azure China または Azure Germany を認証できます。</span><span class="sxs-lookup"><span data-stu-id="43608-124">Option '-Environment' can let you authenticate for Azure China or Azure Germany.</span></span>

   <span data-ttu-id="43608-125">例: Connect-AzureRmAccount -Environment AzureChinaCloud</span><span class="sxs-lookup"><span data-stu-id="43608-125">e.g. Connect-AzureRmAccount -Environment AzureChinaCloud</span></span>

2. <span data-ttu-id="43608-126">アカウントに関連付けられている電子メール アドレスとパスワードを入力します。</span><span class="sxs-lookup"><span data-stu-id="43608-126">Type the email address and password associated with your account.</span></span> <span data-ttu-id="43608-127">Azure により資格情報が認証および保存され、ウィンドウが閉じます。</span><span class="sxs-lookup"><span data-stu-id="43608-127">Azure authenticates and saves the credential information, and then closes the window.</span></span>

<span data-ttu-id="43608-128">Azure アカウントにサインインしたら、Azure PowerShell コマンドレットを使ってサブスクリプションのリソースにアクセスし、管理できます。</span><span class="sxs-lookup"><span data-stu-id="43608-128">Once you have signed in to an Azure account, you can use the Azure PowerShell cmdlets to access and manage the resources in your subscription.</span></span>

## <a name="create-a-windows-virtual-machine-using-simple-defaults"></a><span data-ttu-id="43608-129">単純な既定値を使用して Windows 仮想マシンを作成する</span><span class="sxs-lookup"><span data-stu-id="43608-129">Create a Windows virtual machine using simple defaults</span></span>

<span data-ttu-id="43608-130">`New-AzureRmVM` コマンドレットは、簡略化された構文を提供しているため、新しい仮想マシンを簡単に作成できます。</span><span class="sxs-lookup"><span data-stu-id="43608-130">The `New-AzureRmVM` cmdlet provides a simplified syntax making it easy to create a new virtual machine.</span></span> <span data-ttu-id="43608-131">指定する必要があるパラメーター値は、VM の名前と、VM のローカル管理者アカウントの一連の資格情報の 2 つのみです。</span><span class="sxs-lookup"><span data-stu-id="43608-131">There are only two parameter values you must provide: the name of the VM and a set of credentials for the local administrator account on the VM.</span></span>

<span data-ttu-id="43608-132">最初に、資格情報オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="43608-132">First, create the credential object.</span></span>

```azurepowershell-interactive
$cred = Get-Credential -Message "Enter a username and password for the virtual machine."
```

```output
Windows PowerShell credential request.
Enter a username and password for the virtual machine.
User: localAdmin
Password for user localAdmin: *********
```

<span data-ttu-id="43608-133">次に、VM を作成します。</span><span class="sxs-lookup"><span data-stu-id="43608-133">Next, create the VM.</span></span>

```azurepowershell-interactive
New-AzureRmVM -Name SampleVM -Credential $cred
```

```output
ResourceGroupName        : SampleVM
Id                       : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/SampleVM/providers/Microsoft.Compute/virtualMachines/SampleVM
VmId                     : 43f6275d-ce50-49c8-a831-5d5974006e63
Name                     : SampleVM
Type                     : Microsoft.Compute/virtualMachines
Location                 : eastus
Tags                     : {}
HardwareProfile          : {VmSize}
NetworkProfile           : {NetworkInterfaces}
OSProfile                : {ComputerName, AdminUsername, WindowsConfiguration, Secrets}
ProvisioningState        : Succeeded
StorageProfile           : {ImageReference, OsDisk, DataDisks}
FullyQualifiedDomainName : samplevm-2c0867.eastus.cloudapp.azure.com
```

<span data-ttu-id="43608-134">ここまでは簡単でした。</span><span class="sxs-lookup"><span data-stu-id="43608-134">That was easy.</span></span> <span data-ttu-id="43608-135">ただし、他に何が作成され、VM がどのように構成されているのかと疑問にお感じのことでしょう。</span><span class="sxs-lookup"><span data-stu-id="43608-135">But, you may wonder what else is created and how is the VM configured.</span></span> <span data-ttu-id="43608-136">まず、リソース グループを確認しましょう。</span><span class="sxs-lookup"><span data-stu-id="43608-136">First, let's look at our resource groups.</span></span>

```azurepowershell-interactive
Get-AzureRmResourceGroup | Select-Object ResourceGroupName,Location
```

```output
ResourceGroupName          Location
-----------------          --------
cloud-shell-storage-westus westus
SampleVM                   eastus
```

<span data-ttu-id="43608-137">**cloud-shell-storage-westus** リソース グループは、Cloud Shell を初めて使用するときに作成されます。</span><span class="sxs-lookup"><span data-stu-id="43608-137">The **cloud-shell-storage-westus** resource group is created the first time you use the Cloud Shell.</span></span> <span data-ttu-id="43608-138">**SampleVM** リソース グループは、`New-AzureRmVM` コマンドレットによって作成されました。</span><span class="sxs-lookup"><span data-stu-id="43608-138">The **SampleVM** resource group was created by the `New-AzureRmVM` cmdlet.</span></span>

<span data-ttu-id="43608-139">では、この新しいリソース グループには、他にどのようなリソースが作成されているでしょうか。</span><span class="sxs-lookup"><span data-stu-id="43608-139">Now, what other resources were created in this new resource group?</span></span>

```azurepowershell-interactive
Get-AzureRmResource |
  Where ResourceGroupName -eq SampleVM |
    Select-Object ResourceGroupName,Location,ResourceType,Name
```

```output
ResourceGroupName          Location ResourceType                            Name
-----------------          -------- ------------                            ----
SAMPLEVM                   eastus   Microsoft.Compute/disks                 SampleVM_OsDisk_1_9b286c54b168457fa1f8c47...
SampleVM                   eastus   Microsoft.Compute/virtualMachines       SampleVM
SampleVM                   eastus   Microsoft.Network/networkInterfaces     SampleVM
SampleVM                   eastus   Microsoft.Network/networkSecurityGroups SampleVM
SampleVM                   eastus   Microsoft.Network/publicIPAddresses     SampleVM
SampleVM                   eastus   Microsoft.Network/virtualNetworks       SampleVM
```

<span data-ttu-id="43608-140">VM についての詳細情報を取得してみましょう。</span><span class="sxs-lookup"><span data-stu-id="43608-140">Let's get some more details about the VM.</span></span> <span data-ttu-id="43608-141">次の例は、VM の作成に使用した OS イメージに関する情報を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="43608-141">This examples shows how to retrieve information about the OS Image used to create the VM.</span></span>

```azurepowershell-interactive
Get-AzureRmVM -Name SampleVM -ResourceGroupName SampleVM |
  Select-Object -ExpandProperty StorageProfile |
    Select-Object -ExpandProperty ImageReference
```

```output
Publisher : MicrosoftWindowsServer
Offer     : WindowsServer
Sku       : 2016-Datacenter
Version   : latest
Id        :
```

## <a name="create-a-fully-configured-linux-virtual-machine"></a><span data-ttu-id="43608-142">完全に構成された Linux 仮想マシンの作成</span><span class="sxs-lookup"><span data-stu-id="43608-142">Create a fully configured Linux Virtual Machine</span></span>

<span data-ttu-id="43608-143">前の例では、簡略化された構文と既定のパラメーター値を使用して、Windows 仮想マシンを作成しました。</span><span class="sxs-lookup"><span data-stu-id="43608-143">The previous example used the simplified syntax and default parameter values to create a Windows virtual machine.</span></span> <span data-ttu-id="43608-144">この例では、仮想マシンのすべてのオプションの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="43608-144">In this example, we provide values for all options of the virtual machine.</span></span>

### <a name="create-a-resource-group"></a><span data-ttu-id="43608-145">リソース グループの作成</span><span class="sxs-lookup"><span data-stu-id="43608-145">Create a resource group</span></span>

<span data-ttu-id="43608-146">この例では、リソース グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="43608-146">For this example we want to create a Resource Group.</span></span> <span data-ttu-id="43608-147">Azure ではリソース グループを使うことで、複数のリソースを論理上のグループとして 1 つにまとめて管理することができます。</span><span class="sxs-lookup"><span data-stu-id="43608-147">Resource Groups in Azure provide a way to manage multiple resources that you want to logically group together.</span></span> <span data-ttu-id="43608-148">たとえばアプリケーションまたはプロジェクトのリソース グループを作成し、仮想マシンやデータベース、CDN サービスをそこに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="43608-148">For example, you might create a Resource Group for an application or project and add a virtual machine, a database and a CDN service within it.</span></span>

<span data-ttu-id="43608-149">"MyResourceGroup" という名前のリソース グループを Azure の westeurope リージョンに作成しましょう。</span><span class="sxs-lookup"><span data-stu-id="43608-149">Let's create a resource group named "MyResourceGroup" in the westeurope region of Azure.</span></span> <span data-ttu-id="43608-150">そのためには次のコマンドを入力します。</span><span class="sxs-lookup"><span data-stu-id="43608-150">To do so type the following command:</span></span>

```azurepowershell-interactive
New-AzureRmResourceGroup -Name 'myResourceGroup' -Location 'westeurope'
```

```output
ResourceGroupName : myResourceGroup
Location          : westeurope
ProvisioningState : Succeeded
Tags              :
ResourceId        : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myResourceGroup
```

<span data-ttu-id="43608-151">この新しいリソース グループは、作成する新しい VM に必要なすべてのリソースを格納するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="43608-151">This new resource group will be used to contain all of the resources needed for the new VM we create.</span></span> <span data-ttu-id="43608-152">新しい Linux VM を作成するには、その他の必要なリソースを最初に作成し、構成に割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="43608-152">To create a new Linux VM we must first create the other required resources and assign them to a configuration.</span></span> <span data-ttu-id="43608-153">その構成を使って VM を作成することができます。</span><span class="sxs-lookup"><span data-stu-id="43608-153">Then we can use that configuration to create the VM.</span></span> <span data-ttu-id="43608-154">また、`id_rsa.pub` という名前の SSH 公開キーがユーザー プロファイルの .ssh ディレクトリに必要です。</span><span class="sxs-lookup"><span data-stu-id="43608-154">Also, you will need to have an SSH public key named `id_rsa.pub` in the .ssh directory of your user profile.</span></span>

#### <a name="create-the-required-network-resources"></a><span data-ttu-id="43608-155">必要なネットワーク リソースの作成</span><span class="sxs-lookup"><span data-stu-id="43608-155">Create the required network resources</span></span>

<span data-ttu-id="43608-156">まず、仮想ネットワークの作成プロセスで使用するサブネット構成を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="43608-156">First we need to create a subnet configuration to be used with the virtual network creation process.</span></span> <span data-ttu-id="43608-157">その VM に接続できるように、さらにパブリック IP アドレスも作成します。</span><span class="sxs-lookup"><span data-stu-id="43608-157">We also create a public IP address so that we can connect to this VM.</span></span> <span data-ttu-id="43608-158">そのパブリック アドレスへのアクセスについては、ネットワーク セキュリティ グループを作成してセキュリティを確保します。</span><span class="sxs-lookup"><span data-stu-id="43608-158">We create a network security group to secure access to the public address.</span></span> <span data-ttu-id="43608-159">最後に、前述のリソースをすべて使って仮想 NIC を作成します。</span><span class="sxs-lookup"><span data-stu-id="43608-159">Finally we create the virtual NIC using all of the previous resources.</span></span>

```azurepowershell-interactive
# Variables for common values
$resourceGroup = "myResourceGroup"
$location = "westeurope"
$vmName = "myLinuxVM"

# Definer user name and blank password
$securePassword = ConvertTo-SecureString 'azurepassword' -AsPlainText -Force
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

### <a name="create-the-vm-configuration"></a><span data-ttu-id="43608-160">VM 構成の作成</span><span class="sxs-lookup"><span data-stu-id="43608-160">Create the VM configuration</span></span>

<span data-ttu-id="43608-161">必要なリソースが揃ったので、VM 構成オブジェクトを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="43608-161">Now that we have the required resources we can create the VM configuration object.</span></span>

```azurepowershell-interactive
# Create a virtual machine configuration
$vmConfig = New-AzureRmVMConfig -VMName $vmName -VMSize Standard_D1 |
  Set-AzureRmVMOperatingSystem -Linux -ComputerName $vmName -Credential $cred -DisablePasswordAuthentication |
  Set-AzureRmVMSourceImage -PublisherName Canonical -Offer UbuntuServer -Skus 14.04.2-LTS -Version latest |
  Add-AzureRmVMNetworkInterface -Id $nic.Id

# Configure SSH Keys
$sshPublicKey = Get-Content -Raw "$env:USERPROFILE\.ssh\id_rsa.pub"
Add-AzureRmVMSshPublicKey -VM $vmConfig -KeyData $sshPublicKey -Path "/home/azureuser/.ssh/authorized_keys"
```

### <a name="create-the-virtual-machine"></a><span data-ttu-id="43608-162">仮想マシンの作成</span><span class="sxs-lookup"><span data-stu-id="43608-162">Create the virtual machine</span></span>

<span data-ttu-id="43608-163">これで、VM 構成オブジェクトを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="43608-163">Now we can create the VM using the VM configuration object.</span></span>

```azurepowershell-interactive
New-AzureRmVM -ResourceGroupName $resourceGroup -Location $location -VM $vmConfig
```

<span data-ttu-id="43608-164">VM が作成されたら、その VM のパブリック IP アドレスを SSH で使用し、新しい Linux VM にログオンすることができます。</span><span class="sxs-lookup"><span data-stu-id="43608-164">Now that the VM has been created, you can log on to your new Linux VM using SSH with the public IP address of the VM you created:</span></span>

```bash
ssh xx.xxx.xxx.xxx
```

```output
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

## <a name="creating-other-resources-in-azure"></a><span data-ttu-id="43608-165">その他の Azure リソースを作成する</span><span class="sxs-lookup"><span data-stu-id="43608-165">Creating other resources in Azure</span></span>

<span data-ttu-id="43608-166">ここまでは、リソース グループ、Linux VM、Windows Server VM の作成方法を見てきました。</span><span class="sxs-lookup"><span data-stu-id="43608-166">We've now walked through how to create a Resource Group, a Linux VM, and a Windows Server VM.</span></span> <span data-ttu-id="43608-167">そのほかにも、さまざまな種類の Azure リソースを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="43608-167">You can create many other types of Azure resources as well.</span></span>

<span data-ttu-id="43608-168">たとえば、新しく作成した VM に関連付けるための Azure ネットワーク ロード バランサーを作成するには、次のコマンドを使います。</span><span class="sxs-lookup"><span data-stu-id="43608-168">For example, to create an Azure Network Load Balancer that we could then associate with our newly created VMs, we can use the following create command:</span></span>

```azurepowershell-interactive
New-AzureRmLoadBalancer -Name MyLoadBalancer -ResourceGroupName myResourceGroup -Location westeurope
```

<span data-ttu-id="43608-169">また、次のコマンドを使って、インフラストラクチャ用に新しいプライベート仮想ネットワーク (Azure では通常 "VNet" と呼ばれます) を作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="43608-169">We could also create a new private Virtual Network (commonly referred to as a "VNet" within Azure) for our infrastructure using the following command:</span></span>

```azurepowershell-interactive
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 10.0.0.0/16
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName myResourceGroup -Location westeurope `
  -Name MYvNET3 -AddressPrefix 10.0.0.0/16 -Subnet $subnetConfig
```

<span data-ttu-id="43608-170">Azure と Azure PowerShell の優れている点は、それらを使ってクラウドベースのインフラストラクチャを実現できるだけでなく、管理対象となるプラットフォーム サービスを作成できることです。</span><span class="sxs-lookup"><span data-stu-id="43608-170">What makes Azure and the Azure PowerShell powerful is that we can use it not just to get cloud-based infrastructure but also to create managed platform services.</span></span> <span data-ttu-id="43608-171">その管理されたプラットフォーム サービスにインフラストラクチャを組み合わせることで、さらに強力なソリューションを構築することもできます。</span><span class="sxs-lookup"><span data-stu-id="43608-171">The managed platform services can also be combined with infrastructure to build even more powerful solutions.</span></span>

<span data-ttu-id="43608-172">たとえば Azure PowerShell を使って Azure AppService を作成することができます。</span><span class="sxs-lookup"><span data-stu-id="43608-172">For example, you can use the Azure PowerShell to create an Azure AppService.</span></span> <span data-ttu-id="43608-173">Azure AppService は、管理されたプラットフォーム サービスであり、インフラストラクチャには一切気を遣わずに Web アプリをホストできるのが特徴です。</span><span class="sxs-lookup"><span data-stu-id="43608-173">Azure AppService is a managed platform service that provides a great way to host web apps without having to worry about infrastructure.</span></span> <span data-ttu-id="43608-174">Azure AppService の作成後、次のコマンドを使って AppService 内に 2 つの新しい Azure Web アプリを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="43608-174">After creating the Azure AppService, you can create two new Azure Web Apps within the AppService using the following commands:</span></span>

```azurepowershell-interactive
# Create an Azure AppService that we can host any number of web apps within
New-AzureRmAppServicePlan -Name MyAppServicePlan -Tier Basic -NumberofWorkers 2 -WorkerSize Small -ResourceGroupName myResourceGroup -Location westeurope

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
New-AzureRmWebApp -Name MyWebApp43432 -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westeurope
New-AzureRmWebApp -Name MyWebApp43433 -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westeurope
```

## <a name="listing-deployed-resources"></a><span data-ttu-id="43608-175">デプロイされているリソースの一覧表示</span><span class="sxs-lookup"><span data-stu-id="43608-175">Listing deployed resources</span></span>

<span data-ttu-id="43608-176">Azure 内で実行されているリソースは、`Get-AzureRmResource` コマンドレットを使って一覧表示することができます。</span><span class="sxs-lookup"><span data-stu-id="43608-176">You can use the `Get-AzureRmResource` cmdlet to list the resources running in Azure.</span></span> <span data-ttu-id="43608-177">先ほど新しいリソース グループに作成したリソースを表示する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="43608-177">The following example shows the resources we just created in the new resource group.</span></span>

```azurepowershell-interactive
Get-AzureRmResource |
  Where-Object ResourceGroupName -eq myResourceGroup |
    Select-Object Name,Location,ResourceType
```

```output
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

## <a name="deleting-resources"></a><span data-ttu-id="43608-178">リソースの削除</span><span class="sxs-lookup"><span data-stu-id="43608-178">Deleting resources</span></span>

<span data-ttu-id="43608-179">Azure アカウントをクリーンアップするために、この例で作成したリソースを削除しましょう。</span><span class="sxs-lookup"><span data-stu-id="43608-179">To clean up your Azure account, you want to remove the resources we created in this example.</span></span> <span data-ttu-id="43608-180">不要になったリソースは、`Remove-AzureRm*` コマンドレットを使って削除できます。</span><span class="sxs-lookup"><span data-stu-id="43608-180">You can use the `Remove-AzureRm*` cmdlets to delete the resources you no longer need.</span></span> <span data-ttu-id="43608-181">作成した Windows VM を削除するには、次のコマンドを使います。</span><span class="sxs-lookup"><span data-stu-id="43608-181">To remove the Windows VM we created, using the following command:</span></span>

```azurepowershell-interactive
Remove-AzureRmVM -Name myWindowsVM -ResourceGroupName myResourceGroup
```

<span data-ttu-id="43608-182">リソースを削除してよいか確認するメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="43608-182">You will be prompted to confirm that you want to remove the resource.</span></span>

```output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

<span data-ttu-id="43608-183">多数のリソースを一度に削除することもできます。</span><span class="sxs-lookup"><span data-stu-id="43608-183">You can also use the delete many resources at one time.</span></span> <span data-ttu-id="43608-184">たとえば次のコマンドを実行すると、この概要チュートリアルのすべてのサンプルで使ってきたリソース グループ ("MyResourceGroup") が完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="43608-184">For example, the following command deletes all the resource group "MyResourceGroup" that we've used for all the samples in this Get Started tutorial.</span></span> <span data-ttu-id="43608-185">リソース グループだけでなく、そこに含まれるリソースもすべて削除されます。</span><span class="sxs-lookup"><span data-stu-id="43608-185">This removes the resource group and all of the resources in it.</span></span>

```azurepowershell-interactive
Remove-AzureRmResourceGroup -Name myResourceGroup
```

```output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

<span data-ttu-id="43608-186">このコマンドは、完了までに数分かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="43608-186">This can take several minutes to complete.</span></span>

## <a name="get-samples"></a><span data-ttu-id="43608-187">サンプルを入手する</span><span class="sxs-lookup"><span data-stu-id="43608-187">Get samples</span></span>

<span data-ttu-id="43608-188">Azure PowerShell の使用方法について詳しくは、[Linux VM](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json)、[Windows VM](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json)、[Web Apps](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json)、[SQL Database](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json) 用の一般的なスクリプトが用意されているので、そちらをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="43608-188">To learn more about ways to use the Azure PowerShell, check out our most common scripts for [Linux VMs](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Windows VMs](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Web Apps](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), and [SQL Databases](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json).</span></span>

## <a name="next-steps"></a><span data-ttu-id="43608-189">次の手順</span><span class="sxs-lookup"><span data-stu-id="43608-189">Next steps</span></span>

* [<span data-ttu-id="43608-190">Azure PowerShell を使用してサインインする</span><span class="sxs-lookup"><span data-stu-id="43608-190">Sign in with Azure PowerShell</span></span>](authenticate-azureps.md)
* [<span data-ttu-id="43608-191">Azure PowerShell による Azure サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="43608-191">Manage Azure subscriptions with Azure PowerShell</span></span>](manage-subscriptions-azureps.md)
* [<span data-ttu-id="43608-192">Azure PowerShell を使って Azure にサービス プリンシパルを作成する</span><span class="sxs-lookup"><span data-stu-id="43608-192">Create service principals in Azure using Azure PowerShell</span></span>](create-azure-service-principal-azureps.md)
* <span data-ttu-id="43608-193">以前のリリースからの移行については、リリース ノート ([ https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes](https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes)) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43608-193">Read the Release notes about migrating from an older release: [https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes](https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes).</span></span>
* <span data-ttu-id="43608-194">コミュニティに質問する:</span><span class="sxs-lookup"><span data-stu-id="43608-194">Get help from the community:</span></span>
  * [<span data-ttu-id="43608-195">MSDN の Azure フォーラム</span><span class="sxs-lookup"><span data-stu-id="43608-195">Azure forum on MSDN</span></span>](http://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [<span data-ttu-id="43608-196">stackoverflow</span><span class="sxs-lookup"><span data-stu-id="43608-196">stackoverflow</span></span>](http://go.microsoft.com/fwlink/?LinkId=320213)
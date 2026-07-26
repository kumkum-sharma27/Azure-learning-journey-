# Azure Virtual Machine Deployment

## Objective

Deploy a Windows Virtual Machine in Microsoft Azure Portal.

## Azure Services Used

- Virtual Machine
- Resource Group
- Virtual Network
- Network Security Group
- Public IP Address

## Steps Performed

1. Created Resource Group
2. Created Windows Virtual Machine
3. Configured Networking
4. Connected using RDP
5. Verified successful deployment

## Deployment Screenshot

![Azure VM](azure-vm.png)

## Outcome

Successfully deployed a Windows Virtual Machine in Azure.


## Deployment Screenshots

### Azure VM Running

![Azure VM Running](../images/vm-overview.png)

The Azure virtual machine was successfully created and is in the **Running** state.

### SSH Connection

![SSH Connected](../images/ssh-connected.png)

Successfully connected to the Ubuntu virtual machine using SSH.

## Verification Commands

```bash
hostname
whoami
pwd
```

Example Output

```text
hostname
Kumkums

whoami
kumkums

pwd
/home/kumkums
```

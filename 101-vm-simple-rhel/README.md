# Deployment of OpenLogic CentOS Linux VM (7.5)

<a href="https://portal.azure.cn/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fjessie-pang%2Fazure-quickstart-templates%2Fmaster%2F101-vm-simple-rhel%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>


This template allows deploying a OpenLogic CentOS Linux VM (7.5), using the latest image for the selected CentOS version. This will deploy a Standard D1 VM in the location of your chosen resource group with an additional 100 GiB data disk attached to the VM.

Independently form this template you can deploy a blank CentOS VM using the following Azure CLI commands (adjust parameters as needed):

```
azure config mode arm
azure group create TestCLIRG EastUS
azure vm quick-create TestCLIRG vm1 EastUS Linux RedHat:RHEL:7.2:latest azureuser
```

Note: this template and the above commands use RHEL Pay-As-You-Go VM image which carries an additional charge in addition to the base Linux VM price. Check out [Linux VM pricing](https://www.azure.cn/zh-cn/pricing/details/virtual-machines/#activeTab=#tabContent2-1) for more details.  

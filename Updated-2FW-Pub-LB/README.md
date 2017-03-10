# Azure-2-Firewalls-Public-Load-Balancer

[<img src="http://azuredeploy.net/deploybutton.png"/>](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fgithubusercontent.com%2Fkytx42%2Fmaster%2FAzure%2FUpdated-2FW-Pub-LB%2FazureDeploy.json)


- This template was created to support the deployment of a Public Azure Load Balancer in front of 2 Palo Alto Networks Firewalls.  It supports the following features:
- The 2 firewalls deploys with 4-8 interfaces.  1 MGMT and 3-7 data planes. 
- Static IP addresses are assigned to the interfaces based on the input in the starting ip address fields.
- This template deloys into existing VNETs and storage accounts within the same region.  As a result, the storage account and VNET must be created before deploying this template.

        -The following Storage Account types are supported:
                    -Standard_LRS
                    -Standard_GRS
                    -Standard_RAGRS
                    -Premium_LRS
        -The following VMs are supported:
                    -Standard_D3
                    -Standard_D4
                    -Standard_D3_v2
                    -Standard_D4_v2
                    -Standard_A4
                    -Standard_DS3_v2
                    -Standard_DS4_v2
        -The following VMs Licenses:
                    -Byol
                    -Bundle1
                    -Bundle2
        -The following PAN OS Options:
                    -Latest
                    -7.1.8
                    -7.1.7
        NOTE: Make sure the VMs are supported in the specific Storage Account Type and Azure Region.

# Azure Fundamentals 
## VMs
* In Azure, you are charged for the VM per second
* In Windows, you have an Administrator username and password where as in Linux, you have SSH keys to access the instance
* You need to pay for the Windows  License by default, but can use yours if you already have one 
### Features
* Auto Shutdown option available

## Scaling
* There is a limit to vertical scaling in Azure 
* 96 vCPUs and 384 GB Memory is the upper limit for General Purpose Instances
* Vertical Scaling does ont improve availability (since you're upgrading a one single instance) 
* There is no limit to horizontal scaling

## Security and Governance
* Azure Policy and BluePrint is used for security and Governance

## IaaS 
* Azure Storage offers 5 PB of Storage Capacity 
* Network ingress Costs are free in Azure 

## PaaS
* Azure App Services is a PaaS 
* Includes scaling features, CI/CD, containers, staging and dev environments, etc ...

## Regions
* Usually, there is only one region per country, but in Azure, some countries have multiple regions

### Region Pair
* In Azure, you have something called a region pair, where two regions are paired. And these paired regions have highest speed connections and special treatment during Azure updates 

![](img/region-pairs.png)

### Sovereign Regions
* Sovereign Regions are special clouds not available to the public but associated with the Government. You need special permissions/approval to connect to those cloud regions

## Availability Zones
* Not every region in Azure support AZs
* There are 3 types of services in Azure:
    * **Zonal**: You deploy services to a speicific AZ and duplicate it to other AZs for backup and availability
    * **Zone-Redundant**: Azure automatically deploys across multiple AZs in the region
    * **Always Available**: Services deployed globally across multiple regions such as the Azure Active Directory

## Resource, Resource Groups and Subscriptions

### Resource Groups
* Resources can be grouped with Resource Groups. RGs are associated with a region but it can contain resources from different regions.
* Each Resource **must** belong to **only one** resource group
* Permissions can be assigned at the resource group level
### Subscriptions
* Subscription is a billing unit in Azure
* There is a payment method associated with each subscription
* Subscription Plans include Free Plan, Pay-As-You-Go, Enterprise Agreement ....
* Subscriptions are usually used to seperate out diff depts in a business, Ex: Finance, IT, Sales.... OR seperate by Geography NA, Europe, Asia

![](img/rg-hierarchy.png)

### Management Groups
* Management Groups are used to group multiple subscriptions
![](img/management-groups.png)
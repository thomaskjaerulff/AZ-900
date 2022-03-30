# Azure Core Services

## Core Azure Architectural Components
- Azure is a distributed cloud offering with data centers located in many geographical regions across the world.

- Global distribution means serving customer close to where their users are.

### Geographies and Regions
- Data centers are distributed into various geographies.

- Within each geography are Azure regions.

- Within a region is a grouping of data centers which provide redundancy and availability for services hosted within that region.

- Each region is paired with another in the same geography to allow for replication and prevent natural disasters.

![Geophrahy & Regions](/Assets/geograph-regions.png)

### Availability Zones
- An availability zone is a physically separate zone within a region.

- An availability zone encompasses separate power, networking, and colling, and is intented to guard again data loss or outages caused by failure in any of these categories. 

- Azure includes two categories of services that support availability zones: 
    - Zonal services
    - Zone-redundant services

### Resources and Resource Groups
- Azure resources are manageable items in Azure sunch as virtual machines, databased, virtual networks, and storage accounts. 

- Resource groups are logical containers for one or more resources.

- Use locks on resource groups to prevent deletion. 

- When a resource group is deleted, all the resources in that resource group is also deleted. 

- A resource can exist in only one group (no nesting), but you can add or remove a resource to or from the group as needed. You can also move resources from one group to another. 

- You can use the Azure portal, PowerShell, Azure CLI, or an Azure Resource Manager template to create a resource group.

- You can apply tags to a resource group.

### Azure Resource Manager
- Azure Resource Manager (ARM) is the service that enables you to manage resources, serving as the deployment and management service for Azure.

- Example: when you create a VM in the Azure portal, the portal sends the properties to the ARM application programming interface (API). ARM then communicates with the resource provider to create the VM.

- ARM supports the use of templates (JSON) to automate the deployment of an entire azure environment. 

## Azure Subscriptions and Billing Scope

### Azure Subscriptions
- An azure subscription serves as a logical container for your azure resources but at a higher level.

- Think of a subscription as a big box that contains all your resource group boxes. 

- In a simple azure environment, you are likely to have a single azure subscription. 

- You might want to use multiple azure subscriptions to simplify resource management, billing, and cost containment.

- Azure subscriptions also represents a payment agreement.

### Azure Billing Accounts
- A billing account is a mechanism that you use to pay for Azure services.

- You manage invoices and payments with your billing account, as well as track costs.
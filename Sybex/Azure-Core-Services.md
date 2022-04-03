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

### Billing Scope
- An Azure billing scope is a node within a billing account that enables you to manage invoices, payments, accounts, and other Azure billing-related data.

### Azure Tenants
- An Azure tenant is a specific instance of Azure Active Directory (AAD) that contains accounts and groups.

- In simpler terms, a tenant is a group of users.

- A multitenancy implementation is one in which more than one tenant share Azure resources.

- You can use a single tenant for multiple Microsoft cloud offerings. 

## Core Azure Services

### Virtual Machines
- A virtual machine is an emulation of a computer system that provides the functionality of a physical computer.

- The physical machine that runs the VM is often referred to as the host. The VM is a guest on that host. Software called a hypervisor manages the VM's running on the host. 

- Scalability is another advantage to using VMs. 

- VMs can be moved easily from one host to another because they are software 
based.

### Virtual Machine Scale Sets
- Azure virtual machine scale sets is an orchestrator for Azure virtual machines. 

- Azure virtual machine scale sets let you create and manage a group of identical, load balanced VMs. The number of VM instances can automatically increase or decrease in response to demand or a defined schedule. Scale sets provide high availability to your applications, and allow you to centrally manage, configure, and update a large number of VMs. With virtual machine scale sets, you can build large-scale services for areas such as compute, big data, and container workloads.

- A virtual machine scale set simplifies creating and managing a group of load-balanced VMs.

- Scale sets therefore enable high availability for your VMs and the services that rely on them. It makes it very simple to manage many VMs.

### Availability Sets
- An availability set is a group of virtual machines that are deployed across fault domains and update domains. Availability sets make sure that your application is not affected by single points of failure, like the network switch or the power unit of a rack of servers.

- Availability sets halps you avoid potential outages caused by hardware issues, updates or other events. 

- Two elements that enable availability sets are update domains and fault domains. A fault domain is a logical grouping of hardware that shares a power source and network switch, similar to a physical rack in a data center. An update domain is a logical group of hardware that undergoes maintenance activities or 
reboot events at the same time.

### Azure App Services
- The Azure App Service is a PaaS offering that enables you to quickly develop and deploy 
web applications.

- Supports many development languages, including .NET, Java, Ruby, and Python, among others. 

- Web apps deployed using Azure App Service run and scale on Windows and Linux environments. 

### Azure Container Instances (ACI)
- Docker is an open source project for automating the deployment of containers, and Docker containers provide a means for packaging and deploying applications virtually.

- The container serves as a virtual environment that included the resources necessary for its hosted application to function.

- Containers provides only the resources needed by the application so that you only need to deploy an image to the container, rather than build a VM and manage the OS and other resources. 

- You focus solely on the application. 

- ACI supports both Windows and Linux containers.

![Container Groups](/Assets/container-groups.png)

### Azure Kubernetes Service (AKS)
- AKS is a container orchestration service that monitors container health, provides container scalability, and enables resource sharing among containers in a Kubernetes cluster. 

- Each of the containers in a Kubernetes cluster is called a node. 

### Windows Virtual Desktop (WVD)
- WVD is an Azure services that enables users to run a Windows client in the cloud. 

## Core Azure Storage
### Blob Storage
- Azure Blob storage is optimized to store very large amounts of unstructured data such as text and binary data. 

- Can be accessed through HTTP or HTTPS, the Azure Storage REST API, Azure PowerShell, Azure CLI, or an Azure Storage client library.

- Good for storing either many or large files. 

### Blob Storage Tiers
- Consider how you will access data to determine which storage solution is right for you. Access data frequently or seldom. 

- Azure Storage provides three access tiers: 
    - Hot access: Optimized for storing frequently accessed data. 
    - Cool access: Optimized for data that you access infrequently. 
    - Archive access: Intended for data that you rarely access, if at all. 

### Disk Storage
- Azure disks are virtualized storage presented as a disk and attached to a virtual machine, much like a physical disk in a server.

### File Storage
- Azure Files store files that are available securely from anywhere in the world but not associated with a specific VM or volume letter. 

- Can be accessed using SMB or NFS protocol. 

### Storage Accounts
- Before using storage in Azure, you must create a storage account.

- There are several types of storage accounts: 
    - General-purpose v1: 
    - General-purpose v2:
    - BlockBlobStorage:  
    - FileStorage: 
    - BlobStorage: 

## Core Data Services
### Structured and Unstructured Data
- Structured data is defined by a schema that determines the characteristics and types of data stored in a data set. (Ex. relational database like SQL Server is an example of structured data). 

- Unstructured data does not have a defined structure and is not organized in a predefined way. 

### Azure SQL Database
- Azure SQL Database abstracts all the infrastructure needed to host a SQL database.

- A PaaS offering. 

### SQL Managed Instance
- SQL Managed Instances offers many of the same benefits as the Azure SQL Database service. 

- SQL Managed Instances also offers additional features for auditing, authentication, backups, etc. 

### Cosmos DB
- Azure Cosmos DB is a multimodel database service that enables you to scale data out to multiple Azure regions across the world. 

- Makes data readily available to your users worldwide. 

- Provides excellent elasticity. 

### Azure Database for MySQL
- Azure Database for MySQL gives you the capability to deploy, manage, and use MySQL 
databases without deploying MySQL on a server or VM. 

- If you see a reference to LAMP, think MySQL. 

### Azure Database for PostgreSQL
- Azure Database for PostgreSQL is an Azure-based implementation of PostgreSQL that supports the PostgreSQL database engine with the scalability, elasticity, high availability, and other cloud features you would expect from an Azure service. 

### Azure Database Migration Service
- Azure Database Migration Service supports a variety of database migration scenarios for both one-time (offline) and continuous synchronization (online) migrations.

## Microsoft Marketplace
- Like many Microsoft offerings, third-party providers supplement Microsoft’s cloud offerings. 

- These offerings are available through the Microsoft Marketplace, which encompasses two online stores: Microsoft AppSource and Azure Marketplace. 

- Microsoft AppSource offers business solutions for Azure, Dynamics 365, Microsoft 365, web apps, and Power Platform. 

- Azure Marketplace is an online store that enables you to find and purchase a variety of Azure solutions and managed services. Think of Google Play or App Store. 
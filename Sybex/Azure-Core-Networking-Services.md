# Azure Core Networking Services

## Networking Concepts
### Client-Server and Servless Computing
- Servers hosting applications/services that were consumed by client systems (desktop, notebooks, and mobile devices). 

- Servers are either physical or virtual.

- Serverless computing means that the server is abstracted and the service becomes the primary focus. 

### Network Addressing
- Each device on a network, whether physical or virtual needs a unique identification that enables other devices and services to communicate with it. 

- Think of network addresses as a street address and subnets as describing a specific street in the neighborhood. 

- The network address identifies your device uniquely on its network. 

- Computers have no problem using numbers for addresses, but people do. That is where the Domain Name System (DNS) comes into play. 

### Domain Name System
- Domain Name System (DNS) maps numeric IP addresses to hostnames that are more easily recognized and understood by people. 

- Fx., DNS maps the hostname www.microsoft.com to an IP address of 23.35.205.40. 

- A DNS resolver on your computer communicates with a DNS server whose job is to look up addresses associated with hostnames. 

- Like asking "What's the street address for Thomas Kjærulff, Fuglsangvej 46, 2830 Virum"?

-  The key point is that client applications communicate with DNS servers to obtain the IP addresses associated with hosts like web servers, database servers, printers, and other network resources. The client applications then communicate with those hosts using their IP addresses. Likewise, servers and server applications communicate with one another using IP addresses that they obtain by looking up the 
address from a DNS server.

### Routing
- Networks are segmented into subnets (subnetworks), much like buildings are organized by their streets. 

- Wireless access points function as routers, routing data between the two subnets that host the local network. 

- The public addresses are owned and managed by Microsoft, and 
the private addresses are assigned and managed by you. 

## Virtual Networks
- Virtual Networks (VNets) is a core concept in Azure that enables virtual machines and other services to communicate among themselves with the internet, and in the case of a hybrid environment, with your on-premises networks. 

- When you create a VNet, you specify the private IP address space. 

- A VNet is scoped to a single region and a single subscription. 

- Use Virtual Network peering to connect virtual networks acress regions. 

## Load Balancers
- Load balancing refers to distributing network traffic across multiple resources to improve responsiveness, reliability, and availability. 

- If you deploy a web application with three web servers, you will use a load balancer to distribute the traffic among the three web servers.

- Azure offers three load balancing services: 
    
    - Azure Traffic Manager: routes traffic to the data center that is geographically closest to the user. 
    - Azure Front Door: provides the same capability as traffic manager, but it offers additional features for global deployment of web applications.
    - Azure Application Gateway: performs URL-based routing across multiple instances.
    - Azure Load Balancer: the service you would choose to balance traffic evenly across multiple virtual machines based on IP address.  


## VPN Gateway
- A VPN establishes an encrypted tunnel between two private networks across a public network. 

- For example, you can establish a secure connection between your on-premises data center and your resources in Azure. 

- One option for creating a VPN connection to Azure is to use the Azure VPN Gateway service. 

- Azure VPN Gateway enables you to create VPN connections between Azure virtual networks and between Azure and your on-premises network. 

    - Site-to-site
    - Multi-site
    - Point-to-point
    - VNet-to-VNet

### ExpressRoute
- Azure ExpressRoute enables you to extend your on-premises networks into Azure over a private connection managed by a third-party connectivity provider.

## Content Delivery Networks
- Azure Content Delivery Network (CDN) places web content across a distributed network of servers to make that content readily available to users based on their location.

- You place files in CDN's that has a point of presence (PoP). When users access those files, they come from a cached copies in the CDN. 

- This service reduces latency and improves performance. 

- Each file in the CDN has a time-to-live (TTL) property that determines when the file should be refreshed from the source to the cache. 

- Azure CDN supports CDN caching rules, compression, geofiltering, scalability, and several other features.
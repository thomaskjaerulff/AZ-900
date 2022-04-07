# Azure Security Groups | Network and Application Security Groups (NSG, ASG)

## Network Security Groups
- Designed to **filter traffic** to (inbound) and from (outbound) Azure resources located in - Azure Virtual Network
- Filtering controlled by **rules**
- Ability to have **multiple** inbound and outbound **rules**
- Rules are created by specifying
    - **Source/Destination** (IP addresses, service tags, application security groups)
    - **Protocol** (TCP, UDP, any)
    - **Port** (or Port Ranges, ex. 3389 – RDP, 22 – SSH, 80 HTTP, 443 HTTPS)
    - **Direction** (inbound or outbound)
    - **Priority** (order of evaluation)

## Application Security Groups
- Feature that allows **grouping of virtual machines** located in Azure virtual network
- Designed to **reduce** the **maintenance effort** (assign ASG instead of the explicit IP address)
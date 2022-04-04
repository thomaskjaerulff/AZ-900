# Security, Compliance, Privacy, and Trust

## Network Security
### Defense in Depth
- Defense in depth defines a strategy for multiple layers of defense to protect your facilities, data, services, and users from compromise.

### Azure Firewall
- A firewall is a service that inspects network traffic flowing through it and applies actions to that traffic based on rules you specify. 

- For example, if the only endppoints that you need to serve to your users are HTTP (port 80) and HTTPS (port 443), you would create a rule in your firewall to block all traffic inbound for ports other than 80 and 443. 

- Azure firewall supports three types of rule collections: 
    - NAT rules
    - Network rules
    - Application rules

- Consider Azure Firewall whenever you need to filter traffic based on source IP address and port, destination address and port, and/or protocol. 

### Web Application Firewall
- Azure Web Application Firewall (WAF) is a firewall service that you can deploy with each of the the VPN services to provide firewall services specifically for your web applications. 

- WAF protects your web applications against common vulnerabilities and exploits. 

- WAF works in concert with Application Gateway, Front Door, and CDN, and it is specific to web application scenarios.

### Network Security Groups
- Network Security Groups (NSGs) are an additional firewall service offered in Azure. 

### Application Security Groups
- An application security group (ASG) enables you to group servers based on the application running them and manage security for them as a group. 

## Authentication and Authorization
### Azure Active Directory
- Azure Active Directory (Azure AD) is Microsoft's cloud-based identity and access management service. 

- If you subscribe to Microsoft 365, Office 365, Azure, or Dynamics 365, you already have Azure AD because these subscriptions automatically get an Azure AD tenant with access to all of the free Azure AD services offered by Microsoft.

- You have the following plans available: 
    - Azure Active Directory Free
    - Azure Active Directory Premium P1
    - Azure Active Directory Premium P2

- Azure AD can be your sole directory service or you can integrate with on-premises AD for hybrid cloud scenarios involving on-premises and cloud services by deploying Active Directory Federation Services (ADFS).

- Azure Active Directory supports role-based access control (RBAC).

- Use RBAC in Azure, you create a role assignment that consists of: 
    - Security Principal
    - Role
    - Scope

### Authentication and Authorization
- Authentication identifies a user (who are you?). 

- Authorization determines that actions that an authenticated user can perform (what can you do?).

### Azure Multifactor Authentication
- Multifactor authentication (MFA) is a mechanism that uses more than one factor to authenticate. 

- MFA increases security by requiring a second form of verification. 

### Conditional Access
- Conditional enabled you to use various identity signals to allow or deny access to Azure resources.

- For an example rules based on the user's location, device or the application the user is trying to access. 

### Single Sign-On (SSO)
- Single sign-on (SSO) enables you to use a single set of credentials to access multiple resources. 

## Security Tools and Features
### Azure Security Center
- Azure Security Center is a monitoring service that provides a framework for advanced threat protection of your IT workloads both in the cloud and on-premises. 

- Security Center integrates with Microsoft Defender). 

- Two service levelse: 
    - Free
    - Standard

### Azure Key Vault
- Azure Key Vault enables you to securely store secrets such as tokens, passwords, certificates, cryptographic key, and API keys. 

- Instead of storing the credentials in your custom application, you would store the credentials in Azure Key Vault.

- By storing secrets in Key Vault, you gain the capability to easily monitor and audit access.

### Azure Information protection
- Azure Information Protection (AIP) enables you to classify and protect documents and emails by applying labels to them. 
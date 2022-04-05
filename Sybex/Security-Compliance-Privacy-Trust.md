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

### Azure Advanced Threat Protection
- Azure Advanced Threat Protection (ATP) leverages your on-premises Active Directory to detect and identify threats directed at your organization.

### Azure Sentinel
- Azure Sentinel collects data across your enterprise from users, devices, applications, and infrastructure on-premises and in the cloud, including from multiple clouds. 

- It uses a combination of built-in analytics, leveraging information about known threats, machine learning, and other criteria to automatically detect threats.

- Azure Sentinel uses analytics to correlate alerts from across the environment into incidents, enabling you to track and act on possible threats rather than individual alerts. 

## Azure Governance Methodologies
- Governance describes policies and methods that control how a service is used, roles and responsibilities within the service, and how it should be secured. 

### Azure Policies
- Azure policies define business rules that you can use to assess and ensure compliance with organizational standards in Azure, controlling how Azure resources are deployed and used. 

### Azure Initiatives
- An Azure initiative is a group (collection) of Azure policies. 

### Role-Based Access Control
- Role-based access control (RBAC) is a primary authorization mechanism in Azure that enables you to define who has access to Azure resources and what they can do with those resources. 

- To apply RBAC, you first create a role assignment, which consists of three elements that effectively translate to who, what, and where:
    - Security principal
    - Role definition
    - Scope

- Roles are divided into three types: classic subscription administrator roles, Azure roles, and Azure AD roles. 

- Classic subscription administrator roles include the following: 
    - Account Administrator
    - Service Administrator
    - Co-Administrator

- Azure RBAC adds more granularity to permission assignment in Azure with over 70 built-in roles. 

- For the purposes of the AZ-900 exam, let’s focus on the following four roles:
    - Owner
    - Contributor
    - Reader
    - User Access Administrator

### Resource Locks
- Azure gives you the ability to lock down resources. Resource locks enable you to apply that control. 

- You can apply a ReadOnly or CanNotDelete lock. 

- If you need to delete a resource, you must first remove the lock. Then you can delete the resource. 

### Azure Blueprints
- Azure Blueprint lets you define a repeatable group of Azure resources and associated role assignments and policies to meet your organization’s standards and practices, and then quickly and easily deploy those resources where needed.

- Resource groups, role assignments, policies, and ARM templates are the artifacts within a blueprint that define its structure and enable a potentially large number of resources to be deployed collectively and in a controlled, standardized way.

- ARM templates retain no connection to the resources they deploy. Blueprints do maintain that connection, so you can track and audit what was deployed against what the blueprint specified should be deployed.

- A blueprint is in draft mode until you publish it using a version designation that you define. Once published, a blueprint is available for assignment. Assigning a blueprint deploys the artifacts defined in the blueprint.

### Microsoft Cloud Adoption Framework for Azure
- The Cloud Adoption Framework for Azure is a large collection of resources, including documentation, deployment guidance, templates, best practice documentation, and various tools to help with planning, deploying, and assessing your Azure deployment. 

## Azure Monitoring and Reporting Options
### Azure Monitor
- Azure Monitor provides the capability to collect and analyze telemetry from your cloud and on-premises environments and to take appropriate actions based on that analysis.

- Azure Monitor encompasses several services: 
    - Application Insights
    - Azure Monitor for VMs
    - Azure Monitor for containers
    - Log Analytics
    - Smart Alerts
    - Automated Actions
    - Dashboards
    - Workbooks

- Azure Monitor uses two types of data: 
    - Metrics: Describe some aspect of a system at a given time using numerical values. 
    - Logs:  contain a record of events that happen within a system.

- Monitoring begins automatically as soon as you add a resource to a subscription. 
- Metrics and logs are created for you automatically. 
- Application Insights enables developers to send telemetry data about the applications they develop to Azure. 
- Metrics are numeric values that describe how a resource is performing and/or what it is consuming.
- Logs contain detailed information about events that happen within your Azure environment.
- Log Analytics enables you to view data from multiple sources through queries that you create or that are created by services for you, such as On-Demand Assessments. 

### Azure Service Health 
- Azure Service Health keeps you informed regarding planned maintenance and changes, Azure service issues that affect your environment, and issues within your own environment. 

- Azure Service Health provides the following features: 
    - Azure Status
    - Service Health 
    - Resource Health 

- In addition to giving you a customizable dashboard to track the health of Azure services in the regions where your resources are located and get more information about issues, Service Health enables you to set up service health alert. 

- Works with Azure Monitor. 

### Azure Advisor
- Azure Advisor, which you access through the Azure portal, provides a web-based report intended to help you optimize you Azure environment. 

- Captures a wide range of data points across the environment, evaluating performance criteria, costeffectiveness, reliability, security, and operational excellence. 
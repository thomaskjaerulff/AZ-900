# Cloud Adoption Framework for Azure

**Cloud adoption** is a strategic move by an organization to leverage cloud in their business

# Cloud Adoption Framework
Cloud Adoption Framework for Azure is a set of

- **tools**,
- **best practices**,
- **guidelines** and
- **documentation**

prepared by Microsoft to help companies with their cloud adoption journey.

## Strategy
## 1. Understand your motivation
- Answer the question **WHY MOVE**?
- Common Motivation Triggers include
    - **Migration**
        - Cost Savings on infrastructure
        - Reduction in complexity
        - Operation optimization
        - Increased business agility
    - **Innovation**
        - Reaching a global scale
        - Customer experience improvements
        - Transformation of products or services
        - Market disruption
## 2. Business Outcome
- Answer the question **WHAT TO MEASURE?**
- Defined, concise and observable outcome captured by a specific measure, for example
    - Increase in revenue
    - Increase in profit
    - Cost reduction
    - Global access to customers
    - Reaching new markets
## 3. Business Justification
- Answer the question **WHAT’S MY RETURN ON INVESTMENT?**
- Develop a business case to validate the financial model that supports your motivations and outcomes
- Tools that support this process are
    - Azure TCO (Total Cost of Ownership) calculator - estimate current on-prem costs
    - Azure Pricing Calculator - estimate future Azure costs
    - Azure Cost Management - see current Azure costs
## 4. First Project
- Choose first project to validate your strategy (Proof of concept - POC) based on
    - Business Criteria
        - Currently operating
        - Dedicated owner
        - Strong motivation to move
    - Technical Criteria
        - Minimum dependencies and assets
## Plan
1. Digital Estate (INVENTORY OF ASSETS)
    - Review current landscape and list all projects/solutions (digital assets)
    - Choose one of the five (5) R’s of rationalization
        - Rehost - move as is; typically into containers or IaaS (virtual machines)
        - Refactor - make small code changes and move to PaaS (ex. Azure SQL, Azure App Service, etc.)
        - Rearchitect - make complex code changes to introduce new features or fix incompatible apps
        - Rebuild - create a new application using cloud first design
        - Replace - review available SaaS solutions and replace legacy or unneeded applications
2. Initial Organization Alignment
    - Align people so they will support your adoption plan
    - Map people to capabilities
3. Skills Readiness Plan
    - Review current skills and address the gaps
4. Cloud Adoption Plan - combine everything from steps 1 to 3 into a single cloud adoption plan
## Ready
1. Azure Setup Guide - Review the Azure setup guide to become familiar with the tools and approaches you need to use to create a landing zone.
2. Azure Landing Zone - Choose an appropriate Azure Subscription type that best suits your needs and establish an initial Azure environment.
3. Extend Landing Zone - Expand the initial landing zone to fit your business needs.
4. Best Practices - Review everything and ensure best practices are followed.

## Adopt
## Migrate
1. First Migration - migrate your first application to familiarize yourself with the cloud, guidelines and tools
2. Migration Scenarios - review and prepare migration scenarios/guidelines for your company
    - Virtual Machines - Linux, Windows, etc.
    - Apps - Java, .NET, NodeJS web apps, etc.
    - Data - SQL Server, PostreSQL, File Servers, etc.
    - Other - VMware, Azure Stack, etc.
3. Best Practices - address common migration needs through the application of consistent best practices.
4. Process Improvements - important part of this porcess heavy activity is to identify bottlenecks and improve with every migration

## Innovate
1. Business Value Consensus (VALUE TO STRATEGY)
    1. Create hypothetical customer need
    2. Decide on solution that solves it
    3. Map this to your strategy
2. Innovation Guide (TOOLS) - choose available Azure tools that will help your build this application
3. Best Practices - verify that best practices are followed for all tools in the toolchain
4. Process Improvements - gather feedback from the users and the customers to improve architectural decisions and future products

## Govern & Manage
1. Define governance solutions - Choose solutions to maintain compliance, security and ensure total control of the environment.
    - Those solutions should focus to
        - Address Business Needs
        - Provide Agility
        - Control Risks
2. Manage cloud environment (CLOUD OPERATIONS) - Hand over solutions and environment to cloud operations team for maintenance. Team should ensure that stability and costs are always in perfect balance to meet business commitments. Team should allow environment to grow, evolve and adapt to changing business needs.

## Organize
Ensure that everyone knows what to do and when to do it for every stage in this process. One of the ways to achieve this is via RACI (Responsible, Accountable, Consulted, and Informed) matrix.
# Azure Role-based Access Control (RBAC)

## What is a Role?
**Role** (role definition) is a **collection of actions** that **the assigned identity** will be able to perform.
Role definition is an answer to a question "**What** can be done?"

## What is a Security Principal?
**Security Principal** is an Azure object (identity) that can be assigned to a role (ex. users, groups or applications).
**Security Principal assignment** is an answer to a question "**Who** can do it?"

## What is a Scope?
**Scope** is one or more Azure resources that the access applies to.
**Scope assignment** is an answer to a question "**Where** can it be done?"

## What is a Role Assignment?
**Role assignment** is a combination of the **role definition, security principal and scope**.

## Azure Role-based Access Control (RBAC)
- Authorization system built on Azure Resource Manager (ARM)
- Designed for fine-grained access management of Azure Resources
- Role assignment is combination of
    - Role definition – list of permissions like create VM, delete SQL, assign permissions, etc.
    - Security Principal – user, group, service principal and managed identity and
    - Scope – resource, resource groups, subscription, management group
- Hierarchical
    - Management Groups > Subscriptions > Resource Groups > Resources
- Built-in and Custom roles are supported
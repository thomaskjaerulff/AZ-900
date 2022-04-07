# Azure Resource Locks

## What is an Azure Resource Lock?
- Designed to **prevent accidental deletion** and/or **modification**
- Used in conjunction with RBAC
- Two types of locks
    - **Read-only (ReadOnly)** – only read actions are allowed
    - **Delete (CanNotDelete)** – all actions except delete are allowed
- Scopes are **hierarchical (inherited)**
    - Subscriptions > Resource Groups > Resources
- **Management Groups** can’t be locked
- Only **Owner** and **User Access Administrator** roles can manage locks (**built-in** roles)
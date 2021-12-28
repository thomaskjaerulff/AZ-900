# Azure Policy

- Designed to help with resource **governance, security, compliance, cost management**, etc.
- **Policies** focus on **resource properties** (**RBAC** focused on **user actions**)
- Policy **definition** – Defines what should happen
    - Define the **condition** (if/else) and the **effect** (deny, audit, append, modify, etc.)
    - Examples include allowed resource types, allowed locations, allowed SKUs, inherit resource tags
- **Built-in** and **custom** policies are supported
- Policy **initiative** – a **group** of policy definitions
- Policy **assignment** – assignment of a policy definition/initiative to a scope
    - Scopes can be assigned to
        - management groups,
        - subscriptions,
        - resource groups, and
        - resources
- Policies allow for **exclusions of scopes**
- Checked during **resource creation** or **updates** and **existing ones with remediation tasks**
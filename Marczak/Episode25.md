# Azure Identity Services | Authentication, Authorization & Active Directory (AD)

## Identity
- A user with a username and password.
- Also applications or other servers with secret keys or certificates.
- The fact of being something or someone.

## Authentication
The process of **verification/assertion** of identity

## Authorization
The process of **ensuring** that only **authenticated identities** get access to the resources for which they have been granted access.

## Access Management
The process of **controlling**, **verifying**, **tracking** and **managing access** to authorized users and applications.

## Azure Active Directory
- Identity and Access Management service in Azure
- Identities management – users, groups, applications
- Access management – subscriptions, resource groups, roles, role assignments, authentication & authorization settings, etc.
- Used by multiple Microsoft cloud platforms
    - Azure
    - Microsoft 365
    - Office 365
    - Live.com services (Skype, OneDrive, etc.)

## Multi-factor Authentication (MFA)
- Process of authentication using more than one factor (evidence) to prove identity
- Factor types
    - Knowledge Factor – “Something you know”, ex. password, pin
    - Possession Factor – “Something you have”, ex. phone, token, card, key
    - Physical Characteristic Factor – “Something you are”, ex. fingerprint, voice, face, eye iris
    - Location Factor – “Somewhere you are”, ex. GPS location
- Supported by Azure AD by default (simple on-off switch)
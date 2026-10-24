# Project 01 — Azure Fundamentals

## Objective

Build a foundational Microsoft Azure environment and understand how Azure organizes, monitors, secures, and governs cloud resources.

This lab focused on learning the concepts behind each configuration rather than simply creating resources.

## Environment

- Microsoft Azure
- Region: East US
- Resource Group: `rg-azure-fundamentals`
- Storage Account: Standard / LRS
- Private Blob Storage container

## Lab Architecture

Azure Subscription  
↓  
Resource Group  
↓  
Storage Account  
↓  
Blob Container  
↓  
Blob Object

Governance and security controls were applied at the resource-group level.

## Tasks Completed

1. Created an Azure Resource Group
2. Added organizational tags
3. Reviewed Cost Management
4. Reviewed Azure Activity Logs
5. Created an Azure Storage Account
6. Configured Locally Redundant Storage (LRS)
7. Created a private Blob container
8. Uploaded a test blob
9. Created a Delete resource lock
10. Reviewed Azure Policy compliance
11. Reviewed Azure IAM / RBAC

## Key Concepts Learned

### Resource Groups

A Resource Group is a logical container used to organize related Azure resources.

Resource Groups make it easier to manage:

- permissions
- monitoring
- cost tracking
- governance
- lifecycle management

### Tags

Azure tags are name/value pairs used to organize resources.

Example:

`Environment = Lab`

`Project = AzureFundamentals`

Tags can help with ownership, automation, reporting, governance, and cost analysis.

### Azure Storage

Azure Storage provides scalable cloud storage services.

This lab used Blob Storage for object-based data.

Hierarchy:

Storage Account  
→ Blob Service  
→ Container  
→ Blob

### LRS

Locally Redundant Storage maintains multiple copies of data within a single Azure region.

LRS was selected because this is a learning environment and does not require cross-region disaster resilience.

### Activity Log

Azure Activity Log records management-plane operations such as:

- resource creation
- configuration changes
- deletion attempts
- administrative actions

This provides an audit trail for Azure resource management.

### Resource Locks

A Delete lock was configured to help prevent accidental deletion.

Resource locks are useful for protecting important infrastructure from administrative mistakes.

### Azure Policy

Azure Policy evaluates resources against organizational rules and configuration requirements.

Policy answers:

**What configurations are allowed or required?**

This differs from RBAC.

### Azure RBAC

Role-Based Access Control determines:

**Identity + Role + Scope**

RBAC answers:

**Who can do what, and where?**

Common built-in roles include:

- Reader
- Contributor
- Owner

### RBAC vs Azure Policy

**RBAC:** Who can perform an action?

**Azure Policy:** What resource configurations are allowed or required?

## Security Principles Practiced

- Least privilege
- Private storage access
- Governance
- Resource protection
- Audit logging
- Cost awareness
- Role-based access control

## Troubleshooting Performed

During the lab I encountered and resolved:

- Azure Storage navigation differences
- Storage Account validation errors
- Required Blob service selection
- Storage redundancy configuration
- Azure portal navigation and resource-scope differences

Troubleshooting was documented as part of the learning process.

## Skills Demonstrated

- Azure Resource Management
- Azure Storage
- Blob Storage
- Azure Governance
- Azure Policy
- Azure IAM / RBAC
- Azure Activity Logs
- Cost Management
- Resource Locks
- Cloud Security Fundamentals

## Evidence

The project includes screenshots documenting each major configuration step.

Sensitive values such as subscription IDs, tenant IDs, email addresses, and account identifiers are redacted before publication.

## Next Project

**Project 02 — Microsoft Entra ID & Azure RBAC**

Focus areas:

- Identity
- Authentication
- Groups
- RBAC
- Effective access
- MFA
- Conditional Access
- Least privilege

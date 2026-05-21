# Security, Access and Governance

Security, access, and governance come before hands-on Fabric usage.

Microsoft Fabric is a shared analytics platform. Users may interact with reports, semantic models, Lakehouses, pipelines, notebooks, dataflows, warehouses, and institutional data. This means users should understand their responsibilities before they start creating, editing, sharing, or publishing Fabric assets.

This section explains the basic security and access principles that apply before users begin working in Fabric.

## Why security comes first

Fabric makes it easier for users to create analytics assets, but easier creation also means stronger responsibility.

Before using Fabric, users should understand:

- What they are allowed to access
- Which workspace they should use
- What data they are allowed to work with
- Whether the data is public, internal, confidential, or restricted
- What they are allowed to share
- Whether they are working in a sandbox, department, or production workspace
- Who owns the workspace or asset
- When work should remain experimental
- When work requires review before wider use

The aim is not to slow users down. The aim is to help users work safely and consistently.

![Placeholder: Fabric access and governance layers](../assets/images/fabric-access-governance-layers.png)

> Image placeholder: A layered governance diagram showing user access, workspace role, item permission, data sensitivity, sharing control, and production review as connected layers before users work with Fabric assets.

## Core access principles

| Principle | Meaning |
|---|---|
| Least privilege | Users should only receive the access required for their role or learning need |
| Purpose-based access | Access should be granted for a clear business, learning, or project purpose |
| Workspace accountability | Each workspace should have a clear owner or responsible group |
| Data sensitivity awareness | Users should understand whether data is public, internal, confidential, or restricted |
| Controlled sharing | Reports, data, screenshots, and exports should only be shared with authorised users |
| Production control | Production assets should not be changed casually or without review |
| Reuse before duplication | Users should reuse approved assets where appropriate instead of creating unnecessary duplicates |

## Workspace roles

Fabric workspaces use role-based access. The exact permissions may depend on the item and workspace configuration, but users will generally encounter the following roles.

| Workspace Role | Typical Use | General Expectation |
|---|---|---|
| Viewer | Report consumers and users who only need to view approved content | Can view permitted content but should not edit or manage assets |
| Contributor | Analysts, developers, or learners creating content in an assigned workspace | Can create or edit content where permitted |
| Member | Senior contributors, project leads, or trusted collaborators | Can collaborate more broadly and may manage some workspace content |
| Admin | Workspace owner or administrator | Can manage workspace access, settings, and overall workspace governance |

Having a higher workspace role does not mean a user should freely access, export, or share all data. Users must still follow data sensitivity, sharing, and production expectations.

## Data sensitivity expectations

Users should understand the type of data they are working with before uploading, transforming, or sharing it in Fabric.

| Data Category | Example | Expected Handling |
|---|---|---|
| Public | Open datasets, public website information, published statistics | Suitable for demos, training, and sandbox use |
| Internal | Non-public operational information without sensitive personal details | Use within approved internal workspaces and audiences |
| Confidential | Student, staff, finance, donor, HR, or sensitive operational data | Restrict access, apply appropriate controls, and avoid unnecessary sharing |
| Restricted | Highly sensitive records, personal identifiers, or regulated data | Use only with explicit approval and strong controls |

Sandbox workspaces should use mocked, synthetic, public, or approved non-sensitive data.

Real confidential or restricted data should not be uploaded into sandbox workspaces unless explicitly approved.

## Sharing and export expectations

Users should be careful when sharing Fabric content or exporting data.

Before sharing a report, dataset, screenshot, table, file, or workspace item, users should ask:

- Is the recipient authorised to see this information?
- Does the content contain confidential or restricted data?
- Is this an official output or only an experimental sandbox output?
- Is the report or data asset validated?
- Is export allowed for this data?
- Could the screenshot or export be forwarded beyond the intended audience?

Sharing should follow the principle of least privilege. Users should share only what is needed, with only the people who need it.

## Sandbox, department, and production boundaries

Different workspace types carry different expectations.

| Workspace Type | Security Expectation |
|---|---|
| Sandbox Workspace | Use safe data for learning and experimentation. Outputs are not official. |
| Department Workspace | Use for approved department-level exploration and development. Outputs are not automatically production assets. |
| BIA Production Workspace | Reserved for BIA-managed production assets. Changes require stronger control, validation, and review. |

Users should not treat sandbox or department workspace outputs as official production assets unless they have gone through appropriate review.

## External collaborators

External collaborators may require additional review before access is granted.

Before granting access to an external collaborator, consider:

- Why does the external collaborator need access?
- Do they need view-only access or edit access?
- Which workspace should they access?
- What data will they be able to see?
- Is the data confidential or restricted?
- Is a separate license required?
- Should access be time-bound?
- Who is responsible for removing access later?

External collaborator access should be reviewed only when the need arises and should be aligned with licensing, data sensitivity, and workspace governance expectations.

## Minimum checklist before using Fabric

Before doing hands-on work in Fabric, users should confirm:

- [ ] I know which workspace I should use
- [ ] I understand my workspace role
- [ ] I know whether I am in a sandbox, department, or production workspace
- [ ] I know what data I am allowed to use
- [ ] I understand whether the data is public, internal, confidential, or restricted
- [ ] I know whether sharing or export is allowed
- [ ] I know who owns the workspace or asset
- [ ] I understand whether my output is experimental or production-facing
- [ ] I know when to ask for review before wider sharing or production use

## References and further learning

| Resource | Purpose |
|---|---|
| [Microsoft Fabric permission model](https://learn.microsoft.com/en-us/fabric/security/permission-model) | Explains how different Fabric permissions work together to control access to data |
| [Roles in workspaces in Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/fundamentals/roles-workspaces) | Explains workspace roles such as Admin, Member, Contributor, and Viewer |
| [Share items in Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/fundamentals/share-items) | Explains how Fabric item sharing and item permissions work |
| [Secure data access in Microsoft Fabric](https://learn.microsoft.com/en-us/training/modules/secure-data-access-in-fabric/) | Microsoft Learn module on Fabric permissions, workspace permissions, item permissions, and granular permissions |
| [OneLake security access control model](https://learn.microsoft.com/en-us/fabric/onelake/security/data-access-control-model) | Explains how OneLake security interacts with workspace permissions and data access controls |

## Next section

Proceed to:

[Licensing, Capacity and Compute Awareness](../02-licensing-capacity/)

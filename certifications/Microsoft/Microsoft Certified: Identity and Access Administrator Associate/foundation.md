<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Microsoft%20Certified-%20Identity%20and%20Access%20Administrator%20Associate.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Microsoft Certified: Identity and Access Administrator Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Implement and manage user identities](#implement-and-manage-user-identities) (8 questions)
- [Implement authentication and access management](#implement-authentication-and-access-management) (8 questions)
- [Plan and implement identity governance](#plan-and-implement-identity-governance) (7 questions)
- [Plan and implement workload identities](#plan-and-implement-workload-identities) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:16.189Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Implement and manage user identities | 8 |
| Implement authentication and access management | 8 |
| Plan and implement identity governance | 7 |
| Plan and implement workload identities | 7 |

---

### **Implement and manage user identities**

### 1. What is the primary goal of identity lifecycle management?

- [ ] **A)** Access granted precisely when needed and revoked immediately
- [ ] **B)** All users receive permanent administrative access
- [ ] **C)** Passwords remain unchanged for all identities
- [ ] **D)** Licenses are assigned without any verification

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Identity lifecycle management covers onboarding through offboarding and ensures access is granted and revoked at the correct times to prevent ghost accounts.
 
 
</details>

### 2. Which two user attributes are commonly used as the foundation for dynamic groups and ABAC?

- [ ] **A)** Job title
- [ ] **B)** Department code
- [ ] **C)** Home address
- [ ] **D)** Password hash

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Job title and department code are common identity attributes used in dynamic membership rules and attribute-based access control.
 
 
</details>

### 3. An administrator runs the following PowerShell command. What will the command create?

```powershell
New-AzureADMSGroup -DisplayName "Sales Users" -SecurityEnabled $true -MembershipRule "user.department -eq 'Sales'" -MembershipRuleProcessingState "On"
```

- [ ] **A)** Dynamic security group based on department
- [ ] **B)** Static administrative unit
- [ ] **C)** Microsoft 365 group with shared mailbox
- [ ] **D)** Conditional Access policy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command creates a dynamic security group using a membership rule that evaluates the department attribute.
 
 
</details>

### 4. Which tool is used to synchronize on-premises Active Directory identities with Microsoft Entra ID?

- [ ] **A)** Entra Connect
- [ ] **B)** SCIM
- [ ] **C)** Azure RBAC
- [ ] **D)** Application Proxy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Entra Connect handles synchronization of on-premises Active Directory identities to Microsoft Entra ID for hybrid environments.
 
 
</details>

### 5. Which two statements about B2B guest identities are correct?

- [ ] **A)** Guests must have Conditional Access explicitly applied
- [ ] **B)** Guests are invited through B2B collaboration
- [ ] **C)** External users automatically inherit all tenant policies
- [ ] **D)** Guest access is managed through Azure RBAC roles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Guest identities are invited via B2B collaboration and require explicit Conditional Access and governance because tenant policies do not automatically apply to them.
 
 
</details>

### 6. Refer to the following SCIM payload. Which two statements correctly describe it?

```json
{
  "schemas": ["urn:ietf:params:scim:schemas:core:2.0:User"],
  "userName": "jsmith",
  "active": true,
  "emails": [
    { "primary": true, "value": "jsmith@contoso.com", "type": "work" }
  ]
}
```

- [ ] **A)** It defines a user resource with username and email
- [ ] **B)** It follows the SCIM 2.0 schema
- [ ] **C)** It assigns an Azure RBAC role
- [ ] **D)** It creates a Microsoft 365 group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The payload is a SCIM 2.0 user representation containing identity attributes such as username and work email.
 
 
</details>

### 7. What is the purpose of lifecycle workflows in Microsoft Entra ID?

- [ ] **A)** Identity tasks triggered by joiner, mover, or leaver events
- [ ] **B)** Synchronization rule enforcement
- [ ] **C)** Azure subscription management
- [ ] **D)** Network security configuration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Lifecycle workflows automate identity tasks based on organizational events such as joining, moving, or leaving.
 
 
</details>

### 8. Which of the following statements correctly describe the Joiner-Mover-Leaver process?

- [ ] **A)** Joiners receive initial access
- [ ] **B)** Movers receive updated permissions reflecting new roles
- [ ] **C)** Leavers have all access revoked immediately
- [ ] **D)** Leavers only need their account disabled

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> JML requires giving joiners initial access, updating movers' permissions, and revoking leavers' access to prevent orphaned accounts.
 
 
</details>


---

### **Implement authentication and access management**

### 9. Which statement best describes identity lifecycle management in Microsoft Entra ID?

- [ ] **A)** It is the complete journey of an identity from onboarding to offboarding
- [ ] **B)** It only covers password synchronization between systems
- [ ] **C)** It is used exclusively to manage guest users
- [ ] **D)** It is the process of assigning Azure administrator roles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Identity lifecycle management covers the full identity journey, including provisioning as users join and deprovisioning as they leave.
 
 
</details>

### 10. Which directory attributes are commonly used for dynamic group rules and automated provisioning?

- [ ] **A)** Job title
- [ ] **B)** Department code
- [ ] **C)** Manager
- [ ] **D)** Device OS version

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Job title, department code, and manager are standard user attributes used by dynamic rules, ABAC, and provisioning workflows.
 
 
</details>

### 11. The rule shown in the code block determines group membership. How will membership be assigned?

```plaintext
department -eq "Sales"
```

- [ ] **A)** All users in the tenant
- [ ] **B)** Users whose department attribute equals Sales
- [ ] **C)** Only users manually assigned by an administrator
- [ ] **D)** Users with a job title of Sales Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The dynamic rule adds any user whose department attribute equals Sales. Membership is not manual and is based on the department attribute.
 
 
</details>

### 12. What is the primary purpose of SCIM in Microsoft Entra ID?

- [ ] **A)** To exchange user identity information automatically between identity providers and SaaS applications
- [ ] **B)** To replace password-based authentication with certificates
- [ ] **C)** To create an on-premises Active Directory forest
- [ ] **D)** To manage Azure resource permissions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SCIM standardizes user identity exchange between Microsoft Entra ID and SaaS apps, enabling automated provisioning and consistency.
 
 
</details>

### 13. Which activities are part of the Joiner-Mover-Leaver (JML) process?

- [ ] **A)** Joiners receive initial access based on their role
- [ ] **B)** Movers receive updated permissions that reflect their new roles
- [ ] **C)** Leavers have all access revoked immediately
- [ ] **D)** Guests are automatically converted to employee accounts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> JML covers joiners receiving access, movers receiving updated permissions, and leavers being deprovisioned to avoid orphaned accounts.
 
 
</details>

### 14. The configuration in the code block represents a Lifecycle Workflow. Which identity event does it automate?

```json
{
  "trigger": "employeeLeave",
  "tasks": [
    "removeAllAccess",
    "deleteAccount"
  ]
}
```

- [ ] **A)** Employee join
- [ ] **B)** Employee move
- [ ] **C)** Employee leave
- [ ] **D)** Password reset

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The workflow triggers on employeeLeave and removes access and deletes the account, matching offboarding.
 
 
</details>

### 15. What is the main purpose of an Administrative Unit in Microsoft Entra ID?

- [ ] **A)** They delegate administrative permissions over a subset of users, groups, or devices
- [ ] **B)** They create a separate Microsoft Entra tenant
- [ ] **C)** They replace the need for Conditional Access policies
- [ ] **D)** They synchronize on-premises passwords to the cloud

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Administrative Units allow scoped administration, so admins manage only assigned resources without receiving full global privileges.
 
 
</details>

### 16. Which statements accurately reflect how dynamic group membership rules work in Microsoft Entra ID?

- [ ] **A)** Membership changes are not always instantaneous
- [ ] **B)** A required attribute that is null can prevent a user from being added
- [ ] **C)** Rules are processed by the Microsoft Entra ID engine periodically
- [ ] **D)** Membership is updated at the exact moment an attribute changes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Dynamic groups depend on periodic processing, so changes are not immediate; missing or badly formatted attributes can also block membership.
 
 
</details>


---

### **Plan and implement identity governance**

### 17. In the Joiner-Mover-Leaver (JML) process, what is the primary purpose of the Leaver phase?

- [ ] **A)** To assign new permissions based on role changes
- [ ] **B)** To revoke all access and deprovision the identity immediately
- [ ] **C)** To create a guest account for external collaboration
- [ ] **D)** To validate access through periodic recertification

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Leaver phase focuses on immediate deprovisioning and revoking all access when a user leaves. This prevents orphaned accounts and reduces the risk of security vulnerabilities.
 
 
</details>

### 18. Which two actions should be performed when offboarding a user to avoid orphaned or shadow identities?

- [ ] **A)** Revoke access from all SaaS applications through automated provisioning
- [ ] **B)** Disable or delete the identity from the directory
- [ ] **C)** Only revoke the password and keep the account active
- [ ] **D)** Move the user to a different department before removing access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Proper offboarding requires both revoking application-specific access and disabling or deleting the directory identity. Relying only on password revocation or account disabling can leave shadow and orphaned identities active.
 
 
</details>

### 19. Review the Microsoft Entra ID group creation command. Which users will automatically become members of this group?

```powershell
New-MgGroup -DisplayName "Sales Dynamic Group" -Description "Dynamic security group for Sales users" -MailEnabled:$false -SecurityEnabled:$true -GroupTypes "DynamicMembership" -MembershipRule "(user.department -eq 'Sales')" -MembershipRuleProcessingState "On"
```

- [ ] **A)** All users whose department attribute equals Sales
- [ ] **B)** All users whose job title contains Sales
- [ ] **C)** All users who belong to a nested group
- [ ] **D)** All users manually added by an administrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The membership rule evaluates the department attribute. Any user with department equal to Sales will be automatically added while the rule processing state is On.
 
 
</details>

### 20. Which user attribute is most commonly used as the foundation for dynamic group membership and attribute-based access control?

- [ ] **A)** department
- [ ] **B)** thumbnailPhoto
- [ ] **C)** mobilePhone
- [ ] **D)** passwordProfile

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Attributes such as department, job title, and manager are commonly used in dynamic membership rules. They provide the foundational metadata for automated access decisions and ABAC.
 
 
</details>

### 21. Which two statements accurately describe Microsoft Entra Cloud Sync compared with Microsoft Entra Connect?

- [ ] **A)** It is a lightweight, cloud-based agent for simpler synchronization scenarios
- [ ] **B)** It is well suited for basic synchronization needs with easier management
- [ ] **C)** It can only be used in complex multi-forest environments
- [ ] **D)** It requires a heavier on-premises footprint than Microsoft Entra Connect

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Cloud Sync is a lightweight cloud-based agent designed for simpler requirements and easier management. Entra Connect is the heavier agent for complex multi-forest environments.
 
 
</details>

### 22. What identity governance process is being initiated by the Microsoft Graph PowerShell command shown?

```powershell
$params = @{
  DisplayName = "Financial System Access Review"
  Description = "Certify finance group members"
  Scope = @{
    "@odata.type" = "#microsoft.graph.accessReviewQueryScope"
    query = "/groups/finance/members"
  }
}
New-MgIdentityGovernanceAccessReviewDefinition -BodyParameter $params
```

- [ ] **A)** An access review of the finance group
- [ ] **B)** A dynamic membership rule update
- [ ] **C)** Password writeback configuration
- [ ] **D)** SCIM provisioning to a SaaS application

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command creates an access review definition for the finance group members. Access reviews are used to periodically validate that users still require their assigned permissions.
 
 
</details>

### 23. If an attribute is mastered in on-premises Active Directory and synchronized to Microsoft Entra ID, what happens when an administrator attempts to edit that attribute in the Microsoft Entra admin center?

- [ ] **A)** The attribute is read-only, and any attempted change is either blocked or overwritten by the next sync cycle
- [ ] **B)** The change is immediately written back to on-premises Active Directory
- [ ] **C)** The attribute can be edited only if the administrator is a Global Administrator
- [ ] **D)** The attribute is automatically replicated to all cloud tenants

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When the source of authority is on-premises, the synchronized attribute is read-only in the cloud portal. Direct edits are blocked or overwritten during the next synchronization cycle.
 
 
</details>


---

### **Plan and implement workload identities**

### 24. What is the primary purpose of implementing identity lifecycle management for users in Microsoft Entra ID?

- [ ] **A)** Grant access when needed and revoke when leaving
- [ ] **B)** Keep all user accounts permanently active
- [ ] **C)** Store user passwords in plain text
- [ ] **D)** Replace Conditional Access policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Identity lifecycle management ensures access is granted during onboarding and revoked at offboarding, preventing ghost accounts and security vulnerabilities.
 
 
</details>

### 25. Which three phases are included in the Joiner-Mover-Leaver (JML) framework for identity lifecycle management in Microsoft Entra ID?

- [ ] **A)** Joiner
- [ ] **B)** Mover
- [ ] **C)** Leaver
- [ ] **D)** Reviewer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The JML framework includes Joiner, Mover, and Leaver phases to grant initial access, adjust permissions on role changes, and revoke all access when a user leaves.
 
 
</details>

### 26. An administrator applies the expression in the code block to a Microsoft Entra ID group. Which type of group membership is being configured?

```text
(user.department -eq "Sales")
```

- [ ] **A)** Dynamic membership
- [ ] **B)** Assigned membership
- [ ] **C)** External membership
- [ ] **D)** Hybrid membership

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A rule based on user attributes such as department defines dynamic membership, so membership is evaluated by the Entra ID engine rather than assigned manually.
 
 
</details>

### 27. Which tool is recommended for complex multi-forest synchronization between on-premises Active Directory and Microsoft Entra ID?

- [ ] **A)** Microsoft Entra Connect
- [ ] **B)** Entra Cloud Sync
- [ ] **C)** SCIM provisioning
- [ ] **D)** Password writeback

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Microsoft Entra Connect is the heavy-duty agent designed for complex, multi-forest environments that require advanced synchronization features.
 
 
</details>

### 28. Which statements correctly describe how dynamic membership rules work in Microsoft Entra ID for group management?

- [ ] **A)** Membership is based on user attributes
- [ ] **B)** Membership changes use a propagation delay
- [ ] **C)** Null attributes can prevent membership
- [ ] **D)** Membership updates happen instantly

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Dynamic membership rules use user attributes, require valid attribute values, and are processed with a propagation delay before membership updates appear.
 
 
</details>

### 29. The command in the code block is run for a user who is synchronized from on-premises Active Directory. What is the likely result?

```powershell
Update-MgUser -UserId "user@contoso.com" -JobTitle "Manager"
```

- [ ] **A)** The change is overwritten during the next sync cycle
- [ ] **B)** The change is permanently stored in Microsoft Entra ID
- [ ] **C)** The user is immediately deleted
- [ ] **D)** The command creates a new on-premises user

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> If an attribute is mastered on-premises, editing it in the cloud is overwritten during the next Entra Connect synchronization cycle.
 
 
</details>

### 30. What is the main purpose of creating an Administrative Unit in Microsoft Entra ID for identity management?

- [ ] **A)** Delegate scoped administrative permissions
- [ ] **B)** Store external user credentials
- [ ] **C)** Replace Conditional Access policies
- [ ] **D)** Automate SaaS application provisioning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Administrative Units allow scoped management by delegating permissions over specific users, groups, or devices without granting global privileges.
 
 
</details>

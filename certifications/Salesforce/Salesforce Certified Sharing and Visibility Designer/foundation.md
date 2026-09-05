<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Salesforce/Salesforce%20Certified%20Sharing%20and%20Visibility%20Designer.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Salesforce Certified Sharing and Visibility Designer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Data Access](#data-access) (9 questions)
- [Design and Governance](#design-and-governance) (6 questions)
- [Sharing Model](#sharing-model) (7 questions)
- [Visibility](#visibility) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:47:32.531Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Data Access | 9 |
| Design and Governance | 6 |
| Sharing Model | 7 |
| Visibility | 8 |

---

### **Data Access**

### 1. When a user has access to an Account record, what is the automatic visibility of related child records called?

- [ ] **A)** Explicit sharing
- [ ] **B)** Implicit sharing
- [ ] **C)** Manual sharing
- [ ] **D)** Apex sharing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Implicit sharing grants access to related child records through parent record access, such as Account-to-Contact and Account-to-Opportunity relationships.
 
 
</details>

### 2. Select all common parent-to-child relationships where implicit sharing can grant access to child records.

- [ ] **A)** Account to Contact
- [ ] **B)** Account to Case
- [ ] **C)** Account to Opportunity
- [ ] **D)** Contact to Account

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Implicit sharing commonly flows from Account to Contacts, Cases, and Opportunities. Access does not typically flow from child Contact to parent Account.
 
 
</details>

### 3. Review the Apex class in the code block. Which statement about Field-Level Security is true?

```apex
public with sharing class MyController {
    public List<Account> getAccounts() {
        return [SELECT Id, Name, AnnualRevenue FROM Account];
    }
}
```

- [ ] **A)** It automatically enforces FLS
- [ ] **B)** It does not enforce FLS
- [ ] **C)** It only enforces FLS for Account
- [ ] **D)** It prevents the query from running

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> `with sharing` enforces record-level sharing, not Field-Level Security. Use `Security.stripInaccessible()` or `WITH USER_MODE` to enforce FLS.
 
 
</details>

### 4. In a Master-Detail relationship, what is the child record's ownership model?

- [ ] **A)** Child has its own owner
- [ ] **B)** Child inherits the master's owner
- [ ] **C)** Child is owned by the running user
- [ ] **D)** Child is unowned

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Master-Detail records do not have independent owners. The detail record inherits its owner and security from the master record.
 
 
</details>

### 5. Select two characteristics that are true of Lookup relationships when compared to Master-Detail relationships.

- [ ] **A)** No native roll-up summary fields
- [ ] **B)** Visibility controlled by parent
- [ ] **C)** Optional by design with independent ownership
- [ ] **D)** Automatically delete children with parent

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Lookup relationships are optional, allow independent ownership, and do not support native Roll-Up Summary fields. Deleting parent can nullify the lookup or be restricted.
 
 
</details>

### 6. Given the Apex class in the code block, how does it execute by default?

```apex
public class AccountService {
    public List<Account> getAccounts() {
        return [SELECT Id, Name FROM Account];
    }
}
```

- [ ] **A)** System Mode
- [ ] **B)** User Mode
- [ ] **C)** Object Mode
- [ ] **D)** Mixed Mode

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Apex runs in System Mode by default unless the class uses `with sharing`. This means sharing rules are not enforced automatically.
 
 
</details>

### 7. For high-volume external users, which lightweight sharing mechanism maps a user to records through a common field?

- [ ] **A)** Sharing Sets
- [ ] **B)** Sharing Rules
- [ ] **C)** Role Hierarchy
- [ ] **D)** Manual Sharing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Sharing Sets are designed for high-volume external users and grant access based on field values like Account ID or Contact ID.
 
 
</details>

### 8. Select all true statements about Territory Management.

- [ ] **A)** ETM is the modern standard
- [ ] **B)** Assignment rules move Accounts into Territories
- [ ] **C)** Territory Management grants access to all objects
- [ ] **D)** User assignment moves users into Territories

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> ETM is the modern standard; assignment rules map Accounts to Territories and user assignment maps people to Territories. Territory access is focused mainly on Accounts and Opportunities.
 
 
</details>

### 9. What is the purpose of the security utility method used in the code block?

```apex
List<Account> accts = Security.stripInaccessible(AccessType.READABLE, [SELECT Id, AnnualRevenue FROM Account]).getRecords();
```

- [ ] **A)** Enforce record sharing
- [ ] **B)** Remove inaccessible fields from query results
- [ ] **C)** Delete records without permission
- [ ] **D)** Set field permissions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> `Security.stripInaccessible` enforces Field-Level Security by removing fields from SOQL results that the current user cannot access.
 
 
</details>


---

### **Design and Governance**

### 10. In a Master-Detail relationship, how is the child record's ownership determined?

- [ ] **A)** The child record has its own owner
- [ ] **B)** The child record inherits the master's owner and security settings
- [ ] **C)** The child record is assigned by a sharing rule
- [ ] **D)** The child record uses a lookup field to select an owner

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In a Master-Detail relationship, the child record does not have its own owner and inherits the master record's owner and security settings.
 
 
</details>

### 11. Which statements about Master-Detail and Lookup relationships are accurate?

- [ ] **A)** Deleting a master record deletes its detail records
- [ ] **B)** Lookup relationships support roll-up summary fields natively
- [ ] **C)** A Master-Detail field is required at the database level
- [ ] **D)** Lookup relationships allow independent ownership of child records

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Master-Detail relationships enforce cascading deletion and required fields, while Lookup relationships allow independent ownership and do not support native roll-up summaries.
 
 
</details>

### 12. In an org with Private OWD on Account, what will the method in the code block return for a user with no explicit Account access?

```apex
public with sharing class AccountController {
    public static List<Account> getAccounts() {
        return [SELECT Id, Name FROM Account];
    }
}
```

- [ ] **A)** Only the accounts the user can access
- [ ] **B)** All accounts in the org
- [ ] **C)** An exception because sharing is enforced
- [ ] **D)** An empty list because sharing is disabled

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Apex declared with \"with sharing\" respects the org's sharing settings, so the user only sees accounts they have access to.
 
 
</details>

### 13. Which relationship is the primary driver of implicit visibility from Account to Contact?

- [ ] **A)** Case-to-Account relationship
- [ ] **B)** Account-to-Contact relationship
- [ ] **C)** Opportunity-to-Account relationship
- [ ] **D)** Contact-to-Account relationship

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Account-to-Contact relationship is the primary driver of implicit visibility; access to an Account often grants implicit access to its Contacts.
 
 
</details>

### 14. Which of the following are common traps related to implicit sharing?

- [ ] **A)** Assuming OWD is the only factor
- [ ] **B)** Assuming Private OWD prevents all implicit access to child records
- [ ] **C)** Assuming implicit sharing flows from child to parent
- [ ] **D)** Confusing object-level security with record-level visibility

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Implicit sharing is often misunderstood: OWD is not the only factor, child access can be granted through the parent, and sharing does not flow from child to parent.
 
 
</details>

### 15. In an org with Private OWD on Opportunity, what does the method in the code block return when called by a user without explicit Opportunity access?

```apex
public without sharing class DebugUtility {
    public static Integer getOppCount() {
        return [SELECT COUNT() FROM Opportunity];
    }
}
```

- [ ] **A)** The count of all Opportunity records
- [ ] **B)** The count of only accessible Opportunity records
- [ ] **C)** An error is thrown
- [ ] **D)** The value zero

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Apex declared with \"without sharing\" runs in system mode and bypasses sharing rules, so it returns all records regardless of user access.
 
 
</details>


---

### **Sharing Model**

### 16. What is the primary effect of implicit sharing from a parent record?

- [ ] **A)** Access to certain related child records without explicit sharing rules
- [ ] **B)** Access to every record in the organization
- [ ] **C)** Access only to records owned by the user's manager
- [ ] **D)** Access to child records only after manual sharing is created

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Implicit sharing automatically grants access to related child records when the parent is visible to the user.
 
 
</details>

### 17. Which two statements about Account-to-Contact implicit visibility are correct?

- [ ] **A)** Account access can grant implicit access to related Contacts when Contact visibility is not more restrictive.
- [ ] **B)** The Account-to-Contact relationship is a primary driver of implicit visibility.
- [ ] **C)** Contacts require explicit sharing rules even when the parent Account is visible.
- [ ] **D)** Account access never influences whether a user can see related Contacts.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Account-to-Contact is a primary implicit visibility driver; users with Account access often see Contacts unless Contact visibility is more restrictive.
 
 
</details>

### 18. Review the Apex class in the code block. What does the `with sharing` keyword enforce when this method is executed?

```apex
public with sharing class AccountController {
    public List<Account> getAccounts() {
        return [SELECT Id, Name FROM Account];
    }
}
```

- [ ] **A)** Record-level sharing rules for the running user are enforced.
- [ ] **B)** All record sharing rules are bypassed.
- [ ] **C)** Field-level security is automatically enforced.
- [ ] **D)** Object-level security is ignored and no records are returned.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> With sharing enforces record-level sharing; it does not automatically enforce field- or object-level security.
 
 
</details>

### 19. Why is it a trap to assume Organization-Wide Defaults are the only factor in record visibility?

- [ ] **A)** Implicit sharing may still grant access to child records through the parent record.
- [ ] **B)** OWD has no impact on record-level visibility.
- [ ] **C)** OWD always overrides implicit sharing.
- [ ] **D)** OWD applies only to external users.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Even with Private OWDs, implicit sharing through a parent relationship can expose child records.
 
 
</details>

### 20. Which two statements correctly describe Sharing Sets for external users?

- [ ] **A)** Sharing Sets are a lightweight, high-performance mechanism for high-volume external users.
- [ ] **B)** Sharing Sets map external users to records based on common fields such as Account ID or Contact ID.
- [ ] **C)** Sharing Sets use the same criteria and owner logic as traditional Sharing Rules.
- [ ] **D)** Sharing Sets require Apex triggers to grant record access.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Sharing Sets provide high-volume external users with record access based on field mapping, not traditional sharing rules.
 
 
</details>

### 21. Review the Apex class in the code block. What is the most likely security risk when executing this class?

```apex
public without sharing class DebugAccountService {
    public List<Account> getAccounts() {
        return [SELECT Id, Name FROM Account];
    }
}
```

- [ ] **A)** It may expose records to users who should not see them because sharing rules are bypassed.
- [ ] **B)** It will always trigger a governor limit exception.
- [ ] **C)** It enforces stricter field-level security.
- [ ] **D)** It prevents all users from querying Account records.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Without sharing bypasses record-level sharing rules, so queries can return records the user is not entitled to see.
 
 
</details>

### 22. Which statement accurately compares the territory hierarchy with the role hierarchy?

- [ ] **A)** Role hierarchy manages vertical access by management level; territory hierarchy manages horizontal access by business attributes.
- [ ] **B)** Territory hierarchy and role hierarchy are identical.
- [ ] **C)** Role hierarchy manages horizontal access; territory hierarchy manages vertical access.
- [ ] **D)** A user can belong to only one territory.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Role hierarchy is vertical based on management; territory hierarchy is horizontal based on attributes and supports multiple memberships.
 
 
</details>


---

### **Visibility**

### 23. Which statement best describes implicit sharing in Salesforce?

- [ ] **A)** Access to a parent record can grant access to related child records.
- [ ] **B)** Access to a child record grants access to its parent record.
- [ ] **C)** Implicit sharing only applies to records explicitly shared with the user.
- [ ] **D)** Implicit sharing ignores Organization-Wide Defaults.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Implicit sharing flows from parent records to child records, such as from Account to its related Contacts, Cases, and Opportunities.
 
 
</details>

### 24. Which of the following record types can a user typically gain implicit access to when they have access to an Account? Select all that apply.

- [ ] **A)** Contacts
- [ ] **B)** Cases
- [ ] **C)** Opportunities
- [ ] **D)** Price Books

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Account access can implicitly expose associated Contacts, Cases, and Opportunities, helping users see the full business relationship.
 
 
</details>

### 25. Consider the Apex class declaration in the code block. What access behavior does the sharing keyword enforce?

```apex
public with sharing class AccountController {
    public List<Account> getAccounts() {
        return [SELECT Id, Name FROM Account];
    }
}
```

- [ ] **A)** It enforces record-level sharing for the query.
- [ ] **B)** It enforces Field-Level Security on the selected fields.
- [ ] **C)** It bypasses all record sharing and permissions.
- [ ] **D)** It prevents the query from returning child records.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> With sharing enforces sharing rules and record visibility, but it does not automatically enforce Field-Level Security.
 
 
</details>

### 26. In a Master-Detail relationship, what is the default result when the master record is deleted?

- [ ] **A)** All associated detail records are also deleted.
- [ ] **B)** Detail records remain but the lookup field is blanked.
- [ ] **C)** Deletion is blocked until all detail records are reassigned.
- [ ] **D)** Detail records become private to the system administrator.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Master-Detail relationships enforce strict lifecycle coupling; deleting the master automatically deletes all detail records.
 
 
</details>

### 27. Which of the following are characteristics of a Master-Detail relationship? Select all that apply.

- [ ] **A)** The detail record inherits the master record's owner and security settings.
- [ ] **B)** Roll-up Summary fields can be created on the master record.
- [ ] **C)** Deleting the master record automatically deletes detail records.
- [ ] **D)** The detail record has its own independent owner and sharing rules.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Master-Detail creates tightly coupled visibility, supports roll-up summaries, and cascades deletes; independent ownership is a Lookup trait.
 
 
</details>

### 28. The code block applies a security method to a query result. Which type of access does this method help enforce?

```apex
Account[] accounts = [SELECT Id, Name, AnnualRevenue FROM Account];
List<Account> safeAccounts = Security.stripInaccessible(AccessType.READABLE, accounts).getRecords();
```

- [ ] **A)** Field-Level Security
- [ ] **B)** Record-Level Sharing
- [ ] **C)** Organization-Wide Defaults
- [ ] **D)** Role Hierarchy access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Security.stripInaccessible removes fields the user cannot read, enforcing Field-Level Security in Apex.
 
 
</details>

### 29. Which sharing mechanism is designed for high-volume external users and grants record access based on a matching field value?

- [ ] **A)** Sharing Sets
- [ ] **B)** Sharing Groups
- [ ] **C)** Internal Role Hierarchy
- [ ] **D)** Territory Assignment Rules

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Sharing Sets are a lightweight, high-performance mechanism that maps external users to records through a common field.
 
 
</details>

### 30. Which of the following are common mistakes when designing sharing for external users? Select all that apply.

- [ ] **A)** Assuming the internal Role Hierarchy applies to all Experience Cloud users.
- [ ] **B)** Confusing Sharing Sets with Sharing Rules.
- [ ] **C)** Overlooking the distinction between Internal and External OWDs.
- [ ] **D)** Using Permission Set Groups to grant record access to high-tier external users.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> External sharing designs often fail when designers rely on role hierarchy, mix up Sharing Sets and Rules, or ignore external OWDs.
 
 
</details>

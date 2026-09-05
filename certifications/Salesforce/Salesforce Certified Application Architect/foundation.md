<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Salesforce/Salesforce%20Certified%20Application%20Architect.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Salesforce Certified Application Architect</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Data Architecture](#data-architecture) (7 questions)
- [Development Lifecycle](#development-lifecycle) (7 questions)
- [Identity and Access Management](#identity-and-access-management) (8 questions)
- [Integration Architecture](#integration-architecture) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:47:12.048Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Data Architecture | 7 |
| Development Lifecycle | 7 |
| Identity and Access Management | 8 |
| Integration Architecture | 8 |

---

### **Data Architecture**

### 1. In Salesforce data modeling, which relationship type couples the child record’s lifecycle and security to its parent?

- [ ] **A)** Lookup
- [ ] **B)** Master-Detail
- [ ] **C)** Many-to-Many
- [ ] **D)** Self Relationship

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Master-Detail creates tight coupling, inherits sharing behavior, and causes cascade delete; Lookup keeps child records independent.
 
 
</details>

### 2. Which two statements correctly describe Organization-Wide Defaults (OWD) according to the playbook?

- [ ] **A)** OWDs are the baseline access level for the most restrictive user.
- [ ] **B)** OWDs should be Private or Public Read Only to allow controlled expansion of access.
- [ ] **C)** OWDs grant object access through sharing rules.
- [ ] **D)** OWDs override the Role Hierarchy.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OWDs define a restrictive baseline; access is then expanded through Role Hierarchy and Sharing Rules while remaining scalable.
 
 
</details>

### 3. Review the SOQL query. Which relationship type is demonstrated by filtering on WhatId?

```sql
SELECT Id, Subject, WhatId FROM Event WHERE WhatId != null
```

- [ ] **A)** Master-Detail
- [ ] **B)** Polymorphic
- [ ] **C)** Lookup
- [ ] **D)** Self

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> WhatId is a polymorphic relationship field because it can reference several object types, enabling flexible data structures.
 
 
</details>

### 4. When designing for Large Data Volumes, which feature stores frequently queried fields in a compact table to improve performance?

- [ ] **A)** Custom Index
- [ ] **B)** Skinny Tables
- [ ] **C)** Big Objects
- [ ] **D)** Roll-Up Summary

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Skinny tables are a recognized LDV pattern that improves performance by storing frequently used fields in a smaller table.
 
 
</details>

### 5. Which two traps are specifically associated with large data volumes and query performance?

- [ ] **A)** Indexing Misconceptions
- [ ] **B)** Treating Big Objects like standard objects
- [ ] **C)** Tool Over-Usage Pitfall
- [ ] **D)** Ignoring Data Locality

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Indexing misconceptions and treating Big Objects like standard objects can cause performance issues at scale.
 
 
</details>

### 6. The code block creates a record in Salesforce. Which sharing mechanism is being used?

```apex
AccountShare share = new AccountShare();
share.AccountId = acct.Id;
share.UserOrGroupId = userId;
share.AccountAccessLevel = 'Edit';
insert share;
```

- [ ] **A)** Manual Sharing
- [ ] **B)** Apex Managed Sharing
- [ ] **C)** Criteria-Based Sharing Rule
- [ ] **D)** Role Hierarchy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code inserts an AccountShare record programmatically, which is Apex managed sharing.
 
 
</details>

### 7. Which security principle grants users only the minimum access necessary to perform their job?

- [ ] **A)** Principle of Least Privilege
- [ ] **B)** Organization-Wide Defaults
- [ ] **C)** Role Hierarchy
- [ ] **D)** Sharing Rules

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Least privilege grants the minimum required access, reducing risk and preventing accidental data manipulation.
 
 
</details>


---

### **Development Lifecycle**

### 8. In Salesforce data modeling, which statement best explains the primary functional difference between a Master-Detail relationship and a Lookup relationship?

- [ ] **A)** It prevents all record deletion.
- [ ] **B)** It controls ownership, sharing, and deletion behavior.
- [ ] **C)** It allows multiple parents of different types.
- [ ] **D)** It only affects page layouts.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Master-Detail creates tight coupling where the parent controls ownership, security, and cascade delete; Lookup leaves records independent.
 
 
</details>

### 9. Which two of the following characteristics accurately describe a Master-Detail relationship in the Salesforce data model?

- [ ] **A)** Roll-up summary fields are available
- [ ] **B)** Children can be orphaned if parent is deleted
- [ ] **C)** Child records inherit the parent's sharing model
- [ ] **D)** Records can have multiple parent records

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Master-Detail supports roll-up summaries and makes child security dependent on the parent, but it prevents orphaned children and assumes one parent.
 
 
</details>

### 10. The code block defines a custom relationship field. What is true about this relationship type?

```xml
<field>
    <fullName>Account__c</fullName>
    <type>MasterDetail</type>
    <relationshipName>Accounts</relationshipName>
</field>
```

- [ ] **A)** Child records inherit security and deletion behavior from the parent.
- [ ] **B)** The child is independent and can be deleted separately.
- [ ] **C)** The field allows for multiple parent objects.
- [ ] **D)** The relationship creates a many-to-many junction.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The field type is MasterDetail, so the parent controls security and deletion. Child records cannot be orphaned and do not have independent access.
 
 
</details>

### 11. Why might a Salesforce architect intentionally choose denormalization even though it adds some data redundancy?

- [ ] **A)** To increase data redundancy and storage costs
- [ ] **B)** To improve user experience and reporting simplicity
- [ ] **C)** To avoid using lookup relationships
- [ ] **D)** To enforce stricter field-level security

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Denormalization is often used to improve reporting ease and user experience by reducing complex joins and making data easier to consume.
 
 
</details>

### 12. Which two tactics help architects manage Large Data Volumes in Salesforce effectively?

- [ ] **A)** Use skinny tables
- [ ] **B)** Archive historical data
- [ ] **C)** Index every custom field
- [ ] **D)** Store all data in standard objects

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Skinny tables and archiving help optimize performance in LDV environments, while excessive indexing and forcing data into standard objects are not reliable strategies.
 
 
</details>

### 13. The code block shows a SOQL query. Which factor most directly impacts its performance in an LDV org?

```sql
SELECT Id, Name
FROM Account
WHERE Custom_Indexed_Field__c = :searchTerm
```

- [ ] **A)** Number of fields in the SELECT clause
- [ ] **B)** Whether the filter field is indexed
- [ ] **C)** Use of a bind variable
- [ ] **D)** Length of the object API name

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Selectivity and indexes determine query performance in high-volume orgs; bind variables and field selection are secondary.
 
 
</details>

### 14. What is a polymorphic relationship in the Salesforce data model?

- [ ] **A)** A relationship that relates one record to multiple target object types
- [ ] **B)** A relationship with multiple parent records on one child
- [ ] **C)** A lookup field pointing to a single object
- [ ] **D)** A many-to-many relationship implemented by a junction object

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Polymorphic relationships allow a single object to relate to multiple object types, such as WhatId or WhoId on tasks and events.
 
 
</details>


---

### **Identity and Access Management**

### 15. Based on the playbook, what does the Principle of Least Privilege require in an identity architecture?

- [ ] **A)** Grant every user full object access
- [ ] **B)** Grant the minimum access needed for the role
- [ ] **C)** Grant access only to System Administrators
- [ ] **D)** Grant access based on data volume

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Least privilege means users receive only the minimum access required for their job, limiting the impact of compromised credentials.
 
 
</details>

### 16. Based on the playbook, which statements correctly distinguish object-level security from record-level security? Select all that apply.

- [ ] **A)** Object security controls which records are visible
- [ ] **B)** Record-level sharing cannot override missing object access
- [ ] **C)** Users need both layers to see a record
- [ ] **D)** Sharing rules can override object-level deny

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Object-level security defines what objects and fields are available; record-level security defines which records are visible. Both layers must allow access.
 
 
</details>

### 17. Based on the sharing configuration in the code block, what is the baseline access for Account records?

```text
Account_OWD = Private
Contact_OWD = Controlled by Parent
Role_Hierarchy = Enabled
```

- [ ] **A)** Public Read Only
- [ ] **B)** Private
- [ ] **C)** Public Read/Write
- [ ] **D)** Controlled by Parent

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> OWDs establish the most restrictive baseline; Private is the most restrictive Account default, while Role Hierarchy and sharing rules can expand access.
 
 
</details>

### 18. Based on the playbook, what is the purpose of Organization-Wide Defaults in the sharing model?

- [ ] **A)** Define the most restrictive baseline
- [ ] **B)** Grant access through manual sharing
- [ ] **C)** Replace all profile permissions
- [ ] **D)** Store field-level security settings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Organization-Wide Defaults represent the baseline level of access for the most restrictive user, and other mechanisms expand from that baseline.
 
 
</details>

### 19. Based on the playbook, which statements about Role Hierarchy and Sharing Rules are true? Select all that apply.

- [ ] **A)** Role Hierarchy gives managers access to subordinates
- [ ] **B)** Sharing Rules provide access across hierarchy branches
- [ ] **C)** Role Hierarchy should grant all horizontal access
- [ ] **D)** Sharing Rules only restrict access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Role Hierarchy supports vertical access, while Sharing Rules provide horizontal access. Overusing the hierarchy for all sharing creates hierarchy bloat.
 
 
</details>

### 20. Based on the configuration in the code block, why is this an appropriate scalable access model?

```text
Profile = Minimum Access
Permission Set Group = Sales Support
```

- [ ] **A)** It keeps Profiles slim and uses Permission Sets
- [ ] **B)** It places all permissions in the Profile
- [ ] **C)** It removes the need for sharing rules
- [ ] **D)** It grants every user the same profile

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Modern architecture keeps Profiles minimal and grants additive access through Permission Sets, especially Permission Set Groups, for scalability.
 
 
</details>

### 21. Based on the playbook, why is manual sharing always considered technical debt in high-volume architectures?

- [ ] **A)** It does not scale with dynamic access or volume
- [ ] **B)** It is not a valid sharing mechanism
- [ ] **C)** It automatically removes record access
- [ ] **D)** It requires no maintenance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Manual sharing does not scale with dynamic business logic and data volume, making it technical debt in large architectures.
 
 
</details>

### 22. Based on the playbook, which mechanisms support automated sharing in a scalable architecture? Select all that apply.

- [ ] **A)** Criteria-Based Sharing Rules
- [ ] **B)** Apex Managed Sharing
- [ ] **C)** Manual sharing per record
- [ ] **D)** Broad Profile permissions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Criteria-Based Sharing Rules and Apex Managed Sharing automate access at scale, while manual sharing and broad profiles create technical debt.
 
 
</details>


---

### **Integration Architecture**

### 23. Which relationship type creates a tight coupling between records, affecting security and record lifecycle within the data model?

- [ ] **A)** Master-Detail
- [ ] **B)** Lookup
- [ ] **C)** Many-to-Many
- [ ] **D)** Polymorphic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Master-Detail creates a tight coupling that affects sharing and record deletion. Lookup remains loose and does not control child record lifecycle or security.
 
 
</details>

### 24. Which two characteristics belong to a Master-Detail relationship type in the Salesforce data model when compared to a Lookup relationship?

- [ ] **A)** Parent deletion cascades to child records
- [ ] **B)** Roll-up summaries are available on the master
- [ ] **C)** Child records have independent sharing
- [ ] **D)** Records can be reparented without restriction

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Master-Detail relationships support roll-up summaries and cascade deletes. Children inherit sharing behavior and reparenting is restricted, so those options are false.
 
 
</details>

### 25. Based on the schema, what automatically happens when a Project__c record is deleted?

```text
Project__c (Master)
  Name
  Status__c

Project_Task__c (Detail)
  Project__c (Master-Detail to Project__c)
  Due_Date__c
```

- [ ] **A)** They are deleted with the project
- [ ] **B)** They remain as orphans
- [ ] **C)** They are assigned to a default project
- [ ] **D)** They are converted to Task records

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Because Project_Task__c is a Detail in a Master-Detail relationship, deleting the Project__c master automatically deletes all related Project_Task__c records.
 
 
</details>

### 26. What does a polymorphic relationship allow a record to do in the Salesforce data model?

- [ ] **A)** Relate one object to multiple object types
- [ ] **B)** Relate multiple records to one field
- [ ] **C)** Create a private sharing model
- [ ] **D)** Aggregate data without queries

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Polymorphic relationships, such as WhatId and WhoId, allow a single object to relate to several different object types within one unified interface.
 
 
</details>

### 27. Which two examples use polymorphic relationships, such as those found on Task and Event records in Salesforce?

- [ ] **A)** Task WhatId pointing to Account or Opportunity
- [ ] **B)** Event WhoId pointing to Lead or Contact
- [ ] **C)** Master-Detail from Opportunity to Account
- [ ] **D)** Big Object storing archived events

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Task and Event use polymorphic WhatId and WhoId fields to reference different object types. A Master-Detail is fixed, and Big Objects are for storage, not polymorphic relationships.
 
 
</details>

### 28. Under high-concurrency updates, what risk does this roll-up summary design introduce?

```text
Account__c (Master)
  Total_Opportunity_Amount__c (Roll-up Summary of Opportunity__c.Amount)

Opportunity__c (Detail)
  Account__c (Master-Detail to Account__c)
  Amount__c
```

- [ ] **A)** Row locking on the parent Account__c
- [ ] **B)** Non-selective SOQL queries
- [ ] **C)** Loss of field-level security
- [ ] **D)** Orphaned child records

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Roll-up summary recalculations update the parent record, so frequent child updates can cause row-locking contention on the parent in high-volume environments.
 
 
</details>

### 29. What is a recommended element of a Large Data Volume strategy in Salesforce when designing for scale?

- [ ] **A)** Using skinny tables and indexing
- [ ] **B)** Making every object private
- [ ] **C)** Storing all data in one object
- [ ] **D)** Using manual sharing everywhere

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> LDV strategies rely on skinny tables, selective indexes, archiving, and off-platform storage to maintain query performance and avoid locking issues.
 
 
</details>

### 30. Which two strategies are part of a Large Data Volume architecture when managing millions of records in Salesforce?

- [ ] **A)** Using index-aware query design
- [ ] **B)** Planning archiving or off-platform storage
- [ ] **C)** Adding every field to a custom index
- [ ] **D)** Placing all records in a Big Object

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Index-aware queries and archiving/off-platform storage are LDV best practices. Excessive custom indexes hurt DML performance, and Big Objects are not a universal replacement.
 
 
</details>

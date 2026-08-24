<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Salesforce/Salesforce%20Certified%20Platform%20App%20Builder.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Salesforce Certified Platform App Builder</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [App Deployment](#app-deployment) (3 questions)
- [Business Logic and Process Automation](#business-logic-and-process-automation) (8 questions)
- [Data Modeling and Management](#data-modeling-and-management) (7 questions)
- [Salesforce Fundamentals](#salesforce-fundamentals) (7 questions)
- [User Interface](#user-interface) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:53:24.824Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| App Deployment | 3 |
| Business Logic and Process Automation | 8 |
| Data Modeling and Management | 7 |
| Salesforce Fundamentals | 7 |
| User Interface | 5 |

---

### **App Deployment**

### 1. Which deployment tool is specifically designed for point-and-click metadata migration between two connected Salesforce environments?

- [ ] **A)** Change Sets
- [ ] **B)** Metadata API
- [ ] **C)** Managed Packages
- [ ] **D)** Unmanaged Packages

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Change sets transfer metadata between connected orgs through point-and-click configuration. Metadata API, managed packages, and unmanaged packages serve different deployment needs.
 
 
</details>

### 2. Which statements accurately describe managed packages on the Salesforce platform? Select all that apply.

- [ ] **A)** Managed packages hide underlying source code to protect intellectual property.
- [ ] **B)** Managed packages can be upgraded automatically by the original publisher.
- [ ] **C)** Managed packages leave components fully editable with no namespace control.
- [ ] **D)** Managed packages are designed only for backup purposes and open-source sharing.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Managed packages protect proprietary code with namespaces and hidden source, and support automatic upgrades. They are not for open-source sharing, and components are not fully editable.
 
 
</details>

### 3. You are preparing a Metadata API deployment and see the file shown in the code block. What is the purpose of this file?

```xml
<!-- destructiveChanges.xml -->
<?xml version="1.0" encoding="UTF-8"?>
<Package xmlns="http://soap.sforce.com/2006/04/metadata">
  <types>
    <members>Old_Validation_Rule</members>
    <name>ValidationRule</name>
  </types>
  <version>58.0</version>
</Package>
```

- [ ] **A)** Removes the obsolete metadata component from the target org.
- [ ] **B)** Adds a new page layout to the target org.
- [ ] **C)** Refreshes all Apex test classes.
- [ ] **D)** Copies production data into a sandbox.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A destructiveChanges.xml manifest removes obsolete components, such as old validation rules, during a deployment. It does not add metadata, refresh tests, or copy data.
 
 
</details>


---

### **Business Logic and Process Automation**

### 4. Which declarative tool blocks invalid data from being saved by evaluating a condition before the database commit?

- [ ] **A)** Validation Rule
- [ ] **B)** Formula Field
- [ ] **C)** Workflow Rule
- [ ] **D)** Approval Process

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Validation rules enforce data integrity by evaluating a formula synchronously before save. When the formula is true, the record update is blocked and the custom error is displayed.
 
 
</details>

### 5. Which standard objects are governed by standard business processes? Select all that apply.

- [ ] **A)** Lead
- [ ] **B)** Opportunity
- [ ] **C)** Case
- [ ] **D)** Custom_Object__c

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Standard business processes apply only to Lead, Opportunity, Case, and Solution. Custom objects use standard picklist fields combined with record types instead.
 
 
</details>

### 6. The following formula is used in a validation rule on the Opportunity object. What happens when it evaluates to true?

```formula
AND(StageName = "Closed Won", IsClosed = TRUE)
```

- [ ] **A)** The record save is blocked and an error message is shown
- [ ] **B)** The record is automatically saved
- [ ] **C)** The record is converted to a different object
- [ ] **D)** The stage is updated to Closed Won

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When a validation rule formula returns true, the save operation is cancelled and the error message appears, preventing invalid DML.
 
 
</details>

### 7. Which feature computes a read-only value dynamically from fields on the same or parent record without consuming database storage?

- [ ] **A)** Formula Field
- [ ] **B)** Validation Rule
- [ ] **C)** Record Type
- [ ] **D)** Business Process

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Formula fields are dynamically calculated at query time and can reference parent records using relationship notation without persistent storage.
 
 
</details>

### 8. Which flow types are part of Flow Builder? Select all that apply.

- [ ] **A)** Screen Flows
- [ ] **B)** Record-Triggered Flows
- [ ] **C)** Schedule-Triggered Flows
- [ ] **D)** Process Builder

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Flow Builder includes screen flows, record-triggered flows, schedule-triggered flows, and more. Process Builder is a legacy automation tool, not a flow type.
 
 
</details>

### 9. Study the flow loop shown. What automation best practice is being violated?

```pseudocode
for each record in collection:
    run Update Records for the current record
```

- [ ] **A)** Bulkification is violated because DML is inside a loop
- [ ] **B)** Governor limits are avoided by running update in loop
- [ ] **C)** The flow automatically uses a collection variable
- [ ] **D)** The record should be locked before update

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Placing DML elements inside a loop causes excessive DML statements and can trigger governor limits. Use a collection variable and one update outside the loop.
 
 
</details>

### 10. Which Flow Builder component is a reusable, immutable value defined once and referenced globally?

- [ ] **A)** Automation Constants
- [ ] **B)** Screen Flow
- [ ] **C)** Subflow
- [ ] **D)** Fault Path

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Automation constants are reusable, immutable values defined once and referenced globally, reducing maintenance overhead and preventing hardcoding.
 
 
</details>

### 11. Which action nodes are natively available in an approval process? Select all that apply.

- [ ] **A)** Initial Submission Actions
- [ ] **B)** Final Approval Actions
- [ ] **C)** Final Rejection Actions
- [ ] **D)** Apex Trigger

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Approval processes natively support initial submission, final approval, final rejection, and recall actions. Apex triggers are code-based and not native approval action nodes.
 
 
</details>


---

### **Data Modeling and Management**

### 12. Which Salesforce relationship type natively deletes all child records when the parent record is deleted?

- [ ] **A)** Master-Detail
- [ ] **B)** Lookup
- [ ] **C)** External lookup
- [ ] **D)** Indirect lookup

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Master-Detail relationships enforce cascade deletion, so deleting the master automatically deletes all related detail records.
 
 
</details>

### 13. Which features are natively available on Master-Detail relationships? Choose two.

- [ ] **A)** Roll-Up Summary fields
- [ ] **B)** Cascading delete of details
- [ ] **C)** Independent security per child
- [ ] **D)** Optional parent field

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Master-Detail relationships support roll-up summaries and cascade deletes. Child security is inherited, and the parent field is required.
 
 
</details>

### 14. Based on the configuration in the code block, what happens to Contracts when the parent Account is deleted?

```plaintext
Object: Account
Object: Contract
Relationship: Master-Detail
Delete Behavior: Cascade
```

- [ ] **A)** Contracts are deleted automatically
- [ ] **B)** Contracts are kept unchanged
- [ ] **C)** Contracts lose their Account lookup
- [ ] **D)** Contracts are transferred to another owner

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block describes a Master-Detail relationship with cascade delete behavior. Deleting the Account automatically deletes related Contracts.
 
 
</details>

### 15. What is the maximum record volume the Data Import Wizard can process in a single import operation?

- [ ] **A)** 50,000 records
- [ ] **B)** 5,000,000 records
- [ ] **C)** 10,000 records
- [ ] **D)** 1,000,000 records

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Data Import Wizard is designed for up to 50,000 records. Higher volumes require Data Loader.
 
 
</details>

### 16. Which two standard object types can the Data Import Wizard import directly?

- [ ] **A)** Accounts
- [ ] **B)** Contacts
- [ ] **C)** Opportunities
- [ ] **D)** Cases

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The Data Import Wizard supports Accounts and Contacts. Opportunities and Cases require Data Loader.
 
 
</details>

### 17. Based on the lookup configuration in the code block, what access behavior applies to Audit_Record__c?

```plaintext
Object: Audit_Record__c
Parent Object: Account
Field: Account__c
Relationship: Lookup
Cascade Access: false
```

- [ ] **A)** Each audit record keeps independent security
- [ ] **B)** Audit records inherit Account sharing
- [ ] **C)** Audit records are owned by Account owner
- [ ] **D)** Audit records inherit Account deletion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Lookup relationships do not cascade security or deletion. Child records maintain independent ownership and access.
 
 
</details>

### 18. Which feature calculates COUNT, SUM, MIN, or MAX from detail records on the master record?

- [ ] **A)** Roll-Up Summary field
- [ ] **B)** Formula field
- [ ] **C)** Cross-object lookup
- [ ] **D)** Workflow rule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Roll-Up Summary fields are native to Master-Detail relationships and support COUNT, SUM, MIN, and MAX calculations.
 
 
</details>


---

### **Salesforce Fundamentals**

### 19. What is a primary benefit of Salesforce's multi-tenant architecture for organizations building custom apps?

- [ ] **A)** Shared infrastructure with automatic upgrades
- [ ] **B)** Dedicated servers for every customer
- [ ] **C)** Manual management of patches
- [ ] **D)** Mandatory Apex compilation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Multi-tenant architecture lets customers share one infrastructure while receiving automatic upgrades and secure isolation. This reduces maintenance and helps businesses deliver apps quickly.
 
 
</details>

### 20. Which two advantages does declarative customization provide over programmatic development on Salesforce?

- [ ] **A)** Automatic upgrades reduce ongoing maintenance
- [ ] **B)** Point-and-click configuration lowers technical debt
- [ ] **C)** Unlimited processing is available without limits
- [ ] **D)** Direct database access is granted to admins

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Declarative solutions are maintained by the platform and require less technical debt. Programmatic development still imposes governor limits and does not provide direct database access.
 
 
</details>

### 21. Review the Apex trigger in the code block. Which Salesforce best practice does it violate?

```apex
trigger UpdateAccountStatus on Account (before insert) { for (Account a : Trigger.new) { a.Status__c = 'Active'; } }
```

- [ ] **A)** It uses programmatic logic when a declarative tool would suffice
- [ ] **B)** It follows the declarative hierarchy correctly
- [ ] **C)** It guarantees automatic platform upgrades
- [ ] **D)** It avoids all governor limits

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Writing Apex for a simple field assignment ignores the declarative hierarchy. A formula field or flow can satisfy the requirement with less maintenance and lower risk.
 
 
</details>

### 22. A business needs to track a unique asset not represented by standard CRM objects. What is the recommended declarative solution?

- [ ] **A)** Create a custom object
- [ ] **B)** Store the data in Contact records
- [ ] **C)** Build a separate external database
- [ ] **D)** Configure a Visualforce page

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Custom objects extend the data model to meet unique requirements. Standard objects are not appropriate for unrelated data, and external databases are not a declarative platform solution.
 
 
</details>

### 23. Which two characteristics are true of Master-Detail relationships?

- [ ] **A)** They support roll-up summary fields on the parent record
- [ ] **B)** Deleting the parent deletes related child records
- [ ] **C)** Child records can exist without a parent record
- [ ] **D)** Child records have sharing independent from the parent

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Master-Detail relationships provide roll-up summaries and cascading deletes. Detail records inherit security from the parent and cannot exist without one.
 
 
</details>

### 24. Review the configuration in the code block. Why will the desired roll-up summary not work?

```text
Object: Invoice__c Lookup to Account__c. Roll-Up Summary Field: Total Value on Account.
```

- [ ] **A)** Roll-up summaries require a Master-Detail relationship
- [ ] **B)** Lookup relationships are not supported on custom objects
- [ ] **C)** Invoice records must use the standard Opportunity object
- [ ] **D)** Accounts cannot be parent records

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Roll-up summary fields are only available on the parent object of a Master-Detail relationship. A Lookup relationship does not provide native roll-up capabilities.
 
 
</details>

### 25. What do record types allow administrators to provide to different profiles on the same object?

- [ ] **A)** Different page layouts and picklist values
- [ ] **B)** Different record-level security settings
- [ ] **C)** Different field-level security settings
- [ ] **D)** Different sharing rules and groups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Record types present different page layouts, picklist values, and business processes to profiles. They do not control data visibility, field security, or sharing.
 
 
</details>


---

### **User Interface**

### 26. Which point-and-click tool is used to create custom pages for Salesforce mobile and Lightning Experience?

- [ ] **A)** Lightning App Builder
- [ ] **B)** Page Layout Editor
- [ ] **C)** Schema Builder
- [ ] **D)** Reports Builder

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Lightning App Builder is the declarative point-and-click tool used to customize pages for Lightning Experience and the Salesforce mobile app.
 
 
</details>

### 27. Which page types can be configured in Lightning App Builder? Select all that apply.

- [ ] **A)** Lightning App Page
- [ ] **B)** Lightning Record Page
- [ ] **C)** Lightning Home Page
- [ ] **D)** Global Search Results Page

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Lightning App Builder supports Lightning App Pages, Record Pages, and Home Pages; Global Search Results Page is not a configurable page type in this tool.
 
 
</details>

### 28. Review the metadata snippet in the code block. Which UI element is being configured?

```json
{
  "type": "UtilityBar",
  "items": ["History", "Notes"],
  "scope": "Sales_Console_App"
}
```

- [ ] **A)** A utility bar scoped to a specific Lightning app
- [ ] **B)** A record page assigned to an object
- [ ] **C)** A home page component visible to all users
- [ ] **D)** A mobile navigation menu

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code describes a Utility Bar with History and Notes items scoped to a specific app, matching the utility bar configuration model.
 
 
</details>

### 29. A team needs a custom dashboard-like workspace with reports and charts that appears in the app navigation. Which page type should be created?

- [ ] **A)** Lightning App Page
- [ ] **B)** Lightning Record Page
- [ ] **C)** Lightning Home Page
- [ ] **D)** Utility Bar

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Lightning App Pages are designed to host standalone dashboards, reports, and custom components and can be added to a Lightning app's navigation.
 
 
</details>

### 30. Which declarative features can control when fields or components appear on a Lightning page? Select all that apply.

- [ ] **A)** Component visibility rules
- [ ] **B)** Dynamic Forms field visibility
- [ ] **C)** Form-factor visibility filters
- [ ] **D)** Custom Apex controllers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Component visibility rules, Dynamic Forms field visibility, and form-factor filters are all declarative ways to conditionally show or hide page elements without code.
 
 
</details>

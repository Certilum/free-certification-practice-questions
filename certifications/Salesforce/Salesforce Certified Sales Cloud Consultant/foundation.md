<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Salesforce/Salesforce%20Certified%20Sales%20Cloud%20Consultant.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Salesforce Certified Sales Cloud Consultant</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Consulting and Implementation Strategies](#consulting-and-implementation-strategies) (6 questions)
- [Data Management](#data-management) (3 questions)
- [Practical Application of Sales Cloud Expertise](#practical-application-of-sales-cloud-expertise) (10 questions)
- [Predictive and Generative AI](#predictive-and-generative-ai) (3 questions)
- [Sales Lifecycle](#sales-lifecycle) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:47:27.406Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Consulting and Implementation Strategies | 6 |
| Data Management | 3 |
| Practical Application of Sales Cloud Expertise | 10 |
| Predictive and Generative AI | 3 |
| Sales Lifecycle | 8 |

---

### **Consulting and Implementation Strategies**

### 1. Before the first import into Sales Cloud, what standard must be defined to ensure clean, trustworthy data?

- [ ] **A)** Golden Record standard
- [ ] **B)** Role Hierarchy
- [ ] **C)** Dashboard running user
- [ ] **D)** Manual sharing rule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Golden Record standard defines the deduplicated, correctly formatted target state for each account or contact. Establishing it before import protects forecasting accuracy and rep productivity.
 
 
</details>

### 2. Which statements correctly describe the Extract, Transform, Load process when migrating data into Sales Cloud?

- [ ] **A)** Maps legacy values to Salesforce picklists.
- [ ] **B)** Preserves deep hierarchy relationships.
- [ ] **C)** Only exports data from Salesforce.
- [ ] **D)** Eliminates need to map parent IDs.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> ETL transforms legacy values into Salesforce picklist values and field types. For complex hierarchies, ETL tools are preferred over simple imports because they preserve relationships and parent IDs.
 
 
</details>

### 3. The JSON below defines a migration plan. Based on the code block, which statement is correct?

```json
{
  "migrationOrder": ["Account", "Contact", "Opportunity"],
  "externalIdFields": {
    "Account": "Legacy_Account_Id__c",
    "Contact": "Legacy_Contact_Id__c",
    "Opportunity": "Legacy_Opportunity_Id__c"
  }
}
```

- [ ] **A)** Opportunities load before Accounts via external IDs.
- [ ] **B)** Accounts load first; child records use external IDs.
- [ ] **C)** External IDs are only needed for Contacts.
- [ ] **D)** The order shown creates orphaned opportunities.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The order loads Accounts, then Contacts, then Opportunities. Parent IDs are mapped with External IDs, preventing orphaned child records.
 
 
</details>

### 4. What is the recommended migration approach when a client wants to avoid dual data entry and can accept higher cutover risk?

- [ ] **A)** Big Bang migration
- [ ] **B)** Phased migration
- [ ] **C)** Incremental validation
- [ ] **D)** Reconciliation only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Big Bang migration moves all data in a single cutover window, minimizing dual-entry time but increasing risk. Phased migration reduces risk but requires synchronization and more dual-entry time.
 
 
</details>

### 5. Which tasks should be included in post-migration reconciliation for a successful Sales Cloud data implementation?

- [ ] **A)** Compare record counts with legacy system.
- [ ] **B)** Compare Opportunity Amount totals.
- [ ] **C)** Verify dashboard color schemes.
- [ ] **D)** Ensure picklists have many values.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Post-migration reconciliation checks record counts and financial totals, such as Opportunity Amount, against the legacy system to confirm no data was lost or corrupted.
 
 
</details>

### 6. The code block shows a duplicate rule configured for Account. What happens when a user tries to save a duplicate record?

```json
{
  "matchingRule": "Account_Name_Exact_Match",
  "duplicateRuleAction": "Alert"
}
```

- [ ] **A)** Record is blocked from being saved.
- [ ] **B)** User sees a warning but can save.
- [ ] **C)** Duplicate is automatically merged.
- [ ] **D)** User bypassed with no warning.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> An Alert action warns the user but allows the save to continue, while a Block action would prevent the record from being saved.
 
 
</details>


---

### **Data Management**

### 7. What does the acronym ETL stand for when migrating data from a legacy system into a Sales Cloud implementation?

- [ ] **A)** Extract, Transform, Load
- [ ] **B)** Evaluate, Test, Launch
- [ ] **C)** Export, Transfer, Leverage
- [ ] **D)** Encode, Translate, Locate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ETL is defined as extracting data from legacy systems, transforming it to match Salesforce field types and picklist values, and loading it into the target organization.
 
 
</details>

### 8. Which actions are typically part of scrubbing and deduplicating data before a Sales Cloud migration is performed?

- [ ] **A)** Remove duplicates
- [ ] **B)** Correct formatting
- [ ] **C)** Fill missing mandatory fields
- [ ] **D)** Load records in any order

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Data must be scrubbed to remove duplicates, correct formatting, and fill missing mandatory fields before import. This improves forecast accuracy and sales rep productivity.
 
 
</details>

### 9. Based on the configuration shown in the code block, what happens when a user saves a duplicate Account record?

```json
{
  "matchingRule": {
    "object": "Account",
    "field": "Name",
    "logic": "Fuzzy"
  },
  "duplicateRule": {
    "action": "Block"
  }
}
```

- [ ] **A)** A warning appears and the record is saved
- [ ] **B)** The save is blocked and no duplicate is created
- [ ] **C)** The duplicate is converted into a lead
- [ ] **D)** The duplicate is shared with the manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code block displays a Duplicate Rule with the Block action, so a detected duplicate prevents the record from being saved.
 
 
</details>


---

### **Practical Application of Sales Cloud Expertise**

### 10. What is the primary purpose of establishing a 'Golden Record' standard before a Sales Cloud data migration?

- [ ] **A)** Ensures clean, deduplicated, complete data with required fields.
- [ ] **B)** Assigns sales territories automatically.
- [ ] **C)** Removes the need for data transformation.
- [ ] **D)** Creates a backup of legacy records.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Golden Record is the single high-quality version of a record. Data must be deduplicated, formatted correctly, and have mandatory fields populated before the first import to protect forecasting and rep productivity.
 
 
</details>

### 11. Which statements accurately describe ETL in a Sales Cloud migration?

- [ ] **A)** Extracts data from legacy systems.
- [ ] **B)** Transforms data to match Salesforce field types and picklist values.
- [ ] **C)** Is preferred for complex, hierarchical relationships.
- [ ] **D)** Eliminates the need to load data into the target org.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> ETL means Extract, Transform, and Load. It extracts data, transforms it to match Salesforce field types and picklist values, and loads it. ETL tools are preferred when deep hierarchies must be maintained.
 
 
</details>

### 12. A consultant reviews the migration script in the code block. What does the script demonstrate?

```sql
INSERT INTO Account (Legacy_Account_ID__c, Name) VALUES ('ACC-001', 'Acme Corporation');
INSERT INTO Contact (Legacy_Contact_ID__c, LastName, Legacy_Account_ID__c) VALUES ('CON-001', 'Smith', 'ACC-001');
INSERT INTO Opportunity (Legacy_Opp_ID__c, Name, Legacy_Account_ID__c) VALUES ('OPP-001', 'Expansion', 'ACC-001');
```

- [ ] **A)** Parent records before children via External IDs.
- [ ] **B)** Child records before parent records.
- [ ] **C)** Uses standard Salesforce IDs for parent lookups.
- [ ] **D)** Migrates all objects without sequencing.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The script loads Account before Contact and Opportunity and uses External IDs for parent lookups. This follows the required migration sequence and prevents orphaned child records.
 
 
</details>

### 13. What is a major risk of using a Big Bang migration approach?

- [ ] **A)** Moves all data at once, increasing risk.
- [ ] **B)** Requires long-term dual-entry between systems.
- [ ] **C)** Prevents post-migration reconciliation.
- [ ] **D)** Must be done by business unit.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Big Bang migration moves all data in a single cutover window. It avoids long dual-entry but increases risk because there is no iterative validation before the cutover completes.
 
 
</details>

### 14. Which tasks are part of post-migration data reconciliation?

- [ ] **A)** Compare record counts between source and target.
- [ ] **B)** Verify Opportunity Amount totals match legacy values.
- [ ] **C)** Confirm standard Salesforce IDs match legacy primary keys.
- [ ] **D)** Check for data loss or corruption during transformation.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Reconciliation compares record counts and key totals such as Opportunity Amount. Legacy primary keys should be mapped with External IDs, not standard Salesforce IDs, and data loss must be checked.
 
 
</details>

### 15. A consultant configures external ID fields as shown in the code block. What does this configuration enable during migration?

```plaintext
Account.External_Id__c = Legacy_Account_ID__c
Opportunity.External_Id__c = Legacy_Opportunity_ID__c
Opportunity.Account_External_Id__c = Legacy_Account_ID__c
```

- [ ] **A)** Maps legacy primary keys to parent-child records.
- [ ] **B)** Replaces the need for loading parent records.
- [ ] **C)** Allows loading opportunities before accounts.
- [ ] **D)** Uses standard Salesforce IDs for record matching.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> External ID fields store legacy primary keys and allow parent-child links to be created before new Salesforce record IDs are known, preventing orphaned records.
 
 
</details>

### 16. What is the function of a Matching Rule in Salesforce duplicate management?

- [ ] **A)** Identifies possible duplicates using exact or fuzzy logic.
- [ ] **B)** Blocks duplicate records before they are saved.
- [ ] **C)** Merges duplicate records automatically.
- [ ] **D)** Controls user access to duplicate records.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Matching Rules define the logic used to identify potential duplicates by comparing fields. They can use exact or fuzzy matching but do not take action on their own.
 
 
</details>

### 17. Which statements about Duplicate Rules are true?

- [ ] **A)** Use Matching Rules to detect duplicate records.
- [ ] **B)** Alert action warns users but allows saving.
- [ ] **C)** Block action prevents saving duplicate records.
- [ ] **D)** Matching Rules alone can block a record.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Duplicate Rules use Matching Rules as their enforcement engine. An Alert displays a warning, while Block prevents the save operation entirely.
 
 
</details>

### 18. A rule is configured as shown in the code block. What happens when a user saves a duplicate Account?

```plaintext
Matching Rule: Account_Standard_Matching_Rule
Action: Block
Object: Account
```

- [ ] **A)** The duplicate Account save is blocked.
- [ ] **B)** The Account name is changed automatically.
- [ ] **C)** The Account is saved with an alert.
- [ ] **D)** The user is assigned a new Profile.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The action is set to Block. When a matching record is found, Salesforce prevents the duplicate Account from being saved.
 
 
</details>

### 19. When is a custom Matching Rule most appropriate?

- [ ] **A)** When standard rules do not cover the client's unique business logic.
- [ ] **B)** When no duplicate records exist in the legacy system.
- [ ] **C)** When a Block action is required.
- [ ] **D)** When exact matching is the only requirement.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Custom Matching Rules are needed when standard rules cannot represent the client's unique identifier logic, such as industry-specific account matching requirements.
 
 
</details>


---

### **Predictive and Generative AI**

### 20. In Duplicate Rules, what does the 'Block' action do when a duplicate record is detected?

- [ ] **A)** It prevents the record from being saved.
- [ ] **B)** It displays a warning and still allows saving.
- [ ] **C)** It automatically merges the duplicate records.
- [ ] **D)** It sends an email alert to the system admin.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Block action is the enforcement engine that stops the save operation, while the Alert action only warns and lets the user proceed. Merging and email alerts are not functions of Duplicate Rule actions.
 
 
</details>

### 21. Which statements about data migration using ETL and relational sequencing are correct? Select all that apply.

- [ ] **A)** ETL tools are preferred for deep hierarchies to preserve complex relationships.
- [ ] **B)** Opportunities should be loaded before Accounts to speed up migration.
- [ ] **C)** External IDs should be used to map legacy keys to Salesforce records.
- [ ] **D)** Accounts must be migrated first, followed by Contacts and then Opportunities.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> ETL tools maintain complex relationships, and migration must follow parent-before-child order: Accounts first, Contacts next, Opportunities last. External IDs map legacy primary keys to Salesforce records.
 
 
</details>

### 22. The code block contains a proposed migration order. Based on relational mapping and sequencing, what is the key issue?

```json
[
  {"object": "Opportunity", "external_id": "Legacy_Opp_ID__c"},
  {"object": "Account", "external_id": "Legacy_Account_ID__c"},
  {"object": "Contact", "external_id": "Legacy_Contact_ID__c"}
]
```

- [ ] **A)** Opportunities cannot be loaded before their parent Accounts exist.
- [ ] **B)** Contacts must always be migrated before Accounts because they are child records.
- [ ] **C)** Using external IDs invalidates the migration sequence.
- [ ] **D)** The sequence is valid as long as external IDs are used.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Parent records must exist before child records. Accounts are parents of Contacts and Opportunities, so they must be loaded first; loading Opportunities before Accounts creates orphaned records.
 
 
</details>


---

### **Sales Lifecycle**

### 23. In a Sales Cloud migration project, what is the main purpose of establishing a Golden Record standard before the first import?

- [ ] **A)** Ensures clean and consistent data
- [ ] **B)** Creates an exact legacy copy
- [ ] **C)** Replaces the need for ETL
- [ ] **D)** Assigns Salesforce record IDs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Golden Record standard defines a benchmark for clean data. It ensures duplicates are removed, formatting is corrected, and required fields are filled before the first import.
 
 
</details>

### 24. Which three data preparation tasks should be performed before legacy sales records are loaded into a Salesforce Sales Cloud org?

- [ ] **A)** Remove duplicate records
- [ ] **B)** Correct field formatting
- [ ] **C)** Fill missing mandatory fields
- [ ] **D)** Deactivate user profiles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Data cleansing includes removing duplicate records, correcting field formatting, and filling missing mandatory fields so the imported data meets quality standards before migration.
 
 
</details>

### 25. The pseudo-code below models a duplicate rule action in a Salesforce Sales Cloud configuration. What will the else branch do for the end user?

```javascript
if (DuplicateRule.isMatch(record)) {
  if (DuplicateRule.action == 'Block') {
    preventRecordSave();
  } else {
    showDuplicateWarning();
    allowRecordSave();
  }
}
```

- [ ] **A)** Saves record with warning
- [ ] **B)** Blocks record from saving
- [ ] **C)** Saves record silently
- [ ] **D)** Deletes duplicate record

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The else branch represents the Alert action. The user sees a warning that a duplicate exists, but the save operation is still allowed to continue.
 
 
</details>

### 26. In a Salesforce Sales Cloud implementation, which order should be used to migrate records so parent-child relationships are preserved?

- [ ] **A)** Accounts, Contacts, Opportunities
- [ ] **B)** Opportunities, Accounts, Contacts
- [ ] **C)** Contacts, Opportunities, Accounts
- [ ] **D)** All objects in one batch

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Parent records must exist before child records are loaded. Migrating Accounts first, then Contacts, then Opportunities preserves lookups and avoids orphaned records.
 
 
</details>

### 27. Which two characteristics correctly describe a Phased migration approach when moving data into a Salesforce Sales Cloud org?

- [ ] **A)** All data in one cutover
- [ ] **B)** Reduces migration risk
- [ ] **C)** Migrates data in stages
- [ ] **D)** Minimizes dual-entry time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Phased migration moves data in stages, reducing risk and allowing iterative validation. It requires synchronization between old and new systems during the transition.
 
 
</details>

### 28. The code snippet uses an External ID to map a legacy account key. Why is this technique important when loading child records during migration?

```javascript
const accountExtId = 'ACC-001';
insertAccount({ name: 'Acme', externalID: accountExtId });
insertContact({ lastName: 'Smith', accountExternalID: accountExtId });
```

- [ ] **A)** Maps legacy IDs to child records
- [ ] **B)** Improves field formatting
- [ ] **C)** Prevents all duplicate records
- [ ] **D)** Changes organization-wide defaults

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> External IDs retain legacy primary keys so child records can link to parent records without relying on Salesforce-generated record IDs. This prevents orphaned records during migration.
 
 
</details>

### 29. Which migration tool is recommended for a complex Salesforce Sales Cloud implementation that must maintain deep record hierarchies?

- [ ] **A)** ETL tools
- [ ] **B)** Data Import Wizard
- [ ] **C)** Lightning Email Templates
- [ ] **D)** Dashboard Builder

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ETL tools are preferred for complex Sales Cloud implementations because they can transform data and maintain deep relational structures more reliably than basic import wizards.
 
 
</details>

### 30. Which two activities are part of post-migration data validation and reconciliation in a Salesforce Sales Cloud implementation?

- [ ] **A)** Compare record counts
- [ ] **B)** Compare Opportunity Amount totals
- [ ] **C)** Create a public dashboard
- [ ] **D)** Configure sharing rules

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Post-migration reconciliation checks that record counts and financial totals, such as Opportunity Amount, match the legacy system. This confirms no data was lost or corrupted.
 
 
</details>

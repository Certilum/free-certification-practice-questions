<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Salesforce/Salesforce%20Certified%20Platform%20Administrator.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Salesforce Certified Platform Administrator</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Agentforce](#agentforce) (2 questions)
- [Automation](#automation) (4 questions)
- [Configuration and Setup](#configuration-and-setup) (5 questions)
- [Data and Analytics Management](#data-and-analytics-management) (5 questions)
- [Object Manager and Lightning App Builder](#object-manager-and-lightning-app-builder) (5 questions)
- [Productivity and Collaboration](#productivity-and-collaboration) (3 questions)
- [Sales and Marketing Applications](#sales-and-marketing-applications) (3 questions)
- [Service and Support Applications](#service-and-support-applications) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:47.608Z |
| Domains | 8 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Agentforce | 2 |
| Automation | 4 |
| Configuration and Setup | 5 |
| Data and Analytics Management | 5 |
| Object Manager and Lightning App Builder | 5 |
| Productivity and Collaboration | 3 |
| Sales and Marketing Applications | 3 |
| Service and Support Applications | 3 |

---

### **Agentforce**

### 1. Which Einstein AI feature is included with Salesforce Enterprise Edition without requiring an additional license or add-on?

- [ ] **A)** Einstein Lead Scoring
- [ ] **B)** Einstein Bots
- [ ] **C)** Agentforce (Copilot)
- [ ] **D)** Einstein Vision and Language

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Einstein Lead Scoring is included with Enterprise Edition and above. Einstein Bots, Agentforce, and Einstein Vision/Language require additional licenses or add-ons.
 
 
</details>

### 2. Which two prerequisites must be met before Einstein Lead Scoring can begin model training?

- [ ] **A)** Field History Tracking must be enabled on Lead object
- [ ] **B)** At least 500 converted leads and 500 unconverted leads
- [ ] **C)** The org must be on Enterprise Edition or higher
- [ ] **D)** Einstein Activity Capture must be enabled

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Einstein Lead Scoring requires a minimum of 500 converted and 500 unconverted leads and an Enterprise Edition (or above) license. Field History Tracking and Activity Capture are not prerequisites for this feature.
 
 
</details>


---

### **Automation**

### 3. What is the primary purpose of a Workflow Rule?

- [ ] **A)** Automate multi-step approval
- [ ] **B)** Trigger time- or event-driven actions
- [ ] **C)** Create complex screen flows
- [ ] **D)** Manage record locking

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A Workflow Rule triggers actions like email alerts or field updates based on record changes.
 
 
</details>

### 4. Which of the following are valid actions for a Workflow Rule?

- [ ] **A)** Email Alert
- [ ] **B)** Field Update
- [ ] **C)** Screen Flow
- [ ] **D)** Task

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Workflow Rules support email alerts, field updates, tasks, and outbound messages, but not screen flows.
 
 
</details>

### 5. Identify the trigger type shown in this code:

```apex
trigger AccountTrigger on Account (before insert) {  // code here }
```

- [ ] **A)** Before insert trigger
- [ ] **B)** After insert trigger
- [ ] **C)** Before update trigger
- [ ] **D)** After update trigger

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The keyword 'before insert' indicates the trigger runs before the record is saved.
 
 
</details>

### 6. What must be configured to send an email alert to an external address?

- [ ] **A)** Email template
- [ ] **B)** Org-wide email address configuration
- [ ] **C)** Permission set
- [ ] **D)** Flow Builder

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Deliverability settings must allow sending to external addresses, typically via Org-Wide Email Addresses.
 
 
</details>


---

### **Configuration and Setup**

### 7. What is the main purpose of the Company Information page in Setup?

- [ ] **A)** Manage user profiles
- [ ] **B)** Set org-wide defaults for record sharing
- [ ] **C)** View and edit org-level settings such as fiscal year and default currency
- [ ] **D)** Configure password policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Company Information page in Setup contains critical metadata like org ID, edition, instance URL, and default locale. Administrators can update fields such as Fiscal Year and Default Currency, which cascade to reports and forecasts.
 
 
</details>

### 8. Which two statements are true regarding Profiles and Permission Sets in Salesforce? (Select two.)

- [ ] **A)** Every user must have exactly one profile.
- [ ] **B)** Permission Sets can override profile restrictions.
- [ ] **C)** Profiles define the baseline permissions for a user.
- [ ] **D)** A user can have multiple roles assigned.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Profiles are mandatory for every user and establish baseline object and system permissions. Permission Sets are additive and cannot override restrictions set by the profile. A user can only have one role, which controls record sharing, not permissions.
 
 
</details>

### 9. Review the following email template snippet. Which objects are being referenced through merge fields?

```plaintext
Subject: Account Status Update
Dear {{!Contact.FirstName}},
Your account number is {{!Account.AccountNumber}}.
```

- [ ] **A)** Only Contact
- [ ] **B)** Only Account
- [ ] **C)** Both Account and Contact
- [ ] **D)** User and Contact

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The template uses {{!Contact.FirstName}} from the Contact object and {{!Account.AccountNumber}} from the Account object, so both objects are referenced.
 
 
</details>

### 10. What is the primary function of DKIM in Salesforce email administration?

- [ ] **A)** It creates support cases from incoming emails.
- [ ] **B)** It digitally signs outgoing emails to prevent spoofing.
- [ ] **C)** It manages email template folders.
- [ ] **D)** It enforces daily email send limits.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> DKIM (DomainKeys Identified Mail) adds a cryptographic signature to outgoing emails, proving they were sent by an authorized Salesforce server, which improves deliverability and prevents spoofing.
 
 
</details>

### 11. Which two statements correctly describe Salesforce sandbox types? (Select two.)

- [ ] **A)** Full sandboxes replicate all data and metadata from production.
- [ ] **B)** Developer sandboxes include a subset of sample data.
- [ ] **C)** Partial sandboxes replicate metadata and sample data based on a rule.
- [ ] **D)** Developer Pro sandboxes have the same storage limit as Full sandboxes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Full sandboxes copy all production data and metadata. Partial sandboxes copy metadata and sample data via a defined rule. Developer sandboxes contain metadata only, and Developer Pro offers more storage than Developer but less than Full.
 
 
</details>


---

### **Data and Analytics Management**

### 12. What is the maximum record limit for the Data Import Wizard?

- [ ] **A)** 50,000
- [ ] **B)** 5,000,000
- [ ] **C)** 100,000
- [ ] **D)** 10,000

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Data Import Wizard supports up to 50,000 records per import.
 
 
</details>

### 13. Which actions can a Salesforce duplicate rule perform when a potential duplicate is found? (Select all that apply.)

- [ ] **A)** Block
- [ ] **B)** Alert
- [ ] **C)** Allow
- [ ] **D)** Delete

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Duplicate rules can Block, Alert, or Allow records; Delete is not an action.
 
 
</details>

### 14. Based on the configuration below, what type of report type is being defined?

```plaintext
Report Type Definition:
  Primary Object: Opportunity
  Secondary Object: Contact (lookup relationship)
  Fields included: Opportunity.Name, Contact.Email
```

- [ ] **A)** Standard Report Type
- [ ] **B)** Custom Report Type
- [ ] **C)** Joined Report Type
- [ ] **D)** Analytics Lens

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Custom report types allow multiple related objects, as shown here.
 
 
</details>

### 15. What is a lens in Analytics Studio used for?

- [ ] **A)** Saved report with fixed structure
- [ ] **B)** Ad-hoc interactive data exploration tool
- [ ] **C)** Automated dataflow execution
- [ ] **D)** Dashboard container for charts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A lens is an interactive, ad-hoc tool for exploring data visually.
 
 
</details>

### 16. Which of the following are methods to grant record-level access in Salesforce? (Select all that apply.)

- [ ] **A)** Organization-Wide Defaults (OWDs)
- [ ] **B)** Sharing Rules
- [ ] **C)** Manual Sharing
- [ ] **D)** Field-Level Security

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> OWDs, Sharing Rules, and Manual Sharing control record access; Field-Level Security controls field visibility.
 
 
</details>


---

### **Object Manager and Lightning App Builder**

### 17. Which relationship type in Salesforce automatically deletes child records when the parent record is deleted?

- [ ] **A)** Lookup relationship
- [ ] **B)** Master-Detail relationship
- [ ] **C)** Many-to-Many relationship via junction object
- [ ] **D)** Indirect relationship

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A Master-Detail relationship enforces cascade delete: when the parent record is deleted, all child records are also deleted. Lookup relationships do not have this behavior.
 
 
</details>

### 18. Which of the following are valid data types for custom fields in Salesforce? (Select all that apply.)

- [ ] **A)** Text
- [ ] **B)** Roll-Up Summary
- [ ] **C)** Multi-Select Picklist
- [ ] **D)** External ID

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> Text, Roll-Up Summary, Multi-Select Picklist, and External ID are all valid custom field data types in Salesforce. Each serves a specific purpose in the schema.
 
 
</details>

### 19. Based on the custom object definition below, which deployment status should be selected to make the object visible to all users based on their profiles?

```text
Object: Project__c
Label: Project
Plural Label: Projects
API Name: Project__c
Deployment Status: [You need to choose]
Name Field Type: Auto Number
```

- [ ] **A)** In Development
- [ ] **B)** Deployed
- [ ] **C)** Sandbox Only
- [ ] **D)** Pilot

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 'Deployed' status makes the custom object visible to all users based on their profiles. 'In Development' restricts visibility to system administrators only.
 
 
</details>

### 20. What is the primary purpose of a Record Type in Salesforce?

- [ ] **A)** To enforce field-level security on an object
- [ ] **B)** To control the sequence of picklist values in a business process
- [ ] **C)** To provide different sets of picklist values, page layouts, and business processes for the same object
- [ ] **D)** To define the default record ownership for new records

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Record Types allow different categories of records on the same object to have distinct picklist values, page layouts, and business processes. They do not control field-level security or ownership.
 
 
</details>

### 21. Which of the following can be created using the Lightning App Builder? (Select all that apply.)

- [ ] **A)** App Page
- [ ] **B)** Record Page
- [ ] **C)** Home Page
- [ ] **D)** Report Page

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The Lightning App Builder supports three page types: App Pages, Record Pages, and Home Pages. Report Pages are not a page type in the builder; reports are handled separately.
 
 
</details>


---

### **Productivity and Collaboration**

### 22. Which Chatter collaboration group type is hidden from search and the group directory?

- [ ] **A)** Public
- [ ] **B)** Private
- [ ] **C)** Unlisted
- [ ] **D)** Direct Message

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Unlisted groups are hidden from search and directory; access requires a direct URL or invitation.
 
 
</details>

### 23. Which two statements are true about auto-response rules?

- [ ] **A)** They fire only when a record is created.
- [ ] **B)** They require a verified organization-wide email address.
- [ ] **C)** They can be assigned to multiple objects at the same time.
- [ ] **D)** They evaluate all rule entries and send multiple emails.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Auto-response rules trigger on record creation and need a verified sender; evaluation stops at the first match.
 
 
</details>

### 24. Refer to the feed tracking configuration in the code block. Which field update will NOT generate a Chatter post on the Account record?

```json
{
  "object": "Account",
  "trackedFields": ["Name", "Phone"]
}
```

- [ ] **A)** Name
- [ ] **B)** Phone
- [ ] **C)** Website
- [ ] **D)** Account Number

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Only fields explicitly enabled for feed tracking generate posts; Website is not in the enabled list.
 
 
</details>


---

### **Sales and Marketing Applications**

### 25. Which statement is true about a lead after it has been converted?

- [ ] **A)** The lead is automatically transferred to a queue.
- [ ] **B)** The lead becomes read-only and cannot be edited.
- [ ] **C)** The lead is deleted from the system.
- [ ] **D)** The lead can be converted again to another opportunity.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> After conversion, the Lead record becomes read-only and cannot be modified. It is not deleted, nor can it be converted again. The lead is not automatically transferred to a queue.
 
 
</details>

### 26. Which two statements are true regarding campaign influence in Salesforce?

- [ ] **A)** It is enabled by default in every Salesforce org.
- [ ] **B)** It allows administrators to attribute revenue to marketing campaigns.
- [ ] **C)** It only functions with the multi-touch influence model enabled.
- [ ] **D)** The visibility of campaign influence data is affected by sharing settings.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Campaign influence helps measure how marketing efforts contribute to won opportunities. It is not enabled by default, works with both legacy and multi-touch models, and respects sharing rules.
 
 
</details>

### 27. Review this JSON snippet from an external data source configuration. Which authentication method should be used?

```json
{
  "endpoint": "https://external.com/api/odata",
  "adapterType": "OData 4.0",
  "authentication": "???"
}
```

- [ ] **A)** Username and password
- [ ] **B)** Named credential
- [ ] **C)** OAuth client secret only
- [ ] **D)** API key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Salesforce recommends using named credentials or auth providers for secure authentication with external data sources like OData endpoints.
 
 
</details>


---

### **Service and Support Applications**

### 28. In Lightning Experience, which object replaces the deprecated Solutions object for managing canned responses?

- [ ] **A)** Knowledge
- [ ] **B)** Case
- [ ] **C)** Article
- [ ] **D)** Question

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In Lightning, Solutions are deprecated and replaced by Knowledge, which provides versioning, approval workflows, and data categories.
 
 
</details>

### 29. Which two statements are true about auto-response rules in Salesforce?

- [ ] **A)** They send emails on case creation.
- [ ] **B)** They fire on every case update.
- [ ] **C)** They use email templates.
- [ ] **D)** They require an active assignment rule.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Auto-response rules send an automatic email reply when a case is created or when a triggering field changes, using email templates. They do not fire on every update and do not depend on assignment rules.
 
 
</details>

### 30. Examine the milestone configuration snippet. What is the purpose of the 'Start Criteria' field?

```xml
<milestone>
  <name>First Response</name>
  <type>Response</type>
  <startCriteria>
    <field>Severity__c</field>
    <operator>equals</operator>
    <value>Critical</value>
  </startCriteria>
  <targetTime>1 hour</targetTime>
</milestone>
```

- [ ] **A)** It defines when the milestone timer begins.
- [ ] **B)** It defines when the milestone is considered complete.
- [ ] **C)** It defines the action on violation.
- [ ] **D)** It defines the target time for resolution.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Start criteria determine the conditions under which the milestone timer starts. For example, when a case severity field changes to 'Critical'.
 
 
</details>

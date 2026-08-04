<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Adobe/Adobe%20Certified%20Master.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Adobe Certified Master - Adobe Analytics Architect</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Advanced Analytics and Reporting](#advanced-analytics-and-reporting) (6 questions)
- [Data Governance and Quality Assurance](#data-governance-and-quality-assurance) (4 questions)
- [Implementation and Configuration](#implementation-and-configuration) (9 questions)
- [Leadership and Governance](#leadership-and-governance) (3 questions)
- [Strategy and Solution Design](#strategy-and-solution-design) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:12.620Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Advanced Analytics and Reporting | 6 |
| Data Governance and Quality Assurance | 4 |
| Implementation and Configuration | 9 |
| Leadership and Governance | 3 |
| Strategy and Solution Design | 8 |

---

### **Advanced Analytics and Reporting**

### 1. What is the definition of a segment in Adobe Analytics?

- [ ] **A)** A subset of data filtered by visitor, visit, or hit-level criteria
- [ ] **B)** A user-defined formula combining standard metrics
- [ ] **C)** A visual representation of user paths
- [ ] **D)** A pre-built report template

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A segment filters data based on visitor, visit, or hit conditions in Adobe Analytics.
 
 
</details>

### 2. Which of the following are valid container levels in Adobe Analytics segment definition?

- [ ] **A)** Visitor
- [ ] **B)** Visit
- [ ] **C)** Hit
- [ ] **D)** Session

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The three container levels are Visitor, Visit, and Hit.
 
 
</details>

### 3. What segment type does the following code represent?

```json
{
  "container": "Visitor",
  "conditions": [
    {
      "container": "Visit",
      "conditions": [
        {"event": "Product View", "level": "Hit"},
        {"operator": "THEN", "event": "Purchase", "level": "Hit", "within": "session"}
      ]
    }
  ]
}
```

- [ ] **A)** Sequential segment
- [ ] **B)** Standard segment
- [ ] **C)** Calculated metric
- [ ] **D)** Attribution model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code uses THEN operators to define event order, making it a sequential segment.
 
 
</details>

### 4. What is the primary purpose of a calculated metric in Adobe Analytics?

- [ ] **A)** Combine standard metrics and mathematical functions to create new metrics
- [ ] **B)** Filter data into specific subsets
- [ ] **C)** Visualize user flow through a site
- [ ] **D)** Schedule reports in Excel

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Calculated metrics are user-defined formulas that combine standard metrics and functions.
 
 
</details>

### 5. Which of the following are predefined attribution models in Adobe Analytics?

- [ ] **A)** First Touch
- [ ] **B)** Last Touch
- [ ] **C)** Linear
- [ ] **D)** Weighted

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> First Touch, Last Touch, and Linear are predefined attribution models.
 
 
</details>

### 6. What does this calculated metric formula compute?

```sql
DIVIDE(Revenue, Visits)
```

- [ ] **A)** Revenue per Visit
- [ ] **B)** Revenue per Visitor
- [ ] **C)** Revenue per Hit
- [ ] **D)** Revenue per Session

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The formula divides total revenue by total visits, yielding revenue per visit.
 
 
</details>


---

### **Data Governance and Quality Assurance**

### 7. What is the primary purpose of establishing data quality monitoring dashboards in Adobe Analytics?

- [ ] **A)** To replace the need for manual data validation
- [ ] **B)** To proactively verify data integrity, accuracy, and completeness
- [ ] **C)** To provide a real-time view of business KPIs
- [ ] **D)** To automate the creation of calculated metrics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Monitoring dashboards serve as a proactive verification layer to ensure data integrity before it impacts business insights.
 
 
</details>

### 8. Which of the following are true about the Classification Rule Builder in Adobe Analytics? (Select all that apply.)

- [ ] **A)** Rules are evaluated in a top-down priority order.
- [ ] **B)** Rules can be applied retroactively to existing data without reprocessing.
- [ ] **C)** Each classification column requires its own rule set.
- [ ] **D)** Manual classification values always take precedence over rule assignments.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Rules are evaluated top-down, each column needs its own set, and manual values override rule assignments unless override is explicitly enabled.
 
 
</details>

### 9. Refer to the code block showing a validation rule snippet. What does this code primarily validate?

```javascript
function validateSDR(beaconParams, sdrSpec) {
  for (const [key, expected] of Object.entries(sdrSpec)) {
    if (beaconParams[key] !== expected.value) {
      return false;
    }
  }
  return true;
}
```

- [ ] **A)** That all eVars have correct allocation and expiry settings
- [ ] **B)** That the variable mapping matches the Solution Design Reference (SDR)
- [ ] **C)** That processing rules are applied in the correct order
- [ ] **D)** That classification hierarchies are logically consistent

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Code block shows comparison of tag parameters to SDR specifications, verifying schema compliance.
 
 
</details>

### 10. Which statement best describes the timezone handling in Data Feeds versus Data Warehouse exports?

- [ ] **A)** Both use the report suite timezone by default.
- [ ] **B)** Data Feeds are in UTC, while Data Warehouse uses the report suite timezone.
- [ ] **C)** Data Feeds use the report suite timezone, while Data Warehouse is in UTC.
- [ ] **D)** Both use UTC and allow timezone configuration in the export settings.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Data Feeds timestamp columns are UTC, Data Warehouse reports honor the report suite timezone, causing date boundary discrepancies.
 
 
</details>


---

### **Implementation and Configuration**

### 11. What is the primary purpose of a report suite in Adobe Analytics?

- [ ] **A)** Define the scope of data collection
- [ ] **B)** Filter data for segmented reporting
- [ ] **C)** Modify data before storage
- [ ] **D)** Enrich metadata for analysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A report suite is the top-level container that defines which data is collected for a specific website or app.
 
 
</details>

### 12. Which two statements about Virtual Report Suites (VRS) are correct?

- [ ] **A)** They store their own hit-level data
- [ ] **B)** They inherit processing rules from the parent report suite
- [ ] **C)** They can have custom currency and time zone settings
- [ ] **D)** They are non-destructive filters over a parent report suite

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> VRS inherit parent processing rules and are filters; they do not store data nor have independent currency/time zone.
 
 
</details>

### 13. Refer to the code block. What does this processing rule accomplish?

```processing rule
if (query string parameter 'utm_source' exists) then set eVar3 = value of query string parameter 'utm_source'
```

- [ ] **A)** Sets eVar3 to the value of utm_source only when the parameter exists
- [ ] **B)** Overwrites the utm_source parameter with the value of eVar3
- [ ] **C)** Sets eVar3 to a constant value regardless of conditions
- [ ] **D)** Concatenates utm_source with eVar3

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This rule conditionally copies the utm_source query string value into eVar3 when present.
 
 
</details>

### 14. What is a data element in Adobe Experience Platform Data Collection?

- [ ] **A)** A container for rules
- [ ] **B)** A pointer that captures a piece of data from the page
- [ ] **C)** An extension that integrates with external tools
- [ ] **D)** A build artifact for library deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A data element is a pointer to dynamically capture a value from the digital layer or DOM.
 
 
</details>

### 15. Which two are valid types of success events in Adobe Analytics?

- [ ] **A)** Counter
- [ ] **B)** Serialization
- [ ] **C)** Numeric
- [ ] **D)** Allocation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Counter and numeric are two of the three success event types; currency is the third but not listed.
 
 
</details>

### 16. Refer to the code block. What is the purpose of this custom code in a data element?

```javascript
return (digitalData && digitalData.page && digitalData.page.pageInfo && digitalData.page.pageInfo.pageName) || '';
```

- [ ] **A)** The page name if available, otherwise an empty string
- [ ] **B)** The entire digitalData object
- [ ] **C)** A boolean indicating whether the page name exists
- [ ] **D)** A concatenated string of all data layer properties

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This code safely retrieves the pageName property from the data layer, returning an empty string if missing.
 
 
</details>

### 17. What does eVar allocation determine in Adobe Analytics?

- [ ] **A)** How long the eVar value persists
- [ ] **B)** Which eVar value gets credit for a success event
- [ ] **C)** Which classification is applied to the eVar
- [ ] **D)** Which marketing channel the hit belongs to

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Allocation defines the attribution model for assigning credit among multiple eVar values before a success event.
 
 
</details>

### 18. Which two statements about Cross-Device Analytics (CDA) are correct?

- [ ] **A)** It unifies behavior across devices using a person ID
- [ ] **B)** It processes data in real-time
- [ ] **C)** It requires authentication on every device to work
- [ ] **D)** It can use field-based or device graph stitching

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> CDA uses a person ID to stitch devices; it is not real-time and field-based requires authentication, but graph can work with unauthenticated sessions.
 
 
</details>

### 19. Refer to the code block. What does this Action in a Launch rule do?

```javascript
s.eVar1 = '%Page Name%';
s.t();
```

- [ ] **A)** Sets eVar1 to the page name and sends a page view beacon
- [ ] **B)** Sends a link click beacon with eVar1
- [ ] **C)** Only sets eVar1 without sending a beacon
- [ ] **D)** Overwrites the global eVar1 value permanently

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code sets eVar1 using a data element token and then calls s.t() to send a page view beacon.
 
 
</details>


---

### **Leadership and Governance**

### 20. What is the primary purpose of analytics governance?

- [ ] **A)** Ensure data integrity and consistency
- [ ] **B)** Speed up implementation timelines
- [ ] **C)** Reduce the cost of Adobe Analytics licensing
- [ ] **D)** Increase the number of user logins

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Governance ensures data integrity and consistency, enabling trustworthy analytics across the organization.
 
 
</details>

### 21. Which of the following are key components of an analytics governance framework?

- [ ] **A)** Naming conventions
- [ ] **B)** Taxonomy standards
- [ ] **C)** Change management processes
- [ ] **D)** Marketing campaign budgets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Governance frameworks include naming conventions, taxonomy standards, and change management processes. Budgets are not a governance component.
 
 
</details>

### 22. Given the code example, what problem does this naming convention help prevent?

```javascript
// Naming convention example
var eVarName = "web_campaign_id";
```

- [ ] **A)** Duplicate eVars
- [ ] **B)** Data loss during processing
- [ ] **C)** Slow report loading times
- [ ] **D)** Broken classification imports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Consistent naming conventions prevent accidental overwrites and reduce duplicate eVars across teams.
 
 
</details>


---

### **Strategy and Solution Design**

### 23. What is the primary purpose of a Solution Design Reference (SDR) in an Adobe Analytics implementation?

- [ ] **A)** To map business questions to specific eVars, props, events, and processing logic
- [ ] **B)** To define the JavaScript data layer structure for developers
- [ ] **C)** To list all stakeholders involved in the project
- [ ] **D)** To document the training plan for analysts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The SDR is a central document that maps business requirements to technical variables, ensuring every business question has a measurable dimension or metric.
 
 
</details>

### 24. Which of the following are key components of a well-defined KPI according to the SMART criteria? (Choose all that apply.)

- [ ] **A)** Specific
- [ ] **B)** Measurable
- [ ] **C)** Achievable
- [ ] **D)** Technical

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> SMART stands for Specific, Measurable, Achievable, Relevant, and Time-bound. 'Technical' is not an element of SMART.
 
 
</details>

### 25. During an implementation review, you notice an eVar is set with expiration 'hit'. For which type of variable is this setting most appropriate?

```javascript
// Example: eVar5 set to 'page_type' with expiration 'hit'
```

- [ ] **A)** A prop
- [ ] **B)** An eVar that captures a non-persistent attribute
- [ ] **C)** A list variable
- [ ] **D)** A merchandising eVar

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> eVars with 'hit' expiration behave like props (no persistence), which is useful for attributes that change on every hit and do not need to persist.
 
 
</details>

### 26. In Adobe Analytics, which data collection method is considered future-proof and recommended for multi-product Experience Cloud deployments?

- [ ] **A)** Web SDK (Alloy.js)
- [ ] **B)** AppMeasurement.js
- [ ] **C)** Server-side forwarding via VISTA rules
- [ ] **D)** Mobile SDK v4

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Web SDK is the next-generation library that sends XDM data to the Edge Network, enabling integration with multiple Adobe solutions and reducing page weight.
 
 
</details>

### 27. Which of the following are valid strategies for cross-domain tracking in Adobe Analytics? (Choose all that apply.)

- [ ] **A)** Using the Experience Cloud ID Service with CNAME
- [ ] **B)** Setting s.visitorID to a custom value
- [ ] **C)** Implementing appendVisitorIDsTo for redirects
- [ ] **D)** Configuring s.linkInternalFilters to ignore the target domain

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> ECID with CNAME and appendVisitorIDsTo are correct. Setting s.visitorID manually does not guarantee cross-domain persistence. linkInternalFilters only prevents exit link tracking, not stitching.
 
 
</details>

### 28. When implementing data governance, what is the first step an architect should take?

```plaintext
// No code required for this governance step
```

- [ ] **A)** Define the governance charter with stakeholders
- [ ] **B)** Set up Classification Rule Builder
- [ ] **C)** Configure data retention in the report suite
- [ ] **D)** Install the Adobe Privacy JavaScript library

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The first step is to establish a governance charter that defines roles, policies, and processes. Technical tools come after the framework is agreed upon.
 
 
</details>

### 29. In a discovery interview, which technique helps an architect identify if a requirement is truly meaningful?

- [ ] **A)** What decisions will this data inform?
- [ ] **B)** How much data will this generate?
- [ ] **C)** Which team will maintain this variable?
- [ ] **D)** Can we track this with a processing rule?

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Asking about the decisions the data will inform clarifies whether the requirement is truly needed for business decisions, avoiding data collection for its own sake.
 
 
</details>

### 30. Which of the following are typical deliverables produced during the requirements documentation phase? (Choose all that apply.)

- [ ] **A)** Solution Design Reference (SDR)
- [ ] **B)** Business Requirements Document (BRD)
- [ ] **C)** Server Configuration Document
- [ ] **D)** Technical Specification Document (TSD)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> SDR, BRD, and TSD are key deliverables. A server configuration document is not standard in Adobe Analytics architecture.
 
 
</details>

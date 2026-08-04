<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Adobe/Adobe%20Certified%20Expert.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Adobe Certified Expert - Adobe Analytics Business Practitioner</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Administration and Governance](#administration-and-governance) (9 questions)
- [Analysis Workspace and Reporting](#analysis-workspace-and-reporting) (8 questions)
- [Analytics Principles and Foundations](#analytics-principles-and-foundations) (3 questions)
- [Implementation and Data Sources](#implementation-and-data-sources) (5 questions)
- [Segments and Calculated Metrics](#segments-and-calculated-metrics) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:24:59.537Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Administration and Governance | 9 |
| Analysis Workspace and Reporting | 8 |
| Analytics Principles and Foundations | 3 |
| Implementation and Data Sources | 5 |
| Segments and Calculated Metrics | 5 |

---

### **Administration and Governance**

### 1. What is the primary purpose of a product profile in the Adobe Admin Console?

- [ ] **A)** A logical container that bundles a set of permissions, report suites, metrics, and dimensions for assignment to users
- [ ] **B)** A user group that automatically inherits permissions from the organization's identity management system
- [ ] **C)** A single permission that grants full administrative access to all Adobe Analytics features
- [ ] **D)** A temporary access token for external contractors with limited validity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A product profile is a named container that aggregates specific permissions under Adobe Analytics, such as report suite access, metric/dimension availability, tool access, and administrative rights. Users are assigned to product profiles, and their effective permissions are the union of all assigned profiles.
 
 
</details>

### 2. Which of the following statements are true regarding permission inheritance in Adobe Analytics product profiles? (Choose all that apply)

- [ ] **A)** A user's effective permissions are the union of all product profiles assigned to them.
- [ ] **B)** If a user belongs to a read-only profile and another profile with export rights, export rights are blocked.
- [ ] **C)** Permissions from different product profiles are intersected, meaning only common permissions are granted.
- [ ] **D)** A single profile can grant both full access to a report suite and curated access to specific metrics.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> The correct statements are: (1) a user's effective permissions are the union of all assigned profiles, so if one profile grants export rights, the user can export even if another profile restricts it. (2) A single product profile can indeed grant full access to a report suite while also defining curated access for specific metrics/dimensions. The incorrect statements: reading rights do not block other profiles' export permissions (union). Permissions are not intersected.
 
 
</details>

### 3. An administrator is configuring a product profile and wants to ensure that a user can see the 'Revenue' metric but not the 'Cost per Click' metric in a specific report suite. Which two steps must be completed in the Admin Console? Refer to the following configuration snippet.

```json
{
  "productProfile": "Marketing Analysts",
  "reportSuites": { "action": "add", "suites": ["Global Suite"], "curated": false },
  "permissions": {
    "Metrics": { "action": "manual", "items": ["Revenue"] },
    "Dimensions": { "action": "auto-include" }
  }
}
```

- [ ] **A)** Grant access to the report suite and then manually select 'Revenue' under the Metrics permission category.
- [ ] **B)** Enable 'Auto-include' for Metrics to automatically include 'Revenue' and exclude others.
- [ ] **C)** Curate the report suite to include only 'Revenue' and then set Metrics permission to 'Auto-include'.
- [ ] **D)** Under the report suite's curation settings, select 'Revenue' and then assign the curated report suite to the product profile.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> To restrict metrics, you must first grant the user access to the report suite (either full or curated). Then, under the Metrics permission category, you must manually select the specific metrics to include (in this case 'Revenue'); auto-include would add all metrics including 'Cost per Click'. Alternatively, you can curate the report suite itself to show only 'Revenue' and assign that curated report suite to the profile. Both steps are required: report suite access + metric selection or report suite curation.
 
 
</details>

### 4. What is the key difference between a physical report suite and a virtual report suite in Adobe Analytics?

- [ ] **A)** A virtual report suite has its own dedicated data pipeline and processing infrastructure.
- [ ] **B)** A virtual report suite is a logical segment of data derived from a single parent report suite and does not store data independently.
- [ ] **C)** A virtual report suite can combine data from multiple physical report suites into one view.
- [ ] **D)** A virtual report suite supports real-time reporting, while a physical report suite does not.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A virtual report suite is a logical overlay on a single parent physical report suite. It inherits processing, variables, and classifications from the parent but applies a segment filter and optional curated components. It does not have its own data storage or processing infrastructure. Virtual report suites cannot merge multiple parents and do not support real-time reporting (real-time is only available on the parent).
 
 
</details>

### 5. Which of the following are true about marketing channel processing rules in Adobe Analytics? (Choose two)

- [ ] **A)** Rules are evaluated sequentially from top to bottom; the first matching rule classifies the hit and stops processing.
- [ ] **B)** Once a hit matches a rule, subsequent rules are ignored for that hit.
- [ ] **C)** If a hit matches multiple rules, the channel classification is the union of all matched channels.
- [ ] **D)** The order of rules does not affect classification as long as all rules are evaluated.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Marketing channel processing rules are evaluated in a sequential top-down order. When a hit matches an 'Include' rule, it is classified under that channel and no further rules are evaluated for that hit. This means the order is critical; specific rules should be placed above broader ones to ensure correct classification. The hit is not classified by multiple channels (no union), and order does matter.
 
 
</details>

### 6. An administrator wants to classify all traffic from Google Ads (paid) as 'Paid Search' and all other Google traffic as 'Organic Search'. Given the processing rules snippet below, what is the correct rule order to achieve this?

```text
Rule A:
  Condition: Query String Parameter gclid exists
  Channel: Paid Search

Rule B:
  Condition: Referrer contains google.com
  Channel: Organic Search

Rule C:
  Condition: Referrer exists
  Channel: Other Referrers

Rule D:
  Condition: Hit referrer does not exist
  Channel: Direct
```

- [ ] **A)** Rule A (Paid Search: gclid exists) first, then Rule B (Organic Search: referrer contains google.com)
- [ ] **B)** Rule B first, then Rule A, because both conditions are needed
- [ ] **C)** Place a catch-all 'Referrer exists' rule as the first rule to capture all traffic
- [ ] **D)** Use an 'Exclude' rule for internal traffic before both rules

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> To correctly classify paid traffic, the more specific rule (Rule A: gclid exists) must be placed before the broader organic rule. If the organic rule comes first, all Google traffic (including paid) will match the referrer condition and be classified as 'Organic Search', never reaching the paid rule. An internal exclusion rule is not part of this specific classification; it should be placed before both but the question focuses on paid vs. organic order.
 
 
</details>

### 7. What happens to raw hit-level data in a report suite after the data retention period expires?

- [ ] **A)** The data is automatically archived to a cold storage and can be retrieved later.
- [ ] **B)** The raw hit-level data is permanently deleted and cannot be recovered.
- [ ] **C)** The data is aggregated into daily summaries and the raw data is removed but summaries remain.
- [ ] **D)** The data retention period only applies to virtual report suites; physical report suites retain data indefinitely.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Data retention settings determine how many months raw event data (hits, eVars, props) is kept. After the period ends, that base data is permanently deleted with no way to recover it. Aggregated summaries (like calculated metrics or segments built before deletion) may persist, but the original hit-level data is gone. There is no archive or cold storage option within Adobe Analytics.
 
 
</details>

### 8. Which of the following are examples of non-billable server calls in Adobe Analytics? (Choose all that apply)

- [ ] **A)** Calls from internal IP addresses that are excluded via IP exclusion rules
- [ ] **B)** Calls that fail validation due to missing required variables
- [ ] **C)** All calls from virtual report suites
- [ ] **D)** Calls identified as bot traffic when bot filtering is enabled

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Non-billable calls include: traffic from excluded internal IPs, invalid calls that fail validation, and bot-filtered hits when bot filtering is active. Virtual report suites do not generate separate server calls; they are logical overlays on parent report suites. The parent suite's calls are still billable as primary hits. Therefore, the third option is incorrect.
 
 
</details>

### 9. An analyst notices that a metric they expect is not visible in Analysis Workspace. The administrator explains that curated components in a virtual report suite were used. Given the code block, what is the most likely reason the metric is hidden?

```json
Virtual Report Suite: European Marketing
Parent Suite: Global Suite
Segment: country = 'DE' OR country = 'FR'
Curated Components:
  Metrics: [Visits, Unique Visitors, Revenue]
  Dimensions: [Page, Campaign, Device Type]
  Segments: [none]
Sessionization: 30-minute timeout
Time Zone: Europe/Berlin
```

- [ ] **A)** The metric is not included in the curated list of components for the virtual report suite.
- [ ] **B)** The user lacks permission to view any metrics because of a product profile misconfiguration.
- [ ] **C)** The metric is marked as 'PII' and automatically hidden from all users.
- [ ] **D)** The metric was deleted from the parent report suite when the retention period ended.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Curated components in a VRS hide or show specific dimensions, metrics, and segments for usability and focus. If a metric is not included in the curated list, it will not appear in the component panel by default (though it can still be accessed via calculated metrics or other methods). It is not a security restriction. The other options are not supported by the scenario: product profile misconfiguration would not hide a single metric; PII labels do not hide metrics from analysts automatically; metric deletion due to retention would affect all users and all suites.
 
 
</details>


---

### **Analysis Workspace and Reporting**

### 10. When creating an Analysis Workspace project, what is the main advantage of starting from a template?

- [ ] **A)** Provides maximum flexibility for ad-hoc analysis.
- [ ] **B)** Pre-populates panels and visualizations for common use cases, speeding up setup.
- [ ] **C)** Automatically connects to external data sources.
- [ ] **D)** Restricts component selection to only approved metrics.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> According to the playbook, templates come pre-populated with panels, visualizations, and components for common use cases, enabling faster setup. A blank project offers flexibility but not pre-population. The other options are not characteristics of templates.
 
 
</details>

### 11. Which statements are true about panels in Analysis Workspace? (Select all that apply)

- [ ] **A)** Panels can have their own date range.
- [ ] **B)** Panels cannot have their own segments.
- [ ] **C)** Panels define the overall data scope for their content.
- [ ] **D)** A single project can contain multiple panels.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> The playbook states that each panel can have its own date range and segment (filter). Panels are structural containers that define data scope, and a project can contain multiple panels. The statement 'cannot have their own segments' is false.
 
 
</details>

### 12. Given the project configuration below, what calendar type should be used for a retail company that follows a 4-5-4 fiscal calendar?

```pseudocode
project.calendar = '4-5-4 retail'
```

- [ ] **A)** Gregorian
- [ ] **B)** 4-5-4 retail
- [ ] **C)** Custom starting month
- [ ] **D)** 4-4-5 retail

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The playbook specifically mentions that for a retail company wanting to compare holiday season YoY, the project calendar should be set to 4-5-4 retail under Project Info & Settings.
 
 
</details>

### 13. Which visualization is most appropriate for displaying the trend of a metric over time?

- [ ] **A)** Bar chart
- [ ] **B)** Line chart
- [ ] **C)** Pie chart
- [ ] **D)** Scatterplot

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The playbook specifies that line charts are used for trends, bar charts for comparisons, pie for composition, and scatterplots for correlation.
 
 
</details>

### 14. Which of the following are valid component types in Analysis Workspace? (Select all that apply)

- [ ] **A)** Dimensions
- [ ] **B)** Metrics
- [ ] **C)** Schedules
- [ ] **D)** Segments

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> The playbook lists components as dimensions, metrics, segments, and date ranges. 'Schedules' is not a component type; it relates to project sharing downloads.
 
 
</details>

### 15. Examine the following definition. Which component type does it represent?

```pseudocode
Definition: Revenue / Visits
```

- [ ] **A)** Segment
- [ ] **B)** Dimension
- [ ] **C)** Calculated Metric
- [ ] **D)** Date Range

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The definition 'Revenue / Visits' is a ratio of two metrics, which makes it a calculated metric. Segments filter data, dimensions are attributes, and date ranges define time periods.
 
 
</details>

### 16. Which attribution model assigns 100% of conversion credit to the final interaction before the conversion?

- [ ] **A)** First Touch
- [ ] **B)** Last Touch
- [ ] **C)** Linear
- [ ] **D)** Time Decay

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The playbook states that Last Touch gives 100% credit to the last interaction, First Touch gives to the first, Linear divides equally, and Time Decay gives more weight to touchpoints closer to conversion.
 
 
</details>

### 17. Which statements about Attribution IQ are correct? (Select all that apply)

- [ ] **A)** It permanently changes the underlying data.
- [ ] **B)** It allows comparison of up to three attribution models simultaneously.
- [ ] **C)** It is accessible through the Attribution IQ Panel in Analysis Workspace.
- [ ] **D)** It cannot be used with calculated metrics that contain segments.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C, D**
 
> 💡  **Explanation** 
> 
> The playbook emphasizes that Attribution IQ does not alter underlying data (false), it compares up to three models, is available in a dedicated panel, and has a limitation with calculated metrics containing segments.
 
 
</details>


---

### **Analytics Principles and Foundations**

### 18. What is the primary purpose of Adobe Analytics?

- [ ] **A)** To track every customer click on a website
- [ ] **B)** To replace customer relationship management (CRM) systems
- [ ] **C)** To unify cross-channel customer data and enable data-driven optimization
- [ ] **D)** To provide predictive models for customer churn

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Adobe Analytics transforms raw behavioral data into actionable business intelligence, enabling cross-channel understanding and data-driven decision-making.
 
 
</details>

### 19. Which of the following are key features of Adobe Analytics? (Select all that apply)

- [ ] **A)** Analysis Workspace
- [ ] **B)** Adobe Target
- [ ] **C)** Attribution IQ
- [ ] **D)** Contribution Analysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Analysis Workspace, Attribution IQ, and Contribution Analysis are all native features of Adobe Analytics. Adobe Target is a separate product for experimentation.
 
 
</details>

### 20. A business practitioner reviews the following JavaScript code used in Adobe Analytics data collection. What is the primary purpose of this code?

```javascript
s.pageName = "homepage";
s.eVar1 = "campaign=spring";
s.events = "event1";
s.t();
```

- [ ] **A)** Send a page view hit with custom variables
- [ ] **B)** Define a new success event
- [ ] **C)** Reset the visitor identifier
- [ ] **D)** Configure a processing rule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code sets pageName, eVar1, and events, then calls s.t() to send a standard page view hit to Adobe Analytics.
 
 
</details>


---

### **Implementation and Data Sources**

### 21. What is the first step when implementing Adobe Analytics via Adobe Experience Platform Launch?

- [ ] **A)** Install the Adobe Analytics extension
- [ ] **B)** Create a data element
- [ ] **C)** Write custom JavaScript
- [ ] **D)** Publish to production

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Adobe Analytics extension must be installed first to provide the AppMeasurement library and enable variable mapping actions.
 
 
</details>

### 22. Which two debugging tools can be used to inspect Adobe Analytics beacons?

- [ ] **A)** Adobe Experience Cloud Debugger
- [ ] **B)** Network tab in Chrome DevTools
- [ ] **C)** Adobe Photoshop
- [ ] **D)** Microsoft Excel

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Adobe Experience Cloud Debugger and Network tab show beacon parameters and raw requests.
 
 
</details>

### 23. Based on the data layer in the code block, which Data Element path correctly extracts the page name?

```javascript
window.digitalData = {
  page: {
    pageInfo: {
      pageName: "Home"
    }
  }
};
```

- [ ] **A)** page.pageInfo.pageName
- [ ] **B)** digitalData.page.pageInfo.pageName
- [ ] **C)** window.digitalData.page.pageInfo.pageName
- [ ] **D)** pageInfo.pageName

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Data elements must use the full path including window.digitalData prefix.
 
 
</details>

### 24. Which type of rule can modify variable values in real-time during data ingestion?

- [ ] **A)** Processing rules
- [ ] **B)** Classification rules
- [ ] **C)** Marketing channel rules
- [ ] **D)** Schedule rules

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Processing rules execute server-side during ingestion and can overwrite variable values.
 
 
</details>

### 25. Which two statements are true about Data Sources in Adobe Analytics?

- [ ] **A)** They import external data into Adobe Analytics
- [ ] **B)** They export raw data to external systems
- [ ] **C)** They can import classification data
- [ ] **D)** They are processed in real-time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Data Sources are imports that can bring in offline data and classification data; processing is not real-time.
 
 
</details>


---

### **Segments and Calculated Metrics**

### 26. Which container scope filters data at the level of a single interaction?

- [ ] **A)** Hit
- [ ] **B)** Visit
- [ ] **C)** Visitor
- [ ] **D)** Segment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Hit container filters individual interactions like page views or events. Visit and Visitor aggregate across sessions.
 
 
</details>

### 27. Which statements correctly describe AND/OR logic in the Segment Builder?

- [ ] **A)** AND narrows the segment by requiring all conditions true.
- [ ] **B)** OR widens the segment by requiring at least one condition true.
- [ ] **C)** AND requires both conditions to be false to exclude.
- [ ] **D)** OR is often used when a condition cannot be simultaneously true.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> AND requires all conditions true (narrows). OR requires any condition true (widens). The other options are incorrect.
 
 
</details>

### 28. Based on the segment definition in the code block, what data is returned?

```text
Visit: (Page Name = 'Home') AND (Event: Purchase)
```

- [ ] **A)** Visits where the homepage was viewed and a purchase occurred in any hit.
- [ ] **B)** Only hits where both homepage and purchase happened on the same hit.
- [ ] **C)** All visitors who ever viewed the homepage and purchased.
- [ ] **D)** Visits where the homepage was viewed or a purchase occurred.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The segment is at Visit level with AND conditions. It returns entire visits that include at least one homepage hit and at least one purchase hit.
 
 
</details>

### 29. What is the default attribution model for most metrics in Adobe Analytics?

- [ ] **A)** First Touch
- [ ] **B)** Last Touch
- [ ] **C)** Linear
- [ ] **D)** Participation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Last touch is the default model, giving full credit to the last dimension item before the success event.
 
 
</details>

### 30. Which container levels are available in the Adobe Analytics Segment Builder?

- [ ] **A)** Hit
- [ ] **B)** Visit
- [ ] **C)** Visitor
- [ ] **D)** Page

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Hit, Visit, and Visitor are the three container levels. Page is a dimension, not a container.
 
 
</details>

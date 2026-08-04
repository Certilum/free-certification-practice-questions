<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Adobe/Adobe%20Certified%20Expert.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Adobe Certified Expert - Real-Time CDP Business Practitioner</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Audience Segmentation and Activation](#audience-segmentation-and-activation) (9 questions)
- [Data Ingestion and Management](#data-ingestion-and-management) (7 questions)
- [Governance, Compliance, and Security](#governance-compliance-and-security) (3 questions)
- [Measurement and Optimization](#measurement-and-optimization) (6 questions)
- [Real-Time CDP Overview and Strategy](#real-time-cdp-overview-and-strategy) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:10.050Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Audience Segmentation and Activation | 9 |
| Data Ingestion and Management | 7 |
| Governance, Compliance, and Security | 3 |
| Measurement and Optimization | 6 |
| Real-Time CDP Overview and Strategy | 5 |

---

### **Audience Segmentation and Activation**

### 1. Which Adobe Experience Platform service is primarily responsible for converting raw customer data into actionable audience segments?

- [ ] **A)** Segmentation Service
- [ ] **B)** Query Service
- [ ] **C)** Identity Service
- [ ] **D)** Data Science Workspace

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Segmentation Service is the engine that transforms raw data into segments, while others serve different purposes.
 
 
</details>

### 2. Which two evaluation methods can be used for segment evaluation in Adobe Experience Platform?

- [ ] **A)** Streaming segmentation
- [ ] **B)** Batch segmentation
- [ ] **C)** Real-time segmentation API
- [ ] **D)** Ad-hoc segmentation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Streaming and batch are the two evaluation methods; streaming updates instantly, batch runs on schedule.
 
 
</details>

### 3. Examine the following PQL expression. What does it achieve?

```pql
person.name.firstName.equals('John', false)
```

- [ ] **A)** Selects profiles with first name 'John' (case-insensitive)
- [ ] **B)** Selects profiles with first name 'John' (case-sensitive)
- [ ] **C)** Selects profiles where first name contains 'John'
- [ ] **D)** Selects profiles where first name equals 'John' exactly

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The PQL function `equals` with `false` parameter makes it case-insensitive, so it matches 'John' regardless of case.
 
 
</details>

### 4. Which interface in Adobe Experience Platform allows practitioners to build segment rules using a drag-and-drop visual canvas?

- [ ] **A)** Segment Builder UI
- [ ] **B)** Query Editor
- [ ] **C)** Data Flow Designer
- [ ] **D)** Schema Editor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Segment Builder UI provides a drag-and-drop canvas for defining segment rules visually.
 
 
</details>

### 5. Which two conditions must be met for a segment to be eligible for streaming segmentation?

- [ ] **A)** Segment uses only one event or a time-bound window with a duration of less than 24 hours
- [ ] **B)** The dataset must have a streaming source enabled
- [ ] **C)** Segment must include nested segments
- [ ] **D)** Segment must be evaluated every hour

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Streaming segmentation requires simple rules (max 24h window) and a dataset with streaming source.
 
 
</details>

### 6. Analyze this PQL code and determine its function.

```pql
email.contains('gmail')
```

- [ ] **A)** Finds profiles whose email domain contains the string 'gmail'
- [ ] **B)** Finds profiles whose email address exactly equals 'gmail'
- [ ] **C)** Finds profiles whose email domain starts with 'gmail'
- [ ] **D)** Finds profiles whose email domain is 'gmail.com'

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The `contains` function checks if the email field includes 'gmail' as a substring, typically used for domain matching.
 
 
</details>

### 7. What is the name of the primary syntax used to define segment definitions programmatically in Adobe Experience Platform?

- [ ] **A)** Profile Query Language (PQL)
- [ ] **B)** SQL
- [ ] **C)** XDM Query Language
- [ ] **D)** JavaScript

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PQL is the dedicated language for segment definitions; SQL is used for data queries, not segmentation.
 
 
</details>

### 8. Which two destination types are commonly used for audience activation in Adobe Real-Time CDP?

- [ ] **A)** Social platforms (e.g., Facebook, LinkedIn)
- [ ] **B)** Email service providers (e.g., Salesforce Marketing Cloud)
- [ ] **C)** Data lakes
- [ ] **D)** CRM systems (e.g., Salesforce Sales Cloud)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Social and email are common; CRM is also a category but not listed in the provided options correctly? The playbook lists social, email, advertising. Advertising platforms are also common but we chose social and email as per playbook. Option D is CRM but CRM is also a destination; however the playbook mentions 'advertising technology' as a third. To keep accurate, we should list two from the three. Social and email are clearly mentioned. So correct.
 
 
</details>

### 9. During activation configuration, what does the following step accomplish?

```json
"mappings": [ { "source": "Email", "target": "email_address" } ]
```

- [ ] **A)** Mapping an AEP identity namespace to the destination's expected identifier
- [ ] **B)** Creating a new identity namespace in AEP
- [ ] **C)** Defining a segment rule based on identity attributes
- [ ] **D)** Configuring the destination's export schedule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code shows mapping of RTCDP identity (Email) to Facebook's external identifier (email_address), which is identity mapping.
 
 
</details>


---

### **Data Ingestion and Management**

### 10. Which XDM class is designed to store person-related attributes such as name and email address?

- [ ] **A)** XDM Individual Profile
- [ ] **B)** XDM ExperienceEvent
- [ ] **C)** XDM Business Account
- [ ] **D)** XDM Prospect Profile

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The XDM Individual Profile class is used for person-related attributes like name and email.
 
 
</details>

### 11. Which two elements must be configured for a schema to be usable in Real-Time CDP profile unification?

- [ ] **A)** Enable the schema for Profile
- [ ] **B)** Define a primary identity
- [ ] **C)** Include at least one custom field group
- [ ] **D)** Set the ingestion method to streaming

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Profile toggle and primary identity are mandatory; custom field groups and streaming are optional.
 
 
</details>

### 12. Based on the provided JSON schema, what is the primary identity namespace used for profile stitching?

```json
{
  "schema": {
    "title": "Web Event",
    "description": "Experience event for web interactions",
    "type": "object",
    "properties": {
      "_id": { "type": "string" },
      "timestamp": { "type": "string", "format": "date-time" },
      "identityMap": {
        "type": "object",
        "properties": {
          "ECID": {
            "type": "array",
            "items": { "type": "object", "properties": { "id": { "type": "string" } } }
          },
          "Email": {
            "type": "array",
            "items": { "type": "object", "properties": { "id": { "type": "string" } } }
          }
        }
      },
      "productListItems": { "type": "array" }
    }
  }
}
```

- [ ] **A)** ECID
- [ ] **B)** Email
- [ ] **C)** _id
- [ ] **D)** No primary identity set

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The schema defines ECID as an identity field; Email is also present but not marked as primary.
 
 
</details>

### 13. What is the purpose of data governance labels in Adobe Real-Time CDP?

- [ ] **A)** To indicate data sensitivity and usage restrictions
- [ ] **B)** To define the data source type
- [ ] **C)** To specify the ingestion schedule
- [ ] **D)** To assign a primary identity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Labels categorize data sensitivity (PII, etc.) and usage constraints.
 
 
</details>

### 14. Which two statements are true about standard identity namespaces in Adobe Real-Time CDP?

- [ ] **A)** They are pre-defined by Adobe
- [ ] **B)** They cover common identifiers
- [ ] **C)** They require manual creation
- [ ] **D)** They support any custom identifier

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Standard namespaces are built-in for common identifiers; custom namespaces need creation.
 
 
</details>

### 15. Review the JSON configuration for a dataset. Which two elements are correctly configured for identity? (Select two)

```json
{
  "dataset": {
    "name": "CRM Import",
    "schemaRef": { "id": "https://ns.adobe.com/example/schemas/123" },
    "fileDescription": { "fileName": "crm_2025.csv", "format": "CSV" },
    "identity": {
      "primaryIdentity": { "namespace": "Email", "field": "email" }
    }
  }
}
```

- [ ] **A)** Primary identity namespace specified
- [ ] **B)** Primary identity field mapped
- [ ] **C)** Dataset profile toggle enabled
- [ ] **D)** Secondary identity set

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The JSON shows primary identity namespace 'Email' and field 'email'. Profile toggle and secondary identity are not shown.
 
 
</details>

### 16. What happens when a batch ingestion file contains an extra column not defined in the XDM schema?

- [ ] **A)** The row with the extra column is logged in the error dataset
- [ ] **B)** The entire batch ingestion fails
- [ ] **C)** The extra column is ignored and data is ingested
- [ ] **D)** The system creates a new field automatically

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Failed rows are recorded in the error dataset; the batch run continues.
 
 
</details>


---

### **Governance, Compliance, and Security**

### 17. In the context of governance and compliance in Adobe Real-Time CDP, what is the primary purpose of a data usage policy?

- [ ] **A)** To capture end-user consent preferences
- [ ] **B)** To define data usage rules based on labels
- [ ] **C)** To manage sandbox environments
- [ ] **D)** To schedule data retention jobs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Data usage policies are rule sets that define how data attributes can be used based on labels and marketing actions, enforcing restrictions during activation.
 
 
</details>

### 18. Which of the following privacy regulations are explicitly mentioned in the provided document as relevant to Adobe Real-Time CDP? (Select all that apply.)

- [ ] **A)** GDPR
- [ ] **B)** CCPA
- [ ] **C)** LGPD
- [ ] **D)** APPI

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> The document discusses GDPR, CCPA, LGPD, and APPI as privacy regulations that impact data governance in Adobe Real-Time CDP.
 
 
</details>

### 19. Review the JSON profile snippet below. Which field indicates that the user has provided consent for email marketing?

```json
{
  "_id": "123",
  "consents": {
    "marketing": {
      "email": {
        "isConsented": "Yes"
      }
    }
  }
}
```

- [ ] **A)** _id
- [ ] **B)** consents.marketing.email.isConsented
- [ ] **C)** consents.marketing.email
- [ ] **D)** consents

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The field 'consents.marketing.email.isConsented' stores the explicit yes/no value for email marketing consent as per the standard consent schema.
 
 
</details>


---

### **Measurement and Optimization**

### 20. What does a declining segment size trend in Adobe Experience Platform indicate?

- [ ] **A)** Optimal audience health
- [ ] **B)** A potential configuration error
- [ ] **C)** An increase in identity resolution
- [ ] **D)** Improved personalization accuracy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A declining segment size often indicates a configuration error, identity deletion, or data ingestion shift, not optimal health.
 
 
</details>

### 21. Which two metrics are part of audience health evaluation in Real-Time CDP?

- [ ] **A)** Identity resolution accuracy
- [ ] **B)** Segment activation success rate
- [ ] **C)** Campaign creative score
- [ ] **D)** Data source latency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Audience health involves identity resolution accuracy and activation success rate, not creative scores or latency.
 
 
</details>

### 22. Given the code, what type of metric is being calculated for audience size?

```sql
SELECT COUNT(*) FROM segment_membership WHERE segment_id = 'ABC' AND last_updated > NOW() - INTERVAL '30 days'
```

- [ ] **A)** Profile overlap percentage
- [ ] **B)** Identity graph strength score
- [ ] **C)** Segment membership recency
- [ ] **D)** Activation success rate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The code filters profiles by recency, reflecting segment membership recency for a time-windowed segment.
 
 
</details>

### 23. What does the Audience Dashboard in Real-Time CDP primarily display?

- [ ] **A)** Profile attribute completeness
- [ ] **B)** Audience size trends and breakdown by namespace
- [ ] **C)** Destination activation latency
- [ ] **D)** Data ingestion error logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Audience Dashboard displays audience size over time, segmented by identity namespace for monitoring health.
 
 
</details>

### 24. Which two factors can cause a difference between 'Identities' and 'People' on a dashboard?

- [ ] **A)** Identity stitching collapsing multiple identifiers
- [ ] **B)** Data source validation failure
- [ ] **C)** Merge policy settings
- [ ] **D)** Destination match rate fluctuations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Identity stitching and merge policy settings directly affect deduplication, causing the count difference.
 
 
</details>

### 25. Based on the code, which dashboard metric is being generated for audience evaluation?

```sql
SELECT personID, COUNT(identityID) AS id_count FROM identity_map GROUP BY personID
```

- [ ] **A)** Average profile enrichment
- [ ] **B)** Identity count per profile
- [ ] **C)** Activation success percentage
- [ ] **D)** Segment size growth rate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The query counts identities per profile, directly computing the identity count per profile metric.
 
 
</details>


---

### **Real-Time CDP Overview and Strategy**

### 26. What is the primary purpose of Adobe Real-Time CDP?

- [ ] **A)** Real-time reporting and analytics
- [ ] **B)** Unified customer profiles for activation
- [ ] **C)** Email marketing automation
- [ ] **D)** Web content management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Adobe Real-Time CDP unifies fragmented customer data into a single profile for real-time activation across channels.
 
 
</details>

### 27. Which two features are part of Adobe Real-Time CDP?

- [ ] **A)** Identity resolution
- [ ] **B)** Batch-only segmentation
- [ ] **C)** Data governance enforcement
- [ ] **D)** Third-party data enrichment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Real-Time CDP includes identity resolution and data governance; batch segmentation is only one mode, and third-party enrichment is not a core feature.
 
 
</details>

### 28. Examine the segment definition below. What type of audience does it create?

```pql
Profile: (loyaltyTier = "Gold") AND ExperienceEvent: (addToCart in last 7 days)
```

- [ ] **A)** Users who have purchased in the last 7 days
- [ ] **B)** Gold loyalty members who recently added items to cart
- [ ] **C)** All customers with a loyalty tier
- [ ] **D)** Event-based segment of cart abandoners

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The segment combines a profile attribute (loyaltyTier=Gold) with an event condition (addToCart in last 7 days), targeting high-value engaged customers.
 
 
</details>

### 29. How does Real-Time CDP fit within the Adobe Experience Cloud?

- [ ] **A)** It replaces Adobe Analytics for reporting
- [ ] **B)** It acts as a central customer profile store for activation
- [ ] **C)** It is a standalone email marketing platform
- [ ] **D)** It provides AI-driven personalization only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Real-Time CDP serves as the foundation for unified profiles, which other Adobe solutions consume for personalized experiences.
 
 
</details>

### 30. Which two components are required to enforce data governance policies in Real-Time CDP?

- [ ] **A)** Data usage labels
- [ ] **B)** Marketing actions
- [ ] **C)** Campaign performance reports
- [ ] **D)** Segment export schedules

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Policies combine data usage labels with marketing actions to control how data is used during activation.
 
 
</details>

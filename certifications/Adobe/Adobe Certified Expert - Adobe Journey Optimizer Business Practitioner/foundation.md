<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Adobe/Adobe%20Certified%20Expert.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Adobe Certified Expert - Adobe Journey Optimizer Business Practitioner</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Campaign Orchestration](#campaign-orchestration) (9 questions)
- [Data Management and Integration](#data-management-and-integration) (6 questions)
- [Governance and Administration](#governance-and-administration) (3 questions)
- [Personalization and Content Management](#personalization-and-content-management) (8 questions)
- [Reporting and Analytics](#reporting-and-analytics) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:04.763Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Campaign Orchestration | 9 |
| Data Management and Integration | 6 |
| Governance and Administration | 3 |
| Personalization and Content Management | 8 |
| Reporting and Analytics | 4 |

---

### **Campaign Orchestration**

### 1. What type of campaign in Adobe Journey Optimizer is initiated by an HTTP POST request from an external system?

- [ ] **A)** Scheduled campaign
- [ ] **B)** Trigger-based campaign
- [ ] **C)** Batch campaign
- [ ] **D)** Recurring campaign

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Trigger-based campaigns start when an external system sends an HTTP POST request to the AJO API endpoint.
 
 
</details>

### 2. Which of the following are valid entry types for a journey in AJO? (Choose two.)

- [ ] **A)** Segment Qualification
- [ ] **B)** Read Segment
- [ ] **C)** Batch Campaign
- [ ] **D)** Email Action

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Segment Qualification and Read Segment are valid journey entry types. Batch Campaign is a campaign type, not a journey entry.
 
 
</details>

### 3. Review the following JSON payload for a trigger-based campaign API call. What is the purpose of the 'campaign ID' field?

```json
POST /api/v1/campaigns/trigger
{
  "campaignId": "my_cart_abandonment_campaign",
  "profile": {
    "identity": {
      "namespace": "email",
      "value": "customer@example.com"
    }
  }
}
```

- [ ] **A)** It identifies the customer profile to receive the message
- [ ] **B)** It specifies which trigger-based campaign to activate
- [ ] **C)** It defines the channel surface to use
- [ ] **D)** It sets the start date of the campaign

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The campaign ID links the API call to a specific trigger-based campaign configured in AJO.
 
 
</details>

### 4. What is the default journey timeout in Adobe Journey Optimizer if not customized?

- [ ] **A)** 30 days
- [ ] **B)** 90 days
- [ ] **C)** 91 days
- [ ] **D)** 7 days

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The default journey timeout in AJO is 91 days. After this, all in-flight profiles are ejected.
 
 
</details>

### 5. Which of the following activities in AJO can have an error path configured? (Choose two.)

- [ ] **A)** Email action
- [ ] **B)** Condition node
- [ ] **C)** Push action
- [ ] **D)** Wait activity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Email and Push actions are external activities that can fail; condition and wait are logic nodes and do not have error paths.
 
 
</details>

### 6. The following PQL expression is used in a condition node. What does it check? `${profile.loyaltyTier} == \"Gold\"`

```pql
${profile.loyaltyTier} == "Gold"
```

- [ ] **A)** Whether the profile's loyalty tier is Gold
- [ ] **B)** Whether the profile has a Gold credit card
- [ ] **C)** Whether the profile spent over $500
- [ ] **D)** Whether the profile is in the Gold segment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The condition checks if the profile attribute 'loyaltyTier' equals the string 'Gold'.
 
 
</details>

### 7. In Adobe Journey Optimizer, what happens when you edit a published journey?

- [ ] **A)** The changes are applied immediately to all profiles
- [ ] **B)** A new version is created and the published version remains unchanged
- [ ] **C)** The journey is stopped and you must restart it
- [ ] **D)** You can edit directly without any versioning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Editing a published journey automatically creates a new draft version; the live version continues unchanged.
 
 
</details>

### 8. Which of the following are characteristics of a batch campaign in AJO? (Choose two.)

- [ ] **A)** Processes all segment members at once
- [ ] **B)** Supports recurrence (daily, weekly)
- [ ] **C)** Ideal for large-scale, one-time sends
- [ ] **D)** Triggered by an API call

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Batch campaigns execute for an entire segment in one go and are best for bulk sends. Recurrence is for scheduled campaigns, not batch.
 
 
</details>

### 9. The following is a segment qualification rule for a journey entry. What does this rule trigger? `Segment membership changed: enters segment 'VIP_Customers'`

```text
Segment membership changed: enters segment 'VIP_Customers'
```

- [ ] **A)** When the profile is added to the VIP_Customers segment
- [ ] **B)** When the profile is removed from the VIP_Customers segment
- [ ] **C)** When the profile makes a purchase
- [ ] **D)** When the segment is evaluated at midnight

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Segment qualification triggers on membership change; here it triggers on entrance into the specified segment.
 
 
</details>


---

### **Data Management and Integration**

### 10. What is the primary purpose of a data source in Adobe Journey Optimizer?

- [ ] **A)** To provide data to journeys or segments from AEP datasets or external systems
- [ ] **B)** To create new customer profiles from scratch
- [ ] **C)** To store the journey design and execution logs
- [ ] **D)** To manage user permissions for journey access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A data source is configured to supply data to journeys or segments, either from AEP datasets or external systems, enabling orchestration and personalization.
 
 
</details>

### 11. Which of the following are characteristics of real-time (streaming) ingestion?

- [ ] **A)** Data is available for journey triggers within seconds
- [ ] **B)** It uses file-based imports like CSV or Parquet
- [ ] **C)** It typically ingests client-side events via SDKs
- [ ] **D)** It is best suited for historical CRM data imports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Streaming ingestion uses APIs/SDKs to send real-time events, making data available within seconds for journey triggers. Batch ingestion uses files for historical data.
 
 
</details>

### 12. When configuring a data source for ingestion, what is the first required step?

```plaintext
// No code required for this conceptual question
```

- [ ] **A)** Create a dataset
- [ ] **B)** Create an XDM schema
- [ ] **C)** Create a segment definition
- [ ] **D)** Create a streaming endpoint

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Every data source must align with an existing XDM schema, so creating the schema is the foundational step before setting up datasets or connectors.
 
 
</details>

### 13. What is the role of XDM schemas in data management within Adobe Experience Platform?

- [ ] **A)** They define the structure and semantics of data for ingestion and use
- [ ] **B)** They store raw data files in the data lake
- [ ] **C)** They manage user roles and permissions
- [ ] **D)** They create audience segments automatically

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> XDM schemas standardize data structure, enabling consistent ingestion, profile stitching, and journey orchestration across Adobe Experience Cloud.
 
 
</details>

### 14. Which components are essential for identity mapping in an XDM schema?

- [ ] **A)** A primary identity descriptor
- [ ] **B)** An identity namespace (e.g., Email, ECID)
- [ ] **C)** A dataset that is profile-enabled
- [ ] **D)** A segment definition with identity conditions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Identity mapping requires a primary identity field, an identity namespace, and a profile-enabled dataset to stitch incoming records to unified profiles.
 
 
</details>

### 15. Which segment evaluation method is used for near real-time journey entry triggers in Adobe Journey Optimizer?

- [ ] **A)** Streaming evaluation
- [ ] **B)** Batch evaluation
- [ ] **C)** Edge evaluation
- [ ] **D)** Manual evaluation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Streaming evaluation (also called continuous evaluation) updates segment membership in near real-time, making it suitable for triggering journeys promptly.
 
 
</details>


---

### **Governance and Administration**

### 16. What is the term for a reusable configuration template in Adobe Journey Optimizer that defines technical and delivery parameters for a communication channel?

- [ ] **A)** Channel surface
- [ ] **B)** Message preset
- [ ] **C)** Campaign
- [ ] **D)** Segment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A message preset (channel surface) is a reusable configuration template that defines technical and delivery parameters, abstracting infrastructure choices for practitioners.
 
 
</details>

### 17. Which two prerequisites are necessary for a user to access a specific sandbox in Adobe Journey Optimizer?

- [ ] **A)** Assignment to a product profile
- [ ] **B)** Membership in a user group
- [ ] **C)** Product profile associated with the sandbox
- [ ] **D)** Valid Adobe ID with enterprise federation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The user must be assigned to a product profile that is associated with the desired sandbox. User groups alone do not grant permissions.
 
 
</details>

### 18. Based on the frequency capping rule shown, what does the 'maxCount' property represent?

```json
{"maxCount": 2, "timeWindow": "weekly", "channel": "email"}
```

- [ ] **A)** The maximum number of messages a profile can receive within the time window
- [ ] **B)** The total number of messages allowed across all channels per day
- [ ] **C)** The number of days before the frequency counter resets
- [ ] **D)** The number of times a journey can be re-entered

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'maxCount' property defines the maximum number of sends allowed for a profile within the specified time window, here 2 per week.
 
 
</details>


---

### **Personalization and Content Management**

### 19. Which Handlebars brace style is required to embed an offer image URL in an email template?

- [ ] **A)** Double braces
- [ ] **B)** Triple braces
- [ ] **C)** Single braces
- [ ] **D)** No braces needed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Triple braces render raw HTML, necessary for image URLs to avoid broken tags.
 
 
</details>

### 20. Which two statements about dynamic and conditional content in AJO are correct?

- [ ] **A)** Dynamic content is used for simple value replacement.
- [ ] **B)** Conditional content blocks can contain multiple elements.
- [ ] **C)** Conditional content can be used without a fallback.
- [ ] **D)** Dynamic content requires the if helper.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Dynamic content replaces single values; conditional blocks handle entire sections and need a fallback.
 
 
</details>

### 21. Identify the correct Handlebars expression to display a customer's first name.

```handlebars
{{profile.person.name.firstName}}
```

- [ ] **A)** {{profile.person.name.firstName}}	
- [ ] **B)** {{firstName}}
- [ ] **C)** {{person.name.firstName}}
- [ ] **D)** {{profile.firstName}}

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The full path including profile prefix is required to access profile attributes.
 
 
</details>

### 22. Which segment type is appropriate for a time-sensitive cart abandonment journey?

- [ ] **A)** Batch segment
- [ ] **B)** Streaming segment
- [ ] **C)** Computed attribute
- [ ] **D)** Merge policy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Streaming segments evaluate in real-time, suitable for immediate triggers like cart abandonment.
 
 
</details>

### 23. Which two statements about content fragments in AJO are true?

- [ ] **A)** Fragments can be reused across multiple channels.
- [ ] **B)** Fragments imported from AEM are editable in AJO.
- [ ] **C)** Fragments can include personalization fields.
- [ ] **D)** Fragments can replace full email templates.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Fragments are reusable blocks that support personalization; AEM fragments are read-only in AJO.
 
 
</details>

### 24. What is the correct way to check if an offer is eligible for a given profile?

```handlebars
{{#offer.eligible}}
  Eligible content here
{{/offer.eligible}}
```

- [ ] **A)** 	{{#offer.eligible}}...{{/offer.eligible}}
- [ ] **B)** {{#if offer.eligible}}...{{/if}}
- [ ] **C)** {{#each offer}}{{#if eligible}}...{{/if}}{{/each}}
- [ ] **D)** {{#with offer}}{{#if eligible}}...{{/if}}{{/with}}

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The correct block helper is #offer.eligible, not #if on a property.
 
 
</details>

### 25. What happens in a conditional content block if the condition evaluates to false?

- [ ] **A)** Nothing is displayed
- [ ] **B)** The fallback variant is shown
- [ ] **C)** The journey is skipped
- [ ] **D)** A warning is logged

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Conditional content blocks require a fallback (else branch) to render when no condition passes.
 
 
</details>

### 26. Which two statements about Handlebars escaping in AJO are correct?

- [ ] **A)** Double braces escape HTML characters.
- [ ] **B)** Triple braces are always safe for any content.
- [ ] **C)** Triple braces render raw HTML.
- [ ] **D)** Double braces should be used for offer image URLs.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Double braces escape; triple braces output raw HTML and should only be used for trusted sources.
 
 
</details>


---

### **Reporting and Analytics**

### 27. In Adobe Journey Optimizer, what does a 'drop' in a journey report primarily indicate?

- [ ] **A)** A user exited the journey due to conditions, timeout, or non-delivery.
- [ ] **B)** A user unsubscribed from communications.
- [ ] **C)** A tracking pixel failed to load.
- [ ] **D)** A conversion event was recorded.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In journey reports, a drop means the user left the journey before completing it, commonly due to conditions, timeout, or delivery failures. This is different from a campaign drop which is purely non-delivery.
 
 
</details>

### 28. Which of the following are pre-built dashboards available in Adobe Experience Platform for analyzing customer behavior?

- [ ] **A)** Profile Dashboard
- [ ] **B)** Segmentation Dashboard
- [ ] **C)** Journey Performance Dashboard
- [ ] **D)** Destinations Dashboard

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> The pre‑built dashboards are Profile, Segmentation, and Destinations. There is no pre‑built Journey Performance dashboard; journey analysis requires custom dashboards or the AJO Monitoring view.
 
 
</details>

### 29. Based on the reported A/B test results above, what is the statistical significance of Variant B being the winner?

```json
{
  "experimentId": "exp_1234",
  "variants": [
    {
      "name": "Variant A",
      "probabilityToBeBest": 0.02,
      "metric": "click rate",
      "rate": 12.1
    },
    {
      "name": "Variant B",
      "probabilityToBeBest": 0.98,
      "metric": "click rate",
      "rate": 14.4
    }
  ],
  "confidenceThreshold": 0.95
}
```

- [ ] **A)** 98% probability, which is above the default 95% threshold.
- [ ] **B)** 2.3% uplift, which is considered statistically significant regardless of probability.
- [ ] **C)** The test is inconclusive because the confidence level is below 99%.
- [ ] **D)** The holdout group size was too large, invalidating the result.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AJO uses a Bayesian approach with a default 95% confidence threshold. A 98% probability to be best exceeds that threshold, so Variant B is the statistically significant winner.
 
 
</details>

### 30. In Adobe Journey Optimizer reporting, what is the difference between total opens and unique opens?

- [ ] **A)** Unique opens count each profile only once, while total opens count every open event.
- [ ] **B)** Total opens includes only mobile opens, unique opens includes only desktop opens.
- [ ] **C)** Unique opens are always higher than total opens because of multi-device counting.
- [ ] **D)** Total opens excludes opens that happened within the first hour after send.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AJO reports distinguish unique (one per profile) from total (all events). A discrepancy, such as 1000 total vs 800 unique, simply indicates some recipients opened the message more than once.
 
 
</details>

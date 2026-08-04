<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Adobe/Adobe%20Certified%20Master.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Adobe Certified Master - Adobe Journey Optimizer (AJO) Architect</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Data Modeling and Management for Journeys](#data-modeling-and-management-for-journeys) (6 questions)
- [Journey Design and Orchestration](#journey-design-and-orchestration) (9 questions)
- [Journey Optimizer Architecture and Administration](#journey-optimizer-architecture-and-administration) (7 questions)
- [Monitoring, Troubleshooting, and Optimization](#monitoring-troubleshooting-and-optimization) (3 questions)
- [Personalization and Decisioning](#personalization-and-decisioning) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:15.243Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Data Modeling and Management for Journeys | 6 |
| Journey Design and Orchestration | 9 |
| Journey Optimizer Architecture and Administration | 7 |
| Monitoring, Troubleshooting, and Optimization | 3 |
| Personalization and Decisioning | 5 |

---

### **Data Modeling and Management for Journeys**

### 1. Which XDM class should be used to model time-series behavioral data such as page views or purchases?

- [ ] **A)** XDM Individual Profile
- [ ] **B)** XDM ExperienceEvent
- [ ] **C)** XDM Business Object
- [ ] **D)** XDM Record

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> XDM ExperienceEvent is specifically designed for time-series event data, such as page views, purchases, or other behavioral actions.
 
 
</details>

### 2. Which of the following are standard identity namespaces provided by Adobe?

- [ ] **A)** Email
- [ ] **B)** ECID
- [ ] **C)** Loyalty ID
- [ ] **D)** Phone

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Email, ECID, and Phone are standard namespaces predefined by Adobe. Loyalty ID is a custom namespace defined by the customer.
 
 
</details>

### 3. Given the following segment definition, what evaluation method should be used for real-time journey triggering?

```sql
SELECT * FROM profile WHERE eventType = 'commerce.purchases' AND timestamp >= (now() - INTERVAL 30 MINUTE)
```

- [ ] **A)** Batch
- [ ] **B)** Streaming
- [ ] **C)** Edge
- [ ] **D)** None

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Streaming evaluation supports real-time processing of event-based conditions with time windows, enabling journey triggering within seconds.
 
 
</details>

### 4. Which of the following is a characteristic of the Adobe Experience Platform data source in AJO?

- [ ] **A)** Requires manual configuration of endpoint and authentication
- [ ] **B)** Provides access to Real-time Customer Profile data without additional configuration
- [ ] **C)** Can be used to call external APIs
- [ ] **D)** Supports caching with configurable TTL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Adobe Experience Platform data source is pre-configured and automatically provides access to profile data already resident in AEP, requiring no extra setup.
 
 
</details>

### 5. Which of the following are required components of an event definition in AJO?

- [ ] **A)** An XDM schema
- [ ] **B)** A dataset
- [ ] **C)** A data source
- [ ] **D)** A condition rule (Event ID)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Event definitions require an XDM schema, a dataset based on that schema, and a condition rule that identifies the incoming event. A data source is separate and not part of the event definition.
 
 
</details>

### 6. Given the following event payload, what value should be used in the event definition condition to match this event?

```json
{ "eventType": "commerce.abandonCart", "productId": "123", "price": 49.99 }
```

- [ ] **A)** commerce.abandonCart
- [ ] **B)** productId
- [ ] **C)** price
- [ ] **D)** eventType

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The event definition condition typically uses the 'eventType' field's value (e.g., 'commerce.abandonCart') to uniquely trigger the journey.
 
 
</details>


---

### **Journey Design and Orchestration**

### 7. What is the primary purpose of the Adobe Journey Optimizer (AJO) canvas?

- [ ] **A)** To design multistep and multichannel customer journeys
- [ ] **B)** To create email templates only
- [ ] **C)** To manage user roles and permissions
- [ ] **D)** To store customer profile data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The AJO canvas is a drag-and-drop visual environment for orchestrating sequences of events, actions, decisions, and waits across channels.
 
 
</details>

### 8. Which of the following are valid entry sources for an AJO journey? (Select all that apply.)

- [ ] **A)** Segment qualification
- [ ] **B)** Single event (e.g., mobile app launch)
- [ ] **C)** Scheduled batch
- [ ] **D)** Email open event

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Journeys can start with a segment (batch or streaming), a single event, or a scheduled batch. Email open is not an entry source; it can be a triggering event inside a journey.
 
 
</details>

### 9. Review the following condition syntax. Which PQL expression correctly checks if a profile's loyalty tier is 'Gold'?

```pql
profile.loyalty.tier
```

- [ ] **A)** profile.loyalty.tier == 'Gold'
- [ ] **B)** profile.loyalty.tier = 'Gold'
- [ ] **C)** profile.loyalty.tier equals 'Gold'
- [ ] **D)** profile.loyalty.tier IS 'Gold'

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In PQL, the equality operator is '=='. Single '=' is assignment, 'equals' is not PQL syntax, 'IS' is used for null checks.
 
 
</details>

### 10. What is the default retry behavior for a custom action when it receives a 5xx error?

- [ ] **A)** One retry
- [ ] **B)** No retries
- [ ] **C)** Three retries
- [ ] **D)** Five retries

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Custom actions by default retry once on 5xx errors and timeouts. 4xx errors are not retried unless configured.
 
 
</details>

### 11. Which of the following are true about Decision Split nodes in AJO? (Select all that apply.)

- [ ] **A)** Supports up to 30 branches
- [ ] **B)** Branches are evaluated in order; first true branch is taken
- [ ] **C)** All true branches are executed simultaneously
- [ ] **D)** A default path must be defined

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Decision splits evaluate branches in sequence; only the first true condition wins. Up to 30 branches allowed. A default path is required to avoid dropping profiles.
 
 
</details>

### 12. Study the following JSON payload for an API trigger. What must be included to identify the profile?

```json
{
  "profile": {
    "identifiers": [
      {
        "type": "Email",
        "value": "customer@example.com"
      }
    ]
  },
  "journeyVersionId": "<journey-id>",
  "triggerParameters": {}
}
```

- [ ] **A)** identifiers array with type and value
- [ ] **B)** journeyVersionId
- [ ] **C)** triggerParameters
- [ ] **D)** Experience Cloud ID

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'profile.identifiers' array must contain a namespace (type) and value to resolve the profile. JourneyVersionId identifies the journey, not the profile.
 
 
</details>

### 13. What happens to profiles waiting in a date wait if the journey is republished with a new version?

- [ ] **A)** All pending waits are lost and profiles are dropped
- [ ] **B)** Profiles continue in the new version from the same wait point
- [ ] **C)** Profiles are moved to the default path of the new version
- [ ] **D)** They are paused indefinitely until the new version is deactivated

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When a new version is published, the previous version is stopped. All pending waits are lost; profiles do not carry over.
 
 
</details>

### 14. Which of the following are valid channel actions in AJO? (Select all that apply.)

- [ ] **A)** Email
- [ ] **B)** SMS
- [ ] **C)** Push notification
- [ ] **D)** Custom REST API call

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Email, SMS, Push, In-app, and Direct mail are built-in channel actions. Custom REST API calls are custom actions, not channel actions.
 
 
</details>

### 15. Given the following code snippet from a journey condition, what does the expression evaluate?

```pql
profile.consents.marketing.email.subscription == true
```

- [ ] **A)** Whether the profile's consent for marketing email is true
- [ ] **B)** Whether the profile has an email address
- [ ] **C)** Whether the profile is in the email suppression list
- [ ] **D)** Whether the profile opted out of all communications

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This condition checks the profile's 'consents.marketing.email.subscription' attribute. If true, the profile has consented to marketing emails.
 
 
</details>


---

### **Journey Optimizer Architecture and Administration**

### 16. What is Adobe Journey Optimizer?

- [ ] **A)** A standalone segmentation engine
- [ ] **B)** The native orchestration layer of Adobe Experience Platform
- [ ] **C)** A data ingestion tool for batch uploads
- [ ] **D)** A reporting dashboard for Adobe Campaign

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AJO is the orchestration layer built on AEP, not a standalone tool.
 
 
</details>

### 17. Which of the following are key components of AJO?

- [ ] **A)** Orchestration Service
- [ ] **B)** Decisioning Service
- [ ] **C)** Data Collection layer
- [ ] **D)** Segmentation Service

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Segmentation is handled by AEP, not AJO itself.
 
 
</details>

### 18. Examine the code block. Which XDM class must be used for representing a customer's web visit event in AJO?

```json
{
  "@type": "https://ns.adobe.com/xdm/context/experienceevent",
  "xdm:eventType": "web.webpagedetails.pageViews",
  "xdm:timestamp": "2025-01-01T00:00:00Z",
  "xdm:web": { "webPageDetails": { "URL": "https://example.com" } }
}
```

- [ ] **A)** XDM ExperienceEvent
- [ ] **B)** XDM Individual Profile
- [ ] **C)** XDM Business Account
- [ ] **D)** XDM Segment Definition

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Web visit events are time-series data and use the ExperienceEvent class.
 
 
</details>

### 19. What is the primary role of the Identity Service within AEP?

- [ ] **A)** Stores journey execution logs
- [ ] **B)** Stitches identifiers into a unified Identity Graph
- [ ] **C)** Sends email notifications
- [ ] **D)** Creates XDM schemas

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Identity Service links identifiers like email and ECID to unify profiles.
 
 
</details>

### 20. Which statements are true about batch and streaming ingestion in AEP?

- [ ] **A)** Streaming ingestion provides sub-second latency
- [ ] **B)** Batch ingestion is the only way to import historical data
- [ ] **C)** Both batch and streaming can update the Real-Time Customer Profile
- [ ] **D)** Streaming ingestion requires an XDM event schema

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Historical data can also be streamed; batch also updates profile; streaming needs XDM.
 
 
</details>

### 21. Examine the email surface configuration code. Which DNS record is missing to ensure deliverability?

```json
{
  "name": "US Marketing Email",
  "channel": "email",
  "fromAddress": "marketing@example.com",
  "replyToAddress": "noreply@example.com",
  "ipPool": "pool-1",
  "dkim": "valid-dkim-key"
}
```

- [ ] **A)** SPF
- [ ] **B)** CNAME for tracking
- [ ] **C)** TXT for domain verification
- [ ] **D)** MX record

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SPF is critical for email authentication and delivery; it is not shown here.
 
 
</details>

### 22. What is the primary purpose of sandboxes in AJO?

- [ ] **A)** To separate development, testing, and production environments
- [ ] **B)** To increase data ingestion speed
- [ ] **C)** To manage user passwords
- [ ] **D)** To store backup of journey definitions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Sandboxes isolate environments to prevent cross-contamination and enable safe testing.
 
 
</details>


---

### **Monitoring, Troubleshooting, and Optimization**

### 23. Which AJO report provides real-time metrics for journeys currently in execution?

- [ ] **A)** Live View
- [ ] **B)** Global Report
- [ ] **C)** Customer Journey Analytics
- [ ] **D)** Adobe Analytics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Live View provides real-time metrics refreshed every 30 seconds for the current journey version. Global Report is historical and aggregated.
 
 
</details>

### 24. Which of the following metrics are alertable in AJO journey alerts? (Select three)

- [ ] **A)** Error
- [ ] **B)** Dropped
- [ ] **C)** Converted
- [ ] **D)** Average time in step

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Alertable metrics include entered, exited, error, dropped, and converted. Average time in step is not available for alerts.
 
 
</details>

### 25. Given the following error log snippet from a journey step, identify the most likely cause of the failure.

```json
{
  "timestamp": "2024-07-15T10:30:00Z",
  "journeyVersionId": "abc123",
  "stepId": "sendSMS",
  "status": "Error",
  "errorCode": "step_actionError",
  "errorMessage": "HTTP 401: Unauthorized - Invalid API Key",
  "profileId": "pf123456"
}
```

- [ ] **A)** External API authentication failure
- [ ] **B)** Segment evaluation timeout
- [ ] **C)** Schema validation error in data ingestion
- [ ] **D)** Profile identity mismatch

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The error code 'step_actionError' with HTTP 401 indicates an authentication issue with the external action's API endpoint.
 
 
</details>


---

### **Personalization and Decisioning**

### 26. What is the primary role of a fallback offer in Adobe Journey Optimizer Offer Decisioning?

- [ ] **A)** To serve as the default offer when no personalized offers meet eligibility criteria
- [ ] **B)** To replace the placement configuration when no channel is specified
- [ ] **C)** To provide a secondary ranking method for offers with equal priority
- [ ] **D)** To store the most popular offer based on historical click-through rates

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A fallback offer is the default offer served when no personalized offer in the collection is eligible due to rules, capping, or date constraints. It ensures a consistent customer experience and prevents empty returns.
 
 
</details>

### 27. Which of the following are valid components of a decision policy in Adobe Journey Optimizer? (Select two.)

- [ ] **A)** Associated placement
- [ ] **B)** Frequency capping rules
- [ ] **C)** Fallback offer
- [ ] **D)** AI model training dataset

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> A decision policy comprises an associated placement and a fallback offer. Frequency capping is set at the offer level, not the policy level. AI models are trained separately and referenced by the ranking strategy, not part of the policy definition.
 
 
</details>

### 28. You are writing a Handlebars expression to show a different greeting based on the language_code profile attribute. If the code is 'FR', display 'Bonjour'; otherwise display 'Hello'. Which code block correctly implements this logic?

```handlebars
{{#if (eq profile.language_code 'FR')}}Bonjour{{else}}Hello{{/if}}
```

- [ ] **A)** {{#if (eq profile.language_code 'FR')}}Bonjour{{else}}Hello{{/if}}
- [ ] **B)** {{#if profile.language_code == 'FR'}}Bonjour{{else}}Hello{{/if}}
- [ ] **C)** {{#if (eql profile.language_code 'FR')}}Bonjour{{else}}Hello{{/if}}
- [ ] **D)** {{#if (eq profile.language_code 'fr')}}Bonjour{{else}}Hello{{/if}}

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AJO's expression editor uses the 'eq' helper inside the condition, not a direct comparison operator. The correct syntax is {{#if (eq profile.language_code 'FR')}}...{{/if}}.
 
 
</details>

### 29. What is the purpose of a placement in Adobe Journey Optimizer Offer Decisioning?

- [ ] **A)** It defines the context where an offer will appear, such as email hero image or mobile banner
- [ ] **B)** It stores the content and metadata of a personalized offer
- [ ] **C)** It determines the order of offers returned by the decision engine
- [ ] **D)** It specifies the eligibility rules for a profile to receive an offer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A placement defines the context (e.g., channel, content type) where an offer will be displayed. It is a template that links the offer to a specific location in a message.
 
 
</details>

### 30. Which of the following are types of content that can be managed using AJO Content Blocks? (Select two.)

- [ ] **A)** HTML email footers and headers
- [ ] **B)** Personalization tokens for subject lines
- [ ] **C)** JSON snippets for push notification payloads
- [ ] **D)** Decision ranking formulas

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Content blocks are reusable HTML or JSON fragments stored in the AJO Content Library, used for elements like footers, headers, or push notification bodies. Personalization tokens are inline expressions, not blocks. Ranking formulas are defined in decision policies.
 
 
</details>

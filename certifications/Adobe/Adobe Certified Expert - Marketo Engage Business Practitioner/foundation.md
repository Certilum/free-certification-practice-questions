<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Adobe/Adobe%20Certified%20Expert.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Adobe Certified Expert - Marketo Engage Business Practitioner</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Analyze and Report on Performance](#analyze-and-report-on-performance) (1 questions)
- [Design and Build New Assets and Forms](#design-and-build-new-assets-and-forms) (5 questions)
- [Manage Master Data and List Imports](#manage-master-data-and-list-imports) (4 questions)
- [Manage Person Accounts, Lead Lifecycle, and Scoring](#manage-person-accounts-lead-lifecycle-and-scoring) (6 questions)
- [Manage, Execute, and Measure Email Campaigns](#manage-execute-and-measure-email-campaigns) (5 questions)
- [Manage, Execute, and Measure Other Digital Channels](#manage-execute-and-measure-other-digital-channels) (3 questions)
- [Manage, Execute, and Measure Webinar, Event, and Engagement Programs](#manage-execute-and-measure-webinar-event-and-engagement-programs) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:07.361Z |
| Domains | 7 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Analyze and Report on Performance | 1 |
| Design and Build New Assets and Forms | 5 |
| Manage Master Data and List Imports | 4 |
| Manage Person Accounts, Lead Lifecycle, and Scoring | 6 |
| Manage, Execute, and Measure Email Campaigns | 5 |
| Manage, Execute, and Measure Other Digital Channels | 3 |
| Manage, Execute, and Measure Webinar, Event, and Engagement Programs | 6 |

---

### **Analyze and Report on Performance**

### 1. Which attribution model assigns full revenue credit to the first program that captured a lead?

- [ ] **A)** First-Touch
- [ ] **B)** Multi-Touch Equal
- [ ] **C)** U-Shaped
- [ ] **D)** Custom Weighted

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> First-Touch attribution credits 100% of revenue to the program that first acquired the lead, ideal for top-of-funnel analysis.
 
 
</details>


---

### **Design and Build New Assets and Forms**

### 2. What is the standard breakpoint width used in media queries for responsive email design in Marketo?

- [ ] **A)** 480px
- [ ] **B)** 600px
- [ ] **C)** 768px
- [ ] **D)** 320px

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The standard breakpoint is 600px, following best practices for mobile-first email design.
 
 
</details>

### 3. Which two conditions are necessary for progressive profiling to work on a Marketo landing page form?

- [ ] **A)** The lead must be known (identified via email or cookie).
- [ ] **B)** The form must contain at least five fields.
- [ ] **C)** Progressive profiling must be enabled in the form settings.
- [ ] **D)** The landing page must use a guided template.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Progressive profiling only works for known leads and must be explicitly enabled in the form editor's Progressive Profiling tab.
 
 
</details>

### 4. What is the purpose of the colon and the default text in this Marketo token: `{{lead.First Name:Valued Customer}}`?

```marketo
{{lead.First Name:Valued Customer}}
```

- [ ] **A)** It sets a default value that appears if the lead’s First Name is empty.
- [ ] **B)** It changes the font color of the token.
- [ ] **C)** It triggers a conditional rule to hide the field.
- [ ] **D)** It converts the token into a hyperlink.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The syntax `token:default_value` provides a fallback text when the lead field is empty, improving personalization reliability.
 
 
</details>

### 5. What happens when you approve a form in Marketo?

- [ ] **A)** All landing pages using the form are automatically updated.
- [ ] **B)** The form becomes available for use in landing pages, but existing pages remain unchanged until re-approved.
- [ ] **C)** The form is permanently deleted from the system.
- [ ] **D)** The form is sent to all leads in the database.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Form approval does not cascade to parent landing pages; each page must be re-approved individually to reflect form changes.
 
 
</details>

### 6. Which two token types can be used in email subject lines in Marketo?

- [ ] **A)** Lead tokens
- [ ] **B)** My tokens
- [ ] **C)** Trigger tokens
- [ ] **D)** System tokens

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Lead and My tokens are commonly used in subject lines for personalization. Trigger tokens only resolve in triggered campaigns, and system.unsubscribe is not a valid token.
 
 
</details>


---

### **Manage Master Data and List Imports**

### 7. Which list type requires manual addition or import to change its membership?

- [ ] **A)** Static list
- [ ] **B)** Smart list
- [ ] **C)** Program list
- [ ] **D)** Dynamic list

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A static list holds a manually curated set of leads that does not change automatically. Smart lists update dynamically based on filters.
 
 
</details>

### 8. Which import modes are available when importing leads into a static list?

- [ ] **A)** Skip new and update existing
- [ ] **B)** Skip existing and add new
- [ ] **C)** Add new and update existing
- [ ] **D)** Create new and skip existing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The three valid import modes are: Skip new and update existing, Skip existing and add new, and Add new and update existing. 'Create new and skip existing' is not a valid mode.
 
 
</details>

### 9. Refer to the CSV sample below. When importing this file with default settings, which field does Marketo use to check for duplicate leads?

```csv
email,firstName,lastName
john@test.com,John,Doe
jane@test.com,Jane,Doe
```

- [ ] **A)** email
- [ ] **B)** firstName
- [ ] **C)** lastName
- [ ] **D)** All three combined

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> By default, Marketo uses the email field as the primary identifier for deduplication during list imports.
 
 
</details>

### 10. How does a smart list determine its membership?

- [ ] **A)** Members join by manual import only.
- [ ] **B)** Membership is recalculated based on defined filters.
- [ ] **C)** Members are added automatically from all static lists.
- [ ] **D)** Membership is static until a user runs a refresh.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Smart lists are dynamic; their membership is determined by filters and triggers and is recalculated when evaluated.
 
 
</details>


---

### **Manage Person Accounts, Lead Lifecycle, and Scoring**

### 11. In a Marketo Engage lead lifecycle model, what does a 'status' represent?

- [ ] **A)** A high-level phase that groups multiple statuses.
- [ ] **B)** A specific condition of a lead within a stage.
- [ ] **C)** A rule that defines allowed movement between stages.
- [ ] **D)** A numeric value assigned to a person based on behavior.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A status is a sub-state within a stage that provides granularity, e.g., 'New' or 'Attempted Contact'.
 
 
</details>

### 12. Which of the following are types of scoring rules in Marketo Engage? (Select two.)

- [ ] **A)** Behavioral scoring
- [ ] **B)** Demographic scoring
- [ ] **C)** Temporal scoring
- [ ] **D)** Geographic scoring

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Behavioral scoring tracks actions (interest), demographic scoring evaluates fit (ICP attributes).
 
 
</details>

### 13. Examine the Marketo Smart Campaign flow step described below. What action does it perform?

```marketo
Flow: Change Person Status -> Status: MQL
```

- [ ] **A)** It merges two duplicate person records.
- [ ] **B)** It updates a person’s score by a given amount.
- [ ] **C)** It changes the program status of a person.
- [ ] **D)** It changes the person's lifecycle status.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> The 'Change Person Status' flow step moves a lead to a specific status in the lifecycle model.
 
 
</details>

### 14. What is the purpose of a 'success path' in the lead lifecycle model?

- [ ] **A)** It automatically moves leads forward through all stages.
- [ ] **B)** It prevents a lead from moving backward to a previous stage.
- [ ] **C)** It defines the default status for new leads.
- [ ] **D)** It triggers a notification to sales when a lead reaches that status.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A success path, when enabled on a transition, prevents backward movement to earlier stages once the lead reaches that status.
 
 
</details>

### 15. Which of the following are characteristics of a person record merge in Marketo Engage? (Select two.)

- [ ] **A)** Activities from both records are preserved and linked to the winner.
- [ ] **B)** The merge is reversible within 30 days via the recycle bin.
- [ ] **C)** Field values from the loser are always concatenated with the winner's values.
- [ ] **D)** If both records have the same program status, the winner's status is kept.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Activities are consolidated to the winner. For program memberships, the winner's status is retained if both are in the same program.
 
 
</details>

### 16. The following Marketo Smart List filter is used to identify leads in a specific lifecycle stage. Which field is being filtered?

```marketo
Filter: Stage equals MQL
```

- [ ] **A)** Status
- [ ] **B)** Stage
- [ ] **C)** Score
- [ ] **D)** Program Status

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The filter uses the 'Stage' field, which is derived from the current status and used for reporting.
 
 
</details>


---

### **Manage, Execute, and Measure Email Campaigns**

### 17. Which program type should you use for a one-time newsletter send?

- [ ] **A)** Email Program
- [ ] **B)** Engagement Program
- [ ] **C)** Default Program
- [ ] **D)** Event Program

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Email Program is designed for one-time, batch sends like newsletters. Engagement Program is for drip nurture streams.
 
 
</details>

### 18. Which two statements about audience segmentation are correct?

- [ ] **A)** Segmentation updates dynamically when lead data changes.
- [ ] **B)** Segmentation must be approved before it can be used in emails.
- [ ] **C)** Segmentation is identical to a Smart List.
- [ ] **D)** Segmentation defines the audience for a campaign.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Segmentation is dynamic and requires approval. It is used for content variation, not for audience definition; Smart Lists define audiences.
 
 
</details>

### 19. Given the template snippet, which syntax makes the background color editable?

```html
<div style="background-color: {{template.background}};">Content</div>
```

- [ ] **A)** {{template.background}}
- [ ] **B)** {{background}}
- [ ] **C)** <!-- background -->
- [ ] **D)** <% background %>

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Marketo Email Editor 2.0 uses {{template.variableName}} syntax for template variables that can be overridden per email.
 
 
</details>

### 20. What is the maximum acceptable spam score before sending an email?

- [ ] **A)** 2
- [ ] **B)** 3
- [ ] **C)** 4
- [ ] **D)** 5

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A spam score of 2 or lower is acceptable. Scores above 2 indicate issues that may cause filtering.
 
 
</details>

### 21. Which two metrics are more reliable than open rate due to recent privacy changes?

- [ ] **A)** Click-through rate (CTR)
- [ ] **B)** Click-to-open rate (CTOR)
- [ ] **C)** Bounce rate
- [ ] **D)** Unsubscribe rate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CTR and CTOR are based on clicks, which are not artificially inflated by privacy features like Apple MPP.
 
 
</details>


---

### **Manage, Execute, and Measure Other Digital Channels**

### 22. Which Marketo social app is designed to capture profile data from social networks to pre-fill forms?

- [ ] **A)** Social Button
- [ ] **B)** Referral Offer
- [ ] **C)** Social Sign-In
- [ ] **D)** Social Publishing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Social Sign-In allows leads to authenticate using their social media accounts, capturing profile data to pre-fill Marketo forms.
 
 
</details>

### 23. Which two steps are required to set up a social campaign using a Social Button in Marketo?

- [ ] **A)** Authorize social accounts
- [ ] **B)** Create a social app
- [ ] **C)** Set up a webhook
- [ ] **D)** Configure a push notification

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Before using a Social Button, you must authorize the social networks in Admin and then create a Social App in Marketing Activities.
 
 
</details>

### 24. Refer to the URL in the code block. What does the mkt_tok parameter represent?

```text
https://landing.example.com/offer?utm_source=linkedin&utm_medium=social&mkt_tok=abc123
```

- [ ] **A)** A tracking token for attributing the click to the social share
- [ ] **B)** An authentication token for lead sign-in
- [ ] **C)** A session identifier for the landing page
- [ ] **D)** A token for personalizing the page content

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The mkt_tok parameter is a tracking token added by Marketo to shared URLs, enabling attribution of clicks from social shares.
 
 
</details>


---

### **Manage, Execute, and Measure Webinar, Event, and Engagement Programs**

### 25. In Marketo Engage, which program type should be used for an in-person trade show?

- [ ] **A)** Event Program
- [ ] **B)** Webinar Program
- [ ] **C)** Email Program
- [ ] **D)** Engagement Program

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An Event program is designed for in-person events like trade shows, while Webinar programs are for online sessions. Email and Engagement programs serve different purposes.
 
 
</details>

### 26. Which of the following are true about webinar provider integration in Marketo? (Select all that apply.)

- [ ] **A)** The LaunchPoint service must be enabled globally in Admin.
- [ ] **B)** Custom field mapping is only available for ON24.
- [ ] **C)** Registration data can be synced automatically from Marketo to the provider.
- [ ] **D)** Attendance data is pulled in real-time from all providers.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The integration requires global LaunchPoint setup, and registration sync is automatic for many providers. Custom field mapping is available for multiple providers, and attendance sync is scheduled, not real-time for all.
 
 
</details>

### 27. Review the token snippet below. Which token prefix correctly refers to a custom program-level field?

```marketo
{{lead.Event Date}}
{{my.Event Date}}
{{system.Event Date}}
{{trigger.Event Date}}
```

- [ ] **A)** {{lead.Event Date}}
- [ ] **B)** {{my.Event Date}}
- [ ] **C)** {{system.Event Date}}
- [ ] **D)** {{trigger.Event Date}}

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Program-level custom tokens use the '{{my.}}' prefix. '{{lead.}}' is for lead fields, '{{system.}}' for system values, and '{{trigger.}}' is not a valid Marketo token prefix.
 
 
</details>

### 28. What does the cadence setting in an Engagement Program determine?

- [ ] **A)** How often content is sent from a stream
- [ ] **B)** The total number of emails a lead can receive
- [ ] **C)** Which stream a lead is placed in upon entry
- [ ] **D)** The order in which content pieces are delivered

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cadence defines the interval between content sends from a stream. It does not control total email count, stream assignment, or content order.
 
 
</details>

### 29. Which of the following are true about program membership statuses in Marketo?

- [ ] **A)** Statuses can only move forward in the numeric ladder.
- [ ] **B)** The 'Not in Program' status can be assigned manually.
- [ ] **C)** A lead can have multiple statuses simultaneously.
- [ ] **D)** Changing a status to a lower number requires removing the lead from the program.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Statuses are progressive and cannot be regressed. 'Not in Program' is a pseudo-status that cannot be assigned directly; leads are removed from the program. A lead has one current status per program.
 
 
</details>

### 30. A lead is currently at status 'Registered' (value 2) in an Event program. The channel has statuses: Invited (1), Registered (2), Attended (3). Which action will successfully update the lead to 'Attended'?

```text
Status ladder: Invited (1) -> Registered (2) -> Attended (3)
Lead current: 'Invited' (1)
```

- [ ] **A)** Use a 'Change Program Status' flow step to set 'Attended'.
- [ ] **B)** Use 'Change Program Status' to set 'Registered' and then another step to 'Attended'.
- [ ] **C)** Remove the lead and re-add them with status 'Attended'.
- [ ] **D)** Use 'Change Data Value' to update a status field.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Because statuses are progressive, you can move forward directly (e.g., from 1 to 3) as long as the target number is higher. The flow step 'Change Program Status' can set any higher status. Option 2 also works but is unnecessary. Removing the lead loses membership data, and 'Change Data Value' does not affect program status.
 
 
</details>

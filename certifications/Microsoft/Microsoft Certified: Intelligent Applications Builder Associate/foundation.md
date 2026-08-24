<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/microsoft-certified-associate-badge.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Microsoft Certified: Intelligent Applications Builder Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Build business application logic and automation](#build-business-application-logic-and-automation) (13 questions)
- [Create a foundation for intelligent applications](#create-a-foundation-for-intelligent-applications) (9 questions)
- [Create intelligent applications](#create-intelligent-applications) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:52:54.433Z |
| Domains | 3 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Build business application logic and automation | 13 |
| Create a foundation for intelligent applications | 9 |
| Create intelligent applications | 8 |

---

### **Build business application logic and automation**

### 1. Which type of cloud flow starts automatically when an event occurs in a data source?

- [ ] **A)** Automated
- [ ] **B)** Instant
- [ ] **C)** Scheduled
- [ ] **D)** Recurrence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Automated flows are event-driven and start when a defined event occurs, such as a row being created or an email arriving.
 
 
</details>

### 2. Which three options are primary cloud flow types in Power Automate?

- [ ] **A)** Automated
- [ ] **B)** Instant
- [ ] **C)** Scheduled
- [ ] **D)** Recurrence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Power Automate has three primary cloud flow types: automated, instant, and scheduled. Recurrence is a trigger, not a flow type.
 
 
</details>

### 3. Based on the trigger configuration shown in the code block, which type of cloud flow should the builder select?

```text
trigger type: OpenApiConnection
trigger name: When a row is added
```

- [ ] **A)** Automated
- [ ] **B)** Instant
- [ ] **C)** Scheduled
- [ ] **D)** Desktop flow

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The trigger listens for a data event, such as a row being added, which makes it an automated flow trigger.
 
 
</details>

### 4. A user needs to press a button in a Power Apps app to start an approval. Which type of cloud flow should be created?

- [ ] **A)** Automated
- [ ] **B)** Scheduled
- [ ] **C)** Instant
- [ ] **D)** Business process flow

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Instant flows start on demand through a manual action, such as clicking a button in Power Apps or selecting a Flow button.
 
 
</details>

### 5. Which two statements about business process flows are correct?

- [ ] **A)** They guide users through stages and steps.
- [ ] **B)** They execute unattended backend logic automatically.
- [ ] **C)** They must be activated before users can see them.
- [ ] **D)** They replace all cloud flows in an organization.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Business process flows provide guided stages and steps. They must be activated before they are available to users, and they do not execute unattended automation.
 
 
</details>

### 6. A model-driven app displays the sequence in the code block as an interactive process bar. Which component is being used?

```text
Stage 1: Qualify -> Stage 2: Develop -> Stage 3: Propose -> Stage 4: Close
```

- [ ] **A)** Business process flow
- [ ] **B)** Cloud flow
- [ ] **C)** Business rule
- [ ] **D)** Canvas app

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Business process flows display a stage-based process bar and guide users through defined stages and steps.
 
 
</details>

### 7. Which Power Automate control evaluates a logical expression and sends execution to one of two branches?

- [ ] **A)** Condition
- [ ] **B)** Scope
- [ ] **C)** Parallel branch
- [ ] **D)** Apply to each

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Condition action evaluates a logical expression and routes the flow into either the If yes or If no branch.
 
 
</details>

### 8. Which statuses can be evaluated in the Configure Run After setting?

- [ ] **A)** Succeeded
- [ ] **B)** Failed
- [ ] **C)** Timed out
- [ ] **D)** Skipped

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> Configure Run After supports four statuses: succeeded, failed, timed out, and skipped. All four can be selected as conditions for the next action.
 
 
</details>

### 9. According to the code block, when will the Send email action run?

```yaml
runAfter:
  Update_record:
    - Succeeded
    - Failed
```

- [ ] **A)** Only after Update_record succeeds
- [ ] **B)** Only after Update_record fails
- [ ] **C)** After Update_record succeeds or fails
- [ ] **D)** Only after Update_record times out

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The run-after configuration includes both Succeeded and Failed, so Send email runs after Update_record either succeeds or fails.
 
 
</details>

### 10. Which action should be used to map an array to a new array with selected properties?

- [ ] **A)** Compose
- [ ] **B)** Select
- [ ] **C)** Parse JSON
- [ ] **D)** Create CSV table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Select action maps an array to a new array with configured properties, leaving the original source unchanged.
 
 
</details>

### 11. Which actions are part of the Data Operation group in Power Automate?

- [ ] **A)** Compose
- [ ] **B)** Select
- [ ] **C)** Filter array
- [ ] **D)** Parse JSON

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> Compose, Select, Filter array, and Parse JSON are all part of the Data Operation action group in Power Automate.
 
 
</details>

### 12. What is the output of the expression in the code block when ordernumber is ORD-1001?

```text
concat('Order #', triggerOutputs()?['value/ordernumber'])
```

- [ ] **A)** Order #ORD-1001
- [ ] **B)** Order #
- [ ] **C)** ORD-1001 #Order
- [ ] **D)** An error

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The concat expression combines the text Order # with the trigger output value, producing Order #ORD-1001.
 
 
</details>

### 13. Which component is required to trigger an unattended desktop flow on a machine from a cloud flow?

- [ ] **A)** On-premises data gateway
- [ ] **B)** Microsoft Dataverse
- [ ] **C)** Custom connector
- [ ] **D)** Power Apps

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The on-premises data gateway securely connects cloud flows to on-premises resources and is required to trigger desktop flows.
 
 
</details>


---

### **Create a foundation for intelligent applications**

### 14. Which option set type should you use when multiple Dataverse tables must share the same list of values?

- [ ] **A)** Global choice
- [ ] **B)** Local choice
- [ ] **C)** Lookup column
- [ ] **D)** Multi-Select choice

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A global choice is reusable across tables; a local choice belongs to one table only.
 
 
</details>

### 15. Which two statements are true about business rules in Microsoft Dataverse?

- [ ] **A)** Run client-side on forms
- [ ] **B)** Update records in another table
- [ ] **C)** Hide or show fields
- [ ] **D)** Trigger server-side workflows

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Business rules run on the model-driven form only; they cannot update cross-table records or trigger workflows.
 
 
</details>

### 16. Refer to the relationship metadata in the code block. How should this relationship be implemented in Dataverse?

```json
{
  "fromTable": "Student",
  "toTable": "Course",
  "intersectTable": "CourseRegistration",
  "intersectColumns": ["EnrollmentDate", "Grade"]
}
```

- [ ] **A)** Custom intersection table with 1:N relationships
- [ ] **B)** Standard N:N relationship
- [ ] **C)** One-to-many relationship
- [ ] **D)** Same-table lookup

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Because the association stores EnrollmentDate and Grade, a custom intersection table with 1:N relationships is required.
 
 
</details>

### 17. Which Dataverse access level includes records in a user's business unit and all child business units?

- [ ] **A)** Deep
- [ ] **B)** Basic
- [ ] **C)** Local
- [ ] **D)** Global

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Deep access covers the user's business unit plus child business units; Local covers only the current unit.
 
 
</details>

### 18. Which statements about managed solutions are correct?

- [ ] **A)** Components are read-only after import
- [ ] **B)** Managed solutions can be edited directly in production
- [ ] **C)** Publisher prefix is part of component names
- [ ] **D)** Unmanaged solutions are used for final production deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Managed solutions are read-only after import and use publisher prefixes; production changes require a new managed version.
 
 
</details>

### 19. Use the business rule configuration in the code block. What is this rule able to do on a form?

```json
{
  "scope": "Form",
  "condition": "Severity equals High",
  "actions": [
    "Set Priority to Urgent",
    "Make TargetDate business required"
  ]
}
```

- [ ] **A)** Conditionally set field values and requirements
- [ ] **B)** Create a new record in another table
- [ ] **C)** Trigger a Power Automate flow
- [ ] **D)** Delete child records

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Business rules apply form-based actions such as setting values and making fields required; they cannot create records or trigger flows.
 
 
</details>

### 20. What determines the default prefix for a custom table in Dataverse?

- [ ] **A)** Solution publisher
- [ ] **B)** Environment owner
- [ ] **C)** Default solution
- [ ] **D)** Table creator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The solution publisher defines the custom prefix, such as new_, and it should remain consistent across environments.
 
 
</details>

### 21. Which capabilities are provided by calculated and rollup columns in Dataverse?

- [ ] **A)** Calculate values from fields in the same row
- [ ] **B)** Aggregate values from related records
- [ ] **C)** Trigger real-time workflows
- [ ] **D)** Enforce security roles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Calculated columns use same-row values; rollup columns aggregate related records on a scheduled basis, not in real time.
 
 
</details>

### 22. Use the DLP policy classifications in the code block. Which two statements are true?

```json
{
  "connectors": {
    "SharePoint": "Business",
    "SQL Server": "Business",
    "Gmail": "Non-Business",
    "Personal Email": "Blocked"
  }
}
```

- [ ] **A)** SharePoint and SQL Server are both Business
- [ ] **B)** Gmail is classified as Non-Business
- [ ] **C)** Personal Email is classified as Business
- [ ] **D)** All connectors can be used together

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The policy places SharePoint and SQL Server in Business, Gmail in Non-Business, and Personal Email blocked; mixed categories cannot be used together.
 
 
</details>


---

### **Create intelligent applications**

### 23. Which model-driven app component displays a read-only snapshot of a related record inside a main form?

- [ ] **A)** Quick View Form
- [ ] **B)** Quick Create Form
- [ ] **C)** Main Form
- [ ] **D)** Business Process Flow

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Quick view forms provide a compact read-only snapshot of a related record. Quick create forms are for data entry, while main forms are used for editing and displaying records.
 
 
</details>

### 24. Which statements about business process flows (BPFs) are true? Select all that apply.

- [ ] **A)** They are interactive and user-driven
- [ ] **B)** They can span multiple tables
- [ ] **C)** They run automatically in the background
- [ ] **D)** They replace business rules

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Business process flows guide users through stages manually and can span multiple tables. They are not background automation like Power Automate flows, and they do not replace business rules.
 
 
</details>

### 25. A canvas app uses the following expression to update a variable. What is the scope of this variable?

```powerfx
Set(gblCounter, gblCounter + 1)
```

- [ ] **A)** App-wide
- [ ] **B)** Current screen only
- [ ] **C)** Current gallery only
- [ ] **D)** Current flow only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Set creates and updates global variables that are visible across all screens. UpdateContext would create a screen-scoped context variable.
 
 
</details>

### 26. What is the main purpose of a model-driven app main form?

- [ ] **A)** Viewing and editing a record's data
- [ ] **B)** Browsing a list of records
- [ ] **C)** Running background automation
- [ ] **D)** Defining data source permissions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Main forms are the primary interface for creating, viewing, and editing records. Views are used for browsing lists of records.
 
 
</details>

### 27. Which statements about public and personal views are correct? Select all that apply.

- [ ] **A)** Public views can be shared with other users
- [ ] **B)** Personal views are visible only to the user who created them
- [ ] **C)** System views cannot be modified
- [ ] **D)** Personal views can be set as a table's default view

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Public views are shared with other users, while personal views are private to the creator. System views are customizable, and personal views cannot be set as the default view.
 
 
</details>

### 28. What does the following Power Fx expression accomplish in a canvas app?

```powerfx
IfError(Filter(Orders, OrderID = txtID.Text), Notify("Could not load order", NotificationType.Error))
```

- [ ] **A)** It handles errors gracefully and notifies the user
- [ ] **B)** It creates a new order in the data source
- [ ] **C)** It disables all controls on the screen
- [ ] **D)** It permanently deletes the filtered order

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IfError catches a failing Filter operation and runs Notify to show an error message, enabling graceful error handling.
 
 
</details>

### 29. What is required to connect a canvas app to an on-premises SQL Server?

- [ ] **A)** On-premises data gateway
- [ ] **B)** A custom JavaScript plug-in
- [ ] **C)** A Dataverse virtual table only
- [ ] **D)** A standard Outlook connector

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An on-premises data gateway bridges cloud services to on-premises data sources such as SQL Server.
 
 
</details>

### 30. Which Power Fx functions can create or update state in a canvas app? Select all that apply.

- [ ] **A)** Set
- [ ] **B)** UpdateContext
- [ ] **C)** ClearCollect
- [ ] **D)** ForAll

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Set creates global variables, UpdateContext creates context variables, and ClearCollect creates collections. ForAll loops over data but does not define state.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Blue%20Prism/SS&C%20Blue%20Prism%20ROM™️%202%20Professional" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Blue Prism Certified ROM 2 Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Development and Configuration](#development-and-configuration) (9 questions)
- [Governance and Compliance](#governance-and-compliance) (3 questions)
- [Integration and Interoperability](#integration-and-interoperability) (6 questions)
- [Release and Deployment Management](#release-and-deployment-management) (4 questions)
- [Solution Architecture](#solution-architecture) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:50:52.655Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Development and Configuration | 9 |
| Governance and Compliance | 3 |
| Integration and Interoperability | 6 |
| Release and Deployment Management | 4 |
| Solution Architecture | 8 |

---

### **Development and Configuration**

### 1. What is the primary purpose of a Business Object (BO) in Blue Prism?

- [ ] **A)** Orchestrate end-to-end process flows
- [ ] **B)** Encapsulate logic to interact with external systems
- [ ] **C)** Store configuration values like file paths
- [ ] **D)** Manage session schedules and runtime resources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A Business Object (BO) is the fundamental unit of integration that encapsulates logic to interact with a specific external application, system, or data source. Orchestration is done in the Process layer, configuration is stored in environment variables, and session management is separate.
 
 
</details>

### 2. Which of the following are advanced data types supported by Blue Prism? (Select all that apply.)

- [ ] **A)** Date
- [ ] **B)** TimeSpan
- [ ] **C)** Binary
- [ ] **D)** List

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Blue Prism supports Date, TimeSpan, and Binary as advanced data types. List is not a native data type; Collections are used for indexed structures.
 
 
</details>

### 3. Study the process flow snippet below. What is the most likely outcome when the 'Loop' stage finishes iterating over all rows of an empty collection?

```blueprism
Start -> Loop (over 'Orders' collection) -> [Loop Body: Get Next Row -> Decision] -> End Loop -> Log 'Done'
```

- [ ] **A)** The process continues normally without entering the loop body
- [ ] **B)** An exception is thrown because the collection is empty
- [ ] **C)** The loop executes once with a null row
- [ ] **D)** The process hangs indefinitely

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Loop stage over an empty collection simply skips the loop body and continues to the next stage after the loop end. No exception occurs unless you try to access a row (e.g., Get Next Row) outside the loop.
 
 
</details>

### 4. In a Blue Prism process, what is the correct way to parse a date string into a Date data type?

- [ ] **A)** Use the CDate() function in a Calculation stage
- [ ] **B)** Assign the text directly to a Date data item; Blue Prism auto-converts
- [ ] **C)** Use the FormatDateTime() function in a Decision stage
- [ ] **D)** Use the Utility - Strings - Parse action

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CDate() is the explicit conversion function for text-to-date. Although implicit conversion may work in some contexts, best practice is to use CDate() to ensure clarity and avoid locale issues.
 
 
</details>

### 5. Which of the following are valid methods to filter a collection in Blue Prism? (Select all that apply.)

- [ ] **A)** Utility - Collection Manipulation - Filter Collection
- [ ] **B)** Manual loop with Get Next Row and Decision stage
- [ ] **C)** Query Collection action
- [ ] **D)** Database - SQL Query

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Filter Collection is a built-in action. Manual filtering via loop is also possible but less efficient. 'Query Collection' does not exist. SQL Query is for database access, not for in-memory collections.
 
 
</details>

### 6. In the following process fragment, a sub-page is called with an input collection. Inside the sub-page, the collection is modified by adding a row. After the sub-page returns, what is the state of the original collection in the calling page?

```blueprism
MainPage: 'Orders' (Collection) -> Sub-Page Call (input: Orders) -> ... -> SubPage internal: Add Row to input -> Return -> MainPage continues
```

- [ ] **A)** The original collection remains unchanged because it was passed by value
- [ ] **B)** The original collection includes the new row because it was passed by reference
- [ ] **C)** The process throws an error because you cannot modify a collection inside a sub-page
- [ ] **D)** It depends on whether the sub-page has an output parameter of the same collection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In Blue Prism, when a collection is passed as an input parameter to a sub-page, it is passed by value (a copy). Modifications inside the sub-page do not affect the original. To reflect changes, the collection must also be an output parameter and assigned back.
 
 
</details>

### 7. What is the correct way to store sensitive credentials in a Blue Prism automation?

- [ ] **A)** Hardcode them in a Calculation stage
- [ ] **B)** Store them in an Environment Variable
- [ ] **C)** Use the Credential Store
- [ ] **D)** Encrypt them in a Text file and read at runtime

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Credential Store is Blue Prism's built-in encrypted repository for credentials. Environment variables are not encrypted; hardcoding is insecure; external files are not recommended.
 
 
</details>

### 8. Which of the following are true about Environment Variables in Blue Prism? (Select all that apply.)

- [ ] **A)** They are encrypted at rest
- [ ] **B)** They can vary per environment (Dev, Test, Prod)
- [ ] **C)** They are best used for non-sensitive configuration values
- [ ] **D)** They are resolved at runtime for each session

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C, D**
 
> 💡  **Explanation** 
> 
> Environment Variables are not encrypted. They are defined per environment and resolved at process start. They are suitable for non-sensitive configuration like file paths or server names.
 
 
</details>

### 9. Look at the error handling pattern below. What is the correct stage that must appear immediately after the 'Try' point?

```blueprism
Try -> [???] -> Navigate -> Click -> Catch -> Log Error -> End
```

- [ ] **A)** Recover stage
- [ ] **B)** Catch stage
- [ ] **C)** Resume stage
- [ ] **D)** End stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In Blue Prism, after the 'Try' point, the next stage must be a 'Recover' stage to define a recovery point. The Catch block comes after the protected stages. Resume is not used in this position.
 
 
</details>


---

### **Governance and Compliance**

### 10. What is the primary responsibility of the Change Advisory Board (CAB) in ROM™ 2 governance?

- [ ] **A)** Develop and test automation processes.
- [ ] **B)** Approve or reject changes before they move to production.
- [ ] **C)** Execute bots in production environments.
- [ ] **D)** Manage Blue Prism infrastructure and user accounts.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The CAB reviews and approves changes to production RPA components, ensuring risk and compliance are evaluated before deployment.
 
 
</details>

### 11. Which roles must be separated to enforce segregation of duties in ROM™ 2? (Select all that apply.)

- [ ] **A)** Process Developer and Process Controller
- [ ] **B)** Process Developer and System Administrator
- [ ] **C)** Change Advisory Board member and Release Manager
- [ ] **D)** Process Controller and System Administrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Segregation of duties requires separation of development, operations, and infrastructure roles to prevent conflicts and unauthorized changes.
 
 
</details>

### 12. Refer to the Blue Prism Work Queue configuration snippet. Which data protection principle is satisfied by the encryption setting?

```text
Work Queue Configuration:
  Item: Customer Record
  Data Fields:
    - SSN: {Encrypted: True, Key: DatabaseKey}

```

- [ ] **A)** Data minimization
- [ ] **B)** Lawful processing
- [ ] **C)** Encryption of personal data
- [ ] **D)** Right to erasure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Encrypting sensitive personal data fields directly supports GDPR Article 32 (security of processing) by protecting data confidentiality.
 
 
</details>


---

### **Integration and Interoperability**

### 13. Which integration method does Blue Prism use for consuming SOAP-based web services?

- [ ] **A)** HTTP/SOAP Web Services
- [ ] **B)** REST APIs
- [ ] **C)** DLL Calls
- [ ] **D)** Surface Automation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Blue Prism provides a dedicated 'Web API Services' business object for SOAP, which parses WSDL and handles SOAP envelopes.
 
 
</details>

### 14. Which authentication methods are supported by Blue Prism's HTTP VBO for REST APIs?

- [ ] **A)** Basic Authentication
- [ ] **B)** OAuth2
- [ ] **C)** API Key via custom headers
- [ ] **D)** Kerberos

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Blue Prism supports Basic, OAuth2, and API key authentication for REST APIs. Kerberos is not a standard option for the HTTP VBO.
 
 
</details>

### 15. Examine the process flow for a DLL call. What is the correct action to load a .NET assembly before invoking a method?

```plaintext
// Blue Prism action sequence:
// 1. 'Create Instance' with DLL path and class name
// 2. 'Invoke Method' with method name and parameters
// 3. 'Dispose' to release resources
```

- [ ] **A)** Create Instance
- [ ] **B)** Invoke Method
- [ ] **C)** Load Assembly
- [ ] **D)** Initialize Object

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'Create Instance' action in the Utility - .NET Object VBO loads the DLL and creates an instance of the public class.
 
 
</details>

### 16. Which Blue Prism VBO is used to automate Microsoft Excel without controlling the visible application?

- [ ] **A)** Excel VBO
- [ ] **B)** Outlook VBO
- [ ] **C)** SharePoint VBO
- [ ] **D)** HTTP VBO

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Excel VBO opens workbooks in memory using Interop, not by controlling the visible Excel application.
 
 
</details>

### 17. Which actions are available in Blue Prism's Outlook VBO for email handling?

- [ ] **A)** Send Email
- [ ] **B)** Get Emails
- [ ] **C)** Move Email
- [ ] **D)** Read Calendar

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Outlook VBO supports Send Email, Get Emails, Move Email, and Delete Email. It does not manage calendar items.
 
 
</details>

### 18. In the process flow for reading an email attachment, what is the mandatory action before using the Excel VBO on an attachment?

```plaintext
// Email processing steps:
// 1. Get Emails (filter by subject)
// 2. For each attachment: Save Attachment to temp folder
// 3. Open Workbook (Excel VBO) using saved file path
// 4. Get Worksheet as Collection
```

- [ ] **A)** Save Attachment
- [ ] **B)** Parse JSON
- [ ] **C)** Open Workbook
- [ ] **D)** Create HTTP Request

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Outlook VBO 'Save Attachment' action must be used to save the attachment to disk before the Excel VBO can open it.
 
 
</details>


---

### **Release and Deployment Management**

### 19. What is a release package in Blue Prism?

- [ ] **A)** An immutable snapshot of a set of artifacts at specific versions
- [ ] **B)** A collection of only processes without dependencies
- [ ] **C)** A dynamic set of artifacts that updates automatically during deployment
- [ ] **D)** A log file of deployment actions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A release package is a self-contained, immutable snapshot of selected artifacts (processes, objects, etc.) and their dependencies, serialized into a .bprelease file.
 
 
</details>

### 20. Which of the following can be included in a Blue Prism release package?

- [ ] **A)** Processes
- [ ] **B)** Objects
- [ ] **C)** Action groups
- [ ] **D)** Credentials (with constraints)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> A release package can include processes, objects, action groups, environment variables, and credentials (though credentials are exported as stubs unless allowed). All listed items are eligible.
 
 
</details>

### 21. Given the following release package manifest, which dependency is missing that should be included?

```json
{
  "process": "Reconciliation_V2.0",
  "objects": ["LedgerConnection_SAP v1.2"],
  "action_groups": ["SAPLogin v3.0"],
  "environment_variables": ["SAP_Server", "SAP_User"],
  "credentials": []
}
```

- [ ] **A)** Credential 'SAP_Password'
- [ ] **B)** Environment variable 'SAP_Server'
- [ ] **C)** Object 'LedgerConnection_SAP'
- [ ] **D)** Process 'Reconciliation_V2.0'

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The manifest includes the process, objects, action groups, and environment variables, but the process uses a credential (SAP_Password) which is not listed. The Release Manager would require this dependency to be resolved.
 
 
</details>

### 22. What is the primary purpose of a CI/CD pipeline in Blue Prism?

- [ ] **A)** Automate the build, test, and deployment of release artifacts
- [ ] **B)** Eliminate the need for manual user acceptance testing
- [ ] **C)** Replace the Change Advisory Board
- [ ] **D)** Allow direct deployment from developer machines to production

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CI/CD automates building, testing, and deploying validated artifacts through the release pipeline, but does not replace manual UAT or governance approvals.
 
 
</details>


---

### **Solution Architecture**

### 23. What is the primary mechanism for decoupling the supply of work items from their processing in Blue Prism?

- [ ] **A)** Collections
- [ ] **B)** Work Queues
- [ ] **C)** Data Items
- [ ] **D)** Environment Variables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Work Queues decouple work item supply from processing, enabling resilience and horizontal scaling.
 
 
</details>

### 24. Which two features are essential for building scalable automation solutions in Blue Prism?

- [ ] **A)** Stateless processes
- [ ] **B)** Monolithic process design
- [ ] **C)** Resource pooling
- [ ] **D)** Direct database connections from processes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Stateless processes and resource pooling are key to horizontal scaling; monolithic design and direct DB connections hinder scalability.
 
 
</details>

### 25. Given the Blue Prism snippet below, what does the Resume stage do?

```plaintext
Recover -> Log Message -> Resume
```

- [ ] **A)** Ends exception handling and continues normal flow
- [ ] **B)** Re-throws the exception to the parent page
- [ ] **C)** Terminates the process immediately
- [ ] **D)** Logs the exception and stops

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Resume stage marks the end of the recovery block; after it, normal process flow continues from the next stage.
 
 
</details>

### 26. According to ROM™ 2, where should UI interactions be placed in the layered architecture?

- [ ] **A)** Process Layer
- [ ] **B)** Object Layer
- [ ] **C)** Work Queue Layer
- [ ] **D)** Environment Layer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Object Layer encapsulates all direct application interactions (spying, API calls) to isolate changes from the Process Layer.
 
 
</details>

### 27. Which two factors must be evaluated when defining Business Object granularity?

- [ ] **A)** Reusability across processes
- [ ] **B)** Number of UI elements on the screen
- [ ] **C)** Application screen or logical component boundary
- [ ] **D)** Process layer decision complexity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Business Objects should align with reusable logical components (e.g., a screen) and be assessed for reuse across processes.
 
 
</details>

### 28. Examine the following queue item statuses. Which status is set when a robot successfully processes an item?

```plaintext
Pending -> Active -> [Processing] -> ?
```

- [ ] **A)** Active
- [ ] **B)** Completed
- [ ] **C)** Exception
- [ ] **D)** Deferred

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> After successful processing, the robot calls 'Mark as Completed', setting the item status to Completed.
 
 
</details>

### 29. What is the main difference between high availability and disaster recovery in Blue Prism?

- [ ] **A)** HA handles site loss; DR handles component failure
- [ ] **B)** HA handles component failure; DR handles site loss
- [ ] **C)** Both handle only database failures
- [ ] **D)** DR is automatically built into every Blue Prism license

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> High availability addresses local component failures, while disaster recovery deals with the loss of an entire site or data center.
 
 
</details>

### 30. Which two components must be replicated to the disaster recovery site for a complete Blue Prism DR plan?

- [ ] **A)** Blue Prism database
- [ ] **B)** Runtime Resources
- [ ] **C)** Local user profiles
- [ ] **D)** Client-side browser cache

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The database and Runtime Resources (with supporting Application Servers) are fundamental to resume processing at the DR site.
 
 
</details>

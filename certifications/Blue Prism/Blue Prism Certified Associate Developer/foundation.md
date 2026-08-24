<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Blue%20Prism/Blue%20Prism%20Certified%20Associate%20Developer" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Blue Prism Certified Associate Developer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Blue Prism Environment and Release Management](#blue-prism-environment-and-release-management) (4 questions)
- [Blue Prism Foundation Concepts](#blue-prism-foundation-concepts) (6 questions)
- [Error Handling and Work Queue Management](#error-handling-and-work-queue-management) (6 questions)
- [Governance, Security, and Best Practices](#governance-security-and-best-practices) (3 questions)
- [Process Design and Development](#process-design-and-development) (11 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:50:28.751Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Blue Prism Environment and Release Management | 4 |
| Blue Prism Foundation Concepts | 6 |
| Error Handling and Work Queue Management | 6 |
| Governance, Security, and Best Practices | 3 |
| Process Design and Development | 11 |

---

### **Blue Prism Environment and Release Management**

### 1. What is the file extension used for a bundled release export in Blue Prism?

- [ ] **A)** .bprelease
- [ ] **B)** .bpobject
- [ ] **C)** .bpprocess
- [ ] **D)** .bpkg

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Blue Prism standardized on the .bprelease extension for all exports in modern versions; .bpobject and .bpprocess are legacy extensions.
 
 
</details>

### 2. Which two statements about exporting Blue Prism components are true?

- [ ] **A)** Exporting a process automatically includes all referenced objects.
- [ ] **B)** Exported files are encrypted and digitally signed.
- [ ] **C)** The default file extension for modern Blue Prism exports is .bprelease.
- [ ] **D)** Importing a process requires that all referenced objects exist in the target environment.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Exported files are encrypted and signed for security. .bprelease is the standard extension. Export does not auto-include dependencies, and imports can proceed with missing dependencies (warning is shown).
 
 
</details>

### 3. Based on the deployment parameters shown, which parameter is most critical to avoid runtime failure when moving a process with a custom DLL?

```json
{
  "packageType": "Full",
  "includeCredentials": false,
  "externalDependencies": ["PayCalc.dll"],
  "environmentMapping": "automatic"
}
```

- [ ] **A)** packageType
- [ ] **B)** includeCredentials
- [ ] **C)** externalDependencies
- [ ] **D)** environmentMapping

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> External dependencies (like DLLs) must be explicitly added to the package; otherwise, the process will fail with 'File not found' at runtime.
 
 
</details>

### 4. What is the initial status of a session when it is submitted for execution in Blue Prism?

- [ ] **A)** Running
- [ ] **B)** Pending
- [ ] **C)** Completed
- [ ] **D)** Exception

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A session is created with status 'Pending' (1) before the resource picks it up and changes it to 'Running'.
 
 
</details>


---

### **Blue Prism Foundation Concepts**

### 5. Which Blue Prism component is primarily responsible for orchestrating the end-to-end business process flow?

- [ ] **A)** Process Studio
- [ ] **B)** Object Studio
- [ ] **C)** Control Room
- [ ] **D)** System Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Process Studio is used for designing the end-to-end workflow; Object Studio handles UI interactions, not process orchestration.
 
 
</details>

### 6. Which of the following are true regarding Digital Workers in Blue Prism?

- [ ] **A)** They run processes unattended.
- [ ] **B)** They require a user to be logged into Windows.
- [ ] **C)** They can be added to resource pools.
- [ ] **D)** They consume Development licenses.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Digital Workers run unattended, can be pooled, and consume Runtime licenses, not Development licenses.
 
 
</details>

### 7. Based on the following process snippet, where should the 'Login' action be defined?\n\nProcess:\nStart -> Call 'Login' -> Call 'GetData' -> End

```bp-process
Start -> Call 'Login' -> Call 'GetData' -> End
```

- [ ] **A)** Process Studio
- [ ] **B)** Object Studio
- [ ] **C)** Control Room
- [ ] **D)** System Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Actions like 'Login' are developed in Object Studio as part of a Business Object, then called from Process Studio.
 
 
</details>

### 8. What key principle differentiates Blue Prism from traditional scripting approaches?

- [ ] **A)** Non-invasive integration via UI or API
- [ ] **B)** Requires coding in C#
- [ ] **C)** Modifies the application code
- [ ] **D)** Only runs attended automations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Blue Prism connects through UI or API without changing existing applications, unlike macros that often require system modifications.
 
 
</details>

### 9. Which components are primarily used for designing automation in Blue Prism?

- [ ] **A)** Process Studio
- [ ] **B)** Object Studio
- [ ] **C)** Control Room
- [ ] **D)** System Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Process Studio and Object Studio are development tools; Control Room is for runtime, System Manager for administration.
 
 
</details>

### 10. Given the resource status: 'Resource: Worker01 - Status: Available - Type: Runtime', what type of resource is Worker01?

```text
Resource: Worker01 - Status: Available - Type: Runtime
```

- [ ] **A)** Digital Worker
- [ ] **B)** Interactive Client
- [ ] **C)** Control Room
- [ ] **D)** System Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Runtime type indicates a Digital Worker, which runs unattended processes without user login.
 
 
</details>


---

### **Error Handling and Work Queue Management**

### 11. What is the primary characteristic of a recoverable exception in Blue Prism?

- [ ] **A)** It is a permanent error that requires immediate escalation.
- [ ] **B)** It is a transient error that can be retried without compromising data integrity.
- [ ] **C)** It is an error that always stops the process immediately.
- [ ] **D)** It is an error that is ignored by the exception handling system.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A recoverable exception is a temporary error (e.g., network timeout) that can be retried; permanent errors are non-recoverable.
 
 
</details>

### 12. Which of the following are valid Blue Prism exception handling stages? (Select all that apply.)

- [ ] **A)** Throw
- [ ] **B)** Recover
- [ ] **C)** Resume
- [ ] **D)** Rethrow

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> All four stages (Throw, Recover, Resume, Rethrow) are part of Blue Prism's exception handling capabilities.
 
 
</details>

### 13. Consider the following exception handling flow: Inside a Block stage’s exception page, after catching an exception, the developer places a Resume stage. What is the immediate result?

```blueprism
Block Start
  Calculate Division (may throw exception)
Exception Page:
  Recover
  Log Error
  Resume
```

- [ ] **A)** The process continues from the stage immediately after the Block.
- [ ] **B)** The process re-executes the stage that originally caused the exception.
- [ ] **C)** The process throws a new exception because Resume cannot be used here.
- [ ] **D)** The process ends immediately.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Resume returns control to the exact stage that threw the exception, allowing a retry of that operation.
 
 
</details>

### 14. What status is assigned to a Work Queue item that has failed and requires manual analysis?

- [ ] **A)** Pending
- [ ] **B)** Active
- [ ] **C)** Exception
- [ ] **D)** Deferred

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> An item in Exception status has failed and typically requires manual review before it can be resubmitted.
 
 
</details>

### 15. Which actions can be performed on a Work Queue directly from the Control Room? (Select all that apply.)

- [ ] **A)** Pause the queue
- [ ] **B)** Resume the queue
- [ ] **C)** Force complete an item
- [ ] **D)** Modify the queue's maximum retry count

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Control Room allows pausing/resuming the queue and force completing items, but configuration changes (like max retries) must be done in Process Studio.
 
 
</details>

### 16. Given the code snippet that sets the priority of a Work Queue item, what numeric value represents the highest priority?

```blueprism
Set Priority 1
Add Item to Queue
```

- [ ] **A)** 1
- [ ] **B)** 5
- [ ] **C)** 99
- [ ] **D)** 100

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Priority ranges from 1 (highest) to 99 (lowest); 1 is the most urgent and will be picked first.
 
 
</details>


---

### **Governance, Security, and Best Practices**

### 17. According to Blue Prism best practices, which prefix should be used when naming a process?

- [ ] **A)** PRC_
- [ ] **B)** BO_
- [ ] **C)** EV_
- [ ] **D)** Obj.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Blue Prism recommends the prefix 'PRC_' for processes to clearly identify them as process objects.
 
 
</details>

### 18. Which two naming practices are correct according to Blue Prism conventions? (Choose two.)

- [ ] **A)** Business object name: BO_SAP_MaterialMaster
- [ ] **B)** Action name: getInvoiceData
- [ ] **C)** Data item name: strCustomerID
- [ ] **D)** Process name: Process_Invoice

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> BO_SAP_MaterialMaster follows PascalCase with BO_ prefix; strCustomerID uses camelCase with Hungarian notation. getInvoiceData should be PascalCase; Process_Invoice should use PRC_ prefix.
 
 
</details>

### 19. Examine the Blue Prism stage expression below. Which naming convention error does it contain?

```blueprism
getInvoiceData("12345")
```

- [ ] **A)** The process name uses an underscore after the prefix.
- [ ] **B)** The action name uses camelCase instead of PascalCase.
- [ ] **C)** The data item name uses PascalCase instead of camelCase.
- [ ] **D)** The environment variable name is missing the EV_ prefix.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Actions must be in PascalCase (e.g., 'GetInvoiceData'), not camelCase. 'getInvoiceData' is incorrect.
 
 
</details>


---

### **Process Design and Development**

### 20. In Blue Prism Process Studio, which stage is used to perform an action on a UI element, such as clicking a button?

- [ ] **A)** Navigate Stage
- [ ] **B)** Write Stage
- [ ] **C)** Read Stage
- [ ] **D)** Wait Stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Navigate stage is used to perform actions on application elements, such as clicking, selecting, or launching. Write is for entering data, Read for extracting data, and Wait for pausing execution.
 
 
</details>

### 21. Which of the following are valid data types for a Blue Prism Data Item? (Select all that apply)

- [ ] **A)** Text
- [ ] **B)** Number
- [ ] **C)** Collection
- [ ] **D)** Binary

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> Blue Prism Data Items can be of type Text, Number, Date, Time, DateTime, Flag (Boolean), Binary, and Collection. All four listed are valid.
 
 
</details>

### 22. A developer wants to extract the first 10 characters from a Data Item named `[s_FullName]`. Complete the Calculation stage expression to store the result in a new Data Item named `[s_FirstName]`.

```vb
Left([s_FullName], 10)
```

- [ ] **A)** Left([s_FullName], 10)
- [ ] **B)** Right([s_FullName], 10)
- [ ] **C)** Mid([s_FullName], 1, 10)
- [ ] **D)** Substring([s_FullName], 1, 10)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Blue Prism uses VBA-style functions. `Left` and `Mid` are valid. The correct answer includes at least one of these. `Right` takes from end, and `Substring` is not a native function.
 
 
</details>

### 23. In Blue Prism Object Studio, which type of action is exposed to a calling Process?

- [ ] **A)** Published Action
- [ ] **B)** Private Action
- [ ] **C)** Internal Action
- [ ] **D)** Global Action

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Published Actions are the public interface of a Business Object and can be called from Process Studio. Private actions are internal to the Object.
 
 
</details>

### 24. Which of the following are valid spy modes in Blue Prism’s Application Modeller? (Select all that apply)

- [ ] **A)** Win32
- [ ] **B)** HTML
- [ ] **C)** Active Accessibility
- [ ] **D)** UI Automation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The three classic modes are Win32, HTML, and Active Accessibility. UI Automation is not a standard spy mode in the traditional three, though newer versions may support it; the exam focuses on the core three.
 
 
</details>

### 25. A developer needs to define a collection field named `OrderDate` of type Date. In the Application Modeller’s collection field definition, what data type should be selected?

```plaintext
DateTime
```

- [ ] **A)** Date
- [ ] **B)** Text
- [ ] **C)** Number
- [ ] **D)** DateTime

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Blue Prism does not have a separate 'Date' type in collections; it uses DateTime for both dates and times. The closest correct answers are Date and DateTime, with DateTime being the actual type. The examiner may accept both.
 
 
</details>

### 26. In Blue Prism, which stage requires an element defined in the Application Modeller and can perform actions like clicking or launching?

- [ ] **A)** Navigate
- [ ] **B)** Write
- [ ] **C)** Read
- [ ] **D)** Wait

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Navigate stage is the correct stage for performing actions on elements. Write is for entering text, Read for extracting, Wait for pausing.
 
 
</details>

### 27. Which of the following are true about the Wait stage in Blue Prism? (Select all that apply)

- [ ] **A)** It can wait for a specified time duration.
- [ ] **B)** It can wait for an element to exist or become visible.
- [ ] **C)** It can wait for an element to have a specific attribute value.
- [ ] **D)** It can wait for a process variable to change.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The Wait stage supports time-based waits and element-based waits (e.g., for existence, visibility, attribute state). It cannot directly wait for a process variable change; that would require a loop.
 
 
</details>

### 28. A developer wants to loop over a Collection named `[colOrders]` and process each row. Which stage should be placed at the start of the loop?

```plaintext
Loop
```

- [ ] **A)** Loop Stage
- [ ] **B)** Decision Stage
- [ ] **C)** Calculation Stage
- [ ] **D)** Navigate Stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Loop stage is designed for iterating over collections or counting loops. Decision is for branching, Calculation for expressions, Navigate for UI actions.
 
 
</details>

### 29. In Blue Prism, which mode in the Application Modeller uses pixel coordinates to define an area of the screen?

- [ ] **A)** Region Mode
- [ ] **B)** Element Mode
- [ ] **C)** Attribute Mode
- [ ] **D)** Navigate Mode

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Region Mode defines interactions based on pixel coordinates relative to a parent element or screen. Element Mode uses accessibility properties, Attribute Mode uses HTML attributes.
 
 
</details>

### 30. Which of the following stages can be used to read data from an application into a Data Item? (Select all that apply)

- [ ] **A)** Read Stage
- [ ] **B)** Wait Stage
- [ ] **C)** Navigate Stage
- [ ] **D)** Write Stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Read stage is specifically designed to read data from an element. Wait pauses, Navigate performs actions, Write enters data.
 
 
</details>

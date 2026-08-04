<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Blue%20Prism/Blue%20Prism%20Certified%20Developer" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Developer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Blue Prism Foundation](#blue-prism-foundation) (6 questions)
- [Object Studio](#object-studio) (7 questions)
- [Process Studio](#process-studio) (9 questions)
- [Solution Design and Governance](#solution-design-and-governance) (3 questions)
- [Work Queues and Control Room](#work-queues-and-control-room) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:37.560Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Blue Prism Foundation | 6 |
| Object Studio | 7 |
| Process Studio | 9 |
| Solution Design and Governance | 3 |
| Work Queues and Control Room | 5 |

---

### **Blue Prism Foundation**

### 1. Which of the following best describes a key feature of the Blue Prism platform?

- [ ] **A)** It operates solely through simple script recording without any governance.
- [ ] **B)** It integrates with systems via UI-level interaction or API connectors without altering underlying applications.
- [ ] **C)** It requires developers to have deep knowledge of the underlying system code to automate processes.
- [ ] **D)** It is a cloud-native solution that cannot be deployed on-premises.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Blue Prism is a non-invasive RPA platform that integrates at the UI or API level, leaving underlying legacy systems unchanged. The other options describe scripting tools, emphasize code knowledge, or falsely claim cloud-only deployment.
 
 
</details>

### 2. Which two components are part of the Blue Prism architecture? (Select two.)

- [ ] **A)** Blue Prism Server
- [ ] **B)** Blue Prism Runtime Resource (Robot)
- [ ] **C)** Blue Prism API Gateway
- [ ] **D)** Blue Prism Cloud Orchestrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The Blue Prism Server coordinates scheduling and work allocation, while the Runtime Resource (Robot) executes processes. API Gateway and Cloud Orchestrator are not native core components; Blue Prism uses WCF/REST for communication.
 
 
</details>

### 3. Review the code block below, which shows part of a Release Manager deployment sequence. What should be done first before deploying a package to a target environment?

```plaintext
// Deployment Sequence
// Step 1: ??
// Step 2: Create Release Package in Source
// Step 3: Approve Package
// Step 4: Deploy Package to Target
// Step 5: Verify and Unlock
```

- [ ] **A)** Unlock the source environment
- [ ] **B)** Lock the target environment
- [ ] **C)** Create the release package in the target environment
- [ ] **D)** Approve the package in the source environment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> To prevent concurrent changes, the target environment must be locked before deploying a release package. The other options are either incorrect order or apply to different steps.
 
 
</details>

### 4. In the Blue Prism security model, what is the correct way to store a password used by a process?

- [ ] **A)** Hardcode the password as a text Data Item in the process for simplicity.
- [ ] **B)** Store the password in the Credential Manager, which encrypts it in the database.
- [ ] **C)** Place the password in a configuration file on the runtime resource.
- [ ] **D)** Use a public action in the Business Object to pass the password as a parameter.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Blue Prism's Credential Manager stores passwords encrypted in the database, ensuring security and separation of duties. Hardcoding or using configuration files violates security best practices.
 
 
</details>

### 5. Which two statements are true regarding Business Objects in Blue Prism? (Select two.)

- [ ] **A)** Business Objects can be executed directly from the Control Room without a process.
- [ ] **B)** Business Objects encapsulate application-specific actions and are reusable across processes.
- [ ] **C)** Business Objects should contain process-specific logic to reduce complexity.
- [ ] **D)** Business Objects can have both public and internal actions.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Business Objects are reusable components that contain actions for one application. They are called from processes, not run directly. They should not contain process logic. They have public actions (visible to processes) and internal actions (for internal use).
 
 
</details>

### 6. Examine this snippet from an Object Studio action that spies a UI element. Which spy mode is most appropriate for a Java application?

```plaintext
// Spying a button in a Java Swing application
// Expected attributes: Class=javax.swing.JButton, Name=Submit
// Spy Mode options: Win32, HTML, Accessibility, Region
```

- [ ] **A)** Win32
- [ ] **B)** HTML
- [ ] **C)** Active Accessibility (MSAA)
- [ ] **D)** Region

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Java applications are best spied with Active Accessibility (MSAA) or UI Automation. Win32 may not recognize custom controls, HTML is for web apps, and Region is a fallback for virtual environments.
 
 
</details>


---

### **Object Studio**

### 7. What is the primary purpose of a Business Object (BO) in Blue Prism?

- [ ] **A)** To orchestrate the overall process flow
- [ ] **B)** To encapsulate integration logic with external applications
- [ ] **C)** To manage user credentials and environment variables
- [ ] **D)** To schedule and monitor automated processes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A Business Object (BO) is the atomic unit of integration in Blue Prism. It encapsulates low-level interaction logic with external systems, separating integration complexity from process orchestration.
 
 
</details>

### 8. Which of the following are key components when creating a new Business Object in Object Studio? (Select all that apply.)

- [ ] **A)** Startup and Shutdown sequences
- [ ] **B)** Application Modeller elements
- [ ] **C)** Process-level decision stages
- [ ] **D)** Action pages and input/output parameters

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> A Business Object must define its Startup/Shutdown sequences, Application Modeller spies, and Actions with parameters. Process-level decisions belong in Process Studio, not Object Studio.
 
 
</details>

### 9. Examine the code stage below. After execution, what is the value of the output variable 'result' if the input 'val' is an empty string?

```csharp
if (!string.IsNullOrEmpty(val))
{
    result = val.Trim();
}
else
{
    result = string.Empty;
}
```

- [ ] **A)** Empty string
- [ ] **B)** null
- [ ] **C)** An empty string trimmed
- [ ] **D)** The string 'Empty'

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code returns 'val.Trim()' which for an empty string remains empty. It will not throw an exception.
 
 
</details>

### 10. What is the role of the Application Modeller in Object Studio?

- [ ] **A)** It manages credential storage for the Business Object
- [ ] **B)** It stores process flow definitions
- [ ] **C)** It spies and stores UI element attributes for application interaction
- [ ] **D)** It compiles C# code for code stages

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Application Modeller is used to identify and store UI elements (spies) for the target application. It captures attributes and hierarchy for reliable element recognition.
 
 
</details>

### 11. Which of the following are valid spying techniques in Blue Prism? (Select all that apply.)

- [ ] **A)** Win32
- [ ] **B)** HTML
- [ ] **C)** OCR (Optical Character Recognition)
- [ ] **D)** Region

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Blue Prism supports Win32, HTML, Accessibility, Region, and Text spying. OCR is a separate capability, not a native spying mode in the Application Modeller.
 
 
</details>

### 12. Using the Write stage configuration shown, what will happen when the stage executes if the element is not found?

```text
Write Stage Properties:
- Element: btnSubmit
- Input Type: Single Line
- Text: "Submit"
- Timeout: 10 seconds
- Continue On Error: False
```

- [ ] **A)** Continue without error
- [ ] **B)** Throw an exception
- [ ] **C)** Wait indefinitely until the element appears
- [ ] **D)** Write the text to the active window instead

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Write stage by default throws an exception if the target element is not found. It does not wait or redirect.
 
 
</details>

### 13. What does the wildcard '*' represent when used in an attribute value in the Application Modeller?

- [ ] **A)** Matches exactly one character
- [ ] **B)** Matches zero or more characters
- [ ] **C)** Matches any digit
- [ ] **D)** Matches a literal asterisk

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In Blue Prism, '*' is a wildcard that matches any sequence of zero or more characters. '?' matches exactly one character. Regex is not supported in spy attributes.
 
 
</details>


---

### **Process Studio**

### 14. Which stage type is used in Process Studio to evaluate a Boolean expression and branch the flow?

- [ ] **A)** Decision Stage
- [ ] **B)** Calculation Stage
- [ ] **C)** Action Stage
- [ ] **D)** Page Reference Stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Decision stage evaluates a Boolean expression and directs the flow to either the True or False exit path. Other stages have different functions: Calculation manipulates data, Action invokes a Business Object action, and Page Reference calls a sub-page.
 
 
</details>

### 15. Which of the following are valid data types for a Data Item in Blue Prism? (Select all that apply.)

- [ ] **A)** Text
- [ ] **B)** Number
- [ ] **C)** Collection
- [ ] **D)** Image

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Blue Prism supports Text, Number, Date, Time, DateTime, Boolean, Binary, Password, and Collection types. Image is not a standard data type; binary is used for files.
 
 
</details>

### 16. Examine the following Process Studio flow snippet. What will be the value of [Result] after the flow executes?

```plaintext
Start -> Calculation: [Result] = [X] * 3 (where [X] = 5) -> End
```

- [ ] **A)** 15
- [ ] **B)** 10
- [ ] **C)** 5
- [ ] **D)** 0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The calculation stage multiplies [X] (5) by 3, producing 15, which is stored in [Result].
 
 
</details>

### 17. What is the correct syntax to retrieve an environment variable named 'ServerName' in a calculation expression?

- [ ] **A)** [EnvironmentVariable("ServerName")]
- [ ] **B)** EnvironmentVariable("ServerName")
- [ ] **C)** [EnvironmentVariable('ServerName')]
- [ ] **D)** [GetEnvironmentVariable("ServerName")]

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Blue Prism uses square brackets with the keyword EnvironmentVariable and the key in double quotes. The function syntax without brackets is invalid.
 
 
</details>

### 18. Which of the following are valid stages for exception handling in Process Studio? (Select all that apply.)

- [ ] **A)** Throw Stage
- [ ] **B)** Try-Catch Stage
- [ ] **C)** Recover Stage
- [ ] **D)** Resume Stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> All four are core exception handling stages. Throw raises an exception, Try-Catch defines a protected block, Recover clears the exception context, and Resume continues normal flow.
 
 
</details>

### 19. In the following process flow, how many times will the loop body execute? (Assume [Count] = 0 initially.)

```plaintext
Start -> Decision: [Count] < 3? (True) -> Calculation: [Count] = [Count] + 1 -> Loop back -> End (False)
```

- [ ] **A)** 3
- [ ] **B)** 4
- [ ] **C)** 2
- [ ] **D)** 0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The loop runs while [Count] < 3. It starts at 0, increments each time: 0,1,2 (3 iterations). After the third increment, Count becomes 3 and the condition fails.
 
 
</details>

### 20. What is the purpose of the 'Recover' stage in Blue Prism exception handling?

- [ ] **A)** It clears the current exception context and allows the process to continue.
- [ ] **B)** It re-throws the exception to the parent page.
- [ ] **C)** It logs the exception and terminates the process.
- [ ] **D)** It pauses the process until an operator responds.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Recover stage resets the Exception system variable (clears it) so that normal processing can resume after handling an exception. It does not re-throw or terminate.
 
 
</details>

### 21. Which of the following are characteristics of a Session Variable in Blue Prism? (Select all that apply.)

- [ ] **A)** They are set at the start of a runtime session.
- [ ] **B)** They can be modified during process execution.
- [ ] **C)** They are accessible only within the current session.
- [ ] **D)** They are stored in the Blue Prism database.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Session variables are passed at session launch (e.g., via command line) and are read-only after initialization. They exist only for that session, not persisted in the database.
 
 
</details>

### 22. Review the process flow: Start -> Decision: [IsValid] = True? (True) -> Calculation: [Status] = 'Approved' -> End; (False) -> Calculation: [Status] = 'Rejected' -> End. If [IsValid] = False, what is the value of [Status]?

```plaintext
Start -> Decision: [IsValid] = True? (True) -> Calculation: [Status] = 'Approved' -> End; (False) -> Calculation: [Status] = 'Rejected' -> End
```

- [ ] **A)** 'Rejected'
- [ ] **B)** 'Approved'
- [ ] **C)** Empty string
- [ ] **D)** Null

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The False branch executes, setting Status to 'Rejected'. The calculation stage on the False path is performed as expected.
 
 
</details>


---

### **Solution Design and Governance**

### 23. What is the primary purpose of separating Process and Object in Blue Prism?

- [ ] **A)** To allow multiple developers to work simultaneously
- [ ] **B)** To enable reuse of business actions across multiple processes
- [ ] **C)** To reduce the number of stages in a process
- [ ] **D)** To increase the speed of execution

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Modular design separates processes (orchestration logic) from objects (business action steps). This separation ensures objects can be reused across multiple processes, avoiding duplication and improving maintainability.
 
 
</details>

### 24. Which of the following are true about the Blue Prism delivery framework regarding coexistence and security? (Select two.)

- [ ] **A)** Runtime Resources should be dedicated machines to avoid resource contention with other RPA tools
- [ ] **B)** Credential vault keys are included in release packages
- [ ] **C)** Process Controllers can modify processes
- [ ] **D)** The delivery framework requires role-based access control to enforce segregation of duties

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> The framework mandates dedicated Runtime Resources to avoid conflicts with other automation platforms (coexistence). Role-based access control is enforced to ensure segregation of duties (security). Credential vault keys are never included in release packages, and Process Controllers only execute, not modify, processes.
 
 
</details>

### 25. In the following exception handling pattern, what is the role of the Recovery stage?

```plaintext
Recovery
  -> Validate Data
  -> Process Record
  -> Exception (Rethrow)

```

- [ ] **A)** It catches the exception and allows custom handling
- [ ] **B)** It throws a new exception
- [ ] **C)** It resumes execution at the next stage after the failed one
- [ ] **D)** It logs the exception automatically

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Recovery stage is the 'catch' point—execution jumps here when an exception occurs. It does not handle the exception itself; custom handling (logging, decisions, rethrow) must follow via subsequent stages.
 
 
</details>


---

### **Work Queues and Control Room**

### 26. What is the default status of a newly inserted work queue item in Blue Prism?

- [ ] **A)** Active
- [ ] **B)** Pending
- [ ] **C)** Completed
- [ ] **D)** Locked

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Newly inserted work queue items are always in Pending status, ready to be processed by Get Next Item. Active, Completed, and Locked statuses occur later in the lifecycle.
 
 
</details>

### 27. Which of the following are valid work queue item statuses? (Select all that apply.)

- [ ] **A)** Pending
- [ ] **B)** Active
- [ ] **C)** Deferred
- [ ] **D)** Queued

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Valid statuses include Pending, Active, Completed, Exception, Deferred, and Locked. 'Queued' is not a recognized status in Blue Prism work queues.
 
 
</details>

### 28. What does the following SQL query do when executed against the work queue database?

```sql
SELECT COUNT(*) FROM BPAWorkQueue WHERE status = 0;
```

- [ ] **A)** Counts items with Active status
- [ ] **B)** Counts items with Pending status
- [ ] **C)** Counts items with Completed status
- [ ] **D)** Counts items with Locked status

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In Blue Prism's work queue tables, status 0 corresponds to Pending. The query counts all items that are still waiting to be processed.
 
 
</details>

### 29. If a work queue's Max Attempts is set to 3, how many total attempts can a process make on a single item?

- [ ] **A)** 2
- [ ] **B)** 3
- [ ] **C)** 4
- [ ] **D)** 5

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Max Attempts setting includes the initial attempt. Therefore, with a value of 3, the process has exactly 3 attempts (first try + 2 retries).
 
 
</details>

### 30. Which of the following actions release the lock on a work queue item? (Select all that apply.)

- [ ] **A)** Completing the item
- [ ] **B)** Setting the item to Exception
- [ ] **C)** Deferring the item
- [ ] **D)** Changing the item's priority

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Locks are released when an item is completed, set to Exception, or deferred. Changing priority does not affect the lock; the item remains locked until its status is explicitly changed.
 
 
</details>

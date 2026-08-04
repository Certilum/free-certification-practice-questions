<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Blue%20Prism/Blue%20Prism%20Certified%20Professional%20Developer" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Professional Developer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Advanced Features and Release Management](#advanced-features-and-release-management) (3 questions)
- [Data Handling and Integration](#data-handling-and-integration) (6 questions)
- [Development Execution](#development-execution) (8 questions)
- [Exception Handling and Work Queues](#exception-handling-and-work-queues) (4 questions)
- [Security and Deployment](#security-and-deployment) (3 questions)
- [Solution Design](#solution-design) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:42.675Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Advanced Features and Release Management | 3 |
| Data Handling and Integration | 6 |
| Development Execution | 8 |
| Exception Handling and Work Queues | 4 |
| Security and Deployment | 3 |
| Solution Design | 6 |

---

### **Advanced Features and Release Management**

### 1. Which authentication method is recommended by Blue Prism for machine-to-machine integration in production environments?

- [ ] **A)** Basic Authentication (username/password)
- [ ] **B)** OAuth2 Client Credentials
- [ ] **C)** API Key in Header
- [ ] **D)** Digest Authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Blue Prism recommends OAuth2 Client Credentials for machine-to-machine integration because it provides better security with token-based authentication and scoped access, while basic authentication is simpler but less secure for production.
 
 
</details>

### 2. Which of the following are valid logging levels that can be set on a Process or Object in Blue Prism? (Select all that apply)

- [ ] **A)** Info
- [ ] **B)** Warn
- [ ] **C)** Fatal
- [ ] **D)** Debug

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Blue Prism supports logging levels Info, Warn, Error, and Debug. 'Fatal' is not a standard logging level; the highest severity is 'Error'.
 
 
</details>

### 3. Consider the following JSON payload for starting a Blue Prism process via the Process API. What is incorrect in this payload?

```json
{
  "processName": "MyProcess",
  "InputParameters": {
    "param1": "value1"
  }
}
```

- [ ] **A)** The key 'processName' should be 'ProcessName'
- [ ] **B)** The key 'InputParameters' should be 'inputParameters'
- [ ] **C)** The value for 'processName' must be an integer
- [ ] **D)** The payload is missing a 'sessionId' field

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> According to Blue Prism API documentation, the JSON payload for starting a process uses camelCase keys. The correct key is 'inputParameters' (lowercase 'i'), not 'InputParameters'.
 
 
</details>


---

### **Data Handling and Integration**

### 4. What is the default value of a Number data item when it is first created in Blue Prism?

- [ ] **A)** 0
- [ ] **B)** Empty string
- [ ] **C)** False
- [ ] **D)** Null

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In Blue Prism, Number data items automatically default to 0 when they are first created without an assigned value.
 
 
</details>

### 5. According to Blue Prism, which of the following are considered basic data types? (Select all that apply)

- [ ] **A)** Text
- [ ] **B)** Array
- [ ] **C)** Date
- [ ] **D)** Object

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Blue Prism's basic data types are Text, Number, Date, Time, DateTime, Flag, Password, and Image. Array and Object are not part of the eight basic types.
 
 
</details>

### 6. Refer to the JSON code block. Which key-value pair indicates a successful HTTP response according to the playbook?

```json
{
  "status": 200,
  "body": "OK"
}
```

- [ ] **A)** status: 200
- [ ] **B)** body: OK
- [ ] **C)** Both
- [ ] **D)** None

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A status code of 200 indicates a successful HTTP response, as per standard HTTP semantics.
 
 
</details>

### 7. Which Blue Prism VBO should be used to integrate with a SOAP web service that requires custom SOAP headers?

- [ ] **A)** Web API VBO
- [ ] **B)** HTTP VBO
- [ ] **C)** SMTP VBO
- [ ] **D)** Utility - JSON

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The HTTP VBO is recommended for SOAP because it allows setting custom headers and methods, unlike the Web API VBO which is REST-focused.
 
 
</details>

### 8. Which of the following are true about environment variables in Blue Prism? (Select all that apply)

- [ ] **A)** They persist across sessions.
- [ ] **B)** They can be modified at runtime.
- [ ] **C)** They are encrypted for Password type.
- [ ] **D)** They are session-specific.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Environment variables are global and persistent across sessions. They cannot be modified at runtime, and only the Password type provides encryption and masking.
 
 
</details>

### 9. Refer to the code block showing the Get Credential action outputs. Which of the following are outputs of the Get Credential action? (Select all that apply)

```text
GetCredential('MyKey') returns: Username, Password
```

- [ ] **A)** Username
- [ ] **B)** Password
- [ ] **C)** Credential Key
- [ ] **D)** Expiry Date

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The Get Credential action in Blue Prism outputs the username (Text) and password (Secure String) stored under the given credential key.
 
 
</details>


---

### **Development Execution**

### 10. What is the primary purpose of a Business Object (BO) in Blue Prism?

- [ ] **A)** Encapsulate application interaction logic
- [ ] **B)** Orchestrate business process flow
- [ ] **C)** Manage user credentials and security
- [ ] **D)** Generate release packages for deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Business Object (BO) encapsulates the logic to interact with a specific application, separating technical implementation from business logic.
 
 
</details>

### 11. Which of the following are spy modes available in Blue Prism's Application Modeler? (Select all that apply)

- [ ] **A)** Win32
- [ ] **B)** AA (Accessibility)
- [ ] **C)** Browser (HTML/JS)
- [ ] **D)** OCR (Optical Character Recognition)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Blue Prism supports Win32, AA, and Browser spy modes. OCR is not a built-in spy mode; it is handled differently.
 
 
</details>

### 12. In the code snippet below, which variable is mandatory for most spied objects and must be initialized in the Start Up action?

```blueprism
// Start Up action initialization
Handle = LaunchApplication("App.exe");
AppState = "Running";
```

- [ ] **A)** Handle
- [ ] **B)** AppState
- [ ] **C)** RetryCounter
- [ ] **D)** SessionID

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Handle variable maintains the application session and is mandatory for spied objects. It is set during Start Up.
 
 
</details>

### 13. Which Blue Prism studio is used to create the high-level orchestration logic of an automation?

- [ ] **A)** Process Studio
- [ ] **B)** Object Studio
- [ ] **C)** Application Modeller
- [ ] **D)** Release Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Process Studio is used for high-level orchestration, including decision points, loops, and exception handling.
 
 
</details>

### 14. Which of the following are valid ways to use a Collection in Blue Prism? (Select all that apply)

- [ ] **A)** Store multiple rows of related data
- [ ] **B)** Pass data between Process and Object stages
- [ ] **C)** Hold a single text value
- [ ] **D)** Iterate over rows using a Loop stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Collections hold multiple rows of structured data, can be passed as parameters, and can be iterated via Loop stages. Single values are stored in Data Items.
 
 
</details>

### 15. In the code snippet, which design element is being used to achieve modularity within the same process?

```blueprism
// Main Process Page
Call Sub-Page: SP_ValidateCustomer
   Input: CustomerID = sCustID
   Output: IsValid = bValid
```

- [ ] **A)** Sub-Page
- [ ] **B)** Business Object (VBO)
- [ ] **C)** Process
- [ ] **D)** Action

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Sub-pages are used for internal reuse within a single process, as shown by the call to SP_ValidateCustomer.
 
 
</details>

### 16. Within a Business Object, which stage should be used to recover from an application-specific error and retry?

- [ ] **A)** Exception Stage (Recover)
- [ ] **B)** Decision Stage
- [ ] **C)** Calculation Stage
- [ ] **D)** Wait Stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Exception stage with Recover type is used to catch and handle application-specific errors within a Business Object.
 
 
</details>

### 17. Which of the following are recommended naming conventions in Blue Prism? (Select all that apply)

- [ ] **A)** Business Object name: 'SAP GUI VBO'
- [ ] **B)** Action name: 'GetCustomerData'
- [ ] **C)** Parameter name: 'Input_CustomerID'
- [ ] **D)** Process name: 'Action1'

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Blue Prism recommends descriptive names like 'SAP GUI VBO', PascalCase for actions, and clear parameter direction prefixes. Generic names like 'Action1' should be avoided.
 
 
</details>


---

### **Exception Handling and Work Queues**

### 18. In Blue Prism, which exception stage is used to raise a new exception that discards the original stack trace?

- [ ] **A)** Throw
- [ ] **B)** Rethrow
- [ ] **C)** Catch
- [ ] **D)** Resume

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Throw stage raises a new exception, discarding the original context. Rethrow preserves the original exception details. Catch intercepts exceptions, and Resume continues execution after recovery.
 
 
</details>

### 19. Which of the following are valid statuses for items in a Blue Prism Work Queue? (Select all that apply.)

- [ ] **A)** Pending
- [ ] **B)** In Progress
- [ ] **C)** Deferred
- [ ] **D)** Locked

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Work Queue items can be Pending, In Progress, Completed, Exception, Deferred, or Skipped. 'Locked' is not a valid status; the item is locked implicitly when In Progress.
 
 
</details>

### 20. Analyze the following Blue Prism process snippet. Identify the exception handling stage that is incorrectly placed or missing, and select the correct action to fix it.

```flowchart
Recover -> (link to main path) -> (link to exception path) -> Resume (outside the Recover region)
```

- [ ] **A)** The Resume stage is placed correctly.
- [ ] **B)** The Resume stage should be inside the Recover block.
- [ ] **C)** A Throw stage is missing after the Recover.
- [ ] **D)** The Recover stage should be placed after the Resume.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In Blue Prism, a Resume stage must be placed inside the Recover block (the exception-handling region). If placed outside, it results in a design-time error because Resume requires an exception block context.
 
 
</details>

### 21. In Blue Prism, what is the default dequeue order for a Work Queue if no tag filter is applied?

- [ ] **A)** FIFO (First In, First Out) based on creation date
- [ ] **B)** LIFO (Last In, First Out) based on creation date
- [ ] **C)** Priority (lowest number first)
- [ ] **D)** Random order

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Blue Prism Work Queues default to FIFO order, meaning the oldest pending item (by creation date) is dequeued first. Priority mode must be explicitly configured.
 
 
</details>


---

### **Security and Deployment**

### 22. What should be done to a user who has left the company to maintain audit records?

- [ ] **A)** Delete the user
- [ ] **B)** Disable the user
- [ ] **C)** Remove all roles
- [ ] **D)** Change the password

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Disabling the user preserves the audit trail and allows reactivation if needed. Deleting removes all trace and is irreversible, which breaks audit compliance.
 
 
</details>

### 23. Which items are NOT automatically included when exporting a process?

- [ ] **A)** Credentials
- [ ] **B)** Work Queues
- [ ] **C)** Environment Variables
- [ ] **D)** Objects

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Credentials and Work Queues are environment‑specific and are not auto‑included; they must be exported separately. Environment variables and referenced objects are automatically included when exporting a process.
 
 
</details>

### 24. Based on the query, why is this a security concern?

```sql
SELECT * FROM EncryptionKey;
```

- [ ] **A)** The Master Key should not exist in the database.
- [ ] **B)** The table name is misspelled.
- [ ] **C)** It violates encryption at rest.
- [ ] **D)** It exposes TLS certificates.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Master Key is stored in the Windows Certificate Store, not in the database. An attempt to read it from a table indicates a misunderstanding of where encryption keys reside.
 
 
</details>


---

### **Solution Design**

### 25. What is the primary purpose of a Process Definition Document (PDD) in Blue Prism?

- [ ] **A)** To store compiled code
- [ ] **B)** To bridge business requirements with automation design
- [ ] **C)** To log runtime errors
- [ ] **D)** To manage user credentials

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The PDD is the cornerstone artifact that bridges business requirements with RPA solution design, capturing process details and decision points.
 
 
</details>

### 26. Which elements are typically found in a Blue Prism Process Definition Document? (Select two.)

- [ ] **A)** Process triggers
- [ ] **B)** Compiled object code
- [ ] **C)** Exception handling rules
- [ ] **D)** Hardware serial numbers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> A PDD includes process triggers, volume forecasts, exception rules, credential usage, system interactions, and SLAs.
 
 
</details>

### 27. Examine the process flow below. Which stage type should be used to repeat an action a fixed number of times?

```plaintext
Start -> Loop (max 3) -> Action -> End Loop -> End
```

- [ ] **A)** Navigate
- [ ] **B)** Loop
- [ ] **C)** Decision
- [ ] **D)** Choice

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Loop stage repeats actions a fixed number of times or until a condition is met, ideal for count-based repetition.
 
 
</details>

### 28. What does the 'Resume' stage do after an exception is caught?

- [ ] **A)** Restarts the entire process
- [ ] **B)** Jumps to a recovery point label
- [ ] **C)** Continues from the next stage after the exception block
- [ ] **D)** Logs the exception and stops

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Resume instructs the process to continue execution at the stage immediately following the exception block.
 
 
</details>

### 29. Which of the following are valid input types for a Blue Prism Business Object? (Select two.)

- [ ] **A)** Text parameter
- [ ] **B)** Collection parameter
- [ ] **C)** Queue instance
- [ ] **D)** Control Room session

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Blue Prism Business Objects accept input parameters like Text, Number, Date, and Collection, not Control Room or queue instances.
 
 
</details>

### 30. Refer to the code snippet. Which stage handles transient network errors with limited retries?

```plaintext
Start -> Loop (max 3) -> Call WebService -> if success -> Continue Else -> Log -> LoopEnd -> Recover -> End
```

- [ ] **A)** Exception block with Resume
- [ ] **B)** Loop stage with counter
- [ ] **C)** Recover stage
- [ ] **D)** Decision stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A Loop stage with a counter and a decision to exit after max attempts is the standard way to implement bounded retry logic.
 
 
</details>

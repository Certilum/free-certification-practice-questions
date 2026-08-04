<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Blue%20Prism/Blue%20Prism%20Certified%20Solution%20Designer" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Solution Designer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Advanced Process Design](#advanced-process-design) (5 questions)
- [Security, Compliance, and Governance](#security-compliance-and-governance) (4 questions)
- [Solution Design and Architecture](#solution-design-and-architecture) (8 questions)
- [Stakeholder Management and Communication](#stakeholder-management-and-communication) (4 questions)
- [Technical Infrastructure and Deployment](#technical-infrastructure-and-deployment) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 27 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:47.557Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Advanced Process Design | 5 |
| Security, Compliance, and Governance | 4 |
| Solution Design and Architecture | 8 |
| Stakeholder Management and Communication | 4 |
| Technical Infrastructure and Deployment | 6 |

---

### **Advanced Process Design**

### 1. What is the lowest tier in a three-tier business object layer design?

- [ ] **A)** Application Layer
- [ ] **B)** Business Layer
- [ ] **C)** Object Layer
- [ ] **D)** Process Layer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Application Layer is the lowest tier, handling direct UI/API interactions and marked as Internal in Blue Prism.
 
 
</details>

### 2. Which of the following are features of Blue Prism Work Queues? (Select two)

- [ ] **A)** Persistence across sessions
- [ ] **B)** Built-in load balancing
- [ ] **C)** Single-threaded processing
- [ ] **D)** No automatic retry mechanism

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Work Queues persist data in the database and enable load balancing across robots via locking and retry.
 
 
</details>

### 3. Refer to the code block. What outcome does the Recover stage achieve in this sub-process?

```blueprism
Loop:
    Web Service Call
    Recover:
        Log Error
        Resume Loop
End Loop
```

- [ ] **A)** It logs the error and retries the web service call
- [ ] **B)** It terminates the sub-process immediately
- [ ] **C)** It skips the error and continues with the next iteration
- [ ] **D)** It throws a new exception to the parent process

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Recover stage catches the exception, logs it, and uses Resume to reattempt the web service call, implementing a retry pattern.
 
 
</details>

### 4. Which data structure improves performance when handling large datasets in Blue Prism?

- [ ] **A)** Collection
- [ ] **B)** Multiple Data Items
- [ ] **C)** Queue
- [ ] **D)** Environment Variable

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Collections reduce database round trips and allow bulk operations, significantly improving performance for large datasets.
 
 
</details>

### 5. Which of the following are Blue Prism dashboard types? (Select two)

- [ ] **A)** Process Dashboard
- [ ] **B)** Control Room Dashboard
- [ ] **C)** Resource Dashboard
- [ ] **D)** Exception Dashboard

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Process Dashboard and Control Room Dashboard are the standard real-time monitoring dashboards in Blue Prism.
 
 
</details>


---

### **Security, Compliance, and Governance**

### 6. In the context of Blue Prism's RBAC, which principle dictates that users should be granted only the permissions necessary to perform their job functions?

- [ ] **A)** Principle of Least Privilege
- [ ] **B)** Separation of Duties
- [ ] **C)** Role Inheritance
- [ ] **D)** Default Deny

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RBAC enforces the principle of least privilege, ensuring users have minimal necessary permissions for their roles, thereby reducing security and compliance risks.
 
 
</details>

### 7. Which of the following are recommended practices for ensuring data encryption in transit within a Blue Prism deployment? (Select two)

- [ ] **A)** Enabling TLS/SSL for inter-component communication
- [ ] **B)** Using SQL Server Transparent Data Encryption (TDE)
- [ ] **C)** Applying BitLocker on the database server
- [ ] **D)** Implementing HTTPS for all web service calls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Blue Prism uses TLS/SSL for component communication and recommends HTTPS for external web service integrations to secure data in transit.
 
 
</details>

### 8. Consider a Blue Prism process step that retrieves a credential using the 'Get Credential' action and stores it in a Data Item named 'CredentialValue'. What is a potential security risk if the process does not clear the 'CredentialValue' Data Item after use?

```text
Process Step: Call 'Get Credential' from 'Credential Manager' with input 'Credential Name' = 'SAP_User'. Output assigned to Data Item 'CredentialValue'.
```

- [ ] **A)** The credential remains in memory and could be exposed in a memory dump
- [ ] **B)** The process fails to retrieve the credential again
- [ ] **C)** The credential is automatically deleted after the session ends
- [ ] **D)** The credential is logged in plain text in the Process Log

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Leaving a credential in memory after use increases the risk of exposure; best practice is to overwrite or clear the Data Item immediately.
 
 
</details>

### 9. In a Blue Prism governance framework, which role is responsible for controlling the deployment of artifacts from pre-production to production environments?

- [ ] **A)** Process Controller
- [ ] **B)** Release Manager
- [ ] **C)** Solution Designer
- [ ] **D)** Operational Administrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Release Manager enforces version control and approval gates for deploying artifacts, maintaining segregation of duties.
 
 
</details>


---

### **Solution Design and Architecture**

### 10. What is the main purpose of using resource pools in Blue Prism automation?

- [ ] **A)** To reduce licensing costs
- [ ] **B)** To provide redundancy and load balancing
- [ ] **C)** To store process logs
- [ ] **D)** To manage credentials

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Resource pools group Runtime Resources to ensure redundancy and distribute workload across multiple resources.
 
 
</details>

### 11. Which two components are part of Blue Prism's tiered model?

- [ ] **A)** Interfaces
- [ ] **B)** Work Queues
- [ ] **C)** Business Objects
- [ ] **D)** Credential Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Interfaces handle communication with external systems, and Business Objects encapsulate business actions.
 
 
</details>

### 12. Based on the exception handling stages shown, which stage is used to capture an exception and allow the process to recover?

```plain
Throw Stage
Catch Stage
Recover Stage
End Stage
```

- [ ] **A)** Throw
- [ ] **B)** Catch
- [ ] **C)** Recover
- [ ] **D)** End

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Catch stage captures exceptions and can lead to recovery logic.
 
 
</details>

### 13. What is the main difference between high availability and disaster recovery in Blue Prism?

- [ ] **A)** HA focuses on data backup, DR on process recovery
- [ ] **B)** HA ensures continuous operation within a site, DR recovers from site-wide failures
- [ ] **C)** HA handles database failures, DR handles application failures
- [ ] **D)** HA is for non-production, DR for production

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> High availability maintains uptime within a data center; disaster recovery restores services after a catastrophic event.
 
 
</details>

### 14. Which two methods are recommended for secure credential management in Blue Prism integrations?

- [ ] **A)** Hardcoding credentials in process variables
- [ ] **B)** Using Credential Manager
- [ ] **C)** Storing passwords in plain text configuration files
- [ ] **D)** Using OAuth 2.0 tokens for API authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Credential Manager encrypts secrets; OAuth 2.0 provides token-based authentication for APIs.
 
 
</details>

### 15. The JSON below shows a Blue Prism work queue configuration. Which field controls the number of retry attempts for a queue item?

```json
{
  "MaxAttempts": 3,
  "RetryDelay": 60,
  "ItemsPerSecond": 5
}
```

- [ ] **A)** MaxAttempts
- [ ] **B)** RetryDelay
- [ ] **C)** ItemsPerSecond
- [ ] **D)** QueueName

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'MaxAttempts' field defines the maximum retry attempts for a work queue item.
 
 
</details>

### 16. When integrating with a legacy green-screen application, which Blue Prism interface is most appropriate?

- [ ] **A)** HTTP Interface
- [ ] **B)** Web Service Interface
- [ ] **C)** Terminal Emulator Interface
- [ ] **D)** Database Interface

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Terminal Emulator (TE) automates interactions with legacy green-screen systems.
 
 
</details>

### 17. Which two statements are true about Blue Prism exception handling patterns?

- [ ] **A)** Recovery mode should be used on every stage for maximum resilience.
- [ ] **B)** Structured exception handling uses Try-Catch-Throw stages.
- [ ] **C)** Exceptions should always be logged before recovery or rethrow.
- [ ] **D)** Retry patterns with exponential backoff are only used for business exceptions.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Blue Prism provides Try-Catch-Throw stages; logging before handling is best practice for maintainability.
 
 
</details>


---

### **Stakeholder Management and Communication**

### 18. What is the primary artifact used in Blue Prism's methodology to capture as-is and to-be process flows?

- [ ] **A)** Solution Design Document
- [ ] **B)** Process Definition Document (PDD)
- [ ] **C)** Technical Design Document
- [ ] **D)** Exception Handling Matrix

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Process Definition Document (PDD) is the central artifact in Blue Prism's methodology that captures the 'as-is' and 'to-be' process flow, including all screens, data fields, and decision logic.
 
 
</details>

### 19. Which of the following are mandatory components of a Blue Prism Solution Design Document (SDD)? (Select two)

- [ ] **A)** Version control and approvers list
- [ ] **B)** Detailed cost-benefit analysis
- [ ] **C)** Work Queue configuration
- [ ] **D)** Deployment automation script

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The SDD must include version control and work queue configuration; cost-benefit analysis belongs to the business case, and deployment scripts are not part of the SDD.
 
 
</details>

### 20. Review the following message from a Solution Designer to a business sponsor. What principle of communication is being violated?

```plaintext
We will use a work queue with a collection-based approach to handle fluctuating volumes. The queue will automatically balance load across multiple resources using a prioritized dequeuing strategy.
```

- [ ] **A)** Starting with the 'why' before the 'how'
- [ ] **B)** Using technical jargon for non-technical audience
- [ ] **C)** Failing to document the decision
- [ ] **D)** Not including a timeline

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The message uses Blue Prism terminology like 'work queue' and 'collection' without business context, which confuses non-technical stakeholders. The 'why' (business driver) should come first.
 
 
</details>

### 21. What is the first step in the formal handover procedure from design to development in Blue Prism?

- [ ] **A)** Schedule a handover meeting
- [ ] **B)** Complete design package completeness check
- [ ] **C)** Begin coding immediately
- [ ] **D)** Send the PDD via email

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The design package must be checked for completeness against a predefined checklist before any handover activities, including scheduling meetings.
 
 
</details>


---

### **Technical Infrastructure and Deployment**

### 22. What is the primary reason for maintaining separate infrastructure environments (DEV, TEST, PROD) in Blue Prism?

- [ ] **A)** To reduce licensing costs
- [ ] **B)** To prevent cross-contamination and protect production stability
- [ ] **C)** To allow developers direct access to production data
- [ ] **D)** To simplify network configuration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Isolation prevents bugs in lower environments from affecting production and ensures independent patching and resource allocation.
 
 
</details>

### 23. Which artifacts are typically NOT included when exporting a Blue Prism release for promotion? (Select two.)

- [ ] **A)** Process definitions
- [ ] **B)** Object definitions
- [ ] **C)** Credentials
- [ ] **D)** Environment variable values

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C, D**
 
> 💡  **Explanation** 
> 
> Credentials are encrypted per environment and not exported; environment variable definitions are exported but not their values.
 
 
</details>

### 24. Refer to the deployment script below. What step should be changed to follow best practices for applying a Blue Prism hotfix?

```bash
# deployment_script.sh
# Deployment order for hotfix 3.2.1
echo "Upgrading PROD environment..."
echo "Upgrading TEST environment..."
echo "Upgrading DEV environment..."

```

- [ ] **A)** Upgrade PROD first as it is most critical
- [ ] **B)** Upgrade DEV first, then TEST, then PROD
- [ ] **C)** Upgrade TEST first to validate the hotfix
- [ ] **D)** Upgrade all environments simultaneously

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The correct order is DEV → TEST → PROD to test the upgrade in isolation before applying to production.
 
 
</details>

### 25. Which authentication method requires users to re-enter credentials each time they start a new Blue Prism session?

- [ ] **A)** Active Directory integrated authentication
- [ ] **B)** SAML-based Single Sign-On
- [ ] **C)** Azure Active Directory with MFA
- [ ] **D)** OAuth 2.0 token exchange

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AD integrated authentication requires users to enter domain credentials each session; SSO via SAML uses a persistent IdP session.
 
 
</details>

### 26. Which two characteristics describe a static Blue Prism resource pool? (Select two.)

- [ ] **A)** Resources are allocated on demand via a broker
- [ ] **B)** A fixed set of pre-assigned runtime resources is used
- [ ] **C)** Scaling requires manual addition or removal of resources
- [ ] **D)** Automatic fault tolerance is provided by the broker

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Static pools have a fixed resource set and require manual scaling; dynamic pools use a broker for automatic allocation and fault tolerance.
 
 
</details>

### 27. Examine the logging configuration below. What is the likely impact on a production Blue Prism process if this setting is used?

```xml
<logging>
  <level>Full</level>
  <retention>
    <days>30</days>
  </retention>
</logging>
```

- [ ] **A)** Reduced database storage usage
- [ ] **B)** Significant increase in database write operations
- [ ] **C)** Improved process execution speed
- [ ] **D)** No change to resource utilization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Full logging writes every action to the database, causing high I/O and slower process execution, especially in production.
 
 
</details>

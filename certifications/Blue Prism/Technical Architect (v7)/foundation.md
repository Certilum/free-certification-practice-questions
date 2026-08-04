<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Blue%20Prism/SS&C%20|%20Blue%20Prism®%20Technical%20Architect%20(v7)%20Certification" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Technical Architect (v7)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Advanced Implementation and Support](#advanced-implementation-and-support) (5 questions)
- [Infrastructure and Security](#infrastructure-and-security) (6 questions)
- [Release Management and DevOps](#release-management-and-devops) (3 questions)
- [Solution Architecture](#solution-architecture) (9 questions)
- [Solution Design](#solution-design) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:50.150Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Advanced Implementation and Support | 5 |
| Infrastructure and Security | 6 |
| Release Management and DevOps | 3 |
| Solution Architecture | 9 |
| Solution Design | 7 |

---

### **Advanced Implementation and Support**

### 1. Which spying mode should be used to interact with a Java Swing application in Blue Prism?

- [ ] **A)** UI Automation
- [ ] **B)** Win32 (MSAA)
- [ ] **C)** HTML
- [ ] **D)** Accessibility

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Java Swing uses AWT/Swing controls accessible via Win32 with MSAA. UI Automation requires .NET/UWP applications.
 
 
</details>

### 2. Which of the following are valid considerations when embedding custom C# code in a Blue Prism Business Object? (Select all that apply.)

- [ ] **A)** Code must handle exceptions with try-catch blocks.
- [ ] **B)** Code can freely use System.Reflection without restrictions.
- [ ] **C)** Code should be thread-safe if called from multiple sessions.
- [ ] **D)** Code can reference any .NET assembly regardless of bitness.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Custom code must include error handling, be thread-safe, and avoid dangerous namespaces. Blue Prism runs as 32-bit, so 64-bit DLLs cannot be referenced.
 
 
</details>

### 3. Refer to the code block. What is the purpose of this custom C# code snippet?

```csharp
using System.Security.Cryptography;
using System.IO;
public static string Decrypt(string cipherText, byte[] key, byte[] iv)
{
    using (Aes aes = Aes.Create())
    {
        aes.Key = key;
        aes.IV = iv;
        ICryptoTransform decryptor = aes.CreateDecryptor();
        using (MemoryStream ms = new MemoryStream(Convert.FromBase64String(cipherText)))
        using (CryptoStream cs = new CryptoStream(ms, decryptor, CryptoStreamMode.Read))
        using (StreamReader sr = new StreamReader(cs))
            return sr.ReadToEnd();
    }
}
```

- [ ] **A)** It sends an HTTP GET request using HttpClient.
- [ ] **B)** It decrypts a string using AES algorithm.
- [ ] **C)** It reads a file from the file system.
- [ ] **D)** It creates a new Business Object.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code uses System.Security.Cryptography to perform AES decryption, a common reason to embed custom C# when native actions are insufficient.
 
 
</details>

### 4. Which Blue Prism component is used to receive incoming REST API calls from external systems?

- [ ] **A)** HTTP Utility VBO
- [ ] **B)** Web API Services
- [ ] **C)** Custom Connector Framework
- [ ] **D)** Process Studio

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Web API Services (introduced in v6+) expose REST endpoints for external systems to initiate Blue Prism processes. HTTP Utility VBO is for outbound calls.
 
 
</details>

### 5. Which of the following are valid methods for Blue Prism to integrate with external systems? (Select all that apply.)

- [ ] **A)** HTTP Utility VBO for REST/SOAP
- [ ] **B)** Web API Services for inbound calls
- [ ] **C)** Direct database connection via ODBC
- [ ] **D)** Custom C# code in Business Objects

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> Blue Prism supports all listed methods: HTTP Utility VBO, Web API Services, database queries via ODBC, and custom C# code for unique integrations.
 
 
</details>


---

### **Infrastructure and Security**

### 6. What is the primary requirement for environment isolation in Blue Prism?

- [ ] **A)** Share the same SQL Server instance
- [ ] **B)** Use separate databases for each environment
- [ ] **C)** Use a single credential store for all environments
- [ ] **D)** Allow Runtime Resources to float between environments

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Each environment must have physically or logically separate databases to ensure isolation and security.
 
 
</details>

### 7. Which of the following are encryption methods used in Blue Prism?

- [ ] **A)** AES-256 for data at rest
- [ ] **B)** TLS 1.2 for data in transit
- [ ] **C)** Base64 encoding for credentials
- [ ] **D)** MD5 hashing for audit logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Blue Prism uses AES-256 for encryption at rest and supports TLS 1.2 for secure communication.
 
 
</details>

### 8. Based on the code, which action is recommended for high fragmentation?

```sql
SELECT avg_fragmentation_in_percent FROM sys.dm_db_index_physical_stats(NULL, NULL, NULL, NULL, 'LIMITED') WHERE object_id = OBJECT_ID('BPASession');
```

- [ ] **A)** Run index rebuild
- [ ] **B)** Update statistics only
- [ ] **C)** Shrink the database
- [ ] **D)** Increase log file size

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When fragmentation >30%, index rebuild is needed; the code checks fragmentation level.
 
 
</details>

### 9. What is the first step in a Blue Prism upgrade process?

- [ ] **A)** Upgrade Runtime Resources
- [ ] **B)** Perform a full backup
- [ ] **C)** Install new license keys
- [ ] **D)** Reconfigure network settings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A full infrastructure backup, including database and configurations, is critical before any upgrade.
 
 
</details>

### 10. Which of the following are operational governance policies in Blue Prism?

- [ ] **A)** Separation of Duties
- [ ] **B)** Change and Release Management
- [ ] **C)** Automatic database shrinking
- [ ] **D)** Audit and Logging

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> SoD, change management, and audit logging are core governance policies. Database shrinking is not a governance policy.
 
 
</details>

### 11. Given the release command, which environment should receive the package next?

```powershell
bprelease import -file "MyProcess_v1.0.bprelease" -environment Test
```

- [ ] **A)** Test environment
- [ ] **B)** Production environment
- [ ] **C)** Development environment
- [ ] **D)** Pre-production environment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> After development, release packages are imported into Test for integration and user acceptance testing.
 
 
</details>


---

### **Release Management and DevOps**

### 12. Which Blue Prism tool packages artefacts from one environment and deploys them to another only if the target environment has the same Blue Prism version and existing object dependencies?

- [ ] **A)** Release Manager
- [ ] **B)** ALM API
- [ ] **C)** Environment Manager
- [ ] **D)** Work Queue Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Release Manager (RM) uses a centralized database and creates .bprelease files containing pointers to artefacts. It requires the target environment to have the same Blue Prism version and existing dependencies. External CI/CD tools via ALM API are used for more flexible rollbacks and multi-environment support.
 
 
</details>

### 13. Which of the following are limitations of Blue Prism's native versioning compared to external version control systems? (Select two.)

- [ ] **A)** It does not support branching or merging.
- [ ] **B)** It cannot track changes to work queue definitions.
- [ ] **C)** It is stored in the Blue Prism database and cannot be exported to an external system.
- [ ] **D)** It does not provide a comparison tool for reviewing changes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Blue Prism's native versioning is sequential and flat; it lacks branching, merging, and a built-in diff viewer (though an external compare tool is available). It does track object versions and can be exported via Release Manager, but it does not natively support parallel development.
 
 
</details>

### 14. Review the JSON snippet from an Environment Manager baseline export. Which setting would be considered environment-specific and should be parameterised before deployment?

```json
{
  "DatabaseConnectionString": "Server=DEVSQL01;Database=BPADB;User Id=svc_bp;Password=****;",
  "ProcessPriority": 5,
  "QueueName": "OrderProcessing",
  "LogLevel": "Info"
}
```

- [ ] **A)** DatabaseConnectionString
- [ ] **B)** ProcessPriority
- [ ] **C)** QueueName
- [ ] **D)** LogLevel

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Database connection strings differ per environment and contain sensitive information. They should be replaced with a placeholder and resolved at deployment time using a secrets manager. ProcessPriority, QueueName, and LogLevel are typically consistent across environments or non-sensitive.
 
 
</details>


---

### **Solution Architecture**

### 15. Which tier architecture is recommended for a production Blue Prism environment to isolate the database from runtime clients?

- [ ] **A)** 2-tier architecture with combined App Server and Database
- [ ] **B)** 3-tier architecture with separate Application Server, Interactive Client, and Database
- [ ] **C)** 1-tier architecture with all components on a single server
- [ ] **D)** 2-tier architecture with Interactive Client connecting directly to database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A 3-tier architecture separates the database, application server, and interactive client, ensuring that runtime components do not have direct database access, which aligns with security best practices for production environments.
 
 
</details>

### 16. Which of the following are valid authentication methods supported by Blue Prism v7? (Select all that apply)

- [ ] **A)** Active Directory (AD) authentication
- [ ] **B)** Native Blue Prism authentication
- [ ] **C)** OAuth 2.0 with external provider
- [ ] **D)** Enterprise Single Sign-On (SSO) using integrated Windows authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Blue Prism v7 supports Active Directory authentication, native (internal) authentication, and Enterprise SSO via integrated Windows authentication. OAuth 2.0 is not natively supported.
 
 
</details>

### 17. Review the following connection string configuration for a Blue Prism Runtime Resource. What is the most likely issue with this setup?

```text
Server=localhost;Port=8199;SSL=False
```

- [ ] **A)** The port 8199 is not the default for runtime connections
- [ ] **B)** The server name points to localhost, which would only work if the Application Server is on the same machine
- [ ] **C)** The encryption setting 'SSL' is invalid
- [ ] **D)** The connection string should use HTTPS instead of TCP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Using 'localhost' means the Runtime Resource will only connect to an Application Server running on the same machine. In a typical distributed architecture, the Application Server is remote, so the server name should be the FQDN or IP of the Application Server.
 
 
</details>

### 18. What is the purpose of the Blue Prism Authentication Gateway (BPAG)?

- [ ] **A)** It manages license allocation across runtime resources
- [ ] **B)** It provides single sign-on integration with enterprise directories like Active Directory
- [ ] **C)** It encrypts all communication between Blue Prism components
- [ ] **D)** It performs automated backup of the Blue Prism configuration database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> BPAG is a lightweight identity provider that integrates with Active Directory or LDAP to enable single sign-on (SSO) for Blue Prism clients, simplifying user management and supporting multi-factor authentication.
 
 
</details>

### 19. Which of the following are key considerations when designing high availability for a Blue Prism Application Server? (Select all that apply)

- [ ] **A)** Deploying multiple Application Servers behind a load balancer
- [ ] **B)** Configuring session affinity (sticky sessions) on the load balancer
- [ ] **C)** Ensuring all Application Servers connect to the same database
- [ ] **D)** Using a shared file system for application configuration files

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> For high availability, multiple stateless Application Servers are deployed behind a load balancer that does not require session affinity because session state is held in the database. All servers must connect to the same database to ensure consistency.
 
 
</details>

### 20. Look at the following RBAC excerpt. A user is a member of both 'RPA Developer' and 'RPA Controller' groups. What is the effective permission for 'Manage Credentials' if the Developer role denies it and the Controller role allows it?

```text
Role: RPA Developer
Permissions: Manage Credentials - Deny

Role: RPA Controller
Permissions: Manage Credentials - Allow
```

- [ ] **A)** Allowed, because permissions are cumulative
- [ ] **B)** Denied, because a deny permission overrides any allow
- [ ] **C)** Allowed, because the Controller role is more senior
- [ ] **D)** Denied only if the user is in the Developer group explicitly

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In Blue Prism's RBAC, deny permissions always override allow permissions. Therefore, if any role denies 'Manage Credentials', the effective permission is denied regardless of other roles.
 
 
</details>

### 21. What is the primary purpose of Resource Pools in Blue Prism?

- [ ] **A)** To group runtime resources logically for assignment to processes and environments
- [ ] **B)** To store encrypted credentials for automation processes
- [ ] **C)** To manage load balancing between Application Servers
- [ ] **D)** To isolate different versions of the Blue Prism application server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Resource Pools logically group runtime resources (bots) so they can be assigned to specific processes, schedules, or environments, enabling controlled allocation and scaling of automation capacity.
 
 
</details>

### 22. Which of the following are best practices for securing Blue Prism inter-component communication? (Select all that apply)

- [ ] **A)** Using TLS 1.2+ for all HTTPS connections
- [ ] **B)** Configuring SSL certificates on Application Servers for runtime connections
- [ ] **C)** Allowing all ports between components to simplify deployment
- [ ] **D)** Using network segmentation to place components in different security zones

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Best practices include encrypting communication with TLS 1.2+, deploying certificates for runtime connections (port 8199), and using network segmentation to isolate components. Opening all ports is not secure.
 
 
</details>

### 23. Examine the following SQL Server Always On configuration for a Blue Prism database. What potential issue does this design have for disaster recovery?

```text
Availability Group: BPAG
Replicas:
  Primary: SQL-SRV1 (synchronous commit)
  Secondary: SQL-SRV2 (synchronous commit) - local HA
  Secondary: SQL-DR (asynchronous commit) - DR site
```

- [ ] **A)** Synchronous commit between primary and DR site introduces high latency
- [ ] **B)** Asynchronous commit to the DR site may result in data loss if the primary fails
- [ ] **C)** The number of replicas exceeds Blue Prism supported limit
- [ ] **D)** The seeding mode is set to automatic, which is not supported

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Asynchronous commit to a remote DR site can cause data loss if the primary site fails before replication completes. For zero data loss, synchronous commit is needed, but that may impact performance over long distances.
 
 
</details>


---

### **Solution Design**

### 24. Which of the following best describes the purpose of a Business Object (BO) in Blue Prism?

- [ ] **A)** Orchestrate business logic and decision-making.
- [ ] **B)** Interact with a single application and expose reusable actions.
- [ ] **C)** Manage work queues and exception handling.
- [ ] **D)** Store configuration items and credentials.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A Business Object encapsulates a single application or system, providing reusable, atomic actions. Orchestration belongs to the process layer.
 
 
</details>

### 25. Which two statements are correct regarding exception handling in Blue Prism?

- [ ] **A)** A single 'Catch All' exception block is recommended for all errors.
- [ ] **B)** Exception blocks should be as narrow as possible.
- [ ] **C)** The 'Preserve' stage stops exception propagation.
- [ ] **D)** Custom exceptions can be thrown to signal business rule violations.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Best practice uses specific, narrow exception blocks; Preserve captures details but does not stop propagation. Custom exceptions are valid for business rules.
 
 
</details>

### 26. Given the following Blue Prism stage sequence inside an exception block: Recover → Preserve → Resume Next. What is the purpose of the 'Resume Next' stage?

```blueprism
Recover → Preserve → Resume Next
```

- [ ] **A)** To restart the process from the beginning.
- [ ] **B)** To continue execution from the next stage after the exception block.
- [ ] **C)** To log the exception and abort the process.
- [ ] **D)** To re-throw the exception to the parent process.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Resume Next moves execution to the stage immediately after the exception block, allowing the process to continue with the next step.
 
 
</details>

### 27. In Blue Prism, what is the primary function of a work queue in a multi-robot environment?

- [ ] **A)** Storing temporary data within a single process.
- [ ] **B)** Providing persistent storage for transaction records.
- [ ] **C)** Enabling load balancing by distributing items across robots.
- [ ] **D)** Replacing the need for exception handling.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Work queues allow multiple robots to pick and process items concurrently, balancing the load and preventing duplicate work.
 
 
</details>

### 28. Which two practices are recommended when designing reusable Business Objects?

- [ ] **A)** Embed business logic inside BO actions for efficiency.
- [ ] **B)** Expose implementation details like spy modes for flexibility.
- [ ] **C)** Keep actions atomic and focused on a single operation.
- [ ] **D)** Use input parameters to abstract environment-specific values.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C, D**
 
> 💡  **Explanation** 
> 
> Atomic actions and parameterization promote reusability. Business logic belongs in the process layer, not the BO. Spy modes should not be exposed.
 
 
</details>

### 29. Examine the Blue Prism stage: 'Mark Item as Exception' with 'Retry Attempts' set to 3. What is the effect of this property?

```blueprism
Mark Item as Exception
  Retry Attempts = 3
```

- [ ] **A)** The item will be automatically retried after 3 seconds.
- [ ] **B)** The item will be moved to a dead-letter queue after 3 attempts.
- [ ] **C)** The item will be retried up to 3 times, returning to Pending state after each failure.
- [ ] **D)** The item will be permanently removed from the queue after 3 attempts.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The 'Retry Attempts' property defines the maximum number of times the queue will automatically retry the item before it remains in Exception state.
 
 
</details>

### 30. What is the recommended location for storing credentials in a Blue Prism solution?

- [ ] **A)** Environment Variables
- [ ] **B)** Configuration Items
- [ ] **C)** Credential Manager
- [ ] **D)** Hardcoded in data items

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Credential Manager provides encrypted storage for usernames and passwords. Environment variables and hardcoding are insecure.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Blue%20Prism/Blue%20Prism%20Certified%20Installation%20Engineer%20(Version%206)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Installation Engineer (v6)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Architecture and Infrastructure Planning](#architecture-and-infrastructure-planning) (6 questions)
- [Database and Security Configuration](#database-and-security-configuration) (6 questions)
- [Installation and Configuration](#installation-and-configuration) (9 questions)
- [Post-Installation Validation and Handover](#post-installation-validation-and-handover) (3 questions)
- [Troubleshooting and Maintenance](#troubleshooting-and-maintenance) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:40.138Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Architecture and Infrastructure Planning | 6 |
| Database and Security Configuration | 6 |
| Installation and Configuration | 9 |
| Post-Installation Validation and Handover | 3 |
| Troubleshooting and Maintenance | 6 |

---

### **Architecture and Infrastructure Planning**

### 1. Which Blue Prism v6 component hosts scheduling and load balancing logic?

- [ ] **A)** Interactive Client
- [ ] **B)** Application Server
- [ ] **C)** Resource PC
- [ ] **D)** Database Server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Application Server hosts the BluePrism Server Service, which contains the Scheduler and load balancing logic.
 
 
</details>

### 2. Which of the following are required for a production Blue Prism v6 database server? (Select two)

- [ ] **A)** SQL Server Express
- [ ] **B)** .NET Framework 4.6.1
- [ ] **C)** SQL Server Standard or Enterprise
- [ ] **D)** Collation SQL_Latin1_General_CP1_CI_AS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C, D**
 
> 💡  **Explanation** 
> 
> Blue Prism v6 requires a full SQL Server edition (not Express) and the specified collation for the database.
 
 
</details>

### 3. What does the following Blue Prism connection string parameter ensure?

```text
Data Source=SQL-Cluster;Initial Catalog=BluePrismDB;Integrated Security=True;MultiSubnetFailover=True
```

- [ ] **A)** Enables fast TCP reconnection to a failover cluster with multiple subnets
- [ ] **B)** Enables data encryption between client and server
- [ ] **C)** Disables network load balancing
- [ ] **D)** Forces the connection to a single subnet only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'MultiSubnetFailover=True' parameter allows quick reconnection to a SQL Server availability group spanning multiple subnets.
 
 
</details>

### 4. What is the default port for .NET Remoting between Interactive Client and Application Server in Blue Prism v6?

- [ ] **A)** 8181
- [ ] **B)** 8199
- [ ] **C)** 1433
- [ ] **D)** 8190

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Blue Prism v6 uses .NET Remoting over TCP port 8181 by default for Interactive Client to Application Server communication.
 
 
</details>

### 5. Which statements about Resource PCs in Blue Prism v6 are true? (Select two)

- [ ] **A)** Resource PCs cache process definitions locally for offline execution
- [ ] **B)** Resource PCs fetch process definitions on demand each time they run
- [ ] **C)** Resource PCs connect directly to the database
- [ ] **D)** Resource PCs are licensed per resource

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Resource PCs do not cache definitions and are licensed per resource. They fetch definitions on demand and connect via the Application Server.
 
 
</details>

### 6. This firewall rule is required for communication between which Blue Prism components?

```text
Allow TCP 1433 from 192.168.1.10 to 192.168.1.20
```

- [ ] **A)** Application Server to Database Server
- [ ] **B)** Interactive Client to Application Server
- [ ] **C)** Resource PC to Application Server
- [ ] **D)** Database Server to Application Server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Application Server connects outbound to the SQL Server database using port 1433; firewall must allow this traffic.
 
 
</details>


---

### **Database and Security Configuration**

### 7. What is the minimum required open_cursors value for an Oracle database used with Blue Prism v6?

- [ ] **A)** 100
- [ ] **B)** 300
- [ ] **C)** 500
- [ ] **D)** 1000

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Blue Prism v6 requires open_cursors to be set to at least 300 to avoid ORA‑01000 errors. Default is often too low.
 
 
</details>

### 8. Which two tablespaces are required for a dedicated Blue Prism Oracle schema?

- [ ] **A)** BP_DATA
- [ ] **B)** BP_IDX
- [ ] **C)** SYSTEM
- [ ] **D)** TEMP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Blue Prism requires dedicated data (BP_DATA) and index (BP_IDX) tablespaces. SYSTEM or TEMP are not dedicated and violate best practices.
 
 
</details>

### 9. In the provided TNS entry, identify the missing component that would cause Blue Prism to fail to connect.

```plaintext
(DESCRIPTION=(ADDRESS=(PROTOCOL=TCP)(HOST=oracle_host)(PORT=1521)))
```

- [ ] **A)** SERVICE_NAME
- [ ] **B)** HOST
- [ ] **C)** PORT
- [ ] **D)** PROTOCOL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A service name is required for Blue Prism to identify the database. Without it, TNS cannot resolve the connection.
 
 
</details>

### 10. Which authentication mode requires Active Directory for Blue Prism v6 user login?

- [ ] **A)** Native Authentication
- [ ] **B)** AD Integrated Security
- [ ] **C)** SQL Server Authentication
- [ ] **D)** Windows Local Authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AD Integrated Security uses Windows Active Directory for authentication. Native Authentication uses Blue Prism’s internal user store.
 
 
</details>

### 11. Which two keys are part of Blue Prism’s encryption hierarchy?

- [ ] **A)** Master Key
- [ ] **B)** Instance Key
- [ ] **C)** Public Key
- [ ] **D)** DPAPI Key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The master key encrypts sensitive data; the instance key encrypts the master key for transport. Public and DPAPI are not used.
 
 
</details>

### 12. Based on the code snippet, which command correctly creates the Blue Prism Oracle user?

```sql
-- Options for creating the Blue Prism Oracle user

```

- [ ] **A)** CREATE USER BPSchema IDENTIFIED BY password DEFAULT TABLESPACE BP_DATA TEMPORARY TABLESPACE TEMP;
- [ ] **B)** CREATE USER BPSchema IDENTIFIED BY password DEFAULT TABLESPACE SYSTEM TEMPORARY TABLESPACE TEMP;
- [ ] **C)** CREATE USER BP_User IDENTIFIED BY password DEFAULT TABLESPACE BP_IDX;
- [ ] **D)** CREATE USER BPSchema IDENTIFIED BY password DEFAULT TABLESPACE BP_DATA;

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The correct command uses BP_DATA as default and TEMP as temporary. SYSTEM or missing temporary tablespace are incorrect.
 
 
</details>


---

### **Installation and Configuration**

### 13. What is the correct installation sequence for Blue Prism v6 server components?

- [ ] **A)** Application Server first, then Database, then Interactive Client
- [ ] **B)** Database first, then Application Server, then Interactive Client
- [ ] **C)** Interactive Client first, then Database, then Application Server
- [ ] **D)** Database and Application Server simultaneously

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The database must be created before the Application Server installation to configure the connection string.
 
 
</details>

### 14. Which accounts must have local administrator privileges on the Blue Prism server? (Choose two)

- [ ] **A)** Blue Prism Application Server service account
- [ ] **B)** Runtime Resource service account
- [ ] **C)** Database service account
- [ ] **D)** Interactive Client user account

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Both the Application Server and Runtime Resource service accounts need local admin rights for initial installation and debugging.
 
 
</details>

### 15. What command can be used to confirm the Blue Prism Application Server is listening on port 8181?

```batch
netstat -an | find '8181'
```

- [ ] **A)** netstat -an | find '8181'
- [ ] **B)** ping localhost
- [ ] **C)** telnet localhost 8181
- [ ] **D)** ipconfig /all

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> netstat shows listening ports; port 8181 is the default for Runtime Resource connections.
 
 
</details>

### 16. Why is a Connection Name used when configuring the Blue Prism Application Server?

- [ ] **A)** Identifies the database server instance
- [ ] **B)** Logical group identifier for runtime resources
- [ ] **C)** Username for database access
- [ ] **D)** Encryption key identifier

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Connection Name groups runtime resources; they must match to allow connection.
 
 
</details>

### 17. What are the supported database authentication modes for Blue Prism Application Server? (Choose two)

- [ ] **A)** Windows Integrated Security
- [ ] **B)** SQL Server Authentication
- [ ] **C)** Active Directory – Kerberos
- [ ] **D)** NTLM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The application server supports both Windows Integrated Security and SQL Server Authentication for database connectivity.
 
 
</details>

### 18. Complete the command to set the connection name: BluePrism.DatabaseConfigurator.exe /server:SQLHOST /database:BluePrism /dbuser:sa /dbpassword:xxx /connectionname:?

```batch
BluePrism.DatabaseConfigurator.exe /server:SQLHOST /database:BluePrism /dbuser:sa /dbpassword:xxx /connectionname:Production
```

- [ ] **A)** /connectionname
- [ ] **B)** /connname
- [ ] **C)** /groupname
- [ ] **D)** /resourcename

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The correct parameter is /connectionname, which sets the logical group for runtime resources.
 
 
</details>

### 19. Which TCP port does Blue Prism use for standard LDAP communication with Active Directory?

- [ ] **A)** 389
- [ ] **B)** 636
- [ ] **C)** 3268
- [ ] **D)** 443

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> LDAP default port is 389; port 636 is for LDAPS, and 3268 is for Global Catalog.
 
 
</details>

### 20. What are the required rights for the AD service account used by Blue Prism? (Choose two)

- [ ] **A)** Read on user objects
- [ ] **B)** Read tokenGroupsGlobalAndUniversal
- [ ] **C)** Domain Admin
- [ ] **D)** Account Operator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The account needs read access to user objects and the tokenGroupsGlobalAndUniversal attribute to resolve group memberships.
 
 
</details>

### 21. Provide the correct LDAP connection string for domain controller DC01 in domain ad.example.com.

```other
LDAP://DC01.ad.example.com:389/
```

- [ ] **A)** LDAP://DC01.ad.example.com:389/
- [ ] **B)** LDAP://ad.example.com:636/
- [ ] **C)** GC://DC01.ad.example.com:3268/
- [ ] **D)** LDAP://ad.example.com/DC01

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The standard LDAP URL includes the server FQDN and port 389.
 
 
</details>


---

### **Post-Installation Validation and Handover**

### 22. What is the primary purpose of environment isolation validation in a multi-environment Blue Prism deployment?

- [ ] **A)** To confirm that each environment uses dedicated databases, service accounts, and that no cross-environment network routes exist
- [ ] **B)** To check that the Interactive Client opens without errors
- [ ] **C)** To validate that all runtime resources are running the same Blue Prism version
- [ ] **D)** To ensure the scheduler services are active in all environments

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Environment isolation validation ensures each environment has its own database, connection strings, service accounts, and that firewall rules prevent cross-environment communication. This is a key verification step to avoid data leakage and incorrect resource assignment.
 
 
</details>

### 23. Which of the following are recognized categories of validation scripts for Blue Prism installations?

- [ ] **A)** Component-level scripts that verify a single resource like a server ping or service status
- [ ] **B)** Integration-level scripts that test communication between components such as queue-to-database
- [ ] **C)** End-to-end scripts that mimic a realistic business process from login to output check
- [ ] **D)** Stress-level scripts that push the system beyond capacity until failure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The three validation script categories are: component-level (single resource), integration-level (component communication), and end-to-end (full business process). Stress testing is a separate activity not part of the standard validation script categories.
 
 
</details>

### 24. Refer to the code block. What does this SQL query verify in the Blue Prism environment?

```sql
SELECT VersionNumber FROM BPASchemaVersion;
```

- [ ] **A)** It checks that the database schema version matches the application version
- [ ] **B)** It tests network connectivity to the SQL Server
- [ ] **C)** It validates that the service account has db_datareader permissions
- [ ] **D)** It confirms that the Blue Prism scheduler is running

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query selects the schema version from the BPASchemaVersion table. Comparing this value against the Blue Prism application version is a standard way to verify that the database schema is aligned with the installed software version.
 
 
</details>


---

### **Troubleshooting and Maintenance**

### 25. What is the primary purpose of the Blue Prism Diagnostics utility?

- [ ] **A)** Test connectivity, service status, and encryption
- [ ] **B)** Edit and design new Blue Prism processes
- [ ] **C)** Manage and allocate Blue Prism licenses
- [ ] **D)** Configure database connection strings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Blue Prism Diagnostics utility performs quick health checks on connectivity, service status, and encryption. It does not handle process design, license management, or direct database configuration.
 
 
</details>

### 26. Which of the following are common causes for a Blue Prism service failing to start? (Select two.)

- [ ] **A)** Incorrect service account privileges
- [ ] **B)** Missing prerequisite .NET Framework version
- [ ] **C)** Excessive memory usage on the server
- [ ] **D)** Corrupted BluePrism.config file

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Common causes for service startup failures include misconfigured service accounts (e.g., missing 'Log on as a service' right) and a corrupted or miswritten BluePrism.config file. Missing .NET Framework would prevent installation, not just service start; excessive memory usage typically does not prevent startup.
 
 
</details>

### 27. Review the following PowerShell command:\n\nTest-NetConnection -ComputerName 'AS01' -Port 8181\n\nWhat does this command primarily test?

```powershell
Test-NetConnection -ComputerName 'AS01' -Port 8181
```

- [ ] **A)** DNS resolution of the server name
- [ ] **B)** TCP connectivity to port 8181 on the specified server
- [ ] **C)** CPU usage on the remote server
- [ ] **D)** Database connection to the Blue Prism database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Test-NetConnection command with -Port checks if the specified TCP port (here 8181, the default Blue Prism inter-service communication port) is reachable on the target server. It does not test DNS resolution alone, CPU, or database connectivity.
 
 
</details>

### 28. What is the default TCP port used for inter-service communication in Blue Prism v6?

- [ ] **A)** 1433
- [ ] **B)** 8181
- [ ] **C)** 80
- [ ] **D)** 443

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Blue Prism v6 uses TCP port 8181 by default for inter-service communication between the Application Server and Runtime Resources. Port 1433 is for SQL Server, and ports 80/443 are for HTTP/HTTPS.
 
 
</details>

### 29. Which of the following are valid actions when analyzing a stuck Blue Prism session? (Select two.)

- [ ] **A)** Check the Log Viewer for the last stage executed
- [ ] **B)** Restart the Blue Prism service on the application server
- [ ] **C)** Query the BPAProcessLog table for the session ID
- [ ] **D)** Increase the process priority to High

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> To analyse a stuck session, you should examine the Log Viewer (which shows the last stage executed) or query the BPAProcessLog table directly. Restarting the service may kill the session without revealing the cause, and increasing priority does not address a hang.
 
 
</details>

### 30. Observe the following excerpt from a Windows Event Log:\n\nLog Name: Application\nSource: Blue Prism\nEvent ID: 1003\nLevel: Error\nDescription: The Blue Prism Server license has expired.\n\nWhich event ID indicates a license expiration issue?

```text
Log Name: Application
Source: Blue Prism
Event ID: 1003
Level: Error
Description: The Blue Prism Server license has expired.
```

- [ ] **A)** 1019
- [ ] **B)** 1003
- [ ] **C)** 1004
- [ ] **D)** 1000

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Event ID 1003 from the Blue Prism source indicates a license expiration. Event IDs 1019 and 1020 relate to resource connectivity, and 1000 is a generic crash error.
 
 
</details>

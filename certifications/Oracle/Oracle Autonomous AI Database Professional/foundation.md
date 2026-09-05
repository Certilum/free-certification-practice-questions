<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Oracle%20Autonomous%20AI%20Database%20Professional.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Oracle Autonomous AI Database Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Applying Autonomous Database Serverless Architectures](#applying-autonomous-database-serverless-architectures) (5 questions)
- [Applying Select AI Capabilities](#applying-select-ai-capabilities) (2 questions)
- [Designing Unified Data Management and AI Analytics](#designing-unified-data-management-and-ai-analytics) (4 questions)
- [Implementing Autonomous Database Dedicated Deployments](#implementing-autonomous-database-dedicated-deployments) (5 questions)
- [Implementing Autonomous Database Fundamentals](#implementing-autonomous-database-fundamentals) (5 questions)
- [Implementing MCP Server Integration](#implementing-mcp-server-integration) (1 questions)
- [Managing, Monitoring, and Optimizing Performance](#managing-monitoring-and-optimizing-performance) (5 questions)
- [Understanding Migration and Data Integration](#understanding-migration-and-data-integration) (2 questions)
- [Utilizing and Analyzing Autonomous Database Tools](#utilizing-and-analyzing-autonomous-database-tools) (1 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:52.632Z |
| Domains | 9 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Applying Autonomous Database Serverless Architectures | 5 |
| Applying Select AI Capabilities | 2 |
| Designing Unified Data Management and AI Analytics | 4 |
| Implementing Autonomous Database Dedicated Deployments | 5 |
| Implementing Autonomous Database Fundamentals | 5 |
| Implementing MCP Server Integration | 1 |
| Managing, Monitoring, and Optimizing Performance | 5 |
| Understanding Migration and Data Integration | 2 |
| Utilizing and Analyzing Autonomous Database Tools | 1 |

---

### **Applying Autonomous Database Serverless Architectures**

### 1. In an Oracle Autonomous Database Serverless architecture, what does the term serverless mean for infrastructure management?

- [ ] **A)** Oracle automatically provisions, scales, and manages resources.
- [ ] **B)** Customers must reserve dedicated hardware.
- [ ] **C)** Only storage resources are managed automatically.
- [ ] **D)** The database is limited to short-lived environments.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Serverless architecture means Oracle automatically handles the complete infrastructure provisioning, scaling, and management for Autonomous Database.
 
 
</details>

### 2. Based on Autonomous Database fundamentals, which workload types are supported by Autonomous Database in Oracle Cloud?

- [ ] **A)** Data warehouse
- [ ] **B)** Transaction processing
- [ ] **C)** JSON database
- [ ] **D)** Object storage archive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Autonomous Database supports data warehouse, transaction processing, and JSON database workload types. Object storage archive is not a supported workload.
 
 
</details>

### 3. Review the OCI CLI command provided in the code block, then identify which database workload type is specified by the command.

```bash
oci db autonomous-database create --db-name adbsales --display-name SalesADB --cpu-core-count 2 --data-storage-size-in-tbs 1 --db-workload DW --wait-for-state AVAILABLE
```

- [ ] **A)** Data warehouse
- [ ] **B)** Transaction processing
- [ ] **C)** JSON database
- [ ] **D)** Data lake

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses the --db-workload DW option, which specifies that the provisioned Autonomous Database is a data warehouse workload.
 
 
</details>

### 4. What is a core benefit of the autoscaling capability available in Oracle Autonomous Database Serverless environments?

- [ ] **A)** Resources scale automatically without downtime.
- [ ] **B)** A new database must be created to scale.
- [ ] **C)** Storage scaling requires a maintenance window.
- [ ] **D)** CPU resources remain fixed after provisioning.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Autoscaling automatically adjusts compute resources to match workload demand while the database remains available and does not require downtime.
 
 
</details>

### 5. Which capabilities are included in the always-on security features of Oracle Autonomous Database Serverless?

- [ ] **A)** Encryption of data at rest
- [ ] **B)** Encryption of data in transit
- [ ] **C)** Oracle-managed patching
- [ ] **D)** Customer-managed firewall appliances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Autonomous Database includes automatic encryption of data at rest and in transit, and Oracle applies security patches automatically. Customer-managed firewall appliances are not included.
 
 
</details>


---

### **Applying Select AI Capabilities**

### 6. What is the primary capability of the SELECT AI feature in Oracle Autonomous Database?

- [ ] **A)** Natural language queries
- [ ] **B)** Manual schema design
- [ ] **C)** Data entry automation
- [ ] **D)** Network configuration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SELECT AI translates natural language prompts into SQL queries, allowing users to question data conversationally.
 
 
</details>

### 7. Which two tasks are considered fundamental when implementing an Oracle Autonomous Database?

- [ ] **A)** Automated provisioning
- [ ] **B)** Automatic backups
- [ ] **C)** Manual performance tuning
- [ ] **D)** Manual security patch application

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Autonomous Database automates provisioning and backups; manual tuning and patching are not required.
 
 
</details>


---

### **Designing Unified Data Management and AI Analytics**

### 8. According to the fundamentals of Oracle Autonomous Database, which phrase best describes its defining operational characteristic?

- [ ] **A)** Self-driving, self-securing, and self-repairing operations
- [ ] **B)** Manual tuning and patching by DBAs
- [ ] **C)** Requires daily human administration
- [ ] **D)** On-premises-only deployment model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Oracle Autonomous Database is self-driving, self-securing, and self-repairing, using automation to reduce ongoing manual administration.
 
 
</details>

### 9. Identify which workload types are natively supported by Oracle Autonomous Database in a unified data management environment.

- [ ] **A)** Data warehousing and analytics
- [ ] **B)** Online transaction processing
- [ ] **C)** JSON and document workloads
- [ ] **D)** Machine learning within the database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> Oracle Autonomous Database supports analytics, online transaction processing, JSON documents, and in-database machine learning for unified workloads.
 
 
</details>

### 10. Analyze the provided SQL statement. Which keyword should be added to define a column that uniquely identifies each row?

```sql
CREATE TABLE employees (
  employee_id NUMBER,
  employee_name VARCHAR2(100)
);
```

- [ ] **A)** PRIMARY KEY
- [ ] **B)** FOREIGN KEY
- [ ] **C)** NOT NULL
- [ ] **D)** DEFAULT

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A PRIMARY KEY constraint enforces uniqueness and non-null values, making it the correct way to identify each row.
 
 
</details>

### 11. In the Oracle Autonomous Database model, which administrative task is handled automatically by the system?

- [ ] **A)** Provisioning, tuning, and patching
- [ ] **B)** Writing application code
- [ ] **C)** Designing the data model
- [ ] **D)** Defining business metrics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Autonomous Database automates provisioning, scaling, tuning, and patching, reducing the need for manual DBA work.
 
 
</details>


---

### **Implementing Autonomous Database Dedicated Deployments**

### 12. What is the first infrastructure resource to provision in an Autonomous Database Dedicated deployment?

- [ ] **A)** Autonomous Exadata Infrastructure
- [ ] **B)** Autonomous Container Database
- [ ] **C)** Autonomous VM Cluster
- [ ] **D)** Autonomous Database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Autonomous Exadata Infrastructure provides the dedicated compute, storage, and networking resources on which Autonomous Container Databases and Autonomous Databases run.
 
 
</details>

### 13. Which resources are part of an Autonomous Database Dedicated deployment? Select all that apply.

- [ ] **A)** Autonomous Exadata Infrastructure
- [ ] **B)** Autonomous Container Database
- [ ] **C)** Autonomous Database
- [ ] **D)** Object Storage bucket

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Autonomous Exadata Infrastructure, Autonomous Container Database, and Autonomous Database form the core dedicated deployment stack. Object Storage is used for backups but is not part of the dedicated database stack.
 
 
</details>

### 14. Review the JSON provisioning request in the code block. Which field references the Autonomous Container Database that will host the new Autonomous Database?

```json
{
  "autonomousDatabase": {
    "autonomousContainerDatabaseId": "ocid1.autonomouscontainer.oci..example",
    "databaseName": "SALESDB",
    "cpuCoreCount": 2,
    "dataStorageSizeInTBs": 1
  }
}
```

- [ ] **A)** autonomousDatabase
- [ ] **B)** autonomousContainerDatabaseId
- [ ] **C)** databaseName
- [ ] **D)** cpuCoreCount

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The autonomousContainerDatabaseId property links the Autonomous Database to its Autonomous Container Database in a Dedicated deployment.
 
 
</details>

### 15. Which statement best describes an Autonomous Container Database in a Dedicated deployment?

- [ ] **A)** A physical Exadata rack that stores all customer databases
- [ ] **B)** A logical container that groups and manages one or more Autonomous Databases
- [ ] **C)** A shared Oracle Cloud Infrastructure service used to connect to Autonomous Databases
- [ ] **D)** A backup storage area inside an Autonomous Database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Autonomous Container Database is a logical container that groups one or more Autonomous Databases and manages lifecycle operations on the dedicated infrastructure.
 
 
</details>

### 16. Which two benefits are specific to Autonomous Database Dedicated compared with shared Autonomous Database? Select two.

- [ ] **A)** Dedicated Exadata resources are reserved for one customer.
- [ ] **B)** Maintenance can be scheduled at the Autonomous Container Database level.
- [ ] **C)** There is no customer isolation.
- [ ] **D)** The customer must apply quarterly security patches manually.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Dedicated deployment provides reserved Exadata resources and allows maintenance to be managed at the Autonomous Container Database level, while Oracle handles the underlying patching.
 
 
</details>


---

### **Implementing Autonomous Database Fundamentals**

### 17. What is the main benefit of using Oracle Autonomous Database for provisioning and operations?

- [ ] **A)** It uses automation to provision, tune, patch, and back up the database with minimal human intervention.
- [ ] **B)** It requires DBAs to manually apply quarterly patches to production databases.
- [ ] **C)** It provides only on-premises database deployment.
- [ ] **D)** It separates compute and storage but requires manual scaling.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Autonomous Database uses automation to deliver self-driving capabilities including provisioning, tuning, patching, backups, and high availability.
 
 
</details>

### 18. Which workload types can be deployed with Oracle Autonomous Database services?

- [ ] **A)** Data warehousing
- [ ] **B)** Transaction processing
- [ ] **C)** JSON document storage
- [ ] **D)** Object file system hosting

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Autonomous Database includes Autonomous Data Warehouse, Autonomous Transaction Processing, and Autonomous JSON Database workload options. Object file system hosting is not a database workload type.
 
 
</details>

### 19. Examine the OCI CLI command shown in the code block. Which Autonomous Database workload is being requested?

```bash
oci db autonomous-database create \
  --display-name FinanceDW \
  --db-name FINANCEDW \
  --db-workload DW
```

- [ ] **A)** Autonomous Data Warehouse
- [ ] **B)** Autonomous Transaction Processing
- [ ] **C)** Autonomous JSON Database
- [ ] **D)** Autonomous Database on Dedicated Exadata Infrastructure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The db-workload value DW indicates a data warehouse workload, so the command provisions Autonomous Data Warehouse.
 
 
</details>

### 20. Which task is completely automated by Oracle in an Autonomous Database environment?

- [ ] **A)** Applying database software patches
- [ ] **B)** Writing PL/SQL application code
- [ ] **C)** Defining user access policies
- [ ] **D)** Designing table partitioning strategies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Oracle automatically applies database software patches in Autonomous Database, while application code and database design remain customer responsibilities.
 
 
</details>

### 21. Which activities are automatically performed by Oracle Autonomous Database? Select all that apply.

- [ ] **A)** Backup and recovery
- [ ] **B)** Security patching
- [ ] **C)** Designing application schemas
- [ ] **D)** Installing web servers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Autonomous Database automates backups, recovery, security patching, tuning, and scaling. Application schema design and web server installation remain customer responsibilities.
 
 
</details>


---

### **Implementing MCP Server Integration**

### 22. Which of the following best describes the core operational model of Oracle Autonomous Database?

- [ ] **A)** Self-driving, self-securing, and self-repairing
- [ ] **B)** Manual DBA intervention for every maintenance task
- [ ] **C)** Static provisioning that requires downtime for scaling
- [ ] **D)** A read-only data warehouse with no automated backups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Oracle Autonomous Database relies on automation to handle routine administration, including tuning, scaling, security, and repair, reducing the need for manual DBA work.
 
 
</details>


---

### **Managing, Monitoring, and Optimizing Performance**

### 23. Which Oracle Autonomous Database console component provides real-time and historical performance monitoring, including SQL monitoring and wait-event analysis?

- [ ] **A)** Performance Hub
- [ ] **B)** SQL Developer
- [ ] **C)** Cloud Shell
- [ ] **D)** Database Configuration Assistant

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Performance Hub is the built-in performance monitoring console, providing real-time and historical data such as SQL monitoring, ASH analytics, and wait event information.
 
 
</details>

### 24. Which capabilities are included in Autonomous Database to help manage and optimize performance automatically? (Select all that apply.)

- [ ] **A)** Automatic indexing
- [ ] **B)** Auto scaling of CPU and I/O resources
- [ ] **C)** Performance Hub for diagnostics
- [ ] **D)** Manual SGA/PGA tuning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Autonomous Database automates indexing, resource scaling, and provides Performance Hub. Manual memory tuning is not required or available because memory, SGA, and PGA are automatically managed.
 
 
</details>

### 25. Look at the following SQL statement. What does the output of this command provide?

```sql
SELECT DBMS_AUTO_SQL_TUNING.REPORT_ACTIVITY() AS activity_report FROM dual;
```

- [ ] **A)** A report of automatic SQL tuning recommendations
- [ ] **B)** The real-time SQL execution plan
- [ ] **C)** A list of invalid database objects
- [ ] **D)** The current wait class histogram

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> DBMS_AUTO_SQL_TUNING.REPORT_ACTIVITY returns a report of automatic SQL tuning activities, including recommendations for SQL plan changes and profiles.
 
 
</details>

### 26. When auto scaling is enabled in Autonomous Database, which resource can be scaled automatically in response to workload demand?

- [ ] **A)** CPU and I/O
- [ ] **B)** Maximum database storage size
- [ ] **C)** Number of schemas
- [ ] **D)** Network bandwidth

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Autonomous Database auto scaling dynamically increases CPU and I/O resources as needed, while storage and network bandwidth are not part of the same scaling model.
 
 
</details>

### 27. Which of the following V$ views help monitor autonomous database performance and SQL execution? (Select all that apply.)

- [ ] **A)** V$SQL
- [ ] **B)** V$ACTIVE_SESSION_HISTORY
- [ ] **C)** DBA_HIST_SQLSTAT
- [ ] **D)** DBA_DATA_FILES

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> V$SQL, V$ACTIVE_SESSION_HISTORY, and DBA_HIST_SQLSTAT provide SQL performance and historical activity data. DBA_DATA_FILES describes datafile storage, not performance.
 
 
</details>


---

### **Understanding Migration and Data Integration**

### 28. Which Oracle tool is often used to import an existing database into Autonomous Database?

- [ ] **A)** Oracle Data Pump
- [ ] **B)** Oracle APEX
- [ ] **C)** Oracle Cloud Guard
- [ ] **D)** Oracle Analytics Cloud

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Oracle Data Pump is commonly used to export data from an existing database and import it into Oracle Autonomous Database during a migration.
 
 
</details>

### 29. Which statements correctly describe migration requirements for Oracle Autonomous Database?

- [ ] **A)** Autonomous Database connections must use a TLS wallet.
- [ ] **B)** Oracle Data Pump can be used to import schemas into Autonomous Database.
- [ ] **C)** Autonomous Database requires the DBA to perform manual quarterly patching.
- [ ] **D)** Autonomous Database connections always require a public IP and no encryption.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Autonomous Database enforces TLS for client connections, and Data Pump is a supported migration service. Manual patching is not required because Oracle manages maintenance, and public unencrypted access is not the standard connection method.
 
 
</details>


---

### **Utilizing and Analyzing Autonomous Database Tools**

### 30. Which Oracle Autonomous Database tool provides real-time and historical performance monitoring for database workloads?

- [ ] **A)** Performance Hub
- [ ] **B)** Database Configuration Assistant
- [ ] **C)** Oracle Data Pump
- [ ] **D)** Cloud Shell

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Performance Hub is the Oracle Autonomous Database tool designed for real-time and historical performance analysis.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Snowflake/Snow%20Core" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>SnowPro Core Certification</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Account Management and Data Governance](#account-management-data-governance) (6 questions)
- [Data Collaboration](#data-collaboration) (3 questions)
- [Data Loading, Unloading and Connectivity](#data-loading-unloading-connectivity) (6 questions)
- [Performance Optimization, Querying and Transformation](#performance-optimization-querying-transformation) (6 questions)
- [Snowflake AI Data Cloud Features and Architecture](#snowflake-ai-data-cloud-features-architecture) (9 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T00:25:49.016Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Account Management & Data Governance | 6 |
| Data Collaboration | 3 |
| Data Loading, Unloading & Connectivity | 6 |
| Performance Optimization, Querying & Transformation | 6 |
| Snowflake AI Data Cloud Features & Architecture | 9 |

---

### **Account Management & Data Governance**

### 1. Which Snowflake role is the highest-level super-user role that encompasses both SYSADMIN and USERADMIN privileges?

- [ ] **A)** ACCOUNTADMIN
- [ ] **B)** SYSADMIN
- [ ] **C)** SECURITYADMIN
- [ ] **D)** USERADMIN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ACCOUNTADMIN is the top-level role that includes both SYSADMIN and USERADMIN privileges, providing full account control.
 
 
</details>

### 2. Which of the following statements about the SYSADMIN role are correct? (Select two.)

- [ ] **A)** It can create virtual warehouses.
- [ ] **B)** It can create new roles.
- [ ] **C)** It can manage users.
- [ ] **D)** It can create databases and schemas.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SYSADMIN can create warehouses, databases, and schemas, but cannot create roles or manage users; those require USERADMIN or ACCOUNTADMIN.
 
 
</details>

### 3. Review the following SQL commands. Which privilege is missing that would allow the data_engineer role to query the table?

- [ ] **A)** GRANT USAGE ON DATABASE analytics_db TO ROLE data_engineer;
- [ ] **B)** GRANT USAGE ON SCHEMA analytics_db.public TO ROLE data_engineer;
- [ ] **C)** GRANT SELECT ON ALL TABLES IN SCHEMA analytics_db.public TO ROLE data_engineer;
- [ ] **D)** GRANT CREATE TABLE ON SCHEMA analytics_db.public TO ROLE data_engineer;

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Even with USAGE on the database and SELECT on the table, the role still needs USAGE on the schema to access objects within it.
 
 
</details>

### 4. Which system-defined role has the privilege to create new users and assign roles to them?

- [ ] **A)** SYSADMIN
- [ ] **B)** USERADMIN
- [ ] **C)** PUBLIC
- [ ] **D)** ACCOUNTADMIN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> USERADMIN is specifically designed to create and manage users and roles; ACCOUNTADMIN inherits this but is not the dedicated role.
 
 
</details>

### 5. Which of the following are true about the PUBLIC role? (Select two.)

- [ ] **A)** Every user automatically has the PUBLIC role.
- [ ] **B)** Privileges granted to PUBLIC are only available to new users after the grant.
- [ ] **C)** Granting SELECT on a table to PUBLIC makes it accessible by all current users.
- [ ] **D)** PUBLIC is a system role that cannot be dropped or modified.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> All users automatically get PUBLIC, and granting privileges to PUBLIC immediately affects all current and future users.
 
 
</details>

### 6. After executing the statements below, why can user John still query the table even though his DATA_ANALYST role was revoked?

- [ ] **A)** John still has the ACCOUNTADMIN role that was never revoked.
- [ ] **B)** The SELECT privilege was also granted to the PUBLIC role.
- [ ] **C)** The revocation command failed silently because the role was not granted.
- [ ] **D)** John's default role provides the same access via another role.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> If the table's SELECT privilege was granted to PUBLIC, all users retain access regardless of individual role revocations.
 
 
</details>


---

### **Data Collaboration**

### 7. What is the key advantage of Snowflake Data Sharing compared to traditional data transfer?

- [ ] **A)** Data is copied to the consumer account.
- [ ] **B)** Real-time access without data movement.
- [ ] **C)** Requires complex ETL processes.
- [ ] **D)** Only works with Reader Accounts.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Snowflake Data Sharing provides real-time access to live data without copying or moving it, reducing storage cost and latency.
 
 
</details>

### 8. Which statements are true about Reader Accounts in Snowflake?

- [ ] **A)** They require the consumer to have a Snowflake account.
- [ ] **B)** They are lightweight accounts for data consumption only.
- [ ] **C)** The provider pays for compute costs.
- [ ] **D)** They can write data back to the provider.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Reader Accounts are fully-managed accounts for consumers without Snowflake; provider pays compute and consumers cannot write data.
 
 
</details>

### 9. What SQL command is used to create a share for data sharing?

- [ ] **A)** CREATE SHARE
- [ ] **B)** CREATE LISTING
- [ ] **C)** CREATE READER ACCOUNT
- [ ] **D)** CREATE DATABASE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CREATE SHARE command creates a share object to grant access to a set of database objects.
 
 
</details>


---

### **Data Loading, Unloading & Connectivity**

### 10. What is the primary command for bulk loading data from staged files into a Snowflake table?

- [ ] **A)** COPY INTO
- [ ] **B)** INSERT
- [ ] **C)** MERGE
- [ ] **D)** LOAD DATA

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> COPY INTO is the foundational command for bulk loading data from staged files into tables in Snowflake.
 
 
</details>

### 11. Which of the following are true about Snowpipe? (Choose two.)

- [ ] **A)** It uses serverless compute
- [ ] **B)** It requires a virtual warehouse
- [ ] **C)** It is event-driven
- [ ] **D)** It only supports internal stages

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Snowpipe uses serverless compute and is event-driven; it does not require a virtual warehouse and supports external stages.
 
 
</details>

### 12. Refer to the code block. Which file format is being used for unloading?

- [ ] **A)** CSV
- [ ] **B)** JSON
- [ ] **C)** Parquet
- [ ] **D)** Avro

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The FILE_FORMAT option TYPE=PARQUET indicates Parquet is used for unloading.
 
 
</details>

### 13. Which stage type is automatically created for every Snowflake user?

- [ ] **A)** User stage
- [ ] **B)** Table stage
- [ ] **C)** Named internal stage
- [ ] **D)** External stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Every Snowflake user automatically gets a user stage, referenced as @~.
 
 
</details>

### 14. Which two connectors are commonly used to connect BI tools to Snowflake?

- [ ] **A)** JDBC
- [ ] **B)** ODBC
- [ ] **C)** Python Connector
- [ ] **D)** Spark Connector

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> ODBC is the standard driver for BI tools; JDBC is for Java apps, not commonly directly used by BI tools.
 
 
</details>

### 15. Examine the SQL. What does the ON_ERROR option do?

- [ ] **A)** Skips the entire file
- [ ] **B)** Continues with the next row
- [ ] **C)** Aborts the statement
- [ ] **D)** Skips the file only if >10% errors

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> With ABORT_STATEMENT (default), the entire COPY operation halts on the first error.
 
 
</details>


---

### **Performance Optimization, Querying & Transformation**

### 16. What is the primary purpose of a clustering key in Snowflake?

- [ ] **A)** To improve partition pruning
- [ ] **B)** To create indexes on columns
- [ ] **C)** To enable row-level security
- [ ] **D)** To speed up data loading

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A clustering key reorganizes micro-partitions to improve partition pruning, reducing data scanned during queries.
 
 
</details>

### 17. Which two statements about materialized views are true?

- [ ] **A)** They store precomputed results
- [ ] **B)** They require a base table over 10 GB
- [ ] **C)** They support window functions
- [ ] **D)** They refresh synchronously with every DML

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Materialized views store precomputed results and require a large base table. They do not support window functions and refresh asynchronously.
 
 
</details>

### 18. Examine the SQL: which operation does this profile help diagnose?

- [ ] **A)** Data spilling during join
- [ ] **B)** Poor partition pruning
- [ ] **C)** Excessive result caching
- [ ] **D)** Too many micro-partitions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The profile shows 'Bytes Spilled' on a HashJoin operator, indicating spilling due to insufficient warehouse memory.
 
 
</details>

### 19. Which DML operation does Snowflake internally execute for an UPDATE?

- [ ] **A)** DELETE + INSERT in same transaction
- [ ] **B)** In-place modification of micro-partitions
- [ ] **C)** Row-level locking then update
- [ ] **D)** Drop and recreate the table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Snowflake never modifies micro-partitions in place; an UPDATE is a DELETE followed by an INSERT within the same transaction.
 
 
</details>

### 20. Which two features can improve performance for point-lookup queries?

- [ ] **A)** Search Optimization Service
- [ ] **B)** Clustering key on the lookup column
- [ ] **C)** Materialized view with aggregation
- [ ] **D)** Standard view

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Search Optimization Service and clustering on the lookup column both improve point-lookup performance. Materialized views are for aggregations, not point lookups.
 
 
</details>

### 21. Interpret the Query Profile metric: what does 'Partitions Scanned' indicate?

- [ ] **A)** Number of micro-partitions accessed
- [ ] **B)** Total rows returned by the query
- [ ] **C)** Credits consumed by the warehouse
- [ ] **D)** Amount of memory used

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> 'Partitions Scanned' shows how many micro-partitions were read, directly affecting performance and cost.
 
 
</details>


---

### **Snowflake AI Data Cloud Features & Architecture**

### 22. Analyze the SQL command and determine which layer is being used to store the query result for reuse.

- [ ] **A)** Storage Layer
- [ ] **B)** Compute Layer
- [ ] **C)** Cloud Services Layer
- [ ] **D)** Metadata Layer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The result cache is maintained by the Cloud Services Layer and is shared across warehouses for identical queries within 24 hours.
 
 
</details>

### 23. What is the default auto-suspend timeout for a virtual warehouse?

- [ ] **A)** 5 minutes
- [ ] **B)** 10 minutes
- [ ] **C)** 15 minutes
- [ ] **D)** 60 minutes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The default AUTO_SUSPEND setting is 10 minutes; it can be changed to as low as 1 minute.
 
 
</details>

### 24. Which two statements about multi-cluster warehouses are true? (Choose two.)

- [ ] **A)** They allow scaling out to handle many concurrent queries.
- [ ] **B)** They improve the execution speed of individual complex queries.
- [ ] **C)** They use a scaling policy that can be set to 'economy' or 'standard'.
- [ ] **D)** They automatically increase warehouse size to handle more data.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Multi-cluster warehouses add identical clusters to increase concurrency, not single-query speed. Scaling policy options include economy and standard.
 
 
</details>

### 25. Examine the scenario: A team has 50 concurrent BI users running short queries. Which warehouse configuration is most cost-effective?

- [ ] **A)** Single X-Large warehouse, auto-suspend 10 min
- [ ] **B)** Multi-cluster Small warehouse, standard scaling, auto-suspend 1 min
- [ ] **C)** Single 4X-Large warehouse, no auto-suspend
- [ ] **D)** Multi-cluster Large warehouse, economy scaling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> For many concurrent short queries, multiple small clusters provide concurrency at lower cost; standard scaling minimizes queue time.
 
 
</details>

### 26. What happens to the local SSD cache when a virtual warehouse is suspended?

- [ ] **A)** It is preserved until the warehouse is resumed.
- [ ] **B)** It is cleared and repopulated upon resume.
- [ ] **C)** It is transferred to another warehouse.
- [ ] **D)** It is stored in the Cloud Services Layer.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The local SSD cache is volatile and cleared when a warehouse is suspended. It must be rebuilt from storage on resume.
 
 
</details>

### 27. Which two are true about zero-copy cloning? (Choose two.)

- [ ] **A)** It creates a new physical copy of the data immediately.
- [ ] **B)** It shares the underlying micro-partitions until modifications occur.
- [ ] **C)** It can clone databases, schemas, and tables.
- [ ] **D)** It incurs full storage cost at the time of creation.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Zero-copy cloning creates metadata pointers to the same micro-partitions; storage is shared until either source or clone is modified.
 
 
</details>

### 28. Review the statement: 'CREATE DATABASE prod_clone CLONE prod_db;' Which architectural feature makes this operation nearly instantaneous?

- [ ] **A)** Zero-copy cloning using metadata pointers
- [ ] **B)** Parallel data copy across clusters
- [ ] **C)** Compression of data before copying
- [ ] **D)** Use of external staging area

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Zero-copy cloning leverages Snowflake metadata layer to create a new object without duplicating data, making it instantaneous.
 
 
</details>

### 29. In Snowflake data sharing, what is a Reader Account?

- [ ] **A)** A full Snowflake account with compute resources
- [ ] **B)** A lightweight, managed account that can only consume shared data
- [ ] **C)** An account that can create its own shares
- [ ] **D)** An account that stores data locally

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A Reader Account is a managed account that allows external users to query shared data without owning a Snowflake account.
 
 
</details>

### 30. Which two statements about Snowflake Time Travel are correct? (Choose two.)

- [ ] **A)** It allows users to query historical data up to 90 days.
- [ ] **B)** It is automatically enabled for all table types, including temporary tables.
- [ ] **C)** It supports UNDROP for recovering dropped objects.
- [ ] **D)** It is only available in Business Critical edition.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Time Travel retention can be set up to 90 days for permanent tables; temporary tables have no Time Travel. UNDROP is a Time Travel operation. Standard edition supports 1 day, Enterprise and above support up to 90 days.
 
 
</details>

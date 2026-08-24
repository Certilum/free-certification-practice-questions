<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Snowflake/SnowPro%20Advanced-%20Data%20Engineer.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>SnowPro Advanced: Data Engineer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Data Governance](#data-governance) (4 questions)
- [Data Movement](#data-movement) (8 questions)
- [Data Transformation](#data-transformation) (8 questions)
- [Performance Optimization](#performance-optimization) (6 questions)
- [Storage and Data Protection](#storage-and-data-protection) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:53:44.455Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Data Governance | 4 |
| Data Movement | 8 |
| Data Transformation | 8 |
| Performance Optimization | 6 |
| Storage and Data Protection | 4 |

---

### **Data Governance**

### 1. What is the primary function of a row access policy in Snowflake's data governance framework?

- [ ] **A)** Filters rows based on user context
- [ ] **B)** Masks column values dynamically
- [ ] **C)** Copies data to a new table
- [ ] **D)** Encrypts data at rest

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A row access policy is a schema-level object that conditionally filters which rows are visible based on the executing user's role or attributes.
 
 
</details>

### 2. Which statements correctly describe how Snowflake masking policies operate on sensitive data? Select two that apply.

- [ ] **A)** They are evaluated at query runtime
- [ ] **B)** They permanently alter stored data
- [ ] **C)** They can be associated with tags
- [ ] **D)** They only apply to external tables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Masking policies dynamically transform column values at query time and can be linked to tags; they do not change physical storage.
 
 
</details>

### 3. Given the following SQL masking policy definition, what does this policy do when a user queries the column?

```sql
CREATE MASKING POLICY email_mask AS (val STRING) RETURNS STRING -> CASE WHEN CURRENT_ROLE() = 'COMPLIANCE_AUDITOR' THEN val ELSE 'REDACTED' END;
```

- [ ] **A)** Unmasked only for compliance auditor
- [ ] **B)** Masked for all users
- [ ] **C)** Unmasked for all users
- [ ] **D)** Returns null for compliance auditor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy returns the original value only when the current role is COMPLIANCE_AUDITOR; all other roles see 'REDACTED'.
 
 
</details>

### 4. Which privilege is required to apply a masking policy to a column in a Snowflake table?

- [ ] **A)** APPLY MASKING POLICY
- [ ] **B)** SELECT
- [ ] **C)** CREATE TABLE
- [ ] **D)** USAGE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> To assign a masking policy, the role needs the APPLY MASKING POLICY privilege or ownership on the policy and target.
 
 
</details>


---

### **Data Movement**

### 5. What is the primary purpose of the COPY INTO command in Snowflake?

- [ ] **A)** Bulk load data from stages into tables
- [ ] **B)** Create external tables from cloud storage
- [ ] **C)** Continuously stream row-level records into Snowflake
- [ ] **D)** Purge stale data from Snowflake tables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> COPY INTO is the foundational high-performance DML for bulk loading data from internal or external stages into Snowflake tables.
 
 
</details>

### 6. Which of the following are valid internal stage types in Snowflake?

- [ ] **A)** User stage
- [ ] **B)** Table stage
- [ ] **C)** Named internal stage
- [ ] **D)** External S3 stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Internal stages include user, table, and named internal stages. External stages reference customer-managed cloud storage such as S3.
 
 
</details>

### 7. Given the provided COPY INTO SQL statement, what happens when a stage file has already been loaded successfully?

```sql
COPY INTO sales
FROM @my_stage
FILE_FORMAT = (TYPE = 'CSV' SKIP_HEADER = 1);
```

- [ ] **A)** Skip previously loaded files based on load history
- [ ] **B)** Load all files again because metadata is not checked
- [ ] **C)** Delete source files from the stage
- [ ] **D)** Abort with an error due to duplicate file names

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Snowflake's load history prevents duplicate loads; files already loaded are skipped automatically unless FORCE = TRUE is specified.
 
 
</details>

### 8. How long does Snowflake retain COPY INTO load history metadata for a target table?

- [ ] **A)** 14 days
- [ ] **B)** 64 days
- [ ] **C)** 90 days
- [ ] **D)** 365 days

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Snowflake tracks loaded files using load history metadata maintained for each target table for up to 64 days.
 
 
</details>

### 9. Which file formats are columnar and natively supported by Snowflake?

- [ ] **A)** Parquet
- [ ] **B)** ORC
- [ ] **C)** JSON
- [ ] **D)** Avro

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Parquet and ORC are columnar formats supported by Snowflake. JSON and Avro are not columnar formats.
 
 
</details>

### 10. In the provided COPY INTO command, what is the effect of ON_ERROR = 'SKIP_FILE'?

```sql
COPY INTO events
FROM @event_stage
FILE_FORMAT = (TYPE = 'JSON')
ON_ERROR = 'SKIP_FILE';
```

- [ ] **A)** Skips the malformed file and continues loading other files
- [ ] **B)** Skips invalid rows within a file and loads valid rows
- [ ] **C)** Aborts the entire statement after the first error
- [ ] **D)** Deletes files with errors from the stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ON_ERROR = 'SKIP_FILE' instructs COPY INTO to skip files that contain errors and continue loading the remaining files.
 
 
</details>

### 11. Which Snowflake service is a serverless, event-driven file-based ingestion mechanism?

- [ ] **A)** Snowpipe
- [ ] **B)** Snowpipe Streaming
- [ ] **C)** COPY INTO
- [ ] **D)** External tables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Snowpipe is the serverless, event-driven ingestion service that uses cloud notifications to load files staged in storage.
 
 
</details>

### 12. Which statements about Snowpipe Streaming are true?

- [ ] **A)** It ingests row-level records directly into Snowflake
- [ ] **B)** It bypasses the need to first write files to a stage
- [ ] **C)** It uses a client-side SDK and open channels
- [ ] **D)** It requires files to be uploaded to cloud storage before ingestion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Snowpipe Streaming pushes row-level data via an SDK directly into Snowflake and does not require staging files first.
 
 
</details>


---

### **Data Transformation**

### 13. When a window function includes an ORDER BY clause but no explicit window frame, which frame does Snowflake use by default?

- [ ] **A)** RANGE BETWEEN UNBOUNDED PRECEDING AND CURRENT ROW
- [ ] **B)** ROWS BETWEEN UNBOUNDED PRECEDING AND CURRENT ROW
- [ ] **C)** RANGE BETWEEN CURRENT ROW AND UNBOUNDED FOLLOWING
- [ ] **D)** ROWS BETWEEN UNBOUNDED PRECEDING AND UNBOUNDED FOLLOWING

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When ORDER BY is present and no explicit frame is specified, Snowflake defaults to RANGE BETWEEN UNBOUNDED PRECEDING AND CURRENT ROW, which can affect both results and performance compared with ROW-based framing.
 
 
</details>

### 14. Which metadata columns are automatically added to a tracked table by a Snowflake stream?

- [ ] **A)** METADATA$ACTION
- [ ] **B)** METADATA$ISUPDATE
- [ ] **C)** METADATA$ROW_ID
- [ ] **D)** METADATA$TIMESTAMP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Snowflake streams add METADATA$ACTION, METADATA$ISUPDATE, and METADATA$ROW_ID to the source table schema to track DML operations and row identity.
 
 
</details>

### 15. Based on the query shown, what is the running_total returned for order_id = 2?

```sql
WITH orders(order_id, amount) AS (
    VALUES (1, 100), (2, 200), (3, 300)
)
SELECT order_id, amount,
       SUM(amount) OVER (ORDER BY order_id) AS running_total
FROM orders
ORDER BY order_id;
```

- [ ] **A)** 100
- [ ] **B)** 300
- [ ] **C)** 600
- [ ] **D)** 200

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Without an explicit frame, ORDER BY uses RANGE BETWEEN UNBOUNDED PRECEDING AND CURRENT ROW, so the sum for order_id = 2 includes 100 + 200 = 300.
 
 
</details>

### 16. Which statement is true about a stale stream in Snowflake?

- [ ] **A)** A stale stream cannot be queried, and the underlying data changes are permanently lost.
- [ ] **B)** A stale stream automatically resets its offset and continues tracking changes.
- [ ] **C)** A stale stream can still be queried but cannot be consumed by a DML statement.
- [ ] **D)** A stale stream preserves all changes until the underlying table is recreated.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When a stream falls behind the Time Travel retention period of its source table, it becomes stale, cannot be queried, and the underlying data changes are permanently lost.
 
 
</details>

### 17. Which statements about append-only streams are true?

- [ ] **A)** They track only row insertions.
- [ ] **B)** They can be created on directory tables.
- [ ] **C)** They record updates and deletes.
- [ ] **D)** They offer lower overhead for insert-only ingestion pipelines.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Append-only streams track only INSERT operations, can be created on standard tables or directory tables, and provide lower overhead for write-only ingestion pipelines.
 
 
</details>

### 18. A Snowflake task DAG contains a root task and a child task. The following resumption commands are executed. Which statement is true?

```sql
ALTER TASK child_task RESUME;
ALTER TASK root_task RESUME;
```

- [ ] **A)** The resumption order is correct because child tasks must be resumed before their root task.
- [ ] **B)** The resumption order is incorrect because the root task must be resumed before the child task.
- [ ] **C)** Task resumption order does not matter in Snowflake.
- [ ] **D)** Only the root task needs to be resumed for the entire DAG to execute.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> To activate a task DAG, you must resume child tasks first and then resume the root task. The shown order follows that requirement.
 
 
</details>

### 19. What does SYSTEM$GET_PREDECESSOR_RESULT allow a task to do?

- [ ] **A)** It allows a child task to access output metadata, status flags, or small result sets from completed parent tasks.
- [ ] **B)** It returns the complete result set of every task in the account.
- [ ] **C)** It triggers a predecessor task to run again.
- [ ] **D)** It removes failed predecessor tasks from the DAG.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SYSTEM$GET_PREDECESSOR_RESULT lets downstream tasks retrieve output metadata, status flags, or small result sets from direct predecessors within the same DAG run.
 
 
</details>

### 20. Which features apply to Snowflake dynamic tables?

- [ ] **A)** They materialize the result of a SQL query.
- [ ] **B)** Snowflake automatically schedules and refreshes them based on target lag.
- [ ] **C)** They can be built on top of other dynamic tables.
- [ ] **D)** They require a manual stream and task pipeline for every refresh.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Dynamic tables persist query results, refresh automatically, and can depend on other dynamic tables, removing the need for manual stream and task orchestration.
 
 
</details>


---

### **Performance Optimization**

### 21. Which Snowflake diagnostic tool provides runtime metrics after query execution, such as spilled bytes and operator-level timing?

- [ ] **A)** EXPLAIN plan
- [ ] **B)** Query Profile
- [ ] **C)** Resource Monitor
- [ ] **D)** Metadata Cache

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Query Profile visualizes post-execution metrics including operator timing, bytes scanned, and spill to local or remote storage. EXPLAIN only provides a static execution plan without runtime telemetry.
 
 
</details>

### 22. Select the two statements that correctly describe the EXPLAIN plan in Snowflake.

- [ ] **A)** It generates the logical and optimized execution plan without consuming compute resources.
- [ ] **B)** It reports actual bytes spilled and memory usage from the last execution.
- [ ] **C)** It may include estimated cardinality and join ordering for the query.
- [ ] **D)** It replaces the Query Profile for identifying live concurrency bottlenecks.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> EXPLAIN shows logical and optimized plans, estimated cardinality, and join order without executing the query. It does not capture runtime metrics such as spilled bytes or concurrency bottlenecks.
 
 
</details>

### 23. The code block contains a metadata-only query. Which Snowflake capability resolves it from stored statistics rather than scanning micro-partitions?

```sql
SELECT COUNT(*) FROM sales;
```

- [ ] **A)** Metadata Cache
- [ ] **B)** Search Optimization Service
- [ ] **C)** Automatic Clustering
- [ ] **D)** Materialized View

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Metadata Cache stores structural, statistical, and partition-level information that allows Snowflake to resolve metadata-only operations without scanning micro-partitions or provisioning a virtual warehouse.
 
 
</details>

### 24. During query profile review, a large volume of bytes spilled to remote storage is an indicator of which condition?

- [ ] **A)** Severe memory exhaustion requiring a larger warehouse size
- [ ] **B)** A healthy execution plan with efficient memory use
- [ ] **C)** Effective partition pruning with low cluster overlap
- [ ] **D)** Successful result cache reuse

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Remote storage spills indicate intermediate results exceeded available memory, requiring more memory or compute through a larger warehouse size or query tuning.
 
 
</details>

### 25. Select the two approaches that directly relieve query queuing caused by high user concurrency.

- [ ] **A)** Enabling multi-cluster warehouses with Auto-Scale
- [ ] **B)** Configuring resource monitors to track credit usage
- [ ] **C)** Scaling the warehouse horizontally by adding clusters
- [ ] **D)** Scaling a single warehouse to a larger size

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Query queuing caused by high concurrency is solved by horizontal scaling, such as multi-cluster warehouses. Resource monitors control cost, and vertical scaling speeds individual queries but does not remove queuing.
 
 
</details>

### 26. Read the SQL statement in the code block. What does this operation create for the sales table?

```sql
ALTER TABLE sales CLUSTER BY (transaction_date, store_id);
```

- [ ] **A)** Defines a custom clustering key
- [ ] **B)** Enables the Search Optimization Service
- [ ] **C)** Creates a materialized view
- [ ] **D)** Builds a secondary index

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The SQL statement defines a custom clustering key on the specified columns. Automatic clustering then uses that key to reorder micro-partitions and minimize overlap.
 
 
</details>


---

### **Storage and Data Protection**

### 27. What is the maximum Time Travel retention period supported by Snowflake Standard Edition for permanent tables?

- [ ] **A)** 0 days
- [ ] **B)** 1 day
- [ ] **C)** 7 days
- [ ] **D)** 90 days

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Standard Edition supports a maximum of one day of Time Travel. Enterprise Edition and higher editions allow retention up to 90 days.
 
 
</details>

### 28. Which of the following statements correctly describe the Fail-safe feature in Snowflake's data protection model? Select two.

- [ ] **A)** Fixed seven days, non-configurable.
- [ ] **B)** Directly queryable by administrators.
- [ ] **C)** Available only for permanent tables.
- [ ] **D)** Starts before Time Travel expires.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Fail-safe is a fixed seven-day period applied to permanent tables. It is not accessible by SQL and does not apply to transient or temporary tables.
 
 
</details>

### 29. Review the provided SQL statement and determine the purpose of the operation being executed. Consider how the temporal clause affects the data returned.

```sql
CREATE TABLE restored_customers AS SELECT * FROM customers BEFORE(statement => '01ab23cd-ef56-7890-abcd-ef0123456789');
```

- [ ] **A)** Recreates the customers table
- [ ] **B)** Restores data after the statement
- [ ] **C)** Creates table with pre-statement data
- [ ] **D)** Drops the customers table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The BEFORE(statement =>) clause reads the table as it existed immediately before the specified statement, and CREATE TABLE AS stores that state.
 
 
</details>

### 30. When a zero-copy clone is created in Snowflake, what happens at the storage layer immediately after creation?

- [ ] **A)** Duplicates all data immediately
- [ ] **B)** Creates metadata pointers only
- [ ] **C)** Creates no object until changes
- [ ] **D)** Deletes source storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Zero-copy cloning is metadata-only. It creates a pointer to existing micro-partitions and does not duplicate physical storage until data changes.
 
 
</details>

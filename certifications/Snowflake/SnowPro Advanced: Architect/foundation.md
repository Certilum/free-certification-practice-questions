<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Snowflake/SnowPro%20Advanced-%20Architect.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>SnowPro Advanced: Architect</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Accounts and Security](#accounts-and-security) (8 questions)
- [Data Engineering](#data-engineering) (7 questions)
- [Performance Optimization](#performance-optimization) (6 questions)
- [Snowflake Architecture](#snowflake-architecture) (9 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:48:08.287Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Accounts and Security | 8 |
| Data Engineering | 7 |
| Performance Optimization | 6 |
| Snowflake Architecture | 9 |

---

### **Accounts and Security**

### 1. Which statement best describes idempotency in a data pipeline?

- [ ] **A)** Re-running the same load produces the same result without duplication.
- [ ] **B)** The pipeline can run only once and will never fail.
- [ ] **C)** The pipeline automatically scales to handle large workloads.
- [ ] **D)** Data is encrypted during transit and at rest.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Idempotency in pipelines ensures that repeated executions do not duplicate data, using techniques such as metadata tracking and staging tables.
 
 
</details>

### 2. Which two techniques are commonly used to make Snowflake pipelines idempotent?

- [ ] **A)** Using metadata tracking to record already-processed files
- [ ] **B)** Using staging tables to deduplicate before final insert
- [ ] **C)** Disabling all Tasks after a failed pipeline run
- [ ] **D)** Relying solely on random file names in external storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Metadata tracking and staging tables are recommended to ensure re-runs are idempotent; disabling tasks or using random file names does not provide consistency.
 
 
</details>

### 3. Review the SQL statement in the code block. Which Snowflake object is created and what is its main purpose?

```sql
CREATE STREAM order_changes ON TABLE orders;
```

- [ ] **A)** A stream that captures DML changes on the orders table
- [ ] **B)** A task that runs scheduled SQL every minute
- [ ] **C)** A pipe that loads files from an external stage
- [ ] **D)** A dynamic table that refreshes automatically

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CREATE STREAM creates a Snowflake Stream, which captures DML changes and supports change data capture for incremental processing.
 
 
</details>

### 4. What do Snowflake Streams provide for downstream pipelines?

- [ ] **A)** Incremental processing by capturing DML changes
- [ ] **B)** A permanent audit log of all historical transactions
- [ ] **C)** Automatic query acceleration for large scans
- [ ] **D)** Replacement for virtual warehouses

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Streams enable incremental processing by capturing DML changes, reducing the need for full table scans.
 
 
</details>

### 5. Which two Snowflake features are used for orchestration and scheduled transformation logic?

- [ ] **A)** Tasks
- [ ] **B)** Dynamic Tables
- [ ] **C)** Pipes
- [ ] **D)** Streams

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Tasks provide scheduled or conditional execution, while Dynamic Tables provide declarative continuous refresh. Pipes handle loading; Streams handle CDC.
 
 
</details>

### 6. The code block shows a scheduling object being created and enabled. What type of Snowflake object is it?

```sql
CREATE TASK hourly_task
WAREHOUSE = my_wh
SCHEDULE = '1 MINUTE'
AS INSERT INTO summary SELECT * FROM source;
ALTER TASK hourly_task RESUME;
```

- [ ] **A)** A Snowflake Task
- [ ] **B)** A Snowpipe
- [ ] **C)** A Stream
- [ ] **D)** A Dynamic Table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CREATE TASK and ALTER TASK RESUME create and enable a Snowflake Task for scheduled SQL execution.
 
 
</details>

### 7. What is required to enable automated Snowpipe ingestion from cloud storage?

- [ ] **A)** A cloud messaging service such as SQS or Event Grid
- [ ] **B)** A dedicated multi-cluster warehouse
- [ ] **C)** A Dynamic Table with a refresh schedule
- [ ] **D)** A Snowflake Task running every minute

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Automated Snowpipe requires a cloud notification service like SQS or Event Grid to signal the arrival of new files.
 
 
</details>

### 8. Which two statements about Snowpipe compute are correct?

- [ ] **A)** It uses Snowflake-managed compute resources
- [ ] **B)** Its compute is billed using serverless compute credits
- [ ] **C)** It uses a user-provisioned virtual warehouse
- [ ] **D)** It requires an always-running warehouse

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Snowpipe uses Snowflake-managed serverless compute and is billed through serverless credits, not virtual warehouse billing.
 
 
</details>


---

### **Data Engineering**

### 9. What does idempotency guarantee in a data pipeline?

- [ ] **A)** Re-running the same load produces the same result without duplicate data
- [ ] **B)** The pipeline automatically retries failed tasks every second
- [ ] **C)** Snowpipe uses the customer-provisioned virtual warehouse
- [ ] **D)** All semi-structured data is flattened immediately upon ingestion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Idempotency ensures that re-running a load yields the same final state without duplication, typically using metadata tracking or staging tables.
 
 
</details>

### 10. Which statements about Snowflake Streams for Change Data Capture are true?

- [ ] **A)** They capture DML changes on tables or views
- [ ] **B)** They enable incremental processing and reduce compute overhead
- [ ] **C)** They are consumed when read by a downstream DML operation
- [ ] **D)** They provide a permanent, exhaustive log of every change forever

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Streams capture changes, allow incremental processing, and are consumed upon use; they are not permanent logs.
 
 
</details>

### 11. The SQL statement shown is used to accomplish which task?

```sql
SELECT SYSTEM$PIPE_STATUS('DB.SCHEMA.PIPE');
```

- [ ] **A)** Monitor the status of a pipe and detect errors
- [ ] **B)** Create a new pipe object
- [ ] **C)** Validate a COPY statement before loading
- [ ] **D)** Drop an existing pipe permanently

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SYSTEM$PIPE_STATUS returns metadata about a pipe, enabling architects to monitor its state and identify ingestion problems.
 
 
</details>

### 12. How is Snowpipe compute usage billed?

- [ ] **A)** Serverless compute credits
- [ ] **B)** Virtual warehouse credits
- [ ] **C)** Storage credits
- [ ] **D)** Data transfer credits

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Snowpipe uses Snowflake-managed compute and is billed through serverless compute credits, not customer virtual warehouses.
 
 
</details>

### 13. Which of the following are recognized traps when using Snowpipe for ingestion?

- [ ] **A)** Assuming Snowpipe uses the user's virtual warehouse
- [ ] **B)** Overlooking the need for a cloud messaging service such as SQS or Event Grid
- [ ] **C)** Using Snowpipe for massive, bulk historical migrations
- [ ] **D)** Assuming a Stream can be consumed by multiple tasks without data loss

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Snowpipe uses managed compute, requires notifications, and is not suited for multi-terabyte initial loads; Streams also have consumption limitations.
 
 
</details>

### 14. What does the SQL statement shown create?

```sql
CREATE STREAM orders_stream ON TABLE orders;
```

- [ ] **A)** A stream object that captures changes to the table
- [ ] **B)** A pipe for automatically loading external files
- [ ] **C)** A task with a scheduled execution
- [ ] **D)** A dynamic table that refreshes continuously

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CREATE STREAM creates a stream object that records DML changes on the specified table for incremental processing.
 
 
</details>

### 15. What is a key characteristic of Dynamic Tables in Snowflake?

- [ ] **A)** They provide declarative, continuous data transformation
- [ ] **B)** They require procedural conditional logic for each refresh
- [ ] **C)** They replace the need for Snowflake Tasks entirely
- [ ] **D)** They only work with external cloud storage stages

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Dynamic Tables use a declarative model where Snowflake manages continuous refreshes automatically, contrasting with procedural Tasks.
 
 
</details>


---

### **Performance Optimization**

### 16. In the Snowflake data loading model, which type of compute resources are used when Snowpipe executes an ingestion workload?

- [ ] **A)** Snowflake-managed serverless compute
- [ ] **B)** Customer-provisioned virtual warehouse
- [ ] **C)** Dedicated multi-cluster warehouse
- [ ] **D)** User-specified warehouse from the COPY statement

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Snowpipe ingests data using Snowflake-managed compute, not a customer virtual warehouse, and is billed through serverless credits.
 
 
</details>

### 17. To automate Snowpipe so that file arrival in a stage triggers a load, which two components must be configured?

- [ ] **A)** A cloud messaging service (SQS or Event Grid)
- [ ] **B)** A PIPE object with AUTO_INGEST enabled
- [ ] **C)** A virtual warehouse assigned to the pipe
- [ ] **D)** A scheduled task invoking the pipe

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Automated Snowpipe requires an external notification mechanism and a PIPE object; it does not use a user-provisioned warehouse or scheduled task.
 
 
</details>

### 18. The SQL defines a scheduled task that reads from a stream. What happens to the stream after the task successfully executes?

```sql
CREATE OR REPLACE TASK insert_task
  WAREHOUSE = my_wh
  SCHEDULE = '1 MINUTE'
AS
  INSERT INTO target_table SELECT * FROM my_stream;
```

- [ ] **A)** Stream offset advances and prior changes are hidden
- [ ] **B)** Remains unchanged until a SELECT reads it
- [ ] **C)** Dropped automatically
- [ ] **D)** Keeps all records for the next run

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A stream is consumed by DML operations; after the INSERT executes, the offset advances and the previous changes are no longer visible.
 
 
</details>

### 19. For files that have already been loaded by a Snowpipe, what delivery semantics does the internal metadata guarantee?

- [ ] **A)** Exactly-once delivery
- [ ] **B)** At-least-once delivery
- [ ] **C)** At-most-once with manual deduplication
- [ ] **D)** No deduplication guarantee

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Snowpipe tracks file metadata to prevent duplicate ingestion, providing exactly-once delivery for files already processed.
 
 
</details>

### 20. Which two statements are accurate when describing how Snowpipe operates and should be charged?

- [ ] **A)** It uses Snowflake-managed compute credits
- [ ] **B)** Larger micro-batches are more cost-effective
- [ ] **C)** It runs on the user's virtual warehouse
- [ ] **D)** It is ideal for multi-terabyte initial migrations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Snowpipe uses serverless compute, and aggregating files into larger micro-batches reduces cost; bulk historical migrations should use COPY INTO.
 
 
</details>

### 21. The function shown returns pipe diagnostic information. Which two fields are most useful for detecting an ingestion failure?

```sql
SELECT SYSTEM$PIPE_STATUS('db.schema.pipe');
```

- [ ] **A)** status
- [ ] **B)** lastError
- [ ] **C)** pipeName
- [ ] **D)** owner

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> In SYSTEM$PIPE_STATUS, status and lastError indicate whether the pipe is running and if an error has occurred.
 
 
</details>


---

### **Snowflake Architecture**

### 22. In Snowflake pipeline design, what does it mean for a data load to be idempotent?

- [ ] **A)** Re-running load produces same result without duplicates
- [ ] **B)** Load always scans the entire table
- [ ] **C)** Pipeline uses external orchestration only
- [ ] **D)** Pipeline never encounters failures

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Idempotency means re-running the same load yields the same target state, preventing duplicate or corrupted results.
 
 
</details>

### 23. Which two statements are true about using Snowflake Streams for change data capture in a pipeline?

- [ ] **A)** Streams capture DML changes for incremental processing
- [ ] **B)** All downstream readers consume streams automatically
- [ ] **C)** Streams reduce compute overhead versus full scans
- [ ] **D)** Streams permanently retain all change records

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Streams capture DML changes for incremental pipelines, but they are consumed by reads and are not permanent logs.
 
 
</details>

### 24. Review the PIPE object in the code block. What is its main purpose for continuous ingestion?

```sql
CREATE OR REPLACE PIPE my_pipe
  AUTO_INGEST = TRUE
  AS
  COPY INTO my_table
  FROM @my_stage
  FILE_FORMAT = (TYPE = 'CSV');
```

- [ ] **A)** Encapsulates COPY statement and integration details
- [ ] **B)** Provisions a virtual warehouse
- [ ] **C)** Creates a stream for change tracking
- [ ] **D)** Flattens semi-structured data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A PIPE object encapsulates the COPY statement, integration details, and load metadata, preventing duplicate ingestion of processed files.
 
 
</details>

### 25. Which Snowflake feature provides declarative continuous data transformation without the need for procedural task code?

- [ ] **A)** Tasks
- [ ] **B)** Streams
- [ ] **C)** Dynamic Tables
- [ ] **D)** Snowpipe

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Dynamic Tables provide declarative, set-based continuous refresh and simplify transformation pipelines compared to procedural Tasks.
 
 
</details>

### 26. Which two statements correctly compare Snowpipe and COPY INTO for data loading pipelines in Snowflake?

- [ ] **A)** Snowpipe is best for near real-time micro-batches
- [ ] **B)** COPY INTO is best for large batch loads
- [ ] **C)** Snowpipe is always cheaper than COPY INTO
- [ ] **D)** COPY INTO requires a cloud notification service

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Snowpipe is event-driven and suited for low latency micro-batches; COPY INTO is pull-based and better for large bulk loads.
 
 
</details>

### 27. The function in the code block inspects a pipe. What kind of information does it return?

```sql
SELECT SYSTEM$PIPE_STATUS('mydb.public.my_pipe');
```

- [ ] **A)** Current pipe status and pending file count
- [ ] **B)** Query execution plan details
- [ ] **C)** User login and session history
- [ ] **D)** Daily warehouse credit usage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SYSTEM$PIPE_STATUS returns pipe status and pending file counts, which helps monitor continuous ingestion overall health.
 
 
</details>

### 28. Why can multiple downstream processes fail when they share a single Snowflake Stream without branching?

- [ ] **A)** Stream automatically duplicates all changes
- [ ] **B)** One consumer consumes changes; others miss them
- [ ] **C)** Stream becomes read-only after first read
- [ ] **D)** Stream grows until manually truncated

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Streams are consumed when read; without a branching strategy, one consumer can consume changes another still needs.
 
 
</details>

### 29. Which two components are required for automated, event-driven Snowpipe ingestion from external cloud storage?

- [ ] **A)** Cloud messaging service such as SQS
- [ ] **B)** Storage notification from the cloud provider
- [ ] **C)** User-managed virtual warehouse
- [ ] **D)** Scheduled task from Snowflake

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Automated Snowpipe requires cloud storage notifications and a messaging service; it does not require a user warehouse.
 
 
</details>

### 30. The Task in the code block uses a CRON schedule. What execution time is defined?

```sql
CREATE TASK daily_load
  WAREHOUSE = my_wh
  SCHEDULE = 'USING CRON 0 2 * * *'
  AS
  INSERT INTO target SELECT * FROM source;
```

- [ ] **A)** Once every day at 2:00 AM
- [ ] **B)** Once every hour at 2 minutes past
- [ ] **C)** Every two seconds continuously
- [ ] **D)** Only on Mondays at 2:00 PM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CRON expression `0 2 * * *` schedules the task to run once every day at 02:00 AM, which is a daily schedule.
 
 
</details>

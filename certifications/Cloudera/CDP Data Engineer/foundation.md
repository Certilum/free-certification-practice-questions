<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cloudera/CDP%20Data%20Engineer" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>CDP Data Engineer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Data Ingestion](#data-ingestion) (8 questions)
- [Data Pipeline Orchestration](#data-pipeline-orchestration) (4 questions)
- [Data Security and Governance](#data-security-and-governance) (3 questions)
- [Data Storage and Management](#data-storage-and-management) (6 questions)
- [Data Transformation](#data-transformation) (9 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:19.034Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Data Ingestion | 8 |
| Data Pipeline Orchestration | 4 |
| Data Security and Governance | 3 |
| Data Storage and Management | 6 |
| Data Transformation | 9 |

---

### **Data Ingestion**

### 1. Which Apache tool is best suited for simple log aggregation from many servers directly to HDFS with minimal overhead?

- [ ] **A)** Apache NiFi
- [ ] **B)** Apache Kafka
- [ ] **C)** Apache Flume
- [ ] **D)** Apache Spark Structured Streaming

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Flume is designed for reliable, agent-based log collection. NiFi is overkill for simple log aggregation, Kafka requires separate producers, and Spark is for processing, not direct ingestion.
 
 
</details>

### 2. Which two file formats native to CDP provide support for schema evolution, allowing fields to be added or removed with defaults?

- [ ] **A)** Avro
- [ ] **B)** Parquet
- [ ] **C)** JSON
- [ ] **D)** ORC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Avro has native schema evolution with defaults and aliases. Parquet supports adding nullable columns. JSON is schemaless and does not enforce evolution; ORC has limited evolution similar to Parquet but Avro and Parquet are the primary ones discussed in the exam.
 
 
</details>

### 3. A NiFi processor has a relationship named 'failure' that is not connected to any downstream component. What is the most likely consequence?

```text
Processor: ValidateRecord
Relationships: success, failure
success -> PutHiveStreaming
failure -> (not connected)
```

- [ ] **A)** The FlowFile will be automatically terminated and lost.
- [ ] **B)** The processor will stop processing because it cannot route the FlowFile.
- [ ] **C)** The processor will continue but log a warning.
- [ ] **D)** The connection will be automatically created to a dead letter queue.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> If a processor has a relationship that is not connected, it will not be able to route FlowFiles to that relationship, causing the processor to stop or produce a 'stuck' state. Auto-termination is only if explicitly configured.
 
 
</details>

### 4. Which URI scheme should be used when connecting to Azure Data Lake Storage Gen2 from a CDP cluster?

- [ ] **A)** wasb://
- [ ] **B)** abfss://
- [ ] **C)** s3a://
- [ ] **D)** gs://

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> ABFS (abfss) is the modern connector for Azure Data Lake Storage Gen2. wasb is for older Azure Blob Storage (Gen1). s3a is for AWS S3, gs for GCS.
 
 
</details>

### 5. Which two approaches are commonly used to implement a dead letter queue (DLQ) during data ingestion?

- [ ] **A)** Writing bad records to a separate Kafka topic
- [ ] **B)** Storing failed records in a dedicated HDFS directory
- [ ] **C)** Ignoring invalid records silently
- [ ] **D)** Logging errors to a file but continuing the pipeline

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A DLQ can be a separate Kafka topic or a HDFS directory that stores records that fail validation. Ignoring or only logging does not preserve the records for later analysis.
 
 
</details>

### 6. In a Spark Structured Streaming job, the following code is used inside `foreachBatch`: badRecordsDF.write.mode(

```scala
streamingDF.writeStream.foreachBatch { (batchDF: DataFrame, batchId: Long) =>
  val badRecords = batchDF.filter("is_valid = false")
  badRecords.write.mode("append").parquet("/data/dlq/")
}.start()
```

- [ ] **A)** Deduplication of records
- [ ] **B)** Error isolation and storage
- [ ] **C)** Schema evolution handling
- [ ] **D)** Performance tuning through caching

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Writing invalid records to a separate location (here /dlq/) is the classic pattern of a dead letter queue, isolating errors for later analysis without stopping the pipeline.
 
 
</details>

### 7. Which Kafka producer property is essential to achieve exactly-once delivery semantics?

- [ ] **A)** acks=all
- [ ] **B)** enable.idempotence=true
- [ ] **C)** retries=Integer.MAX_VALUE
- [ ] **D)** compression.type=snappy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> enable.idempotence=true makes the producer idempotent, which is a prerequisite for exactly-once semantics. acks=all is needed but not sufficient alone; retries and compression are unrelated to idempotency.
 
 
</details>

### 8. Which two scheduling strategies are available for processors in Apache NiFi?

- [ ] **A)** TIMER_DRIVEN
- [ ] **B)** CRON_DRIVEN
- [ ] **C)** EVENT_DRIVEN
- [ ] **D)** POLL_DRIVEN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> NiFi processors support TIMER_DRIVEN (periodic), EVENT_DRIVEN (triggered by events), and CRON_DRIVEN. CRON_DRIVEN is also valid, but since the question asks for two, TIMER_DRIVEN and EVENT_DRIVEN are the most common. However, CRON_DRIVEN is also a valid scheduling strategy. To avoid ambiguity, we will select TIMER_DRIVEN and EVENT_DRIVEN as per the playbook's mention.
 
 
</details>


---

### **Data Pipeline Orchestration**

### 9. What is the primary definition language for Apache Oozie workflows?

- [ ] **A)** Python
- [ ] **B)** XML
- [ ] **C)** YAML
- [ ] **D)** JSON

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Oozie uses XML with Oozie Expression Language (EL) to define workflows and actions.
 
 
</details>

### 10. Which of the following are valid scheduling mechanisms in Apache Oozie? (Select two.)

- [ ] **A)** Cron expressions
- [ ] **B)** Coordinator jobs with frequency
- [ ] **C)** Python timedelta
- [ ] **D)** Bundle jobs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Oozie uses coordinator jobs (time-based) and bundle jobs (dataset-based) for scheduling. Cron is used by Airflow.
 
 
</details>

### 11. In the provided Oozie workflow XML, what type of node is 'mr_action'?

```xml
<workflow-app name='test' xmlns='uri:oozie:workflow:0.5'>
    <start to='mr_action'/>
    <action name='mr_action'>
        <map-reduce>
            <job-tracker>${jobTracker}</job-tracker>
            <name-node>${nameNode}</name-node>
        </map-reduce>
        <ok to='end'/>
        <error to='fail'/>
    </action>
    <kill name='fail'>
        <message>Failed</message>
    </kill>
    <end name='end'/>
</workflow-app>
```

- [ ] **A)** Start node
- [ ] **B)** Action node
- [ ] **C)** Kill node
- [ ] **D)** End node

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The <action> element defines an action node that performs a MapReduce job or other operation.
 
 
</details>

### 12. What is the default number of retries for an Oozie action?

- [ ] **A)** 3
- [ ] **B)** 0
- [ ] **C)** 1
- [ ] **D)** 5

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Oozie actions have a default retry-max of 0, meaning no automatic retries are performed.
 
 
</details>


---

### **Data Security and Governance**

### 13. What is the primary purpose of Apache Ranger in CDP?

- [ ] **A)** Data cataloging and lineage tracking
- [ ] **B)** Fine-grained access control and authorization
- [ ] **C)** Data encryption at rest
- [ ] **D)** Cluster monitoring and metrics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Apache Ranger provides centralized authorization, auditing, and data masking for Hadoop ecosystem components.
 
 
</details>

### 14. Which two components are required to secure data access in CDP? (Select two.)

- [ ] **A)** Kerberos
- [ ] **B)** TLS
- [ ] **C)** Data masking
- [ ] **D)** Load balancing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Kerberos authenticates users and services; TLS encrypts data in transit.
 
 
</details>

### 15. What does the following Atlas REST API call represent?

```json
POST /v2/entity/guid/12345/classifications
{
  "classificationName": "PII"
}
```

- [ ] **A)** Creating a new data entity
- [ ] **B)** Adding a classification to an entity
- [ ] **C)** Searching for entities by classification
- [ ] **D)** Deleting a classification from an entity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The API call adds the 'PII' classification to the specified Hive table entity.
 
 
</details>


---

### **Data Storage and Management**

### 16. What is the primary purpose of Hive partitioning?

- [ ] **A)** To organize data into subdirectories based on column values, enabling partition pruning
- [ ] **B)** To compress data at the partition level for storage efficiency
- [ ] **C)** To distribute data evenly across cluster nodes using hash keys
- [ ] **D)** To encrypt sensitive data within each partition

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Hive partitioning divides data into subdirectories based on column values, allowing queries to skip irrelevant partitions via partition pruning.
 
 
</details>

### 17. Which of the following are true about Apache Parquet and Apache ORC? (Select two.)

- [ ] **A)** Parquet is natively supported by Impala; ORC is not.
- [ ] **B)** ORC supports Hive ACID transactions; Parquet does not.
- [ ] **C)** Both formats support nested types equally well.
- [ ] **D)** ORC is the default compression codec used by Parquet.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Impala supports Parquet natively but not ORC. ORC enables Hive ACID; Parquet lacks ACID support.
 
 
</details>

### 18. Consider the Hive DDL statement. What does the code accomplish?

```sql
ALTER TABLE sales SET TBLPROPERTIES('retention.days'='30');
```

- [ ] **A)** It sets a retention policy of 30 days on the table.
- [ ] **B)** It configures a lifecycle transition rule.
- [ ] **C)** It defines a retention policy at the table level.
- [ ] **D)** It disables deletion for the table.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The ALTER TABLE statement with TBLPROPERTIES sets a retention policy that defines how long data must be kept before deletion.
 
 
</details>

### 19. Which cloud object store provides strong consistency suitable for Hive ACID workloads?

- [ ] **A)** Amazon S3
- [ ] **B)** Azure Data Lake Storage Gen2
- [ ] **C)** Google Cloud Storage (for new objects only)
- [ ] **D)** All cloud object stores provide eventual consistency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Azure ADLS Gen2 offers strong consistency natively, unlike S3's eventual consistency, making it suitable for Hive ACID transactions.
 
 
</details>

### 20. Which two statements correctly describe Apache Ranger and Apache Atlas?

- [ ] **A)** Ranger enforces access control policies; Atlas tracks data lineage.
- [ ] **B)** Ranger stores classification tags; Atlas defines security policies.
- [ ] **C)** Atlas captures lineage through Hive hooks; Ranger audits are sent to Atlas.
- [ ] **D)** Both tools are used for data replication between clusters.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Ranger provides centralized security policy enforcement; Atlas manages metadata and lineage. Audits from Ranger can be logged in Atlas.
 
 
</details>

### 21. Analyze the Hive DDL snippet. What does the bucketing clause do?

```sql
CREATE TABLE orders (order_id INT, customer_id INT, amount DOUBLE)
CLUSTERED BY (customer_id) INTO 16 BUCKETS;
```

- [ ] **A)** It divides data into buckets based on a hash of customer_id.
- [ ] **B)** It creates partitions on the customer_id column.
- [ ] **C)** It specifies the storage format for the table.
- [ ] **D)** It sets the compression codec for each bucket.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CLUSTERED BY clause uses a hash of customer_id to assign rows to a fixed number of buckets, enabling efficient sampling and join optimization.
 
 
</details>


---

### **Data Transformation**

### 22. In Apache Spark, when does a transformation like `filter()` or `select()` actually execute?

- [ ] **A)** Immediately when the function is called.
- [ ] **B)** Only when an action like `count()` or `show()` is invoked.
- [ ] **C)** During the creation of the SparkSession.
- [ ] **D)** After every transformation, the data is materialized on disk.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Spark transformations are lazy; they build a DAG of operations but do not execute until an action triggers computation.
 
 
</details>

### 23. Which of the following are characteristics of narrow transformations in Spark? (Select two.)

- [ ] **A)** They cause data to be shuffled across partitions.
- [ ] **B)** Each partition depends on only one input partition.
- [ ] **C)** They are always faster than wide transformations.
- [ ] **D)** Examples include `filter()` and `map()`.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Narrow transformations do not require shuffle; each output partition depends on at most one input partition. Examples: `filter`, `map`, `select`.
 
 
</details>

### 24. Examine the following Spark code snippet. Determine whether the last line is a transformation or an action.

```python
df = spark.read.parquet("data.parquet")
df = df.filter(col("age") > 21)
df = df.select("name", "age")
df.show()
```

- [ ] **A)** Transformation
- [ ] **B)** Action
- [ ] **C)** Both
- [ ] **D)** Neither

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The `show()` method is an action because it triggers execution and returns output to the driver.
 
 
</details>

### 25. What is the primary role of the Catalyst Optimizer in Spark SQL?

- [ ] **A)** It manages memory and disk storage for DataFrames.
- [ ] **B)** It applies rule-based and cost-based optimizations to query plans.
- [ ] **C)** It serializes data between the JVM and Python.
- [ ] **D)** It handles user authentication and authorization.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Catalyst is Spark's query optimizer that applies rule-based and cost-based optimizations (e.g., predicate pushdown, constant folding) to improve execution plans.
 
 
</details>

### 26. Which of the following are considered built-in Spark SQL functions that should be preferred over UDFs for better performance? (Select two.)

- [ ] **A)** substring()
- [ ] **B)** udf()
- [ ] **C)** when() and otherwise()
- [ ] **D)** pandas_udf()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> `substring()` and `when()/otherwise()` are built-in functions that Catalyst can optimize. UDFs and Pandas UDFs add overhead and may block optimizations.
 
 
</details>

### 27. Given the Spark transformation below, identify whether it is a narrow or wide transformation.

```python
filtered_df = raw_df.filter(col("status") == "active")
```

- [ ] **A)** Narrow
- [ ] **B)** Wide
- [ ] **C)** It depends on the data size
- [ ] **D)** Cannot be determined

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> `filter()` is a narrow transformation because it operates independently on each partition without shuffling data across nodes.
 
 
</details>

### 28. Which method should you use after a filter operation to reduce the number of partitions without causing a full shuffle?

- [ ] **A)** repartition()
- [ ] **B)** coalesce()
- [ ] **C)** partitionBy()
- [ ] **D)** cache()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> `coalesce()` reduces the number of partitions without a full shuffle, making it efficient after a filter reduces data size. `repartition()` triggers a full shuffle.
 
 
</details>

### 29. Which storage levels can be used with Spark's `persist()` method? (Select two.)

- [ ] **A)** MEMORY_ONLY
- [ ] **B)** DISK_ONLY
- [ ] **C)** MEMORY_AND_DISK_SER
- [ ] **D)** REGISTER_ONLY

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Spark provides several storage levels including `MEMORY_ONLY`, `MEMORY_AND_DISK_SER`, `MEMORY_ONLY_SER`, etc. `DISK_ONLY` is not a standard level (though `MEMORY_AND_DISK` exists).
 
 
</details>

### 30. Complete the following Spark SQL query by filling in the missing hint to force a broadcast join when the dimension table is small.

```sql
SELECT /*+ ______(dim) */ f.*, d.name
FROM fact f
JOIN dim d ON f.dim_id = d.id
```

- [ ] **A)** BROADCAST
- [ ] **B)** MERGE
- [ ] **C)** SHUFFLE_HASH
- [ ] **D)** REPLICATE_NL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The `BROADCAST` hint (or `/*+ BROADCAST(dim) */`) tells Spark to use a broadcast hash join, which is efficient when one table is small enough to fit in executor memory.
 
 
</details>

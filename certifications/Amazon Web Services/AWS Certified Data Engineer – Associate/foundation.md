<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Amazon%20Web%20Services%20Training%20and%20Certification/AWS%20Certified%20Data%20Engineer%20–%20Associate" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>AWS Certified Data Engineer – Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Data Governance and Security](#data-governance-and-security) (6 questions)
- [Data Ingestion and Orchestration](#data-ingestion-and-orchestration) (8 questions)
- [Data Processing and Transformation](#data-processing-and-transformation) (8 questions)
- [Data Storage and Data Management](#data-storage-and-data-management) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:25.889Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Data Governance and Security | 6 |
| Data Ingestion and Orchestration | 8 |
| Data Processing and Transformation | 8 |
| Data Storage and Data Management | 8 |

---

### **Data Governance and Security**

### 1. What happens when an IAM policy allows s3:GetObject but the S3 bucket policy denies it?

- [ ] **A)** Allow
- [ ] **B)** Deny
- [ ] **C)** Conditionally allow
- [ ] **D)** Not evaluated

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> An explicit deny in any authorization layer overrides an allow from another layer.
 
 
</details>

### 2. Which types of fine-grained access does Lake Formation support? (Select two)

- [ ] **A)** Column-level
- [ ] **B)** Row-level
- [ ] **C)** Bucket-level
- [ ] **D)** Object-level

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Lake Formation supports column-level and row-level filtering for fine-grained access.
 
 
</details>

### 3. Refer to the bucket policy snippet. Which condition key enforces HTTPS?

```json
{
  "Condition": {
    "Bool": {
      "aws:SecureTransport": "false"
    }
  }
}
```

- [ ] **A)** aws:SecureTransport
- [ ] **B)** aws:SourceIp
- [ ] **C)** s3:x-amz-server-side-encryption
- [ ] **D)** aws:SourceVpc

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The condition key aws:SecureTransport with Bool condition enforces HTTPS.
 
 
</details>

### 4. Which S3 server-side encryption option incurs no KMS charges?

- [ ] **A)** SSE-S3
- [ ] **B)** SSE-KMS
- [ ] **C)** SSE-C
- [ ] **D)** Client-side encryption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SSE-S3 is free because S3 manages the keys without using KMS charges.
 
 
</details>

### 5. Which statements about SSE-KMS are true? (Select two)

- [ ] **A)** It uses envelope encryption
- [ ] **B)** It charges per API request
- [ ] **C)** It does not support encryption context
- [ ] **D)** It requires the client to manage keys

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SSE-KMS uses envelope encryption and incurs KMS API charges for each object operation.
 
 
</details>

### 6. Examine the IAM policy. Which action is necessary to allow Lake Formation data access?

```json
{
  "Effect": "Allow",
  "Action": "lakeformation:GetDataAccess",
  "Resource": "*"
}
```

- [ ] **A)** lakeformation:GetDataAccess
- [ ] **B)** athena:StartQueryExecution
- [ ] **C)** s3:GetObject
- [ ] **D)** kms:Decrypt

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The IAM role must have lakeformation:GetDataAccess to retrieve temporary credentials from Lake Formation.
 
 
</details>


---

### **Data Ingestion and Orchestration**

### 7. Which AWS service is primarily designed for batch ETL processing and includes a serverless Spark-based engine?

- [ ] **A)** AWS Glue
- [ ] **B)** Amazon Kinesis Data Streams
- [ ] **C)** Amazon MSK
- [ ] **D)** AWS DMS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AWS Glue is a serverless Spark-based ETL engine designed for batch processing. Kinesis Data Streams is for real-time streaming, MSK is managed Kafka, and DMS is for database migration.
 
 
</details>

### 8. Which of the following are features of Amazon Kinesis Data Streams? (Select two.)

- [ ] **A)** Data is split into shards with fixed write and read capacity.
- [ ] **B)** It automatically batches and compresses records before delivery to S3.
- [ ] **C)** Records are ordered per shard for processing.
- [ ] **D)** It is a fully managed service that requires no shard management.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Kinesis Data Streams uses shards with fixed throughput, and records are strictly ordered per shard. Automatic batching and compression are features of Kinesis Data Firehose. Shard management is required unless using On-Demand mode.
 
 
</details>

### 9. Examine the following code snippet for an AWS Glue job. What is the purpose of the `transformation_ctx` parameter used in the `create_dynamic_frame.from_catalog` call?

```python
datasource = glueContext.create_dynamic_frame.from_catalog(database = "sales_db", table_name = "orders", transformation_ctx = "datasource0")
```

- [ ] **A)** It specifies the IAM role for the job run.
- [ ] **B)** It enables job bookmarks to track processed data for incremental processing.
- [ ] **C)** It defines the output table name in the Data Catalog.
- [ ] **D)** It sets the number of Spark partitions for the DynamicFrame.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The `transformation_ctx` parameter is used by AWS Glue to uniquely identify the transformation and store bookmark state for incremental processing. It does not control IAM roles, output tables, or partition count.
 
 
</details>

### 10. Which AWS service is used to migrate databases to AWS with minimal downtime by using change data capture (CDC)?

- [ ] **A)** AWS Database Migration Service (DMS)
- [ ] **B)** AWS Glue
- [ ] **C)** Amazon Kinesis Data Firehose
- [ ] **D)** Amazon MSK

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AWS DMS is specifically designed for database migration with CDC support, allowing near-zero downtime. Glue is for ETL, Kinesis Firehose for streaming delivery, and MSK for Kafka clusters.
 
 
</details>

### 11. Which of the following are valid use cases for Amazon Kinesis Data Firehose? (Select two.)

- [ ] **A)** Delivering streaming data to Amazon S3 with near-real-time latency.
- [ ] **B)** Processing millions of events per second with sub-millisecond latency and custom consumers.
- [ ] **C)** Ingesting log data from applications and delivering it to Amazon Redshift after transformation.
- [ ] **D)** Maintaining strict record ordering across all data for downstream applications.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Firehose is ideal for near-real-time delivery to S3 and Redshift with optional Lambda transformation. Sub-millisecond latency and strict ordering are not supported; those require Kinesis Data Streams or MSK.
 
 
</details>

### 12. Given the following AWS Step Functions state machine snippet, what state type is used to run multiple branches concurrently?

```json
{
  "Comment": "Sample State Machine",
  "StartAt": "FirstTask",
  "States": {
    "FirstTask": {
      "Type": "Task",
      "Resource": "arn:aws:lambda:...",
      "Next": "Branch1"
    },
    "Branch1": {
      "Type": "Parallel",
      "Branches": [
        {
          "StartAt": "TaskA",
          "States": {
            "TaskA": { "Type": "Task", "Resource": "arn:aws:lambda:...", "End": true }
          }
        },
        {
          "StartAt": "TaskB",
          "States": {
            "TaskB": { "Type": "Task", "Resource": "arn:aws:lambda:...", "End": true }
          }
        }
      ],
      "End": true
    }
  }
}
```

- [ ] **A)** Task
- [ ] **B)** Parallel
- [ ] **C)** Map
- [ ] **D)** Choice

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The `Parallel` state in Step Functions allows multiple branches to run concurrently. `Task` is for single actions, `Map` iterates over an array, and `Choice` implements conditional branching.
 
 
</details>

### 13. What is the primary purpose of AWS Glue Workflows?

- [ ] **A)** To schedule and coordinate Glue jobs and crawlers within the Glue ecosystem.
- [ ] **B)** To manage cross-account data ingestion from streaming sources.
- [ ] **C)** To provide a serverless Spark runtime for batch processing.
- [ ] **D)** To integrate with external API endpoints for data extraction.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Glue Workflows are designed for orchestrating Glue jobs and crawlers. They do not handle streaming ingestion, serve as compute engines, or integrate with external APIs natively.
 
 
</details>

### 14. Which of the following are key features of Amazon EventBridge? (Select two.)

- [ ] **A)** Event archiving with unlimited retention and replay capability.
- [ ] **B)** Automatic schema discovery for custom events.
- [ ] **C)** Built-in support for database migration orchestration.
- [ ] **D)** Direct integration with AWS Glue as a target without Lambda mediation.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> EventBridge offers event archiving/replay and schema discovery (via Schema Registry). It does not natively orchestrate database migrations, and Glue is not a direct target; it typically requires Lambda or Step Functions as an intermediary.
 
 
</details>


---

### **Data Processing and Transformation**

### 15. Which AWS service provides a serverless Spark environment with integrated data cataloging and schema inference?

- [ ] **A)** AWS Glue
- [ ] **B)** Amazon EMR
- [ ] **C)** AWS Lambda
- [ ] **D)** Amazon Redshift Spectrum

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AWS Glue is a serverless Spark service that provides a Data Catalog and automatic schema inference, suitable for ETL jobs with minimal operational overhead.
 
 
</details>

### 16. Which of the following are capabilities of Amazon EMR for data processing? (Select TWO)

- [ ] **A)** Supports custom cluster configurations with Spark, Hive, and Presto
- [ ] **B)** Provides a serverless execution model with no cluster management
- [ ] **C)** Includes a built-in Data Catalog for schema management
- [ ] **D)** Allows use of spot instances to reduce compute costs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Amazon EMR offers full control over Hadoop components (Spark, Hive, Presto) and can use spot instances for cost savings. It is not serverless and does not include a built-in Data Catalog (Glue is separate).
 
 
</details>

### 17. You are writing an external table definition in Amazon Redshift to query data in S3. Which SQL statement is correct for this purpose?

```sql
CREATE EXTERNAL TABLE spectrum.sales (
  sale_id INT,
  amount DECIMAL(10,2)
)
ROW FORMAT SERDE 'org.apache.hadoop.hive.serde2.lazy.LazySimpleSerDe'
STORED AS TEXTFILE
LOCATION 's3://my-bucket/sales/';
```

- [ ] **A)** CREATE EXTERNAL TABLE
- [ ] **B)** CREATE TABLE AS SELECT
- [ ] **C)** CREATE MATERIALIZED VIEW
- [ ] **D)** CREATE FOREIGN TABLE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Redshift Spectrum uses CREATE EXTERNAL TABLE to define a schema for data in S3, allowing SQL queries without loading the data.
 
 
</details>

### 18. Which SQL statement does Amazon Redshift use to create a new table from a query and store the results physically?

- [ ] **A)** CREATE TABLE AS
- [ ] **B)** SELECT INTO
- [ ] **C)** CREATE VIEW AS
- [ ] **D)** INSERT INTO SELECT

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Redshift uses CREATE TABLE AS (CTAS) to create a new table and populate it with query results. SELECT INTO is not supported in Redshift.
 
 
</details>

### 19. Which of the following are required when using the SQL Query node in AWS Glue Studio? (Select TWO)

- [ ] **A)** Input sources must be registered as temporary views before the SQL node
- [ ] **B)** The SQL node can only process data from Amazon Redshift
- [ ] **C)** The SQL node uses Spark SQL syntax
- [ ] **D)** The SQL node exports results directly to a Redshift cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> In Glue Studio, before using the SQL Query node, the DynamicFrames must be registered as temporary views. The node accepts Spark SQL, not standard SQL. It does not directly write to Redshift.
 
 
</details>

### 20. You want to convert a CSV table in Amazon Athena to Parquet format with partitioning. Which statement accomplishes this?

```sql
CREATE TABLE clickstream_parquet
WITH (
  format = 'PARQUET',
  external_location = 's3://my-bucket/transformed/',
  partitioned_by = ARRAY['event_date']
)
AS SELECT * FROM clickstream_csv;
```

- [ ] **A)** CREATE TABLE parquet_table WITH (format='PARQUET', partitioned_by=ARRAY['date']) AS SELECT * FROM csv_table
- [ ] **B)** CREATE TABLE parquet_table AS SELECT * FROM csv_table FORMAT PARQUET PARTITIONED BY (date)
- [ ] **C)** ALTER TABLE csv_table SET FORMAT PARQUET PARTITIONED BY (date)
- [ ] **D)** CREATE EXTERNAL TABLE parquet_table STORED AS PARQUET PARTITIONED BY (date) AS SELECT * FROM csv_table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Athena's CTAS syntax uses WITH (format='PARQUET', partitioned_by=ARRAY['date']) to specify output format and partitioning. Other options use incorrect syntax or are not valid.
 
 
</details>

### 21. What is AWS Deequ primarily used for in data processing pipelines?

- [ ] **A)** Automating data quality checks on large datasets using Spark
- [ ] **B)** Providing a visual interface for data profiling and cleansing
- [ ] **C)** Orchestrating complex ETL workflows with state machines
- [ ] **D)** Monitoring real-time streaming data for anomalies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Deequ is an open-source library for defining and running data quality constraints on Spark DataFrames, integrated with AWS Glue. DataBrew is the visual profiling service.
 
 
</details>

### 22. Which of the following are examples of custom validation logic that complement Deequ? (Select TWO)

- [ ] **A)** Checking referential integrity across multiple tables
- [ ] **B)** Validating that a column contains only numeric values
- [ ] **C)** Detecting schema drift by comparing DataFrame schema to a canonical schema
- [ ] **D)** Ensuring a column has no missing values

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Deequ handles standard checks like completeness and data types. Cross-table referential integrity and schema drift require custom logic because they involve multiple sources or are not covered by Deequ's built-in constraints.
 
 
</details>


---

### **Data Storage and Data Management**

### 23. Which Amazon S3 storage class is best for frequently accessed data?

- [ ] **A)** S3 Standard
- [ ] **B)** S3 Glacier Deep Archive
- [ ] **C)** S3 One Zone-IA
- [ ] **D)** S3 Glacier Flexible Retrieval

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> S3 Standard provides low latency and high throughput for frequently accessed data.
 
 
</details>

### 24. Which S3 storage classes are suitable for archival data? (Select two.)

- [ ] **A)** S3 Glacier Instant Retrieval
- [ ] **B)** S3 Glacier Deep Archive
- [ ] **C)** S3 Standard-IA
- [ ] **D)** S3 One Zone-IA

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Glacier Instant Retrieval and Glacier Deep Archive are archival storage classes.
 
 
</details>

### 25. Analyze the DDL and choose the correct distribution style.

```sql
CREATE TABLE orders (order_id INT, customer_id INT, order_date DATE) DISTSTYLE KEY DISTKEY (customer_id);
```

- [ ] **A)** KEY distribution on customer_id
- [ ] **B)** EVEN distribution
- [ ] **C)** ALL distribution
- [ ] **D)** AUTO distribution

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> For large tables joined on a column, KEY distribution collocates related rows.
 
 
</details>

### 26. Which DynamoDB partition key design prevents hot partitions?

- [ ] **A)** Use high-cardinality attributes
- [ ] **B)** Use sequential numbers
- [ ] **C)** Use a single attribute only
- [ ] **D)** Use date as partition key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> High-cardinality keys distribute writes evenly across partitions, avoiding hotspots.
 
 
</details>

### 27. Which statements about Amazon Aurora are true? (Select two.)

- [ ] **A)** Supports up to 15 read replicas
- [ ] **B)** Storage auto-scales up to 128 TB
- [ ] **C)** Write instance can auto-scale vertically
- [ ] **D)** Only supports MySQL compatibility

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Aurora scales storage to 128 TB and provides up to 15 low-lag read replicas.
 
 
</details>

### 28. Examine the data sample and choose the best file format.

```json
{
  "query": "SELECT userId, SUM(amount) FROM transactions GROUP BY userId",
  "columns_used": ["userId", "amount"],
  "total_columns": 15
}
```

- [ ] **A)** Parquet
- [ ] **B)** Avro
- [ ] **C)** CSV
- [ ] **D)** JSON

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Parquet is columnar and efficient for analytical queries that select few columns.
 
 
</details>

### 29. When should you use a transient EMR cluster?

- [ ] **A)** Run a batch job and terminate
- [ ] **B)** Run interactive queries all day
- [ ] **C)** Store persistent data in HDFS
- [ ] **D)** Replace a production database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Transient clusters are cost-effective for batch ETL jobs that terminate after completion.
 
 
</details>

### 30. Which two actions can an S3 Lifecycle policy perform? (Select two.)

- [ ] **A)** Transition objects to Glacier
- [ ] **B)** Expire objects after a period
- [ ] **C)** Replicate objects across regions
- [ ] **D)** Encrypt objects at rest

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Lifecycle rules can transition storage classes and expire objects. Replication and encryption are separate features.
 
 
</details>

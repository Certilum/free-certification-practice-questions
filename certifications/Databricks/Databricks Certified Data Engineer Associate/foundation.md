<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Databricks/Databricks%20Certified%20Data%20Engineer%20Associate.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Databricks Certified Data Engineer Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Data Ingestion and Loading](#data-ingestion-and-loading) (6 questions)
- [Data Transformation and Modeling](#data-transformation-and-modeling) (6 questions)
- [Databricks Intelligence Platform](#databricks-intelligence-platform) (2 questions)
- [Governance and Security](#governance-and-security) (5 questions)
- [Implementing CI/CD](#implementing-ci-cd) (3 questions)
- [Troubleshooting, Monitoring, and Optimization](#troubleshooting-monitoring-and-optimization) (3 questions)
- [Working with Lakeflow Jobs](#working-with-lakeflow-jobs) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:26.850Z |
| Domains | 7 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Data Ingestion and Loading | 6 |
| Data Transformation and Modeling | 6 |
| Databricks Intelligence Platform | 2 |
| Governance and Security | 5 |
| Implementing CI/CD | 3 |
| Troubleshooting, Monitoring, and Optimization | 3 |
| Working with Lakeflow Jobs | 5 |

---

### **Data Ingestion and Loading**

### 1. Which cloud storage URI format is correct for Azure Data Lake Storage Gen2?

- [ ] **A)** wasbs://container@storage.blob.core.windows.net/path
- [ ] **B)** abfss://container@storage.dfs.core.windows.net/path
- [ ] **C)** azure://container@storage.dfs.core.windows.net/path
- [ ] **D)** https://storageaccount.blob.core.windows.net/path

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The correct URI for ADLS Gen2 is abfss://, which uses the Azure Blob File System driver.
 
 
</details>

### 2. Which of the following file formats are natively supported by Auto Loader?

- [ ] **A)** CSV
- [ ] **B)** Parquet
- [ ] **C)** Excel
- [ ] **D)** JSON

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Auto Loader supports CSV, Parquet, JSON, Avro, ORC, and text files. Excel is not supported natively.
 
 
</details>

### 3. Based on the provided Auto Loader code, what is the purpose of the 'cloudFiles.schemaLocation' option?

```python
spark.readStream.format("cloudFiles") \
  .option("cloudFiles.format", "csv") \
  .option("cloudFiles.schemaLocation", "/tmp/schema") \
  .load("s3://bucket/data")
```

- [ ] **A)** Specifies where ingested data is written
- [ ] **B)** Stores inferred schema for evolution
- [ ] **C)** Sets the checkpoint location for fault tolerance
- [ ] **D)** Defines the cloud storage URI

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The schemaLocation stores the inferred schema persistently, enabling schema evolution across multiple batches.
 
 
</details>

### 4. Which of the following is the recommended approach for incremental file ingestion in Databricks?

- [ ] **A)** Spark Structured Streaming
- [ ] **B)** Auto Loader (cloudFiles)
- [ ] **C)** COPY INTO
- [ ] **D)** dbutils.fs.ls()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Auto Loader (cloudFiles) is purpose-built for incremental file ingestion, handling schema evolution and exactly-once semantics.
 
 
</details>

### 5. Which of the following are valid output modes for Structured Streaming?

- [ ] **A)** append
- [ ] **B)** complete
- [ ] **C)** overwrite
- [ ] **D)** update

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Structured Streaming supports append, complete, and update output modes. Overwrite is a batch-mode option.
 
 
</details>

### 6. In the JDBC read code, if the 'id' column is of type VARCHAR, what will happen when the query is executed?

```python
df = spark.read.format("jdbc") \
  .option("url", "jdbc:mysql://host:3306/db") \
  .option("dbtable", "employees") \
  .option("numPartitions", 10) \
  .option("partitionColumn", "id") \
  .load()
```

- [ ] **A)** Runs successfully with 10 partitions
- [ ] **B)** Fails because partitionColumn must be numeric, date, or timestamp
- [ ] **C)** Ignores partitionColumn and uses single partition
- [ ] **D)** Converts VARCHAR to integer automatically

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> partitionColumn requires an integer, date, or timestamp column to split ranges; a string column causes an error.
 
 
</details>


---

### **Data Transformation and Modeling**

### 7. What is the primary purpose of the Delta transaction log?

- [ ] **A)** Store data files
- [ ] **B)** Record metadata and enable ACID transactions
- [ ] **C)** Provide schema inference
- [ ] **D)** Manage cluster resources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The transaction log records every change, enabling ACID transactions and time travel.
 
 
</details>

### 8. Which statements are true about managed Delta tables in Databricks? (Select two)

- [ ] **A)** Data is stored in a user-specified location
- [ ] **B)** Dropping the table deletes the underlying data
- [ ] **C)** They can be shared across workspaces without additional configuration
- [ ] **D)** They are created using CREATE TABLE without LOCATION

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Managed tables store data in the default DBFS location and dropping removes data. They do not specify a LOCATION.
 
 
</details>

### 9. Given a Delta table with many small files, which command should be run to improve read performance?

```sql
OPTIMIZE sales_table;
```

- [ ] **A)** VACUUM
- [ ] **B)** OPTIMIZE
- [ ] **C)** MERGE
- [ ] **D)** DESCRIBE HISTORY

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> OPTIMIZE compacts small files into larger ones, improving scan performance.
 
 
</details>

### 10. What happens when you try to write data with a mismatched schema to a Delta table?

- [ ] **A)** The write fails
- [ ] **B)** The schema is automatically evolved
- [ ] **C)** The data is stored in a separate table
- [ ] **D)** The write succeeds with nulls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Delta Lake enforces schema on write by default; mismatched columns cause failure.
 
 
</details>

### 11. Which Delta Live Tables expectation actions will drop failing rows without causing pipeline failure? (Select two)

- [ ] **A)** expect_or_fail
- [ ] **B)** expect_or_drop
- [ ] **C)** expect
- [ ] **D)** expect_all

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> expect_or_drop silently drops failing rows; expect_all applies multiple rules but does not drop on its own.
 
 
</details>

### 12. You have a Delta table queried with filters on date and region. Which column would be most effective for partitioning to improve query performance?

```sql
CREATE TABLE sales (id INT, date STRING, amount DOUBLE) USING DELTA PARTITIONED BY (date);
```

- [ ] **A)** user_id
- [ ] **B)** date
- [ ] **C)** region
- [ ] **D)** amount

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Partitioning on low-cardinality columns used in filters, like date, improves query pruning.
 
 
</details>


---

### **Databricks Intelligence Platform**

### 13. What is the primary purpose of the workspace root storage in a Databricks workspace?

- [ ] **A)** To store production data tables and analytics results
- [ ] **B)** To serve as the default location for DBFS, cluster logs, and system tables
- [ ] **C)** To host Unity Catalog metadata and permission definitions
- [ ] **D)** To provide a globally accessible bucket shared across all workspaces

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The workspace root storage is an initial cloud storage bucket automatically created during workspace provisioning. It is used for DBFS, cluster logs, and system tables, but it is not intended for production data. Best practice is to use external locations governed by Unity Catalog for production workloads.
 
 
</details>

### 14. Which two of the following authentication methods can be used to set up the Databricks command line interface?

- [ ] **A)** Personal Access Token (PAT) generated from the workspace
- [ ] **B)** Environment variables DATABRICKS_HOST and DATABRICKS_TOKEN
- [ ] **C)** Using the workspace root storage credential
- [ ] **D)** Using the cluster’s IAM role attached to the workspace

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The Databricks CLI can be authenticated using a personal access token (PAT) or environment variables (DATABRICKS_HOST and DATABRICKS_TOKEN). Workspace root storage credentials and cluster IAM roles are not used for CLI authentication. This is covered in the section on navigating the UI and using the CLI.
 
 
</details>


---

### **Governance and Security**

### 15. What is the top-level container in Unity Catalog's three-level namespace?

- [ ] **A)** Metastore
- [ ] **B)** Catalog
- [ ] **C)** Schema
- [ ] **D)** Table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A metastore is the top-level container for metadata in Unity Catalog, housing catalogs, schemas, and tables.
 
 
</details>

### 16. Which of the following are valid Unity Catalog privileges?

- [ ] **A)** SELECT
- [ ] **B)** MODIFY
- [ ] **C)** USAGE
- [ ] **D)** OWNERSHIP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> SELECT, MODIFY, and USAGE are standard Unity Catalog privileges; OWNERSHIP is a special authority that cannot be granted.
 
 
</details>

### 17. Which SQL command correctly grants SELECT on the table 'sales' to the group 'analysts'?

```sql
GRANT SELECT ON TABLE sales TO analysts;
```

- [ ] **A)** GRANT SELECT ON TABLE sales TO analysts;
- [ ] **B)** GRANT SELECT ON sales TO analysts;
- [ ] **C)** ALLOW SELECT ON sales TO analysts;
- [ ] **D)** GRANT READ ON TABLE sales TO analysts;

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The correct syntax uses GRANT SELECT ON TABLE followed by the table name and TO with the principal.
 
 
</details>

### 18. Which privilege is needed to see a schema's existence without accessing its data?

- [ ] **A)** SELECT
- [ ] **B)** USAGE
- [ ] **C)** MODIFY
- [ ] **D)** CREATE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> USAGE on a schema permits listing its objects but not reading data; SELECT is needed for data access.
 
 
</details>

### 19. Which statements about Unity Catalog tags are true?

- [ ] **A)** Tags can be applied at catalog, schema, table, and column levels.
- [ ] **B)** Tags propagate automatically from a catalog to all child objects.
- [ ] **C)** Tags can be referenced by attribute-based access control (ABAC) policies.
- [ ] **D)** Table tags are set using the ALTER TABLE command with SET TAGS.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Tags are scoped per object (no inheritance), usable in ABAC, and managed via ALTER TABLE ... SET TAGS.
 
 
</details>


---

### **Implementing CI/CD**

### 20. What is the primary purpose of integrating Git with Databricks?

- [ ] **A)** To enable collaboration, reproducibility, and automated deployments
- [ ] **B)** To store notebooks directly in DBFS for easy sharing
- [ ] **C)** To schedule jobs without any manual intervention
- [ ] **D)** To import data from external sources into the workspace

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Git integration enables collaboration, reproducibility, and automation, which are essential for CI/CD pipelines.
 
 
</details>

### 21. Which two actions are required to update a remote Git repository from a Databricks Repo?

- [ ] **A)** Commit the changes locally
- [ ] **B)** Push the committed changes
- [ ] **C)** Pull the latest changes from remote
- [ ] **D)** Create a pull request on the remote provider

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> To update the remote repository, you must first commit locally, then push. Pulling only fetches updates; PRs are for merging branches.
 
 
</details>

### 22. What does the command 'databricks bundle deploy -t prod' achieve?

```bash
databricks bundle deploy -t prod
```

- [ ] **A)** It deploys the bundle artifacts and configures resources in the production workspace
- [ ] **B)** It validates the bundle YAML syntax without connecting to a workspace
- [ ] **C)** It runs the job defined in the bundle immediately
- [ ] **D)** It destroys all resources that were previously deployed by the bundle

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'deploy' command uploads artifacts and creates or updates Databricks resources in the specified target environment.
 
 
</details>


---

### **Troubleshooting, Monitoring, and Optimization**

### 23. In the context of analyzing Spark performance, what kind of information does the Spark UI provide real-time visibility into?

- [ ] **A)** Only driver logs and environmental configurations
- [ ] **B)** Job, stage, and task execution details
- [ ] **C)** Only storage memory and cache metrics
- [ ] **D)** Only SQL query plans and DAG visualization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Spark UI provides real-time visibility into jobs, stages, tasks, storage, SQL execution, and environment configuration.
 
 
</details>

### 24. Which two statements correctly describe benefits of Z-order clustering on Delta tables?

- [ ] **A)** It reduces the amount of data scanned via data skipping
- [ ] **B)** It completely replaces the need for table partitioning
- [ ] **C)** It colocates correlated data values within the same files
- [ ] **D)** It automatically runs VACUUM to remove old files after optimization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Z-order clustering improves data skipping and colocates similar values in files. Partitioning remains beneficial and VACUUM must be run separately.
 
 
</details>

### 25. Examine the code below. What is the purpose of adding the 'salt' column in this data skew mitigation technique?

```python
df_with_salt = df.withColumn("salt", (rand() * 10).cast("int"))
```

- [ ] **A)** To increase the total number of shuffle partitions
- [ ] **B)** To artificially distribute skewed keys across more partitions
- [ ] **C)** To reduce the number of shuffle partitions
- [ ] **D)** To enable the broadcast join optimization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Adding a random salt to skewed join keys allows data to be distributed more evenly across partitions, mitigating skew.
 
 
</details>


---

### **Working with Lakeflow Jobs**

### 26. What is the recommended cluster type for running production jobs in Databricks to ensure isolation and cost efficiency?

- [ ] **A)** All-purpose cluster
- [ ] **B)** Job cluster
- [ ] **C)** High-concurrency cluster
- [ ] **D)** Interactive cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Job clusters are ephemeral, isolated, and auto-terminated, making them cost-effective and secure for production jobs. All-purpose clusters are shared and incur idle costs.
 
 
</details>

### 27. Which two statements correctly describe job triggers in Databricks?

- [ ] **A)** Scheduled jobs use cron expressions and always run regardless of previous outcomes.
- [ ] **B)** Event-driven triggers can be configured for file arrival or Delta table updates.
- [ ] **C)** Concurrent runs are enabled by default for scheduled jobs.
- [ ] **D)** Manual triggers require a valid cron expression.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Cron triggers are stateless (correct). Event-driven triggers support file arrival/Delta table (correct). Concurrent runs are disabled by default. Manual triggers do not use cron.
 
 
</details>

### 28. The following JSON represents a Databricks job definition. What is missing to ensure the job retries twice on failure?

```json
{
  "name": "ETL Pipeline",
  "tasks": [
    {
      "task_key": "ingest",
      "notebook_task": {
        "notebook_path": "/Users/me/ingest"
      }
    }
  ]
}
```

- [ ] **A)** Add 'max_retries': 2 to the task definition.
- [ ] **B)** Add 'retry_policy': {'max_retries': 2} to the job level.
- [ ] **C)** Add 'timeout_seconds': 3600 to limit execution time.
- [ ] **D)** Add 'schedule': {'quartz_cron_expression': '0 0 */2 * * ?'} to run every 2 hours.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The field 'max_retries' specifies the number of retry attempts. The default is 0; setting it to 2 enables two retries.
 
 
</details>

### 29. What is the purpose of a job cluster's 'autotermination_minutes' setting?

- [ ] **A)** It sets the maximum run time of the job.
- [ ] **B)** It defines the idle time before the cluster is automatically terminated.
- [ ] **C)** It determines the interval between retries.
- [ ] **D)** It configures the time zone for the job schedule.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Autotermination_minutes specifies how long a job cluster stays alive after the last activity before being shut down to save costs.
 
 
</details>

### 30. Which two options are valid destinations for job notifications in Databricks?

- [ ] **A)** Email
- [ ] **B)** SMTP Relay
- [ ] **C)** Webhook
- [ ] **D)** Databricks CLI

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Email and webhook are directly configurable in job notifications. SMTP Relay is not a configurable destination; Databricks provides built-in email relay.
 
 
</details>

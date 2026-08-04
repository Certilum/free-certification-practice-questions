<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Databricks/Databricks%20Certified%20Data%20Engineer%20Professional.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Databricks Certified Data Engineer Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Cost and Performance Optimisation](#cost-and-performance-optimisation) (4 questions)
- [Data Governance](#data-governance) (2 questions)
- [Data Ingestion and Acquisition](#data-ingestion-and-acquisition) (2 questions)
- [Data Modelling](#data-modelling) (1 questions)
- [Data Sharing and Federation](#data-sharing-and-federation) (2 questions)
- [Data Transformation, Cleansing, and Quality](#data-transformation-cleansing-and-quality) (3 questions)
- [Debugging and Deploying](#debugging-and-deploying) (3 questions)
- [Developing Code for Data Processing using Python and](#developing-code-for-data-processing-using-python-and) (7 questions)
- [Ensuring Data Security and Compliance](#ensuring-data-security-and-compliance) (3 questions)
- [Monitoring and Alerting](#monitoring-and-alerting) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:29.489Z |
| Domains | 10 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Cost and Performance Optimisation | 4 |
| Data Governance | 2 |
| Data Ingestion and Acquisition | 2 |
| Data Modelling | 1 |
| Data Sharing and Federation | 2 |
| Data Transformation, Cleansing, and Quality | 3 |
| Debugging and Deploying | 3 |
| Developing Code for Data Processing using Python and | 7 |
| Ensuring Data Security and Compliance | 3 |
| Monitoring and Alerting | 3 |

---

### **Cost and Performance Optimisation**

### 1. What is the default value of spark.sql.shuffle.partitions in Spark?

- [ ] **A)** 100
- [ ] **B)** 200
- [ ] **C)** 400
- [ ] **D)** 1000

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The default is 200. This controls the number of partitions after shuffle operations.
 
 
</details>

### 2. Which of the following are part of Spark executor sizing?

- [ ] **A)** spark.executor.cores
- [ ] **B)** spark.executor.memory
- [ ] **C)** spark.executor.instances
- [ ] **D)** spark.sql.shuffle.partitions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Executor sizing includes cores, memory, and instance count. Shuffle partitions are a separate tuning area.
 
 
</details>

### 3. Given the following configuration, what is the most likely performance issue?

```python
spark.sql.shuffle.partitions = 10
# cluster has 100 cores
```

- [ ] **A)** Too few partitions cause memory spill
- [ ] **B)** Too many partitions cause scheduling overhead
- [ ] **C)** Not enough memory per executor
- [ ] **D)** Data skew due to key distribution

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Setting partitions to 10 on a 100-core cluster creates large partitions that may exceed memory and spill to disk.
 
 
</details>

### 4. What is the primary purpose of the Photon engine in Databricks?

- [ ] **A)** Query execution via native C++ vectorization
- [ ] **B)** Storage layout optimization using Z-ordering
- [ ] **C)** Data compression during write operations
- [ ] **D)** Streaming job reliability with checkpointing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Photon is a native C++ vectorized query engine that speeds up SQL and DataFrame operations.
 
 
</details>


---

### **Data Governance**

### 5. How many Unity Catalog metastores can be assigned to a single Databricks workspace?

- [ ] **A)** One
- [ ] **B)** Two
- [ ] **C)** As many as needed
- [ ] **D)** None

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Only one metastore can be assigned per workspace; however, one metastore can serve multiple workspaces.
 
 
</details>

### 6. Which two of the following are securable objects in Unity Catalog?

- [ ] **A)** Metastore
- [ ] **B)** Cluster
- [ ] **C)** Schema
- [ ] **D)** Notebook

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Metastore and Schema are securable objects in the Unity Catalog hierarchy; Clusters and Notebooks are not.
 
 
</details>


---

### **Data Ingestion and Acquisition**

### 7. A data pipeline ingests 50,000 small JSON files per minute from an S3 bucket. Which Auto Loader mode should be used to minimize latency?

- [ ] **A)** Directory listing mode with a low polling interval of 1 minute
- [ ] **B)** File notification mode using S3 bucket notifications and SQS
- [ ] **C)** Directory listing mode with the default polling interval of 10 minutes
- [ ] **D)** File notification mode but without setting up a schema location

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> File notification mode uses cloud-native event services (e.g., SQS, Event Grid) to detect new files with low latency (<1 minute), making it ideal for high-throughput scenarios. Directory listing mode has higher latency and is not suitable for thousands of files per minute.
 
 
</details>

### 8. Which schema evolution modes are available for Auto Loader when ingesting files with varying structures?

- [ ] **A)** rescue
- [ ] **B)** rescueAndEvolve
- [ ] **C)** failOnNewColumns
- [ ] **D)** mergeSchema

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Auto Loader supports three evolution modes: 'none' (fail on mismatch), 'rescue' (write mismatched data to _rescued_data), and 'rescueAndEvolve' (add new columns and rescue mismatches). 'failOnNewColumns' and 'mergeSchema' are not valid values for cloudFiles.schemaEvolutionMode; 'mergeSchema' is a Delta Lake write option.
 
 
</details>


---

### **Data Modelling**

### 9. Which schema is recommended as the best practice for the gold layer of the Medallion architecture on Databricks?

- [ ] **A)** Star schema
- [ ] **B)** Snowflake schema
- [ ] **C)** Third normal form (3NF)
- [ ] **D)** Flat table (no dimensions)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The document states that star schemas are the gold standard for the gold layer, optimized for BI and AI workloads.
 
 
</details>


---

### **Data Sharing and Federation**

### 10. What is the name of the open protocol developed by Databricks specifically designed for secure, governed, and real-time data sharing across heterogeneous platforms?

- [ ] **A)** Delta Sharing
- [ ] **B)** Apache Spark
- [ ] **C)** Unity Catalog
- [ ] **D)** Lakehouse Federation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Delta Sharing is an open protocol developed by Databricks for secure, governed, and real-time data sharing across heterogeneous platforms without copying data.
 
 
</details>

### 11. Consider the following statements regarding Delta Sharing shares in Databricks and choose the ones that are accurate. (Select two options.)

- [ ] **A)** A share is a logical container for tables, views, or volumes.
- [ ] **B)** A share can include tables from multiple catalogs within the same metastore.
- [ ] **C)** A share is created using the CREATE SHARE command.
- [ ] **D)** A share can be renamed after creation using ALTER SHARE RENAME.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Shares are created with CREATE SHARE, can contain tables/views/volumes from a single metastore, and are immutable – they cannot be renamed.
 
 
</details>


---

### **Data Transformation, Cleansing, and Quality**

### 12. What does DLT expect_all_or_drop do when a row violates a constraint?

- [ ] **A)** The violating row is kept but flagged in the event log.
- [ ] **B)** The violating row is dropped from the output table.
- [ ] **C)** The entire batch fails and is rolled back.
- [ ] **D)** The pipeline stops and an alert is sent.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> expect_all_or_drop removes rows that fail any constraint from the target table while logging the violation in the event log.
 
 
</details>

### 13. Which two statements are correct about Great Expectations integration in Databricks?

- [ ] **A)** Great Expectations can validate Spark DataFrames using Pandas conversion.
- [ ] **B)** DLT built-in expectations are identical to Great Expectations in functionality.
- [ ] **C)** The mostly parameter allows a percentage of failures per expectation.
- [ ] **D)** Great Expectations cannot be used with Databricks notebooks.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Great Expectations supports Pandas validation and the mostly parameter sets a threshold for acceptable failures.
 
 
</details>

### 14. What is the result of the PySpark null handling operation?

```python
df = spark.createDataFrame([(1, None), (2, 'Alice'), (3, 'Bob')], ['id', 'name'])
df_clean = df.na.fill('Unknown', subset=['name'])
df_clean.show()
```

- [ ] **A)** All nulls in 'name' are replaced with 'Unknown', others unchanged.
- [ ] **B)** All nulls in all columns are replaced with 'Unknown'.
- [ ] **C)** The code throws an error because 'name' column has no nulls.
- [ ] **D)** Only the first null is replaced; subsequent nulls remain.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> df.na.fill(value, subset) replaces only nulls in specified columns, so only nulls in 'name' are replaced.
 
 
</details>


---

### **Debugging and Deploying**

### 15. Which Spark UI tab is primarily used to view task-level metrics like duration and shuffle spill?

- [ ] **A)** Jobs
- [ ] **B)** Stages
- [ ] **C)** Storage
- [ ] **D)** Environment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Stages tab shows task-level metrics including duration, shuffle read/write, and spill, making it the primary debugging tab.
 
 
</details>

### 16. Which of the following are symptoms of data skew in a Spark job? (Select all that apply.)

- [ ] **A)** A few tasks take significantly longer than the median.
- [ ] **B)** All tasks have similar execution times.
- [ ] **C)** High shuffle spill (memory and disk) for certain tasks.
- [ ] **D)** The Storage tab shows cached data evenly distributed.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Data skew manifests as a long tail of task durations and high spill metrics due to imbalanced partitions.
 
 
</details>

### 17. Examine the following code snippet used for unit testing a Spark transformation. What does this test verify?

```python
from chispa import assert_df_equals
import pipeline_lib as pl

def test_clean_customers(spark_fixture):
    input_df = spark_fixture.createDataFrame([(None, 100)], ["name", "id"])
    expected_df = spark_fixture.createDataFrame([("unknown", 100)], ["name", "id"])
    result_df = pl.clean_customers(input_df)
    assert_df_equals(result_df, expected_df)
```

- [ ] **A)** That the transformation renames columns correctly.
- [ ] **B)** That null names are replaced with 'unknown' and the id column is preserved.
- [ ] **C)** That the DataFrame schema contains exactly two columns.
- [ ] **D)** That the transformation filters out rows with null names.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The test inputs a DataFrame with a null name and expects the output to have 'unknown' and the same id, verifying the cleaning logic.
 
 
</details>


---

### **Developing Code for Data Processing using Python and**

### 18. What is the primary abstraction for distributed data processing in Apache Spark?

- [ ] **A)** RDD
- [ ] **B)** DataFrame
- [ ] **C)** Dataset
- [ ] **D)** SparkContext

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RDD stands for Resilient Distributed Dataset and is the fundamental data structure of Apache Spark, representing an immutable, partitioned collection of records that can be processed in parallel.
 
 
</details>

### 19. Which of the following are characteristics of a Spark DataFrame? (Select all that apply.)

- [ ] **A)** It is distributed across a cluster
- [ ] **B)** It has row and column structure
- [ ] **C)** It is stored on a single machine
- [ ] **D)** It supports lazy evaluation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> DataFrames in Spark are distributed collections of data organized into named columns, and they leverage lazy evaluation for performance optimization. They are not stored on a single machine but partitioned across the cluster.
 
 
</details>

### 20. Analyze the following PySpark code block and determine the type of operation performed.

```python
df_filtered = df.filter(df.age > 30)
```

- [ ] **A)** Transformation
- [ ] **B)** Action
- [ ] **C)** Shuffle
- [ ] **D)** Persist

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code shows a filter operation, which is a narrow transformation that returns a new DataFrame without triggering any computation until an action is called.
 
 
</details>

### 21. Which method is used to read a Parquet file into a DataFrame in Databricks?

- [ ] **A)** spark.read.parquet()
- [ ] **B)** spark.read.csv()
- [ ] **C)** spark.read.json()
- [ ] **D)** spark.read.text()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The spark.read.parquet() method is the standard way to read Parquet files into a DataFrame in PySpark. Parquet is a columnar storage format commonly used with Spark.
 
 
</details>

### 22. Which of the following are Spark actions? (Select all that apply.)

- [ ] **A)** count()
- [ ] **B)** collect()
- [ ] **C)** filter()
- [ ] **D)** show()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> count(), collect(), and show() are actions that force Spark to evaluate transformations and return results. filter() is a transformation that creates a new DataFrame without computation.
 
 
</details>

### 23. Identify the error in the following PySpark code if any. If there is an error, select 'Error'. Otherwise, select 'Valid'.

```python
df = spark.range(100)
df_count = df.count()
```

- [ ] **A)** Error
- [ ] **B)** Valid
- [ ] **C)** Missing import
- [ ] **D)** Syntax warning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code uses `spark` without defining it. In a Databricks notebook, `spark` is automatically available, but this snippet incorrectly uses `SparkSession` with a lowercase `s`. The correct way is `SparkSession.builder.getOrCreate()`, but typically `spark` is already defined. However, the line `spark = SparkSession.builder.getOrCreate()` is valid only if SparkSession is imported. Here, neither import nor definition exists; thus it would error.
 
 
</details>

### 24. What does the `select()` transformation do in PySpark?

- [ ] **A)** It selects specific columns from a DataFrame
- [ ] **B)** It filters rows based on a condition
- [ ] **C)** It renames columns
- [ ] **D)** It sorts the DataFrame

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The `select()` method returns a new DataFrame that contains only the specified columns (or expressions). It is a transformation that does not trigger computation.
 
 
</details>


---

### **Ensuring Data Security and Compliance**

### 25. What is the primary purpose of a row filter in Unity Catalog?

- [ ] **A)** It automatically removes entire rows from query results based on the caller's identity or attributes.
- [ ] **B)** It masks specific column values to hide sensitive data from unauthorized users.
- [ ] **C)** It restricts users from inserting new rows into a table.
- [ ] **D)** It encrypts row data at rest to prevent data breaches.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Row filters are SQL functions that return a Boolean expression. When a query runs, rows evaluating to FALSE or NULL are suppressed. This filters rows based on the caller (e.g., CURRENT_USER()), not column masking, write restrictions, or encryption.
 
 
</details>

### 26. Which statements accurately describe column masks in Unity Catalog? (Select two.)

- [ ] **A)** Column masks are SQL expressions that transform or hide column values at query time.
- [ ] **B)** Column masks prevent users from seeing the column in DESCRIBE TABLE output.
- [ ] **C)** Column masks can show different values based on the caller's group membership.
- [ ] **D)** Column masks are applied to INSERT and UPDATE statements to protect data integrity.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Column masks are applied at query time to SELECT results. They transform values (e.g., mask SSN) and can use IS_MEMBER to differentiate users. Masks do not affect schema viewing (DESCRIBE) nor write operations.
 
 
</details>

### 27. Review the following SQL statement and identify what it accomplishes:

```sql
ALTER TABLE sales SET ROW FILTER region_filter;
```

- [ ] **A)** It attaches a row filter named 'region_filter' to the 'sales' table, so that every SELECT on the table will invoke the filter.
- [ ] **B)** It creates a new view named 'region_filter' over the 'sales' table.
- [ ] **C)** It alters the 'sales' table to include a new column named 'region_filter'.
- [ ] **D)** It removes an existing row filter from the 'sales' table.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The ALTER TABLE ... SET ROW FILTER syntax attaches a previously created row filter function to a table. This ensures all queries against the table automatically apply the filter logic.
 
 
</details>


---

### **Monitoring and Alerting**

### 28. What does the /api/2.1/jobs/runs/list endpoint return?

- [ ] **A)** Paginated run metadata including state and timings
- [ ] **B)** Detailed job definition and cluster configuration
- [ ] **C)** A list of all job IDs in the workspace
- [ ] **D)** The Spark UI event logs for the last run

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The /api/2.1/jobs/runs/list endpoint returns paginated metadata about job runs, including state, start time, duration, and other run-level information.
 
 
</details>

### 29. Which comparison operators are valid for a Databricks dashboard alert? (Select all that apply)

- [ ] **A)** =
- [ ] **B)** !=
- [ ] **C)** <
- [ ] **D)** >

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> Dashboard alerts support the comparison operators =, !=, <, >, <=, >=, as well as a 'no data' condition. The four listed are all valid.
 
 
</details>

### 30. Refer to the Spark UI stage output below. Based on this information, which of the following statements are correct? (Select all that apply)

```text
Task time distribution:
  min: 2s
  median: 5s
  max: 60s
```

- [ ] **A)** The stage exhibits partition skew
- [ ] **B)** The stage is running efficiently with no issues
- [ ] **C)** A straggler task is present
- [ ] **D)** The task duration is uniformly distributed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> A very long max task duration compared to median indicates a straggler task, which is a sign of partition skew.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Azure%20Data%20Engineer%20Associate.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Azure Data Engineer Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Design and implement data storage](#design-and-implement-data-storage) (6 questions)
- [Develop data processing](#develop-data-processing) (14 questions)
- [Secure, monitor, and optimize data storage and data processing](#secure-monitor-and-optimize-data-storage-and-data-processing) (10 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:52:36.120Z |
| Domains | 3 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Design and implement data storage | 6 |
| Develop data processing | 14 |
| Secure, monitor, and optimize data storage and data processing | 10 |

---

### **Design and implement data storage**

### 1. Which Azure service is optimized for OLTP relational workloads that require ACID transactions and complex SQL joins?

- [ ] **A)** Azure SQL Database
- [ ] **B)** Azure Synapse Analytics dedicated SQL pool
- [ ] **C)** Azure Data Lake Storage Gen2
- [ ] **D)** Azure Cosmos DB

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure SQL Database is a relational OLTP service with ACID support. Synapse dedicated pools are analytical, ADLS Gen2 is storage, and Cosmos DB is NoSQL.
 
 
</details>

### 2. Which two Azure services are commonly included in an analytical data storage strategy for petabyte-scale workloads?

- [ ] **A)** Azure Synapse Analytics
- [ ] **B)** Azure Data Lake Storage Gen2
- [ ] **C)** Azure SQL Database
- [ ] **D)** Azure Cosmos DB

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Synapse Analytics provides MPP and columnar querying, while ADLS Gen2 offers scalable lake storage for analytics. Azure SQL Database is transactional, and Cosmos DB is a NoSQL store.
 
 
</details>

### 3. Review the Azure CLI command in the code block. Which storage redundancy option is configured for the new storage account?

```bash
az storage account create --name salesdata --resource-group rg --location eastus --sku Standard_GRS
```

- [ ] **A)** Locally redundant storage (LRS)
- [ ] **B)** Zone-redundant storage (ZRS)
- [ ] **C)** Geo-redundant storage (GRS)
- [ ] **D)** Read-access geo-redundant storage (RA-GRS)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The `--sku Standard_GRS` parameter selects geo-redundant storage, which copies data to a secondary region. It does not enable read access to that secondary region.
 
 
</details>

### 4. What is meant by polyglot persistence in an Azure data architecture?

- [ ] **A)** Using multiple specialized stores in one solution
- [ ] **B)** Replicating data to multiple regions
- [ ] **C)** Migrating all databases to one SQL database
- [ ] **D)** Enabling hot and cool tiers in one account

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Polyglot persistence intentionally uses multiple data stores, each matched to specific data models or workload needs, instead of forcing all data into one platform.
 
 
</details>

### 5. Which two actions are part of data lifecycle management to reduce Azure Blob Storage costs?

- [ ] **A)** Moving data to cool or archive tiers
- [ ] **B)** Creating additional file partitions
- [ ] **C)** Applying rules based on access patterns
- [ ] **D)** Choosing geo-redundant storage for all containers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Lifecycle management can move blobs to cooler tiers and apply rules based on access patterns. More partitions and GRS increase cost and do not reduce lifecycle expense.
 
 
</details>

### 6. The code block contains a statement for creating a table in a data lake. Which storage format is specified in this statement?

```sql
CREATE TABLE sales (id INT, amount DECIMAL(10,2)) USING DELTA LOCATION '/lake/silver/sales'
```

- [ ] **A)** Parquet
- [ ] **B)** CSV
- [ ] **C)** Delta Lake
- [ ] **D)** JSON

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Using Delta Lake configures an open format that adds ACID transactions, time travel, and schema enforcement to data lake tables.
 
 
</details>


---

### **Develop data processing**

### 7. Which Azure service is designed primarily to orchestrate data movement and transformation across enterprise-scale data pipelines?

- [ ] **A)** Azure Data Factory
- [ ] **B)** Azure Databricks
- [ ] **C)** Azure Event Hubs
- [ ] **D)** Azure Stream Analytics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Data Factory is the orchestration service for cloud-scale data integration. Databricks provides Spark compute, Event Hubs handles ingestion, and Stream Analytics processes streams.
 
 
</details>

### 8. Which of the following are Integration Runtime types used by Azure Data Factory and Synapse pipelines? Select all that apply.

- [ ] **A)** Azure Integration Runtime
- [ ] **B)** Self-Hosted Integration Runtime
- [ ] **C)** SSIS Integration Runtime
- [ ] **D)** Databricks Integration Runtime

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Azure, Self-Hosted, and SSIS Integration Runtimes are supported. There is no Databricks Integration Runtime; Databricks is a linked compute service.
 
 
</details>

### 9. Review the JSON trigger definition shown in the code block. Which trigger type does it represent?

```json
{
  "name": "MyTumblingTrigger",
  "type": "TumblingWindowTrigger",
  "pipeline": "MyPipeline",
  "frequency": "Hour",
  "interval": 1
}
```

- [ ] **A)** Schedule trigger
- [ ] **B)** Tumbling window trigger
- [ ] **C)** Event trigger
- [ ] **D)** Manual trigger

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> TumblingWindowTrigger performs time-based, stateful processing with a defined frequency and interval, unlike a simple schedule trigger.
 
 
</details>

### 10. Which Azure Data Factory activity is used to submit a Spark notebook to an Azure Databricks workspace?

- [ ] **A)** Databricks Notebook Activity
- [ ] **B)** Copy Activity
- [ ] **C)** Stored Procedure Activity
- [ ] **D)** Web Activity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Databricks Notebook Activity submits notebook workloads to a Databricks workspace, separating orchestration from Spark compute.
 
 
</details>

### 11. Which of the following mechanisms can initiate a pipeline execution according to Azure Data Factory? Select all that apply.

- [ ] **A)** Schedule trigger
- [ ] **B)** Tumbling window trigger
- [ ] **C)** Event-based trigger
- [ ] **D)** SQL Agent job

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Schedule, tumbling window, and event triggers initiate pipelines. SQL Server Agent is not a native ADF trigger type.
 
 
</details>

### 12. The code block shows a Spark DataFrame write operation. What is the final write behavior?

```python
from pyspark.sql import SparkSession
df = spark.read.json('input')
df_clean = df.filter(df['age'] > 18)
df_clean.write.mode('overwrite').parquet('output')

```

- [ ] **A)** Overwrites existing data
- [ ] **B)** Appends to existing data
- [ ] **C)** Fails if output exists
- [ ] **D)** Ignores existing data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The .mode('overwrite') option replaces any existing data at the output location with the new DataFrame.
 
 
</details>

### 13. Which Azure service is a fully managed, serverless stream processing engine using a SQL-based query language?

- [ ] **A)** Azure Stream Analytics
- [ ] **B)** Azure Event Hubs
- [ ] **C)** Azure Databricks
- [ ] **D)** Azure Data Factory

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Stream Analytics is fully managed and serverless, using the Stream Analytics Query Language to process streaming data.
 
 
</details>

### 14. Which of the following are valid window types in Azure Stream Analytics? Select all that apply.

- [ ] **A)** Tumbling window
- [ ] **B)** Hopping window
- [ ] **C)** Sliding window
- [ ] **D)** Snapshot window

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Azure Stream Analytics supports tumbling, hopping, sliding, and session windows. Snapshot is not one of its window types.
 
 
</details>

### 15. The code block shows a Spark Structured Streaming query. What does the watermark parameter control?

```python
streamDF = spark.readStream.format('json').load('input')
result = streamDF.withWatermark('eventTime', '10 minutes').groupBy(window('eventTime', '5 minutes')).count()

```

- [ ] **A)** Sets how long to wait for late-arriving event data
- [ ] **B)** Defines the number of output partitions
- [ ] **C)** Controls the batch interval for micro-batches
- [ ] **D)** Specifies the Event Hubs consumer group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Watermarking tells Spark how long to wait for late-arriving data before dropping state, preventing unbounded state growth.
 
 
</details>

### 16. Which mechanism in Spark Structured Streaming prevents unbounded state growth caused by late-arriving events?

- [ ] **A)** Watermarking
- [ ] **B)** Checkpointing
- [ ] **C)** Consumer groups
- [ ] **D)** Private endpoints

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Watermarking manages how long stateful operations wait for late events, preventing memory issues from unbounded state.
 
 
</details>

### 17. Which Azure technologies are appropriate for high-throughput streaming with complex stateful transformations? Select all that apply.

- [ ] **A)** Spark Structured Streaming
- [ ] **B)** Azure Databricks
- [ ] **C)** Azure Synapse Spark pool
- [ ] **D)** Azure Logic Apps

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Spark Structured Streaming on Databricks or Synapse handles complex stateful processing. Logic Apps is not designed for heavy stream processing.
 
 
</details>

### 18. The code block contains an Azure Stream Analytics query. What kind of window does it use?

```sql
SELECT tollId, COUNT(*) AS Count
FROM input TIMESTAMP BY entryTime
GROUP BY tollId, TumblingWindow(minute, 5)

```

- [ ] **A)** Tumbling window
- [ ] **B)** Hopping window
- [ ] **C)** Sliding window
- [ ] **D)** Session window

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TumblingWindow(minute, 5) creates a non-overlapping five-minute window for each tollId.
 
 
</details>

### 19. What is the primary role of Azure Event Hubs in a real-time data architecture?

- [ ] **A)** Event ingestion broker
- [ ] **B)** Stream processing engine
- [ ] **C)** Data warehouse
- [ ] **D)** Pipeline orchestrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Event Hubs is a highly scalable ingestion broker that captures and stores events for downstream processing.
 
 
</details>

### 20. Which of the following statements about Azure Event Hubs partitions are correct? Select all that apply.

- [ ] **A)** Partitions allow concurrent consumption
- [ ] **B)** Partition keys distribute load evenly
- [ ] **C)** Ordered event processing is maintained per partition
- [ ] **D)** Partition count can be changed dynamically after creation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Event Hubs partitions support concurrency, load distribution, and per-partition ordering. Partition counts cannot be changed after creation.
 
 
</details>


---

### **Secure, monitor, and optimize data storage and data processing**

### 21. What is the primary purpose of Azure Monitor in an Azure data platform?

- [ ] **A)** Collecting telemetry and operational metrics from Azure resources
- [ ] **B)** Tracking data lineage across pipelines
- [ ] **C)** Scheduling data factory pipeline runs
- [ ] **D)** Storing transformed analytical data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Monitor captures platform metrics and telemetry. Governance, scheduling, and data storage are handled by other services.
 
 
</details>

### 22. Which destinations can receive diagnostic logs and metrics from Azure data services?

- [ ] **A)** Log Analytics workspace
- [ ] **B)** Event Hubs
- [ ] **C)** Azure Storage account
- [ ] **D)** Azure DevOps organization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Diagnostic settings can send logs to Log Analytics, Event Hubs, or Storage. Azure DevOps is not a diagnostic destination.
 
 
</details>

### 23. Look at the KQL query in the code block. Where is this query executed?

```kql
ADFPipelineRun
| where Status == "Failed"
| project PipelineName, RunId, FailureType
```

- [ ] **A)** Log Analytics workspace
- [ ] **B)** Azure Synapse SQL pool
- [ ] **C)** Azure Data Lake Storage
- [ ] **D)** Azure Databricks cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query references the ADFPipelineRun table, which is stored in a Log Analytics workspace for pipeline diagnostics.
 
 
</details>

### 24. Which table distribution is generally preferred for large fact tables in Azure Synapse Analytics?

- [ ] **A)** Hash distribution on a join column
- [ ] **B)** Replicated distribution
- [ ] **C)** Round Robin distribution
- [ ] **D)** Heap distribution

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Hash distribution on a well-chosen join column minimizes data movement. Replicated is for small dimension tables.
 
 
</details>

### 25. Which practices help optimize query performance in Azure Databricks Delta Lake?

- [ ] **A)** Applying Z-Ordering to frequently filtered columns
- [ ] **B)** Enabling Delta Lake caching
- [ ] **C)** Periodically running OPTIMIZE and VACCUM
- [ ] **D)** Disabling file compaction

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Z-Ordering, caching, and maintenance operations like OPTIMIZE and VACCUM improve Delta Lake performance.
 
 
</details>

### 26. The code block creates a table in Azure Synapse Analytics. Which distribution strategy is being applied?

```sql
CREATE TABLE dbo.FactSales
WITH (DISTRIBUTION = HASH(SalesOrderId))
AS SELECT * FROM SalesStage;
```

- [ ] **A)** Hash
- [ ] **B)** Round Robin
- [ ] **C)** Replicated
- [ ] **D)** Broadcast

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The DISTRIBUTION = HASH clause defines a hash-distributed table based on SalesOrderId.
 
 
</details>

### 27. Which Azure Data Factory metric is commonly watched to detect self-hosted Integration Runtime bottlenecks?

- [ ] **A)** Queue length
- [ ] **B)** Number of pipelines
- [ ] **C)** Data Integration Units
- [ ] **D)** Number of linked services

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A long queue length on a self-hosted Integration Runtime indicates a processing bottleneck.
 
 
</details>

### 28. Which security controls are designed for Azure Data Lake Storage Gen2?

- [ ] **A)** Azure RBAC and POSIX ACLs
- [ ] **B)** Private endpoints
- [ ] **C)** Managed identities for Azure resources
- [ ] **D)** Public access keys embedded in connection strings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> ADLS Gen2 supports RBAC, ACLs, private endpoints, and managed identities. Hardcoded keys violate least privilege.
 
 
</details>

### 29. An Azure resource is configured with the identity setting in the code block. What is the primary benefit?

```json
{
  "identity": {
    "type": "SystemAssigned"
  }
}
```

- [ ] **A)** It enables secure authentication without hardcoded credentials
- [ ] **B)** It grants public internet access to the resource
- [ ] **C)** It automatically encrypts all data in transit
- [ ] **D)** It replaces the need for role-based access control

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> System-assigned managed identities authenticate to Azure resources without storing secrets or credentials in code.
 
 
</details>

### 30. Which Azure service acts as the identity provider for users and services accessing data platforms?

- [ ] **A)** Microsoft Entra ID
- [ ] **B)** Azure Key Vault
- [ ] **C)** Azure Policy
- [ ] **D)** Microsoft Purview

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Microsoft Entra ID authenticates users, service principals, and managed identities across Azure services.
 
 
</details>

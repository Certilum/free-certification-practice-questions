<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Google%20Cloud/Professional%20Data%20Engineer%20Certification" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Professional Data Engineer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Building and operationalizing data processing systems](#building-and-operationalizing-data-processing-systems) (8 questions)
- [Designing data processing systems](#designing-data-processing-systems) (7 questions)
- [Ensuring solution quality](#ensuring-solution-quality) (9 questions)
- [Operationalizing machine learning models](#operationalizing-machine-learning-models) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:52:24.972Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Building and operationalizing data processing systems | 8 |
| Designing data processing systems | 7 |
| Ensuring solution quality | 9 |
| Operationalizing machine learning models | 6 |

---

### **Building and operationalizing data processing systems**

### 1. Which Google Cloud service is a unified, serverless data-processing option for both batch and stream workloads?

- [ ] **A)** Cloud Dataflow
- [ ] **B)** Cloud Dataproc
- [ ] **C)** Cloud Composer
- [ ] **D)** Cloud Data Fusion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Dataflow is the Google Cloud service that implements the Apache Beam model and supports both batch and streaming data processing in a fully managed, serverless way.
 
 
</details>

### 2. Which two Google Cloud services can be used to build managed data-processing pipelines?

- [ ] **A)** Cloud Dataflow
- [ ] **B)** Cloud Dataproc
- [ ] **C)** Cloud Storage
- [ ] **D)** Cloud IAM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Cloud Dataflow and Cloud Dataproc are managed services for data processing. Cloud Storage stores data and Cloud IAM governs access, so they are not processing services.
 
 
</details>

### 3. In the pipeline code shown, which transform is used to keep only the even numbers?

```python
with beam.Pipeline() as p:
    result = (p | beam.Create([1,2,3,4])
                | beam.Filter(lambda x: x % 2 == 0)
                | beam.CombineGlobally(sum))
```

- [ ] **A)** beam.Filter
- [ ] **B)** beam.Create
- [ ] **C)** beam.Map
- [ ] **D)** beam.CombineGlobally

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> beam.Filter applies a predicate and keeps elements for which the predicate returns true, so it selects even numbers in the pipeline.
 
 
</details>

### 4. Which Apache Beam component is responsible for reading data from an external source in a Dataflow pipeline?

- [ ] **A)** I/O connector
- [ ] **B)** Pipeline
- [ ] **C)** Transform
- [ ] **D)** Runner

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An I/O connector reads data from an external source and can also write results to a sink; transforms process data within the pipeline.
 
 
</details>

### 5. Which two Google Cloud services are designed for low-latency streaming data ingestion and processing?

- [ ] **A)** Cloud Pub/Sub
- [ ] **B)** Cloud Dataflow
- [ ] **C)** Cloud Storage
- [ ] **D)** Cloud SQL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Cloud Pub/Sub ingests streaming messages, while Cloud Dataflow processes those messages in a streaming pipeline. Cloud Storage and Cloud SQL do not provide streaming ingestion.
 
 
</details>

### 6. In the command shown, what is the name of the cluster that receives the Spark job?

```bash
gcloud dataproc jobs submit spark \
    --cluster=example-cluster \
    --region=us-central1 \
    --class=org.example.WordCount \
    -- gs://bucket/input.txt
```

- [ ] **A)** example-cluster
- [ ] **B)** us-central1
- [ ] **C)** org.example.WordCount
- [ ] **D)** gs://bucket/input.txt

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The --cluster flag identifies the Dataproc cluster where the Spark job is submitted; example-cluster is the cluster name.
 
 
</details>

### 7. Which fully managed object storage service is typically used as a data lake for batch pipelines on Google Cloud?

- [ ] **A)** Cloud Storage
- [ ] **B)** Cloud SQL
- [ ] **C)** Cloud Spanner
- [ ] **D)** BigQuery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Storage is Google Cloud's durable, object-based storage and is commonly used as a landing zone or data lake for batch processing.
 
 
</details>

### 8. Which two statements accurately describe Cloud Dataflow?

- [ ] **A)** It is fully managed and serverless.
- [ ] **B)** It can automatically scale workers.
- [ ] **C)** It requires a persistent cluster.
- [ ] **D)** It only supports batch data.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Cloud Dataflow is a fully managed, serverless service and can autoscale. It supports both batch and streaming workloads and does not need a persistent cluster.
 
 
</details>


---

### **Designing data processing systems**

### 9. Which Google Cloud service is a fully managed serverless data warehouse that can run SQL queries directly on large datasets?

- [ ] **A)** BigQuery
- [ ] **B)** Cloud Storage
- [ ] **C)** Pub/Sub
- [ ] **D)** Cloud Spanner

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> BigQuery is Google Cloud's serverless data warehouse. It supports SQL queries and petabyte-scale analysis while separating storage from compute.
 
 
</details>

### 10. Which two statements correctly describe topics and subscriptions in Cloud Pub/Sub?

- [ ] **A)** One topic can have multiple subscriptions.
- [ ] **B)** A subscription pushes messages to the topic.
- [ ] **C)** Multiple subscriptions can receive the same published message independently.
- [ ] **D)** A topic is created automatically every time a message is published.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> A Pub/Sub topic is a named channel to which publishers send messages. Each subscription receives copies of messages, so multiple subscriptions can independently consume the same stream.
 
 
</details>

### 11. Look at the SQL query in the code block. Which join type is used to combine the two tables?

```sql
SELECT e.name, d.department_name
FROM employees e
LEFT JOIN departments d
ON e.department_id = d.id;
```

- [ ] **A)** LEFT OUTER JOIN
- [ ] **B)** INNER JOIN
- [ ] **C)** RIGHT OUTER JOIN
- [ ] **D)** CROSS JOIN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query uses LEFT JOIN, a synonym for LEFT OUTER JOIN, which returns all rows from the left table and only matching rows from the right.
 
 
</details>

### 12. What is the main purpose of partitioning tables in BigQuery?

- [ ] **A)** It reduces the amount of data scanned by pruning partitions.
- [ ] **B)** It automatically encrypts data at rest.
- [ ] **C)** It converts streaming data into structured data.
- [ ] **D)** It prevents users from updating table schemas.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Partitioning divides a table into segments based on a column, often date. Queries can prune scanned partitions, improving performance and lowering costs.
 
 
</details>

### 13. Which two practices help reduce cost when designing a Google Cloud batch data processing pipeline?

- [ ] **A)** Use preemptible VMs for fault-tolerant Dataproc workloads.
- [ ] **B)** Store rarely accessed raw data in Cloud Storage Coldline.
- [ ] **C)** Keep a large pool of always-on Dataflow workers idle.
- [ ] **D)** Copy every batch result into multiple world-wide buckets.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Preemptible VMs cost much less for short-lived batch jobs, and Cloud Storage Coldline is a low-cost storage class for archival data.
 
 
</details>

### 14. Examine the Apache Beam pipeline in the code block. Which transform produces a collection of word and count pairs?

```python
import apache_beam as beam

with beam.Pipeline() as p:
    lines = p | 'Read' >> beam.io.ReadFromText('gs://data/input.txt')
    words = lines | 'Split' >> beam.FlatMap(lambda x: x.split())
    counts = words | 'Count' >> beam.combiners.Count.PerElement()
```

- [ ] **A)** beam.combiners.Count.PerElement()
- [ ] **B)** beam.GroupByKey()
- [ ] **C)** beam.CombineValues()
- [ ] **D)** beam.io.ReadFromText()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Count.PerElement() is a beam combinator that counts how many times each element appears and outputs key-count pairs.
 
 
</details>

### 15. Which Google Cloud service is primarily used to orchestrate data processing workflows with managed Apache Airflow?

- [ ] **A)** Cloud Composer
- [ ] **B)** Dataflow
- [ ] **C)** Dataproc
- [ ] **D)** Cloud Functions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Composer is a managed Apache Airflow service used to schedule, monitor, and orchestrate complex data pipelines.
 
 
</details>


---

### **Ensuring solution quality**

### 16. Which Google Cloud service is used to create and enforce data quality rules across distributed data assets in a data mesh?

- [ ] **A)** Dataplex
- [ ] **B)** Dataflow
- [ ] **C)** BigQuery
- [ ] **D)** Cloud Composer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Dataplex centralizes data governance across distributed storage systems. It lets you define and enforce data quality rules for BigQuery and Cloud Storage.
 
 
</details>

### 17. When operating production data pipelines, which two practices are part of a data quality strategy in Google Cloud? Choose two.

- [ ] **A)** Automated quality checks
- [ ] **B)** Pipeline monitoring
- [ ] **C)** Manual schema changes
- [ ] **D)** Disabling audit logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Automated quality checks verify completeness, freshness, and accuracy. Pipeline monitoring detects failures and delays. Manual changes and disabled logs reduce visibility and quality.
 
 
</details>

### 18. A data engineer runs the SQL query shown in the code block. What is the function of this query in BigQuery?

```sql
SELECT COUNT(*) FROM `project.dataset.orders`;
```

- [ ] **A)** Counts rows in the table
- [ ] **B)** Deletes the table
- [ ] **C)** Updates column names
- [ ] **D)** Creates a view

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The SELECT COUNT(*) statement counts every row in the specified table. This common check is used to verify that data has been loaded correctly.
 
 
</details>

### 19. Which Google Cloud service should be used to collect operational metrics and send alerts when a data pipeline is unhealthy?

- [ ] **A)** Cloud Monitoring
- [ ] **B)** Cloud Logging
- [ ] **C)** Data Catalog
- [ ] **D)** Dataplex

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Monitoring collects performance metrics, builds dashboards, and sends alerts. This helps data engineers maintain solution quality by detecting unhealthy pipelines quickly.
 
 
</details>

### 20. Which two Google Cloud services allow data engineers to manage, search, and govern metadata for data assets? Choose two.

- [ ] **A)** Data Catalog
- [ ] **B)** Dataplex
- [ ] **C)** Cloud Storage
- [ ] **D)** Cloud Functions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Data Catalog provides metadata search and tagging. Dataplex extends governance with domains, policies, quality, and access controls, helping teams manage data assets across the organization.
 
 
</details>

### 21. A shell command runs after a data quality check in a Cloud Composer task. What is the effect of the command in the code block?

```bash
echo 'Quality check failed' && exit 1
```

- [ ] **A)** It stops the pipeline with an error
- [ ] **B)** It restarts the pipeline
- [ ] **C)** It logs a warning and continues
- [ ] **D)** It deletes the output data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The exit 1 command terminates the script with a nonzero status. This signals that quality validation failed and stops the pipeline from continuing with bad data.
 
 
</details>

### 22. What mechanism in Google Cloud controls which users or services are allowed to access data resources and perform actions?

- [ ] **A)** IAM roles
- [ ] **B)** Dataflow jobs
- [ ] **C)** Cloud Scheduler
- [ ] **D)** BigQuery slots

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Identity and Access Management (IAM) controls who can perform actions on resources. Configuring IAM roles is a core part of governing Google Cloud data assets.
 
 
</details>

### 23. Which two actions should be taken when loading data into a data lake to avoid introducing poor-quality data? Choose two.

- [ ] **A)** Validate schema on ingest
- [ ] **B)** Check for nulls and duplicates
- [ ] **C)** Skip data type checks
- [ ] **D)** Ignore record source

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Validating schemas and checking nulls or duplicates at ingestion prevents bad data from entering the lake. Skipping checks or ignoring source produces lower-quality datasets.
 
 
</details>

### 24. What does the gcloud command in the code block retrieve from Cloud Monitoring when a data engineer executes it?

```bash
gcloud monitoring metrics list --filter="metric.type:dataflow.googleapis.com/job/error_count"
```

- [ ] **A)** Dataflow job errors
- [ ] **B)** Pub/Sub message backlogs
- [ ] **C)** Cloud Storage bucket sizes
- [ ] **D)** BigQuery slot usage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The gcloud command filters metrics by the Dataflow job error_count metric descriptor. It returns information about errors in Dataflow jobs, which is useful for quality monitoring.
 
 
</details>


---

### **Operationalizing machine learning models**

### 25. What is the primary purpose of the Vertex AI Feature Store on the Google Cloud platform?

- [ ] **A)** Central repository for storing, sharing, and reusing ML features
- [ ] **B)** Tool for manually labeling large training datasets
- [ ] **C)** Service for creating custom visualization dashboards
- [ ] **D)** Infrastructure for running SQL queries on transactional data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Vertex AI Feature Store provides a centralized place to store, share, and reuse ML features, reducing duplicate engineering work and supporting online and offline serving.
 
 
</details>

### 26. Which practices are recommended when operationalizing machine learning models on the Google Cloud platform in production?

- [ ] **A)** Automating retraining using Vertex AI Pipelines
- [ ] **B)** Registering model artifacts in Vertex AI Model Registry
- [ ] **C)** Monitoring model performance and data drift
- [ ] **D)** Deploying directly from local notebooks without version tracking

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Operationalization relies on automation, versioning, and monitoring. MLOps best practices include pipeline automation, central model registry, and continuous drift monitoring.
 
 
</details>

### 27. Analyze the Python snippet and identify the parameter that defines the target endpoint for online prediction.

```python
from google.cloud import aiplatform

endpoint = aiplatform.Endpoint(
    endpoint_name="projects/my-project/locations/us-central1/endpoints/123"
)
prediction = endpoint.predict(instances=[{"feature1": 1.0, "feature2": 2.0}])

```

- [ ] **A)** endpoint_name
- [ ] **B)** instances
- [ ] **C)** predict
- [ ] **D)** aiplatform

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The endpoint_name argument passes the fully qualified endpoint resource path, determining which deployed model receives the online prediction request.
 
 
</details>

### 28. What is the main purpose of using batch prediction in Vertex AI on Google Cloud?

- [ ] **A)** Generating predictions for a large dataset asynchronously
- [ ] **B)** Serving real-time predictions with minimal latency
- [ ] **C)** Training models on tabular data
- [ ] **D)** Visualizing model evaluation metrics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Batch prediction processes large amounts of data offline and asynchronously, making it suitable for jobs that do not require immediate responses.
 
 
</details>

### 29. Which items can be associated with a model version in Vertex AI Model Registry on Google Cloud?

- [ ] **A)** Model artifact
- [ ] **B)** Serving container
- [ ] **C)** Version alias
- [ ] **D)** BigQuery destination table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A model version includes the serialized model artifact, a serving container specification, and optional version aliases that support safe deployment and serving.
 
 
</details>

### 30. Analyze the JSON configuration and identify the field that specifies the source of the input data for a batch prediction job.

```json
{
  "model": "projects/project/models/model_id",
  "inputConfig": {
    "instancesFormat": "jsonl",
    "inputPath": "gs://bucket/input.jsonl"
  },
  "outputConfig": {
    "predictionsFormat": "jsonl",
    "outputPath": "gs://bucket/output"
  }
}
```

- [ ] **A)** inputPath
- [ ] **B)** outputPath
- [ ] **C)** model
- [ ] **D)** predictionsFormat

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The inputPath field points to the storage location of the input data, allowing the batch prediction job to read instances from the specified path.
 
 
</details>

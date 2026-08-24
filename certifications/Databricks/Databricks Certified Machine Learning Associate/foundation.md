<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Databricks/Databricks%20Certified%20Machine%20Learning%20Associate.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Databricks Certified Machine Learning Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Databricks Machine Learning](#databricks-machine-learning) (11 questions)
- [ML Workflows](#ml-workflows) (6 questions)
- [Model Deployment](#model-deployment) (4 questions)
- [Model Development](#model-development) (9 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:51:59.231Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Databricks Machine Learning | 11 |
| ML Workflows | 6 |
| Model Deployment | 4 |
| Model Development | 9 |

---

### **Databricks Machine Learning**

### 1. What is the primary purpose of the Machine Learning persona in the Databricks workspace?

- [ ] **A)** A tailored UI that surfaces ML assets
- [ ] **B)** A separate compute cluster for ML workloads
- [ ] **C)** An automatic model deployment service
- [ ] **D)** A cloud storage account for datasets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Machine Learning persona changes workspace navigation to highlight ML-specific assets; it does not provision compute or deployment resources.
 
 
</details>

### 2. Which ML-specific assets appear in the left navigation sidebar when using the Databricks Machine Learning persona? (Select all that apply.)

- [ ] **A)** Experiments
- [ ] **B)** Models
- [ ] **C)** Feature Store
- [ ] **D)** SQL warehouses

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The Machine Learning persona surfaces Experiments, Models, and Feature Store in the left navigation; SQL warehouses are not part of this ML asset set.
 
 
</details>

### 3. The code snippet in the code block sets a custom tracking URI inside a Databricks notebook. What is the recommended action?

```python
mlflow.set_tracking_uri("http://localhost:5000")
```

- [ ] **A)** Remove it and use the managed tracking server
- [ ] **B)** Keep it for all runs
- [ ] **C)** Replace localhost with a cloud database
- [ ] **D)** Use it only for model registry operations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Databricks provides a managed MLflow tracking server; hardcoding a tracking URI overrides the default and is not recommended.
 
 
</details>

### 4. What is the Databricks Runtime for Machine Learning?

- [ ] **A)** A cluster environment pre-loaded with ML libraries
- [ ] **B)** A standard runtime with no pre-installed packages
- [ ] **C)** A tool for manually managing CUDA drivers
- [ ] **D)** A cloud object storage service for models

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> DBR for ML is a preconfigured runtime with libraries such as TensorFlow, PyTorch, scikit-learn, and MLflow included.
 
 
</details>

### 5. Which libraries are pre-installed in the Databricks Runtime for Machine Learning? (Select all that apply.)

- [ ] **A)** TensorFlow
- [ ] **B)** PyTorch
- [ ] **C)** XGBoost
- [ ] **D)** PostgreSQL JDBC driver

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> DBR for ML includes TensorFlow, PyTorch, scikit-learn, XGBoost, and MLflow out of the box.
 
 
</details>

### 6. The code block shows a manual package installation step on a standard cluster. What is the recommended alternative for a machine learning workload?

```python
pip install tensorflow torch xgboost
```

- [ ] **A)** Use a Databricks Runtime for Machine Learning cluster
- [ ] **B)** Keep the install script
- [ ] **C)** Run the install on every node manually
- [ ] **D)** Switch to CPU-only instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The recommended best practice is to use DBR for ML, which already bundles the required ML libraries and avoids manual dependency management.
 
 
</details>

### 7. Which Databricks feature integrates Git version control directly into the workspace for notebooks and code?

- [ ] **A)** Databricks Repos
- [ ] **B)** DBFS
- [ ] **C)** Notebook export
- [ ] **D)** Cluster Policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Databricks Repos provides native Git integration, allowing users to clone, branch, pull, push, and manage code inside the workspace.
 
 
</details>

### 8. Which Git providers can be linked to Databricks Repos according to the documentation? (Select all that apply.)

- [ ] **A)** GitHub
- [ ] **B)** GitLab
- [ ] **C)** Bitbucket
- [ ] **D)** Microsoft Word

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Databricks Repos supports Git providers such as GitHub, GitLab, and Bitbucket; Microsoft Word is not a Git provider.
 
 
</details>

### 9. The code block shows a CLI command a user is considering for bringing a repository into Databricks. What is the correct approach?

```bash
git clone https://github.com/org/repo.git
```

- [ ] **A)** Use Databricks Repos to clone the repository
- [ ] **B)** Upload the repository as a notebook
- [ ] **C)** Manually copy code into workspace folders
- [ ] **D)** Use DBFS CLI to sync the repository

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Databricks Repos provides native Git cloning and synchronization, so users do not need to run external Git CLI commands.
 
 
</details>

### 10. What is an MLflow Experiment?

- [ ] **A)** A logical grouping of runs
- [ ] **B)** A single training execution
- [ ] **C)** A registered model version
- [ ] **D)** A deployment endpoint

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An MLflow Experiment groups runs by use case or project, allowing users to compare parameters, metrics, and artifacts.
 
 
</details>

### 11. Which capabilities are provided by the MLflow Model Registry? (Select all that apply.)

- [ ] **A)** Model versioning
- [ ] **B)** Stage transitions
- [ ] **C)** CI/CD webhooks
- [ ] **D)** Editing source datasets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The MLflow Model Registry supports versioning, stage transitions, webhooks, and governance, but it does not edit source datasets.
 
 
</details>


---

### **ML Workflows**

### 12. What does an MLflow Project provide for packaging reusable machine learning code?

- [ ] **A)** A standard format for code, configuration files, and dependency definitions
- [ ] **B)** A method for manually linking notebooks in sequence
- [ ] **C)** An external scheduler for cloud infrastructure
- [ ] **D)** A storage format for large datasets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MLflow Projects package reusable data science code with configuration files and dependency definitions so that the same code can run consistently across environments.
 
 
</details>

### 13. Which two Databricks components are essential for building reproducible multi-step ML pipelines?

- [ ] **A)** MLflow Projects
- [ ] **B)** Databricks Jobs
- [ ] **C)** Interactive notebooks only
- [ ] **D)** Hardcoded workspace file paths

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> MLflow Projects define entry points and dependencies, while Databricks Jobs orchestrate tasks in production. Manual notebook linking and hardcoded paths are not reproducible pipeline best practices.
 
 
</details>

### 14. Examine the provided code snippet. Which MLflow concept is being defined?

```yaml
name: fraud-pipeline
entry_points:
  main:
    parameters:
      data_path: {type: string}
    command: "python run.py --data-path {data_path}"
```

- [ ] **A)** An MLflow Project entry point
- [ ] **B)** A Databricks Job task DAG
- [ ] **C)** A Feature Store primary key definition
- [ ] **D)** A Model Registry stage transition

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code defines an MLproject file with a parameterized entry point, which is the standard format used by MLflow Projects.
 
 
</details>

### 15. What is the main purpose of point-in-time correctness in the Databricks Feature Store?

- [ ] **A)** To prevent data leakage by joining features valid at the exact event timestamp
- [ ] **B)** To increase model training speed on large datasets
- [ ] **C)** To automatically remove duplicate rows from feature tables
- [ ] **D)** To manually configure cluster autoscaling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Point-in-time correctness performs time-travel joins between historical observations and feature values, preventing future feature data from leaking into training sets.
 
 
</details>

### 16. Which two practices are recommended when managing feature tables in Databricks?

- [ ] **A)** Specify primary keys when creating feature tables
- [ ] **B)** Use the FeatureStoreClient to write and read feature tables
- [ ] **C)** Read tables directly with spark.read.table for all operations
- [ ] **D)** Skip timestamp handling when joining features for training

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Primary keys are mandatory for joins and online lookups, and the FeatureStoreClient preserves metadata for automated serving. Direct Spark reads and ignoring timestamps break feature store functionality.
 
 
</details>

### 17. Look at the code snippet. What is the role of the primary_keys argument?

```python
from databricks.feature_store import FeatureStoreClient
fs = FeatureStoreClient()
fs.create_table(
    name="ml.features.customer_features",
    primary_keys=["customer_id"],
    schema=feature_df.schema
)
```

- [ ] **A)** It enables point-in-time joins and online feature lookups
- [ ] **B)** It specifies the cluster size for the feature table
- [ ] **C)** It determines the MLflow experiment name
- [ ] **D)** It selects the model registry stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Primary keys are required for point-in-time joins and automated online feature retrieval when serving models registered with Feature Store metadata.
 
 
</details>


---

### **Model Deployment**

### 18. Which Databricks capability is designed for automated, scheduled execution of machine learning models to score large datasets and store predictions in Delta Lake?

- [ ] **A)** Batch inference pipelines
- [ ] **B)** Real-time model serving endpoints
- [ ] **C)** Unity Catalog
- [ ] **D)** MLflow experiment tracking

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Batch inference pipelines score large data volumes on a schedule and store predictions in Delta Lake, unlike real-time endpoints.
 
 
</details>

### 19. Which two statements accurately describe how Databricks Lakehouse Monitoring helps track production models? Choose two.

- [ ] **A)** Automatically profiles data and logs metrics to Delta
- [ ] **B)** Detects data drift and concept drift
- [ ] **C)** Requires an external monitoring tool
- [ ] **D)** Stores prediction logs in MLflow Model Registry

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Lakehouse Monitoring automatically profiles data, detects drift against a baseline, and writes metrics to Delta tables natively.
 
 
</details>

### 20. The code block below is used to perform which primary task in a Databricks batch inference workflow?

```python
import mlflow
from pyspark.sql.functions import struct

model_uri = "models:/recommendation_model/@champion"
loaded_model = mlflow.pyfunc.spark_udf(spark, model_uri)
predictions_df = df.withColumn("prediction", loaded_model(struct(*df.columns)))
predictions_df.write.format("delta").mode("append").save("/mnt/delta/recommendations")
```

- [ ] **A)** Batch scoring with a Spark UDF
- [ ] **B)** Real-time REST API serving
- [ ] **C)** Model registry registration
- [ ] **D)** Training a new model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code loads an MLflow model as a Spark UDF and writes scored predictions to a Delta Lake table.
 
 
</details>

### 21. In MLflow, what happens automatically each time a model is registered under an existing registered model name?

- [ ] **A)** The model version number is incremented
- [ ] **B)** The model is promoted to Production
- [ ] **C)** The previous model version is deleted
- [ ] **D)** A serving endpoint is created

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Registering under an existing model name increments the version number, preserving earlier versions for auditability and rollback.
 
 
</details>


---

### **Model Development**

### 22. Which technology is used for distributed feature engineering at scale on Databricks?

- [ ] **A)** Apache Spark
- [ ] **B)** Pandas
- [ ] **C)** Scikit-learn
- [ ] **D)** Excel

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Apache Spark processes data across worker nodes, enabling scalable feature engineering. Single-node tools like Pandas are unsuitable for massive datasets.
 
 
</details>

### 23. Which actions are common traps during large-scale data preparation in Databricks?

- [ ] **A)** Calling .toPandas() on a huge distributed DataFrame
- [ ] **B)** Fitting scalers before splitting into training and validation sets
- [ ] **C)** Using Delta Lake schema enforcement
- [ ] **D)** Using Spark MLlib transformers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Collecting Spark data to the driver and fitting global transformations before splitting are common causes of OOM and data leakage.
 
 
</details>

### 24. What issue is likely when executing the displayed code on a 500 GB Delta table?

```python
driver_df = spark.table('transactions').toPandas()
```

- [ ] **A)** Driver out-of-memory
- [ ] **B)** Data leakage
- [ ] **C)** Model underfitting
- [ ] **D)** Network latency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Calling .toPandas() moves all data to the driver, which easily exhausts driver memory on multi-terabyte tables.
 
 
</details>

### 25. For a tabular dataset that fits in one node's memory, which library is most appropriate?

- [ ] **A)** Scikit-learn
- [ ] **B)** Spark MLlib
- [ ] **C)** Horovod
- [ ] **D)** Delta Lake

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Scikit-learn is ideal for in-memory tabular data. Spark MLlib is only necessary when data exceeds single-node memory.
 
 
</details>

### 26. Which frameworks are described as distributed training options in the Databricks ecosystem?

- [ ] **A)** Horovod
- [ ] **B)** PyTorch Lightning
- [ ] **C)** Spark MLlib
- [ ] **D)** Single-node XGBoost

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Horovod, PyTorch Lightning, and Spark MLlib support distributed training. Single-node XGBoost runs locally unless integrated with distributed backends.
 
 
</details>

### 27. Why is the displayed Hyperopt configuration inappropriate for a multi-node Databricks cluster?

```python
best = fmin(fn, space, algo=tpe.suggest, trials=Trials(), max_evals=100)
```

- [ ] **A)** Uses Trials instead of SparkTrials
- [ ] **B)** Uses too many evaluations
- [ ] **C)** Specifies an invalid search space
- [ ] **D)** Forgets to log to MLflow

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Hyperopt requires SparkTrials as the backend to distribute trials across cluster workers; standard Trials stays on the driver.
 
 
</details>

### 28. What does MLflow automatically record for each Hyperopt trial?

- [ ] **A)** Parameters, metrics, and artifacts
- [ ] **B)** Only model predictions
- [ ] **C)** Only the model weights
- [ ] **D)** No run information

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MLflow logs parameters, metrics, and artifacts for every trial, enabling comparison, reproduction, and best-model selection.
 
 
</details>

### 29. Which metrics are recommended for evaluating an imbalanced classification model?

- [ ] **A)** Precision
- [ ] **B)** Recall
- [ ] **C)** F1-score
- [ ] **D)** Accuracy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Precision, recall, and F1-score account for minority-class performance; accuracy is misleading when classes are imbalanced.
 
 
</details>

### 30. What is the effect of executing the displayed code in a Databricks notebook?

```python
with mlflow.start_run():
    mlflow.log_metric('f1', 0.87)
```

- [ ] **A)** Logs the F1 metric to the current MLflow run
- [ ] **B)** Trains a classifier
- [ ] **C)** Registers a model to Unity Catalog
- [ ] **D)** Deletes the current run

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet starts an MLflow run and logs a metric named f1 with value 0.87 to that run.
 
 
</details>

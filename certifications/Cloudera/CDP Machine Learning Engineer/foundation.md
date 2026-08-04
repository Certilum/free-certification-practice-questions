<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cloudera/CDP%20Certified%20Machine%20Learning%20Engineer" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>CDP Machine Learning Engineer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Data Engineering for ML](#data-engineering-for-ml) (7 questions)
- [Machine Learning Operations (MLOps)](#machine-learning-operations-mlops) (6 questions)
- [Machine Learning Pipeline Design](#machine-learning-pipeline-design) (10 questions)
- [Model Deployment and Serving](#model-deployment-and-serving) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:21.616Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Data Engineering for ML | 7 |
| Machine Learning Operations (MLOps) | 6 |
| Machine Learning Pipeline Design | 10 |
| Model Deployment and Serving | 7 |

---

### **Data Engineering for ML**

### 1. Which CDP source is specifically designed for fast analytics on rapidly changing data?

- [ ] **A)** Apache Hive
- [ ] **B)** HDFS
- [ ] **C)** Apache Kudu
- [ ] **D)** Apache Impala

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Kudu is built for fast analytics on changing data, offering upserts and low-latency scans.
 
 
</details>

### 2. Which two data extraction strategies are recommended for production ML pipelines in CDP?

- [ ] **A)** Performing full table scans daily
- [ ] **B)** Using partition pruning in Hive queries
- [ ] **C)** Pulling only incremental changes (delta extraction)
- [ ] **D)** Extracting raw HDFS files directly with hdfs dfs -get

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Partition pruning and incremental extraction reduce I/O and resource usage in production ML pipelines.
 
 
</details>

### 3. Examine the Hive query below. What is missing to make it efficient for large-scale extraction?

```sql
SELECT user_id, amount, event FROM user_activity WHERE year = 2025;
```

- [ ] **A)** A partition filter on the 'dt' column
- [ ] **B)** A LIMIT clause
- [ ] **C)** A DISTINCT keyword
- [ ] **D)** A JOIN with a smaller table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Without a partition filter (e.g., WHERE dt='2025-03-01'), Hive scans all partitions, causing poor performance.
 
 
</details>

### 4. Which CDP tool is best suited for interactive data profiling and lightweight corrections on Kudu tables?

- [ ] **A)** Apache Spark
- [ ] **B)** Apache Impala
- [ ] **C)** Apache Hive
- [ ] **D)** Apache NiFi

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Impala offers interactive SQL with low latency and supports UPDATE/DELETE on Kudu tables, ideal for ad hoc data cleaning.
 
 
</details>

### 5. Which two Spark DataFrame methods are commonly used to handle missing values?

- [ ] **A)** dropna()
- [ ] **B)** fillna()
- [ ] **C)** UPDATE FROM Kudu
- [ ] **D)** DELETE FROM Hive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Spark provides dropna() to remove rows with nulls and fillna() to replace nulls with a value.
 
 
</details>

### 6. Given the Spark SQL code that imputes median values, what is the effect on the feature's variance?

```sql
SELECT COALESCE(salary, MEDIAN(salary) OVER()) AS salary FROM employees;
```

- [ ] **A)** Variance increases
- [ ] **B)** Variance decreases
- [ ] **C)** Variance remains unchanged
- [ ] **D)** Variance becomes zero

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Imputing with the median concentrates values around the median, reducing overall variance of the column.
 
 
</details>

### 7. When missingness of a variable depends on other observed variables, the mechanism is called:

- [ ] **A)** Missing Completely at Random (MCAR)
- [ ] **B)** Missing at Random (MAR)
- [ ] **C)** Missing Not at Random (MNAR)
- [ ] **D)** Missing by Design (MBD)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> MAR occurs when missingness is related to observed variables but not the missing value itself.
 
 
</details>


---

### **Machine Learning Operations (MLOps)**

### 8. What does the acronym CI/CD represent in machine learning operations?

- [ ] **A)** Continuous Integration and Continuous Delivery
- [ ] **B)** Continuous Integration and Continuous Deployment
- [ ] **C)** Code Integration and Code Deployment
- [ ] **D)** Continuous Improvement and Development

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CI/CD stands for Continuous Integration and Continuous Delivery, automating code, data, and model changes from development to production.
 
 
</details>

### 9. Select two components that are part of the MLflow model registry.

- [ ] **A)** Model versions
- [ ] **B)** Experiment runs
- [ ] **C)** Stage transitions
- [ ] **D)** Model training code

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The MLflow model registry manages model versions and stage transitions. Experiment runs are tracked separately by MLflow Tracking.
 
 
</details>

### 10. Which method logs a hyperparameter during an MLflow experiment run?

```python
mlflow.log_param("learning_rate", 0.01)
```

- [ ] **A)** mlflow.log_param
- [ ] **B)** mlflow.log_metric
- [ ] **C)** mlflow.set_tag
- [ ] **D)** mlflow.log_artifact

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The mlflow.log_param() function is used to log key-value parameters such as learning rate.
 
 
</details>

### 11. What type of trigger is used when retraining is started after model accuracy drops below a threshold?

- [ ] **A)** Performance-driven trigger
- [ ] **B)** Time-based trigger
- [ ] **C)** Data-driven trigger
- [ ] **D)** Event-driven trigger

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A performance-driven trigger retrains the model when its metrics fall below a defined threshold, such as accuracy dropping below 85%.
 
 
</details>

### 12. Select two capabilities of Apache Ranger for securing ML workflows.

- [ ] **A)** Fine-grained access control
- [ ] **B)** Data lineage tracking
- [ ] **C)** Column-level masking
- [ ] **D)** Model versioning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Apache Ranger provides fine-grained access control and dynamic data masking. Data lineage is provided by Apache Atlas.
 
 
</details>

### 13. From the given stages, select two that are standard in an ML CI/CD pipeline.

```python
pipeline_stages = ["Data Validation", "Model Training", "Canary Deployment", "Full Production"]
```

- [ ] **A)** Data Validation
- [ ] **B)** Code Compilation
- [ ] **C)** Canary Deployment
- [ ] **D)** Manual Testing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Typical ML CI/CD pipelines include Data Validation and Canary Deployment stages to ensure quality and safe rollout.
 
 
</details>


---

### **Machine Learning Pipeline Design**

### 14. Which component in Cloudera CDP is primarily used for streaming data ingestion with low latency?

- [ ] **A)** Apache Kafka
- [ ] **B)** Apache NiFi
- [ ] **C)** Apache Spark
- [ ] **D)** Apache Hive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Apache Kafka is the primary streaming engine in CDP, offering a durable, partitioned log for low-latency data ingestion.
 
 
</details>

### 15. Which tools are suitable for scheduled batch data ingestion in CDP? (Choose two.)

- [ ] **A)** Apache Spark
- [ ] **B)** Apache Hive
- [ ] **C)** Apache Kafka
- [ ] **D)** Apache NiFi

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Apache Spark and Hive on Tez are used for batch processing; Kafka and NiFi are primarily for streaming.
 
 
</details>

### 16. Refer to the code block. What is the role of the StringIndexer transformer?

```python
from pyspark.ml.feature import StringIndexer
indexer = StringIndexer(inputCol="category", outputCol="categoryIndex")
```

- [ ] **A)** Converts string column to numeric indices
- [ ] **B)** Scales numeric features to unit variance
- [ ] **C)** Fills missing values with median
- [ ] **D)** Creates interaction terms

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> StringIndexer encodes a string column to a column of indices, commonly used for categorical features.
 
 
</details>

### 17. What is the primary goal of feature selection in machine learning pipelines?

- [ ] **A)** Reduce dimensionality and overfitting
- [ ] **B)** Increase model complexity
- [ ] **C)** Add more raw data
- [ ] **D)** Speed up data ingestion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Feature selection reduces dimensionality and mitigates overfitting by keeping only relevant features.
 
 
</details>

### 18. Which techniques are commonly used to handle missing values in feature engineering? (Select all that apply.)

- [ ] **A)** Impute with mean
- [ ] **B)** Drop rows with missing values
- [ ] **C)** Add a missing value indicator column
- [ ] **D)** Fill with zeros

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Common handling includes imputation, dropping rows, and adding indicators; filling with zeros can introduce bias.
 
 
</details>

### 19. Refer to the code block. What metric is being calculated by the evaluator?

```python
from pyspark.ml.evaluation import BinaryClassificationEvaluator
evaluator = BinaryClassificationEvaluator(metricName="areaUnderROC")
```

- [ ] **A)** AUC-ROC
- [ ] **B)** Precision
- [ ] **C)** Recall
- [ ] **D)** F1-Score

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code uses BinaryClassificationEvaluator with metricName='areaUnderROC', which computes AUC-ROC.
 
 
</details>

### 20. In Apache Airflow, what does the acronym DAG stand for?

- [ ] **A)** Directed Acyclic Graph
- [ ] **B)** Data Aggregation Group
- [ ] **C)** Dynamic Application Grid
- [ ] **D)** Distributed Algorithm Gateway

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> DAG stands for Directed Acyclic Graph, the core abstraction for defining task dependencies in Airflow.
 
 
</details>

### 21. Which components are essential for automating ML pipelines in CDP? (Select two.)

- [ ] **A)** Model Registry
- [ ] **B)** Feature Store
- [ ] **C)** Data Profiling
- [ ] **D)** Manual Deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Model Registry and Feature Store are essential for versioning, lineage, and consistency in automated pipelines.
 
 
</details>

### 22. Refer to the code block. What is the purpose of the randomSplit method?

```python
train, test = df.randomSplit([0.8, 0.2], seed=42)
```

- [ ] **A)** Split data into training and test sets
- [ ] **B)** Scale features
- [ ] **C)** Handle missing values
- [ ] **D)** Encode categorical variables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> randomSplit is used to randomly split a DataFrame into two or more subsets, often for training and testing.
 
 
</details>

### 23. Which Spark MLlib transformer converts a categorical string column to numeric indices?

- [ ] **A)** StringIndexer
- [ ] **B)** OneHotEncoder
- [ ] **C)** VectorAssembler
- [ ] **D)** StandardScaler

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> StringIndexer converts string input to integer indices, commonly the first step for categorical features.
 
 
</details>


---

### **Model Deployment and Serving**

### 24. What is the primary purpose of model serialization in the ML lifecycle?

- [ ] **A)** To compress model artifacts for storage efficiency
- [ ] **B)** To capture the complete state of a trained model into a portable format
- [ ] **C)** To increase the speed of model training iterations
- [ ] **D)** To automatically deploy the model to a Kubernetes cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Model serialization saves the entire model state (architecture, parameters, metadata) into a durable format, enabling reproducibility and deployment.
 
 
</details>

### 25. Which of the following are features of CDSW model deployments? (Select two)

- [ ] **A)** Automatic containerization of model code and dependencies
- [ ] **B)** Requires manual creation of Docker images
- [ ] **C)** Supports canary releases with traffic splitting
- [ ] **D)** Deployments are stateful and preserve session data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> CDSW automatically packages the model into a container and supports canary releases for gradual rollouts. It is stateless and does not require manual Docker builds.
 
 
</details>

### 26. Review the code snippet below. What is the purpose of the `predict()` function defined inside `Model` class?

```python
class Model:
    def __init__(self):
        self.model = joblib.load('model.pkl')
    def predict(self, features):
        return self.model.predict(features)
```

- [ ] **A)** It loads the model from disk each time a request is received
- [ ] **B)** It is the inference function that will be exposed as the REST API endpoint
- [ ] **C)** It trains the model with incoming data
- [ ] **D)** It serializes the model into ONNX format

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The `predict` function is the core inference method. CDSW deployments call this function to return a prediction for an input payload.
 
 
</details>

### 27. What type of drift occurs when the distribution of input features changes over time?

- [ ] **A)** Concept drift
- [ ] **B)** Data drift
- [ ] **C)** Model drift
- [ ] **D)** Upstream drift

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Data drift (or covariate shift) is the change in the distribution of input features, while concept drift refers to a change in the relationship between inputs and outputs.
 
 
</details>

### 28. Which of the following are components of scaling inference in CDP? (Select two)

- [ ] **A)** Horizontal Pod Autoscaling (HPA) based on CPU or custom metrics
- [ ] **B)** Static model parallelism across multiple GPUs
- [ ] **C)** Serverless endpoints that can scale to zero when idle
- [ ] **D)** Training data pipeline optimization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> HPA and serverless (Knative) are CDP-native scaling methods. Model parallelism is for training, not serving. Data pipelines are separate from inference scaling.
 
 
</details>

### 29. Examine the MLflow logging code. What flavor is used for the logged model?

```python
import mlflow.pyfunc
mlflow.pyfunc.log_model(artifact_path='model', python_model=MyWrapper())
```

- [ ] **A)** python_function
- [ ] **B)** sklearn
- [ ] **C)** tensorflow
- [ ] **D)** pytorch

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> `mlflow.pyfunc.log_model` logs a `python_function` flavor, which wraps any Python model with a standard predict interface.
 
 
</details>

### 30. What is the first step when deploying a model from CDSW to a Kubernetes production cluster?

- [ ] **A)** Export the model artifact and create a Docker image
- [ ] **B)** Apply the Kubernetes deployment YAML directly from CDSW
- [ ] **C)** Schedule a CML job to run the model as a batch job
- [ ] **D)** Create a new CDSW project and retrain the model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The model must first be exported and containerized before it can be deployed to Kubernetes. CDSW does not directly push to Kubernetes.
 
 
</details>

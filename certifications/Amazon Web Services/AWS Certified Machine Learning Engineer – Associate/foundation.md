<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Amazon%20Web%20Services%20Training%20and%20Certification/AWS%20Certified%20Machine%20Learning%20Engineer%20–%20Associate" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>AWS Certified Machine Learning Engineer – Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Data Preparation for Machine Learning](#data-preparation-for-machine-learning) (5 questions)
- [Deployment and Orchestration](#deployment-and-orchestration) (8 questions)
- [ML Operations (MLOps)](#ml-operations-mlops) (5 questions)
- [ML Security and Compliance](#ml-security-and-compliance) (4 questions)
- [Model Development](#model-development) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:31.432Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Data Preparation for Machine Learning | 5 |
| Deployment and Orchestration | 8 |
| ML Operations (MLOps) | 5 |
| ML Security and Compliance | 4 |
| Model Development | 8 |

---

### **Data Preparation for Machine Learning**

### 1. Which AWS service is commonly used as a central data lake for ML data ingestion?

- [ ] **A)** Amazon S3
- [ ] **B)** Amazon Kinesis
- [ ] **C)** Amazon Redshift
- [ ] **D)** AWS Glue

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Amazon S3 is the most common target for ML data ingestion due to its durability, scalability, and low cost.
 
 
</details>

### 2. Which two AWS services are used for real-time streaming data ingestion? (Select TWO)

- [ ] **A)** Amazon Kinesis Data Streams
- [ ] **B)** Amazon Kinesis Data Firehose
- [ ] **C)** Amazon S3
- [ ] **D)** Amazon Redshift COPY

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Kinesis Data Streams and Kinesis Data Firehose are primary services for ingesting streaming data in real-time.
 
 
</details>

### 3. Examine the code snippet below. Which step is missing before this normalization can be applied to test data?

```python
from sklearn.preprocessing import StandardScaler
import pandas as pd

train_df = pd.read_csv('s3://bucket/train.csv')
scaler = StandardScaler()
train_scaled = scaler.fit_transform(train_df)

# Missing step: save scaler to S3
```

- [ ] **A)** Saving the fitted scaler to S3
- [ ] **B)** Shuffling the test data
- [ ] **C)** One-hot encoding categories
- [ ] **D)** Dropping duplicates first

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The fitted scaler must be saved to S3 so it can be loaded and applied to test data during inference.
 
 
</details>

### 4. What is the purpose of using a validation set during model training?

- [ ] **A)** To evaluate final model performance
- [ ] **B)** To tune hyperparameters and early stop
- [ ] **C)** To train the model parameters
- [ ] **D)** To generate synthetic data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The validation set guides hyperparameter tuning and early stopping without influencing the final test evaluation.
 
 
</details>

### 5. Which techniques can be used to handle missing values in a dataset? (Select TWO)

- [ ] **A)** Mean imputation
- [ ] **B)** Dropping rows
- [ ] **C)** Adding random noise
- [ ] **D)** Increasing sample size

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Mean imputation and dropping rows are basic but effective ways to handle missing values, depending on the pattern.
 
 
</details>


---

### **Deployment and Orchestration**

### 6. What is the primary purpose of Amazon SageMaker real-time endpoints?

- [ ] **A)** To process large datasets asynchronously
- [ ] **B)** To serve predictions with low latency on a per-request basis
- [ ] **C)** To train models using batch data
- [ ] **D)** To store model artifacts in a versioned repository

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Real-time endpoints provide a persistent HTTPS endpoint for low-latency, synchronous predictions, ideal for customer-facing applications.
 
 
</details>

### 7. Which two statements are true about SageMaker Serverless Inference? (Choose two.)

- [ ] **A)** It supports GPU instances for deep learning
- [ ] **B)** It automatically scales to zero when idle
- [ ] **C)** It requires you to specify an instance type
- [ ] **D)** It charges per inference request and compute time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Serverless Inference auto-scales to zero, has no idle cost, and charges per request + compute. It does not support GPU or require instance type selection.
 
 
</details>

### 8. Refer to the code snippet. What SageMaker resource is being created?

```python
import boto3

sagemaker = boto3.client('sagemaker')
response = sagemaker.create_endpoint_config(
    EndpointConfigName='my-endpoint-config',
    ProductionVariants=[
        {
            'VariantName': 'v1',
            'ModelName': 'my-model',
            'InstanceType': 'ml.m5.large',
            'InitialInstanceCount': 2
        }
    ]
)
```

- [ ] **A)** A SageMaker Model
- [ ] **B)** An Endpoint Configuration
- [ ] **C)** A Transform Job
- [ ] **D)** A Monitoring Schedule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code creates an EndpointConfiguration resource with a production variant, including instance type and model ARN.
 
 
</details>

### 9. What is the purpose of the BatchStrategy parameter in a SageMaker Batch Transform job?

- [ ] **A)** It defines the maximum payload size
- [ ] **B)** It determines whether records are sent singly or in multi-record batches
- [ ] **C)** It sets the number of concurrent transform instances
- [ ] **D)** It specifies the output S3 bucket path

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> BatchStrategy controls how records are grouped: SingleRecord sends each record individually, MultiRecord sends multiple records together.
 
 
</details>

### 10. Which two AWS services can be used to trigger a SageMaker Batch Transform job? (Choose two.)

- [ ] **A)** AWS Lambda
- [ ] **B)** Amazon CloudWatch Logs
- [ ] **C)** Amazon EventBridge
- [ ] **D)** AWS CloudFormation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Lambda and EventBridge can invoke Batch Transform via SDK or scheduled rules. CloudWatch Logs does not directly trigger jobs; CloudFormation provisions infrastructure.
 
 
</details>

### 11. Examine the code. What does this AWS Lambda function do?

```python
import boto3

def lambda_handler(event, context):
    sagemaker = boto3.client('sagemaker')
    response = sagemaker.create_transform_job(
        TransformJobName='batch-job-001',
        ModelName='my-model',
        TransformInput={
            'DataSource': {
                'S3DataSource': {
                    'S3DataType': 'S3Prefix',
                    'S3Uri': 's3://bucket/input/'
                }
            },
            'ContentType': 'text/csv'
        },
        TransformOutput={
            'S3OutputPath': 's3://bucket/output/'
        },
        TransformResources={
            'InstanceType': 'ml.m5.large',
            'InstanceCount': 1
        }
    )
    return response
```

- [ ] **A)** It creates a SageMaker endpoint
- [ ] **B)** It starts a SageMaker training job
- [ ] **C)** It initiates a SageMaker Batch Transform job
- [ ] **D)** It updates an endpoint configuration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Lambda calls create_transform_job with parameters for batch inference, indicating it is starting a transform job.
 
 
</details>

### 12. In AWS MLOps, which service is designed specifically to orchestrate machine learning workflows?

- [ ] **A)** AWS CodePipeline
- [ ] **B)** Amazon SageMaker Pipelines
- [ ] **C)** AWS Step Functions
- [ ] **D)** AWS CodeBuild

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SageMaker Pipelines is purpose-built for ML workflows, handling training, evaluation, and registration steps via a DAG.
 
 
</details>

### 13. Which two components are part of a SageMaker Model Registry workflow? (Choose two.)

- [ ] **A)** Register a model version with metadata
- [ ] **B)** Deploy a model directly from the registry without a Model object
- [ ] **C)** Set an approval status for a model version
- [ ] **D)** Run a Batch Transform job

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The Model Registry supports registering model versions with metadata and setting approval statuses. Deploying requires a SageMaker Model object, not direct registry deployment.
 
 
</details>


---

### **ML Operations (MLOps)**

### 14. Which AWS service is purpose-built for creating ML retraining pipelines with native steps like training and conditional evaluation?

- [ ] **A)** Amazon SageMaker Pipelines
- [ ] **B)** AWS Step Functions
- [ ] **C)** AWS Glue
- [ ] **D)** Amazon EventBridge

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Amazon SageMaker Pipelines is a fully managed CI/CD service for ML that includes native steps such as TrainingStep, ConditionStep, and RegisterModelStep, making it purpose-built for retraining pipelines.
 
 
</details>

### 15. Which two statements about Amazon SageMaker Model Registry are true? (Choose two.)

- [ ] **A)** It stores the actual model artifacts.
- [ ] **B)** It provides versioning and approval status tracking.
- [ ] **C)** It can automatically deploy approved models to endpoints.
- [ ] **D)** It integrates with SageMaker Pipelines for automated registration.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> The Model Registry stores references to model artifacts in S3, not the artifacts themselves. It tracks version and approval status but does not auto-deploy; deployment requires a separate process. It does integrate with SageMaker Pipelines via RegisterModelStep.
 
 
</details>

### 16. Refer to the code block. Which AWS service's logs are being queried?

```cloudwatch-logs-insights
fields @timestamp, @message
| filter @message like /ERROR/
| sort @timestamp desc
| limit 20
```

- [ ] **A)** AWS CloudTrail
- [ ] **B)** Amazon CloudWatch Logs
- [ ] **C)** Amazon S3 access logs
- [ ] **D)** AWS CloudTrail Insights

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The query uses CloudWatch Logs Insights syntax (fields, filter, sort, limit) and filters for error messages, indicating the log source is Amazon CloudWatch Logs.
 
 
</details>

### 17. Which instance purchasing option offers the largest discount but can be interrupted by AWS?

- [ ] **A)** On-Demand
- [ ] **B)** Spot Instances
- [ ] **C)** Reserved Instances
- [ ] **D)** Savings Plans

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Spot Instances offer the deepest discounts (up to 90%) but can be interrupted with a two-minute warning. They are ideal for fault-tolerant batch training that uses checkpointing.
 
 
</details>

### 18. Which two event types can trigger a SageMaker Pipeline execution for retraining? (Choose two.)

- [ ] **A)** New file upload to an S3 bucket
- [ ] **B)** Scheduled cron expression via EventBridge
- [ ] **C)** Change in an IAM policy
- [ ] **D)** New version registration in Model Registry

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SageMaker Pipelines can be triggered by S3 events (e.g., new data) or scheduled cron rules. IAM policy changes do not trigger pipelines, and Model Registry version creation can be an output, not a trigger.
 
 
</details>


---

### **ML Security and Compliance**

### 19. Which S3 server-side encryption mode provides a CloudTrail audit trail for each decrypt request?

- [ ] **A)** SSE-S3
- [ ] **B)** SSE-KMS
- [ ] **C)** SSE-C
- [ ] **D)** Client-side encryption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SSE-KMS logs each KMS Decrypt API call in AWS CloudTrail, providing an audit trail. SSE-S3 does not log individual decrypt requests, and SSE-C does not use AWS for key management.
 
 
</details>

### 20. Which two IAM actions must a SageMaker training job execution role have to read training data from an S3 bucket encrypted with SSE-KMS?

- [ ] **A)** s3:GetObject
- [ ] **B)** kms:Decrypt
- [ ] **C)** s3:ListBucket
- [ ] **D)** kms:GenerateDataKey

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The training job must perform s3:GetObject to retrieve the object and kms:Decrypt to decrypt it. kms:GenerateDataKey is used for encryption, not decryption. s3:ListBucket is not required for reading a single object.
 
 
</details>

### 21. An ML engineer creates the following VPC endpoint policy for S3. What is the effect of this policy?

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::my-bucket/*"
    }
  ]
}
```

- [ ] **A)** Allows only GetObject on the bucket named my-bucket through the endpoint
- [ ] **B)** Allows all S3 actions on my-bucket through the endpoint
- [ ] **C)** Allows GetObject on all S3 buckets
- [ ] **D)** Denies access to S3 through the endpoint

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy allows the s3:GetObject action only on the resource arn:aws:s3:::my-bucket/*. It does not allow other actions or other buckets. The endpoint policy is evaluated in addition to IAM policies.
 
 
</details>

### 22. Under the AWS Shared Responsibility Model, who is responsible for enabling encryption on training data stored in Amazon S3?

- [ ] **A)** AWS
- [ ] **B)** The customer
- [ ] **C)** Both AWS and the customer
- [ ] **D)** Neither (encryption is optional)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AWS is responsible for the security of the cloud (infrastructure), but the customer is responsible for security in the cloud, including data encryption. The customer must enable and manage encryption settings for S3 (e.g., SSE-KMS).
 
 
</details>


---

### **Model Development**

### 23. What is the primary difference between a built-in algorithm and a custom architecture in Amazon SageMaker?

- [ ] **A)** Built-in algorithms abstract infrastructure concerns
- [ ] **B)** Custom architectures are always faster
- [ ] **C)** Built-in algorithms require custom Docker containers
- [ ] **D)** Custom architectures have no hyperparameters

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Built-in algorithms abstract infrastructure, while custom architectures require more manual setup.
 
 
</details>

### 24. Which business constraints act as primary filters when selecting an algorithm in SageMaker?

- [ ] **A)** Inference latency
- [ ] **B)** Throughput
- [ ] **C)** Cost of hardware
- [ ] **D)** Number of hidden layers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Latency, throughput, and cost are primary constraints; hidden layers are a model architecture detail.
 
 
</details>

### 25. In the code snippet, what does the highlighted line within the run context log?

```python
with Run(experiment_name='my-exp', sagemaker_session=sess) as run:
    run.log_metric('accuracy', 0.95)
```

- [ ] **A)** A metric named 'accuracy' with value 0.95
- [ ] **B)** A parameter named 'accuracy' with value 0.95
- [ ] **C)** An artifact file named 'accuracy'
- [ ] **D)** A tag for the run

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> run.log_metric logs a metric (accuracy) and its value (0.95).
 
 
</details>

### 26. Which hyperparameter optimization strategy is known to be sample-efficient?

- [ ] **A)** Bayesian
- [ ] **B)** Random
- [ ] **C)** Hyperband
- [ ] **D)** Grid

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Bayesian optimization is sample-efficient, using prior results to guide search.
 
 
</details>

### 27. Which metrics should be used when evaluating a classifier on an imbalanced dataset?

- [ ] **A)** Precision
- [ ] **B)** Recall
- [ ] **C)** F1 score
- [ ] **D)** Accuracy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Precision, recall, and F1 give insight into minority class performance; accuracy can mislead.
 
 
</details>

### 28. In the SageMaker Clarify snippet, what does the 'facet_name' parameter identify?

```python
clarify.run_bias(
    data_config=data_config,
    bias_config=BiasConfig(label_values_or_threshold=[1], facet_name='gender'),
    model_config=model_config,
    ...)
```

- [ ] **A)** The sensitive attribute column (e.g., gender)
- [ ] **B)** The target label column
- [ ] **C)** The name of the model
- [ ] **D)** The S3 output path

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> facet_name defines the sensitive group attribute for bias analysis.
 
 
</details>

### 29. What does demographic parity measure in bias detection?

- [ ] **A)** Difference in positive prediction rates between groups
- [ ] **B)** Difference in true positive rates between groups
- [ ] **C)** Difference in false positive rates between groups
- [ ] **D)** Difference in accuracy between groups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Demographic parity looks at prediction rates (positive outcomes) across groups.
 
 
</details>

### 30. Which AWS services can be used to perform error analysis on ML models?

- [ ] **A)** SageMaker Clarify
- [ ] **B)** SageMaker Model Monitor
- [ ] **C)** SageMaker Debugger
- [ ] **D)** Amazon Rekognition

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Clarify, Model Monitor, and Debugger are for custom model analysis; Rekognition is a pre-built service.
 
 
</details>

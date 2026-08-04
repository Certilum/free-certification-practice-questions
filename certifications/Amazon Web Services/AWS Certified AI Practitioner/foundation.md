<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Amazon%20Web%20Services%20Training%20and%20Certification/AWS%20Certified%20AI%20Practitioner" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>AWS Certified AI Practitioner</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [AI and ML Services on AWS](#ai-and-ml-services-on-aws) (7 questions)
- [Data Preparation for ML](#data-preparation-for-ml) (4 questions)
- [Deployment and Operations](#deployment-and-operations) (6 questions)
- [Fundamentals of AI and ML](#fundamentals-of-ai-and-ml) (6 questions)
- [ML Model Development](#ml-model-development) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T05:39:00.657Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| AI and ML Services on AWS | 7 |
| Data Preparation for ML | 4 |
| Deployment and Operations | 6 |
| Fundamentals of AI and ML | 6 |
| ML Model Development | 7 |

---

### **AI and ML Services on AWS**

### 1. Which AWS service is used for automatic speech recognition to convert audio into text?

- [ ] **A)** Amazon Polly
- [ ] **B)** Amazon Transcribe
- [ ] **C)** Amazon Rekognition
- [ ] **D)** Amazon Comprehend

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Amazon Transcribe is the AWS service for automatic speech recognition (ASR).
 
 
</details>

### 2. Which of the following are correct use cases for Amazon Rekognition? (Select two.)

- [ ] **A)** Detecting objects in images
- [ ] **B)** Translating text between languages
- [ ] **C)** Analyzing sentiment in customer reviews
- [ ] **D)** Identifying faces in videos

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Amazon Rekognition provides image and video analysis, including object detection and facial recognition.
 
 
</details>

### 3. Analyze the code block. What does this code do when invoked in a Python script using the AWS SDK (boto3)?

- [ ] **A)** Synthesize speech from text
- [ ] **B)** Transcribe audio to text
- [ ] **C)** Translate text to another language
- [ ] **D)** Detect objects in an image

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code calls Amazon Polly's synthesize_speech method to convert text into an audio stream.
 
 
</details>

### 4. Which SageMaker component is used to orchestrate the end-to-end ML workflow as a directed acyclic graph (DAG)?

- [ ] **A)** SageMaker Studio
- [ ] **B)** SageMaker Pipelines
- [ ] **C)** SageMaker Model Registry
- [ ] **D)** SageMaker Ground Truth

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SageMaker Pipelines creates and manages ML workflows as DAGs.
 
 
</details>

### 5. Which two statements about Amazon SageMaker training jobs are correct? (Select two.)

- [ ] **A)** They can use managed spot instances to reduce cost.
- [ ] **B)** They automatically deploy the model after training.
- [ ] **C)** They support distributed training across multiple compute instances.
- [ ] **D)** They require the use of built-in algorithms only.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Training Jobs can use spot instances and distributed training; deployment is a separate step.
 
 
</details>

### 6. Examine the following SageMaker API call from the AWS CLI. What does the '--resource-type' value indicate about the resource being created?

- [ ] **A)** A model version in Model Registry
- [ ] **B)** A training job
- [ ] **C)** A hyperparameter tuning job
- [ ] **D)** An endpoint configuration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The command 'create-hyper-parameter-tuning-job' creates a tuning job to optimize hyperparameters.
 
 
</details>

### 7. Which AWS service is designed to provide personalized product recommendations in real-time based on user behavior?

- [ ] **A)** Amazon Personalize
- [ ] **B)** Amazon Forecast
- [ ] **C)** Amazon Rekognition
- [ ] **D)** Amazon Comprehend

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Amazon Personalize provides real-time personalization and recommendations.
 
 
</details>


---

### **Data Preparation for ML**

### 8. Which data type has a rigid, predefined schema and is stored in relational databases?

- [ ] **A)** Structured
- [ ] **B)** Unstructured
- [ ] **C)** Semi-structured
- [ ] **D)** None of the above

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Structured data has a rigid, predefined schema and is stored in relational databases like Amazon RDS.
 
 
</details>

### 9. Which two of the following are data cleaning techniques mentioned in the document?

- [ ] **A)** Normalization
- [ ] **B)** Deduplication
- [ ] **C)** Feature engineering
- [ ] **D)** Handling missing values

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Data cleaning techniques include removing duplicate records and handling missing values. Normalization and feature engineering are separate preprocessing steps.
 
 
</details>

### 10. Given the following SQL query, which AWS service is being used to execute it?

- [ ] **A)** AWS Glue
- [ ] **B)** Amazon Athena
- [ ] **C)** Amazon Redshift
- [ ] **D)** Amazon RDS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Amazon Athena is the serverless query service that runs SQL directly on data in S3.
 
 
</details>

### 11. What is the minimum number of samples per category recommended for sufficiency in classification?

- [ ] **A)** 50
- [ ] **B)** 100
- [ ] **C)** 500
- [ ] **D)** 1000

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The document states that sufficiency requires at least 100 samples per category for classification.
 
 
</details>


---

### **Deployment and Operations**

### 12. What is the primary purpose of an Amazon SageMaker endpoint?

- [ ] **A)** Store training data
- [ ] **B)** Host trained models for inference
- [ ] **C)** Run batch transform jobs
- [ ] **D)** Monitor model drift

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A SageMaker endpoint is a managed HTTPS service that hosts a trained model to serve real-time inference requests.
 
 
</details>

### 13. Which two drift types can Amazon SageMaker Model Monitor detect?

- [ ] **A)** Data drift
- [ ] **B)** Concept drift
- [ ] **C)** Code drift
- [ ] **D)** Infrastructure drift

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SageMaker Model Monitor detects data drift (changes in input feature distribution) and concept drift (changes in the relationship between features and target).
 
 
</details>

### 14. After executing the following AWS CLI command, what approval status is assigned to the registered model version?

- [ ] **A)** Approved
- [ ] **B)** PendingApproval
- [ ] **C)** Rejected
- [ ] **D)** Accepted

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> By default, when registering a model via the CLI without specifying an approval status, it is set to PendingApproval.
 
 
</details>

### 15. What is a production variant in SageMaker?

- [ ] **A)** A separate model container within an instance
- [ ] **B)** A set of compute resources serving a model with a traffic weight
- [ ] **C)** A version of the training dataset
- [ ] **D)** An auto-scaling policy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A production variant is a group of compute instances that serve a specific model and receive a weighted portion of inference traffic.
 
 
</details>

### 16. Which two components are required to set up SageMaker Model Monitor?

- [ ] **A)** A baseline dataset with statistics
- [ ] **B)** Data capture enabled on the endpoint
- [ ] **C)** An Amazon EMR cluster
- [ ] **D)** A SageMaker Notebook instance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Model Monitor requires a baseline (statistical summary of training data) and data capture on the endpoint to collect inference payloads.
 
 
</details>

### 17. The code snippet creates a SageMaker Pipeline step. What is the purpose of the 'ConditionStep' in this pipeline?

- [ ] **A)** It runs a training job in parallel
- [ ] **B)** It evaluates metrics and determines whether to register the model
- [ ] **C)** It deploys the model to an endpoint
- [ ] **D)** It copies data from S3

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The ConditionStep checks if evaluation metrics meet a threshold, and only if true, proceeds to register the model.
 
 
</details>


---

### **Fundamentals of AI and ML**

### 18. Which machine learning paradigm uses labeled data to train a model to predict outcomes?

- [ ] **A)** Supervised learning
- [ ] **B)** Unsupervised learning
- [ ] **C)** Reinforcement learning
- [ ] **D)** Transfer learning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Supervised learning requires labeled data; the model maps inputs to outputs using known target labels.
 
 
</details>

### 19. Which of the following are AWS managed AI services? (Select two.)

- [ ] **A)** Amazon Rekognition
- [ ] **B)** Amazon Comprehend
- [ ] **C)** Amazon SageMaker
- [ ] **D)** AWS Lambda

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Rekognition and Comprehend are managed AI services; SageMaker is a platform for custom ML, and Lambda is serverless compute.
 
 
</details>

### 20. The following code snippet uses an AWS API to detect objects in an image. Which AWS service is being invoked?

- [ ] **A)** Amazon Rekognition
- [ ] **B)** Amazon Textract
- [ ] **C)** Amazon Comprehend
- [ ] **D)** Amazon Lex

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code calls the Rekognition API to detect labels (objects) in an image. Textract extracts text, Comprehend analyzes text, Lex builds chatbots.
 
 
</details>

### 21. What is the first step in an ML pipeline according to best practices?

- [ ] **A)** Data collection
- [ ] **B)** Business problem definition
- [ ] **C)** Model training
- [ ] **D)** Model deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The first step is to define the business problem and success metrics before any data work begins.
 
 
</details>

### 22. Which two actions are examples of responsible AI practices? (Select two.)

- [ ] **A)** Bias detection with SageMaker Clarify
- [ ] **B)** Manual hyperparameter tuning
- [ ] **C)** Model explainability documentation
- [ ] **D)** Increasing model complexity to improve accuracy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Bias detection and explainability are core responsible AI practices; tuning and complexity are technical steps, not ethics-related.
 
 
</details>

### 23. The code trains a model using historical customer data with a column 'churned' as the target. What type of ML problem is this?

- [ ] **A)** Supervised classification
- [ ] **B)** Unsupervised clustering
- [ ] **C)** Reinforcement learning
- [ ] **D)** Regression

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The target 'churned' is a binary label, so this is supervised classification. Regression predicts continuous values, not categories.
 
 
</details>


---

### **ML Model Development**

### 24. Which algorithm is best suited for predicting a continuous numerical target variable?

- [ ] **A)** Linear Regression
- [ ] **B)** Logistic Regression
- [ ] **C)** Decision Tree
- [ ] **D)** K-Means

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Linear Regression is used for continuous target variables; Logistic Regression is for classification.
 
 
</details>

### 25. Which of the following are supervised learning algorithms? (Select two.)

- [ ] **A)** Linear Regression
- [ ] **B)** Logistic Regression
- [ ] **C)** K-Means Clustering
- [ ] **D)** Principal Component Analysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Linear Regression and Logistic Regression are supervised; K-Means and PCA are unsupervised.
 
 
</details>

### 26. Review the code snippet. Which parameter controls the type of instance used for training?

- [ ] **A)** instance_type
- [ ] **B)** instance_count
- [ ] **C)** volume_size
- [ ] **D)** role

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The instance_type parameter in SageMaker estimators determines the EC2 instance type for training.
 
 
</details>

### 27. Which hyperparameter tuning strategy is most efficient for a large search space?

- [ ] **A)** Grid Search
- [ ] **B)** Random Search
- [ ] **C)** Bayesian Optimization
- [ ] **D)** Manual Search

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Bayesian Optimization builds a surrogate model to choose promising hyperparameters, making it efficient for large spaces.
 
 
</details>

### 28. Which metrics are appropriate for evaluating a model on an imbalanced dataset? (Select two.)

- [ ] **A)** Accuracy
- [ ] **B)** Precision
- [ ] **C)** Recall
- [ ] **D)** F1 Score

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Precision, Recall, and F1 are all suitable; but for two selections, Precision and Recall (or F1) are correct. The question expects any two of the three.
 
 
</details>

### 29. Examine the training output. What does the divergence of validation loss from training loss indicate?

- [ ] **A)** Overfitting
- [ ] **B)** Underfitting
- [ ] **C)** Convergence
- [ ] **D)** Data drift

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When validation loss increases after a point while training loss decreases, the model is overfitting.
 
 
</details>

### 30. Which SageMaker service should you use to orchestrate a multi-step ML workflow?

- [ ] **A)** SageMaker Training Job
- [ ] **B)** SageMaker Pipelines
- [ ] **C)** SageMaker Experiments
- [ ] **D)** AWS Step Functions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SageMaker Pipelines is designed for orchestrating end-to-end ML workflows as a DAG.
 
 
</details>

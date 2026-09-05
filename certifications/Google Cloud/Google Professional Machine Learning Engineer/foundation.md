<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Google%20Cloud/Google%20Professional%20Machine%20Learning%20Engineer.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Google Professional Machine Learning Engineer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Data engineering and preprocessing](#data-engineering-and-preprocessing) (5 questions)
- [MLOps (pipeline automation, deployment, monitoring)](#mlops-pipeline-automation-deployment-monitoring) (10 questions)
- [Model development and evaluation](#model-development-and-evaluation) (9 questions)
- [Problem framing and solution design](#problem-framing-and-solution-design) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:45.455Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Data engineering and preprocessing | 5 |
| MLOps (pipeline automation, deployment, monitoring) | 10 |
| Model development and evaluation | 9 |
| Problem framing and solution design | 6 |

---

### **Data engineering and preprocessing**

### 1. What is the primary benefit of using transfer learning with a pre-trained model on a specialized dataset?

- [ ] **A)** It accelerates training and reduces data requirements.
- [ ] **B)** It removes the need for any validation data.
- [ ] **C)** It always produces higher accuracy than training from scratch.
- [ ] **D)** It automatically sets all hyperparameters for the model.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Transfer learning reuses pre-trained models to speed up training and reduce the data needed for specialized tasks.
 
 
</details>

### 2. Which two strategies are commonly used to scale distributed training across multiple accelerators or nodes?

- [ ] **A)** Data parallelism
- [ ] **B)** Model parallelism
- [ ] **C)** Bayesian optimization
- [ ] **D)** Early stopping

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Distributed training scales by splitting data across workers or by splitting the model itself; Bayesian optimization and early stopping are tuning techniques.
 
 
</details>

### 3. In the code block, which configuration element determines the range and type of allowed values for each hyperparameter?

```python
from google.cloud import aiplatform

tuning_job = aiplatform.HyperparameterTuningJob(
    display_name="housing_price_tuning",
    metric_spec={"rmse": "minimize"},
    parameter_spec={
        "learning_rate": aiplatform.DoubleParameterSpec(min=1e-5, max=1e-1, scale="log"),
        "batch_size": aiplatform.IntegerParameterSpec(min=16, max=256, scale="linear"),
    },
    max_trial_count=30,
    parallel_trial_count=3,
)
```

- [ ] **A)** Metric specification
- [ ] **B)** Parameter specification
- [ ] **C)** Maximum trial count
- [ ] **D)** Parallel trial count

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The parameter_spec defines the search space for Vertex AI Vizier, including discrete and continuous ranges for each hyperparameter.
 
 
</details>

### 4. How does L1 regularization, also known as Lasso, control model complexity?

- [ ] **A)** It adds the absolute value of the weights as a penalty term.
- [ ] **B)** It adds the squared magnitude of the weights as a penalty term.
- [ ] **C)** It randomly disables a fraction of neurons during training.
- [ ] **D)** It stops training when the validation loss stops improving.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> L1 regularization penalizes the absolute value of weights, encouraging sparsity and reducing overfitting.
 
 
</details>

### 5. Which metrics are generally more informative than accuracy when evaluating a highly imbalanced classification dataset?

- [ ] **A)** Precision
- [ ] **B)** Recall
- [ ] **C)** F1-score
- [ ] **D)** Accuracy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Accuracy is misleading when one class dominates; precision, recall, and F1-score provide a better view of performance on the minority class.
 
 
</details>


---

### **MLOps (pipeline automation, deployment, monitoring)**

### 6. In the context of MLOps on Google Cloud, what is the primary purpose of transfer learning when applied to a specialized dataset?

- [ ] **A)** Reusing a pre-trained model
- [ ] **B)** Starting training from scratch
- [ ] **C)** Tuning hyperparameters automatically
- [ ] **D)** Adding penalties to model weights

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Transfer learning leverages a pre-trained model as a starting point, reducing training time and data requirements for specialized tasks.
 
 
</details>

### 7. According to the playbook, which of the following techniques are used to prevent overfitting by penalizing model complexity or improving generalization?

- [ ] **A)** L1 (Lasso)
- [ ] **B)** L2 (Ridge)
- [ ] **C)** Dropout
- [ ] **D)** Data augmentation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> L1, L2, and Dropout are regularization approaches mentioned; dropout randomly drops neurons, while L1/L2 penalize large weights.
 
 
</details>

### 8. Consider the following Keras snippet, where a pre-trained model is used to build a new classifier. What is the effect of setting the trainable attribute of the base model to False?

```python
from tensorflow import keras
base_model = keras.applications.ResNet50(weights='imagenet', include_top=False)
base_model.trainable = False
x = keras.layers.GlobalAveragePooling2D()(base_model.output)
x = keras.layers.Dense(10, activation='softmax')(x)
model = keras.Model(inputs=base_model.input, outputs=x)
```

- [ ] **A)** The pre-trained weights are not updated
- [ ] **B)** The pre-trained weights are updated with a low learning rate
- [ ] **C)** The pre-trained weights are randomly reinitialized
- [ ] **D)** The pre-trained weights are pruned to zero

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When trainable is False, the layer weights are frozen and do not receive gradient updates, preserving their pre-trained representations.
 
 
</details>

### 9. What is the role of Vertex AI Vizier in the Google Cloud MLOps workflow?

- [ ] **A)** Automates hyperparameter tuning with Bayesian optimization
- [ ] **B)** Stores and versions trained model artifacts
- [ ] **C)** Transforms raw data into engineered features
- [ ] **D)** Deploys models to edge devices

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Vertex AI Vizier is a black-box optimization service that uses Bayesian optimization to automatically find optimal hyperparameters.
 
 
</details>

### 10. Which of the following are hyperparameters that control the training process instead of being learned automatically from the data?

- [ ] **A)** Learning rate
- [ ] **B)** Batch size
- [ ] **C)** Weights and biases
- [ ] **D)** Number of hidden layers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Learning rate, batch size, and number of layers are set before training, whereas weights and biases are learned from data.
 
 
</details>

### 11. Review the provided Vertex AI Vizier code block. What aspect of the tuning job is being configured?

```python
study = vizier.create_study(
    display_name='search_example',
    search_space={
        'learning_rate': Continuous(0.0001, 0.1),
        'batch_size': Discrete([16, 32, 64]),
        'optimizer': Categorical(['adam', 'sgd'])
    }
)
```

- [ ] **A)** Search space definition
- [ ] **B)** Objective metric selection
- [ ] **C)** Early stopping policy
- [ ] **D)** Data validation schema

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code defines the search space by listing each hyperparameter and the range or set of values allowed for tuning.
 
 
</details>

### 12. How is Precision defined in binary classification evaluation?

- [ ] **A)** Of all predicted positive cases, how many were actually positive
- [ ] **B)** Of all actual positive cases, how many were predicted positive
- [ ] **C)** The accuracy across all predicted cases
- [ ] **D)** The area under the ROC curve

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Precision, or positive predictive value, measures how many of the positively predicted instances are truly positive.
 
 
</details>

### 13. In which of the following situations is high Recall particularly important due to the high cost of false negatives?

- [ ] **A)** Medical diagnosis
- [ ] **B)** Fraud detection
- [ ] **C)** Spam detection
- [ ] **D)** Dog breed classification

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Recall matters most when false negatives are dangerous, such as medical diagnosis and fraud detection; spam detection prioritizes precision due to false-positive cost.
 
 
</details>

### 14. Given the Python variables in the code snippet, which evaluation metric is the resulting value?

```python
precision = 0.8
recall = 0.6
f1_score = 2 * (precision * recall) / (precision + recall)
print(f1_score)
```

- [ ] **A)** F1-score
- [ ] **B)** Accuracy
- [ ] **C)** AUC-ROC
- [ ] **D)** Mean squared error

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code calculates F1-score, the harmonic mean of precision and recall, combining both metrics into a single value.
 
 
</details>

### 15. In transfer learning, what distinguishes pure feature extraction from fine-tuning?

- [ ] **A)** The pre-trained backbone is frozen and only the new head is trained
- [ ] **B)** All layers of the pre-trained model are unfrozen and retrained
- [ ] **C)** The entire model is trained from scratch with a low learning rate
- [ ] **D)** The model is pruned to reduce latency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In feature extraction, the pre-trained weights are frozen and only the task-specific head is trained on new data.
 
 
</details>


---

### **Model development and evaluation**

### 16. What is transfer learning in machine learning?

- [ ] **A)** Training a model from scratch using randomly initialized weights
- [ ] **B)** Leveraging pre-trained models on specialized datasets to accelerate training and reduce data requirements
- [ ] **C)** Using a model's predictions to generate synthetic training data
- [ ] **D)** Automatically searching for optimal hyperparameters for a model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Transfer learning uses a pre-trained model as a starting point and adapts it to a specialized task, reducing training time and data requirements.
 
 
</details>

### 17. Which of the following are regularization techniques mentioned as ways to prevent overfitting?

- [ ] **A)** L1 (Lasso)
- [ ] **B)** L2 (Ridge)
- [ ] **C)** Dropout
- [ ] **D)** Early stopping

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The playbook lists L1 (Lasso), L2 (Ridge), and Dropout as regularization techniques used to prevent overfitting by penalizing model complexity.
 
 
</details>

### 18. Consider the code snippet used to construct a neural network. Which element in the snippet is considered a model parameter learned during training?

```python
model = build_model(learning_rate=0.01, dropout_rate=0.2, hidden_units=128)
model.weights
```

- [ ] **A)** learning_rate=0.01
- [ ] **B)** dropout_rate=0.2
- [ ] **C)** hidden_units=128
- [ ] **D)** model.weights

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> Model parameters are values like weights and biases that are learned during training. Hyperparameters such as learning rate, dropout rate, and hidden units control the training process.
 
 
</details>

### 19. What is Vertex AI Vizier primarily used for on Google Cloud?

- [ ] **A)** Automating hyperparameter tuning using advanced algorithms like Bayesian optimization
- [ ] **B)** Storing and versioning trained model artifacts
- [ ] **C)** Managing distributed training across multiple GPUs
- [ ] **D)** Monitoring model performance in production

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Vertex AI Vizier is the primary GCP tool for hyperparameter tuning, using algorithms like Bayesian optimization to find optimal configurations.
 
 
</details>

### 20. Which of the following statements about hyperparameters and model parameters are correct?

- [ ] **A)** Hyperparameters control the training process, such as learning rate and batch size.
- [ ] **B)** Model parameters, such as weights and biases, are learned during training.
- [ ] **C)** Hyperparameters are tuned on validation data, not the test set.
- [ ] **D)** The test set is the appropriate data for hyperparameter tuning.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Hyperparameters control training and are tuned on validation data. Model parameters (weights, biases) are learned during training. The test set is only for final unbiased evaluation.
 
 
</details>

### 21. Given the Vertex AI Vizier search space and budget shown in the snippet, what is the most likely consequence?

```json
{
  "search_space": {
    "learning_rate": { "min": 1e-6, "max": 1.0 },
    "batch_size": { "min": 1, "max": 1024 }
  },
  "budget": 50
}
```

- [ ] **A)** Results will be conclusive and optimal
- [ ] **B)** The tuning job may fail to converge because the search space is too large for the allocated budget
- [ ] **C)** The model will automatically reduce the search space
- [ ] **D)** The search space must include categorical hyperparameters

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A search space that is too large for the allocated budget can lead to inconclusive tuning results, as noted in the playbook's trap on neglecting search space complexity.
 
 
</details>

### 22. Which evaluation metric answers: 'Of all actual positive instances, how many did the model correctly identify?'

- [ ] **A)** Precision
- [ ] **B)** Recall
- [ ] **C)** F1-score
- [ ] **D)** AUC-ROC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Recall, also called sensitivity or true positive rate, measures the proportion of actual positive instances correctly identified by the model.
 
 
</details>

### 23. In which of the following scenarios is high recall especially critical?

- [ ] **A)** Medical diagnosis where missing a disease case is extremely dangerous
- [ ] **B)** Fraud detection where failing to identify fraudulent transactions has high cost
- [ ] **C)** Spam detection where incorrectly flagging a legitimate email is very harmful
- [ ] **D)** A model where false positives are much more costly than false negatives

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> High recall is critical when false negatives are costly, such as in medical diagnosis and fraud detection. Spam detection with harmful false positives requires high precision.
 
 
</details>

### 24. The snippet computes an evaluation metric using precision and recall. What is the resulting value of the metric?

```python
precision = 0.8
recall = 0.4
f1_score = 2 * (precision * recall) / (precision + recall)
```

- [ ] **A)** 0.40
- [ ] **B)** 0.53
- [ ] **C)** 0.60
- [ ] **D)** 0.80

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The harmonic mean of precision and recall is 2 * (0.8 * 0.4) / (0.8 + 0.4) = 0.5333, approximately 0.53.
 
 
</details>


---

### **Problem framing and solution design**

### 25. What is the main benefit of using transfer learning when building a specialized model on a domain-specific dataset?

- [ ] **A)** Reduces data requirements and accelerates training
- [ ] **B)** Increases training time considerably
- [ ] **C)** Removes the need for validation data
- [ ] **D)** Guarantees zero model loss

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Transfer learning uses pre-trained models on specialized datasets to accelerate training and reduce data requirements, as noted in the foundational guide.
 
 
</details>

### 26. Which methods are regularization techniques used to prevent overfitting by penalizing model complexity? Choose all that apply.

- [ ] **A)** L1 (Lasso)
- [ ] **B)** L2 (Ridge)
- [ ] **C)** Dropout
- [ ] **D)** Batch size expansion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The playbook lists L1, L2, and Dropout as regularization techniques that prevent overfitting by penalizing model complexity or adding noise.
 
 
</details>

### 27. Review the code block and identify the Vertex AI service that is used to create the hyperparameter tuning job shown in the snippet.

```python
from google.cloud import aiplatform
from google.cloud.aiplatform import hyperparameter_tuning as hpt

job = aiplatform.HyperparameterTuningJob(
    display_name='tune-model',
    metric_spec={'accuracy': 'maximize'},
    parameter_spec={
        'learning_rate': hpt.DoubleParameterSpec(min=0.0001, max=0.1, scale='log')
    },
    max_trial_count=20,
    parallel_trial_count=5
)
```

- [ ] **A)** Vertex AI Vizier
- [ ] **B)** Vertex AI Model Garden
- [ ] **C)** Vertex AI Feature Store
- [ ] **D)** Vertex AI Pipelines

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This code creates a HyperparameterTuningJob with metric and parameter specs, which is part of Vertex AI Vizier's managed tuning service.
 
 
</details>

### 28. Why is it risky to choose a model solely because it has the highest training accuracy without checking validation performance?

- [ ] **A)** It may overfit and fail on validation data
- [ ] **B)** It is always too slow to train
- [ ] **C)** It will use too little memory
- [ ] **D)** It produces only false negatives

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The guide warns that choosing a model solely for high training accuracy ignores the training-validation gap and can cause overfitting.
 
 
</details>

### 29. Which statements about hyperparameters and the tuning process are correct according to the playbook? Choose all that apply.

- [ ] **A)** They are not learned during training
- [ ] **B)** They control the training process
- [ ] **C)** They should be tuned on validation data
- [ ] **D)** They include weights and biases learned by the model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Hyperparameters control training, are not learned from data, and should be tuned on validation data, not the test set.
 
 
</details>

### 30. Inspect the code block and identify the operation being applied to the layers of the pre-trained neural network.

```python
import tensorflow as tf
base_model = tf.keras.applications.ResNet50(weights='imagenet')
base_model.trainable = True
for layer in base_model.layers[:-2]:
    layer.trainable = False
```

- [ ] **A)** Freezing layers
- [ ] **B)** Layer normalization
- [ ] **C)** Data augmentation
- [ ] **D)** Hyperparameter tuning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Setting trainable to False freezes layers, preventing backpropagation from destroying pre-learned hierarchical features during the new task.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/IAPP/AIGP.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>AI Governance Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Understanding how laws, standards, and frameworks apply to AI](#understanding-how-laws-standards-and-frameworks-apply-to-ai) (7 questions)
- [Understanding how to govern AI deployment and use](#understanding-how-to-govern-ai-deployment-and-use) (9 questions)
- [Understanding how to govern AI development](#understanding-how-to-govern-ai-development) (8 questions)
- [Understanding the foundations of AI governance](#understanding-the-foundations-of-ai-governance) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:58.234Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Understanding how laws, standards, and frameworks apply to AI | 7 |
| Understanding how to govern AI deployment and use | 9 |
| Understanding how to govern AI development | 8 |
| Understanding the foundations of AI governance | 6 |

---

### **Understanding how laws, standards, and frameworks apply to AI**

### 1. What is the defining characteristic of supervised learning?

- [ ] **A)** Models learn by trial and error with a reward function.
- [ ] **B)** Models are trained on labeled datasets containing input features and desired outputs.
- [ ] **C)** Models find hidden patterns in unlabeled data.
- [ ] **D)** Models generate synthetic data from learned distributions.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Supervised learning is defined by training on labeled data with both input features and desired output. The other options describe different learning paradigms.
 
 
</details>

### 2. Which factors are primary risk vectors for introducing systemic bias in supervised learning? Select all that apply.

- [ ] **A)** Quality of the ground truth data
- [ ] **B)** Representativeness of the training data
- [ ] **C)** Labeling accuracy
- [ ] **D)** Number of hidden layers in the model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The playbook identifies ground truth quality, representativeness, and labeling accuracy as primary risk vectors for bias. Model architecture is not the cause identified here.
 
 
</details>

### 3. Based on the configuration in the code block, which machine learning paradigm is described?

```python
config = {
    'method': 'agent',
    'training_signal': 'reward_function',
    'feedback_loop': 'trial_and_error'
}
```

- [ ] **A)** Supervised Learning
- [ ] **B)** Unsupervised Learning
- [ ] **C)** Reinforcement Learning
- [ ] **D)** Generative Modeling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The configuration shows an agent using a reward function and trial-and-error feedback, which is the defining structure of reinforcement learning.
 
 
</details>

### 4. In machine learning, what happens during the training phase?

- [ ] **A)** The model learns from the data.
- [ ] **B)** The model is applied to new, unseen data.
- [ ] **C)** The model is validated against production traffic.
- [ ] **D)** The model is tested for drift.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Training is the phase where a model learns from data. Applying the model to unseen data occurs during inference.
 
 
</details>

### 5. According to governance guidance, which risks are associated with the inference phase? Select all that apply.

- [ ] **A)** Model drift
- [ ] **B)** Real-time reliability
- [ ] **C)** Data privacy during training
- [ ] **D)** Bias in training labels

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Inference risks involve model drift and real-time reliability. Data privacy and training-label bias are risks associated with the training phase.
 
 
</details>

### 6. Given the accuracy metrics in the code block, which condition is most likely present?

```python
training_accuracy = 0.99
validation_accuracy = 0.62
```

- [ ] **A)** Overfitting
- [ ] **B)** Underfitting
- [ ] **C)** Model drift
- [ ] **D)** Reward hacking

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> High training accuracy with much lower validation accuracy indicates the model memorized noise in the training data rather than generalizing.
 
 
</details>

### 7. A biased model shows high accuracy. What is the most effective initial governance response?

- [ ] **A)** Replace the algorithm with a more advanced model.
- [ ] **B)** Inspect the training data for quality and labeling issues.
- [ ] **C)** Add more hidden layers to the model.
- [ ] **D)** Ignore the bias because accuracy is strong.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Bias is often rooted in the training data, not the architecture. Improving data quality and labeling accuracy is the better governance response.
 
 
</details>


---

### **Understanding how to govern AI deployment and use**

### 8. In supervised learning, what are the primary governance risk vectors for introducing systemic bias?

- [ ] **A)** Quality, representativeness, and labeling accuracy of ground truth data
- [ ] **B)** Complexity of the model architecture
- [ ] **C)** Volume of data generated during inference
- [ ] **D)** Design of the agent's reward function

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Supervised learning relies on labeled ground truth, so data quality, representativeness, and labeling accuracy are the key bias risk vectors.
 
 
</details>

### 9. Which governance considerations apply to unsupervised learning? Select all that apply.

- [ ] **A)** Interpretability of the hidden patterns it discovers
- [ ] **B)** Auditing clusters for unintended discriminatory correlations
- [ ] **C)** Labeling accuracy of ground truth data
- [ ] **D)** Reward hacking prevention

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Unsupervised learning uses unlabeled data; governance centers on interpretability and auditability of discovered patterns, not labels or rewards.
 
 
</details>

### 10. The provided code block defines a learning signal for an AI agent. Which governance risk is most directly associated with this mechanism?

```python
def reward(state):
    return 100 if state.goal_reached else 0
```

- [ ] **A)** Reward hacking
- [ ] **B)** Overfitting
- [ ] **C)** Model drift
- [ ] **D)** Synthetic data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Reinforcement learning relies on reward functions, and reward hacking occurs when the agent meets the objective through harmful shortcuts.
 
 
</details>

### 11. Which governance risk is most associated with the inference phase?

- [ ] **A)** Model drift and real-time reliability
- [ ] **B)** Data privacy and bias from training data
- [ ] **C)** Labeling accuracy of ground truth
- [ ] **D)** Copyright of training content

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Training risks involve privacy and bias; inference risks center on model drift and real-time reliability.
 
 
</details>

### 12. Which statements about overfitting and underfitting are correct? Select all that apply.

- [ ] **A)** Overfitting means the model memorizes noise in the training data and fails to generalize.
- [ ] **B)** Underfitting means the model fails to capture the underlying trend.
- [ ] **C)** Both conditions create reliability risks in production.
- [ ] **D)** Both conditions are caused by reward hacking.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Overfitting memorizes noise, underfitting misses trends, and both compromise accurate, predictable production outcomes.
 
 
</details>

### 13. The provided code block represents a phase in the AI lifecycle. Which governance risks should be reviewed for this phase?

```python
model.fit(X_train, y_train)
```

- [ ] **A)** Data privacy and bias
- [ ] **B)** Real-time reliability
- [ ] **C)** Provenance of generated content
- [ ] **D)** Reward hacking

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block shows training, where the main risks are data privacy and bias in the training data.
 
 
</details>

### 14. Which statement correctly describes model drift?

- [ ] **A)** It is a natural statistical phenomenon caused by changing real-world data distributions.
- [ ] **B)** It is a software bug in the model code.
- [ ] **C)** It can be permanently fixed by selecting a better algorithm.
- [ ] **D)** It only occurs in generative AI.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Model drift is not a code error; it reflects natural degradation caused by changes in real-world data distributions.
 
 
</details>

### 15. Which of the following are common AI governance traps? Select all that apply.

- [ ] **A)** Confusing AI with machine learning
- [ ] **B)** Assuming accuracy equals fairness
- [ ] **C)** Treating hallucination as only a bug
- [ ] **D)** Selecting technical validation as a governance structure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> The playbook identifies all of these as common traps, including conceptual confusion, fairness assumptions, hallucination framing, and misuse of validation.
 
 
</details>

### 16. The provided code block shows an optimization goal. Which model category does this objective represent?

```python
loss = 1 if prediction != label else 0
optimize(loss)
```

- [ ] **A)** Discriminative model minimizing classification error
- [ ] **B)** Generative model maximizing data likelihood
- [ ] **C)** Reinforcement learning agent maximizing reward
- [ ] **D)** Unsupervised clustering model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Discriminative models aim to minimize classification error; the code compares predictions against labels.
 
 
</details>


---

### **Understanding how to govern AI development**

### 17. Which machine learning paradigm trains models on labeled datasets that contain both input features and the desired output for each example?

- [ ] **A)** Supervised learning
- [ ] **B)** Unsupervised learning
- [ ] **C)** Reinforcement learning
- [ ] **D)** Generative AI

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Supervised learning uses labeled datasets with inputs and desired outputs. Governance must audit ground truth quality because labeling errors can introduce systemic bias.
 
 
</details>

### 18. Which governance risks are specifically associated with unsupervised learning, according to the risk profile in the playbook?

- [ ] **A)** Lack of interpretability of discovered patterns
- [ ] **B)** Unintended discriminatory correlations in clusters
- [ ] **C)** Reward hacking from a malfunctioning reward function
- [ ] **D)** Labeling inaccuracies in ground truth

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Unsupervised learning risks focus on interpretability and hard-to-audit clusters that may encode discriminatory correlations. Reward hacking belongs to reinforcement learning; labeling issues belong to supervised learning.
 
 
</details>

### 19. The code block shows an agent selecting actions and receiving rewards while updating its policy. Which learning paradigm does this represent?

```python
def train_agent(environment, reward_function, episodes):
    for _ in range(episodes):
        action = agent.act(environment.state)
        reward = reward_function(action)
        agent.update(action, reward)
```

- [ ] **A)** Reinforcement learning
- [ ] **B)** Supervised learning
- [ ] **C)** Unsupervised learning
- [ ] **D)** Discriminative AI

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The loop uses actions, rewards, and policy updates, which is the hallmark of reinforcement learning. Governance should watch for reward hacking in such systems.
 
 
</details>

### 20. How should model drift be interpreted from a governance perspective, according to the playbook's description?

- [ ] **A)** A statistical phenomenon from changing data distributions
- [ ] **B)** A software bug requiring code changes
- [ ] **C)** The same as overfitting during training
- [ ] **D)** A labeling error in the training dataset

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Model drift is a natural statistical phenomenon from changing real-world data, not a code bug. Governance should treat it as an ongoing monitoring concern.
 
 
</details>

### 21. Which statements correctly match governance risks with either the training phase or the inference phase of a model lifecycle?

- [ ] **A)** Data privacy is a training-phase risk
- [ ] **B)** Model drift is an inference-phase risk
- [ ] **C)** Real-time reliability is a training-phase risk
- [ ] **D)** Labeling accuracy is an inference-phase risk

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Training risks include data privacy and bias, while inference risks include model drift and real-time reliability. The other pairings reverse these relationships.
 
 
</details>

### 22. The code block reports training accuracy as high and validation accuracy as lower. Which model condition does this pattern suggest?

```python
training_accuracy = 0.99
validation_accuracy = 0.71
```

- [ ] **A)** Overfitting
- [ ] **B)** Underfitting
- [ ] **C)** Model drift
- [ ] **D)** Reward hacking

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> High training accuracy with lower validation accuracy indicates the model memorized noise and failed to generalize, which is overfitting.
 
 
</details>

### 23. What belief characterizes the governance trap of confusing data quality with model architecture when outcomes are biased?

- [ ] **A)** A better algorithm automatically fixes biased outcomes
- [ ] **B)** Bias is usually rooted in the model architecture
- [ ] **C)** Data quality is irrelevant once the model is deployed
- [ ] **D)** Algorithm choice has no effect on bias

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The trap is assuming a better algorithm fixes biased outcomes; bias often is rooted in the training data itself.
 
 
</details>

### 24. Which statements reflect sound governance responses to the Black Box Fallacy for highly complex deep learning models?

- [ ] **A)** Implement explainability (XAI) tools
- [ ] **B)** Govern the model through appropriate explainability methods
- [ ] **C)** Abandon complex models because they cannot be governed
- [ ] **D)** Treat high complexity as making the model unmanageable

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The Black Box Fallacy is the belief that complex models are inherently unmanageable. Governance should use XAI tools to address complexity.
 
 
</details>


---

### **Understanding the foundations of AI governance**

### 25. Which machine learning paradigm uses labeled datasets that contain both input features and the desired output?

- [ ] **A)** Supervised Learning
- [ ] **B)** Unsupervised Learning
- [ ] **C)** Reinforcement Learning
- [ ] **D)** Semi-supervised Learning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Supervised learning trains on labeled ground truth. Governance risk vectors include the quality, representativeness, and labeling accuracy of the ground truth data.
 
 
</details>

### 26. Which governance risks are associated with reinforcement learning? Select all that apply.

- [ ] **A)** Reward hacking, where the agent achieves the mathematical objective through unintended shortcuts
- [ ] **B)** Agent behavior that violates human safety constraints while optimizing the reward function
- [ ] **C)** Inaccurate ground truth labels introducing systemic bias
- [ ] **D)** Hidden clusters in unlabeled data that are difficult to audit

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Reinforcement learning governance risks center on reward hacking and agents taking unintended or harmful shortcuts that violate human safety constraints. Label bias is a supervised learning concern, and hidden clusters are an unsupervised learning concern.
 
 
</details>

### 27. Review the code excerpt below and select the governance concern that should be evaluated.

```python
def reward_function(state, action):
    if state == target:
        return 100
    return -1
```

- [ ] **A)** The agent may find unintended shortcuts that maximize reward but violate safety constraints
- [ ] **B)** The model is memorizing noise in the training data
- [ ] **C)** The ground truth labels are inaccurate
- [ ] **D)** The model cannot generalize to new inputs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A reward function that only rewards reaching the target can lead to reward hacking, where the agent achieves the mathematical objective through unintended or harmful shortcuts that violate safety constraints.
 
 
</details>

### 28. During the inference phase, what is the model doing?

- [ ] **A)** It applies what it learned during training to new, unseen data
- [ ] **B)** It learns from labeled training examples
- [ ] **C)** It creates synthetic data for future training
- [ ] **D)** It evaluates the loss function on training data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Inference is the phase where the model applies its learned patterns to new, unseen data. Governance risks at inference include model drift and real-time reliability.
 
 
</details>

### 29. Which risks require governance oversight during the inference phase? Select all that apply.

- [ ] **A)** Model drift
- [ ] **B)** Real-time reliability
- [ ] **C)** Bias in training labels
- [ ] **D)** Privacy violations during model training

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Inference risks include model drift and real-time reliability. Bias in training labels and privacy violations during training are primarily training-phase concerns.
 
 
</details>

### 30. Review the code output comparison below and determine which reliability risk is indicated.

```python
training_accuracy = 0.99
validation_accuracy = 0.61
if training_accuracy - validation_accuracy > 0.2:
    print("Potential reliability risk")
```

- [ ] **A)** Overfitting: the model memorized noise in the training data and failed to generalize
- [ ] **B)** Underfitting: the model failed to capture the underlying trend
- [ ] **C)** Model drift: the real-world data distribution changed
- [ ] **D)** Hallucination: the model generated non-factual content

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A large gap between high training accuracy and lower validation accuracy indicates overfitting, where the model memorizes training noise and fails to generalize to unseen data.
 
 
</details>

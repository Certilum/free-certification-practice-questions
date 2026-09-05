<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/NVIDIA/NVIDIA%20Certified%20Professional%20-%20Agentic%20AI.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>NVIDIA Certified Professional - Agentic AI</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Agent Architecture and Design](#agent-architecture-and-design) (4 questions)
- [Agent Development](#agent-development) (4 questions)
- [Cognition, Planning, and Memory](#cognition-planning-and-memory) (3 questions)
- [Deployment and Scaling](#deployment-and-scaling) (4 questions)
- [Evaluation and Tuning](#evaluation-and-tuning) (4 questions)
- [Human-AI Interaction and Oversight](#human-ai-interaction-and-oversight) (2 questions)
- [Knowledge Integration and Data Handling](#knowledge-integration-and-data-handling) (3 questions)
- [NVIDIA Platform Implementation](#nvidia-platform-implementation) (2 questions)
- [Run, Monitor, and Maintain](#run-monitor-and-maintain) (2 questions)
- [Safety, Ethics, and Compliance](#safety-ethics-and-compliance) (2 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:39.280Z |
| Domains | 10 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Agent Architecture and Design | 4 |
| Agent Development | 4 |
| Cognition, Planning, and Memory | 3 |
| Deployment and Scaling | 4 |
| Evaluation and Tuning | 4 |
| Human-AI Interaction and Oversight | 2 |
| Knowledge Integration and Data Handling | 3 |
| NVIDIA Platform Implementation | 2 |
| Run, Monitor, and Maintain | 2 |
| Safety, Ethics, and Compliance | 2 |

---

### **Agent Architecture and Design**

### 1. What technique involves prompting a model to generate intermediate reasoning steps to solve complex problems?

- [ ] **A)** Simple Instruction
- [ ] **B)** Chain-of-Thought (CoT)
- [ ] **C)** Few-Shot Prompting
- [ ] **D)** Task Decomposition

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Chain-of-Thought (CoT) prompting encourages the model to generate intermediate reasoning steps, facilitating complex problem solving.
 
 
</details>

### 2. In the ReAct framework, which three components form the iterative reasoning and acting loop?

- [ ] **A)** Thought
- [ ] **B)** Action
- [ ] **C)** Observation
- [ ] **D)** User Input

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The ReAct framework combines reasoning traces (thought), task-specific actions (action), and results (observation).
 
 
</details>

### 3. Look at the few-shot example below. Is the reasoning pattern correctly implemented for agentic generalization?

```text
Example 1:
Input: 'What is the weather?'
Output: 'It is sunny.'

Example 2:
Input: 'Check stock.'
Output: 'Stock is 5.'
```

- [ ] **A)** Yes, it includes reasoning steps
- [ ] **B)** No, it only provides input/output
- [ ] **C)** No, it lacks observation
- [ ] **D)** Yes, it uses simple instructions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Correct few-shot reasoning for agents requires (Input/Thought/Action/Output) rather than just (Input/Output).
 
 
</details>

### 4. What is the primary purpose of Task Decomposition in agent architecture?

- [ ] **A)** To increase context window size
- [ ] **B)** To prevent the agent from being overwhelmed
- [ ] **C)** To automate tool execution directly
- [ ] **D)** To reduce the number of reasoning steps

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Task decomposition breaks high-level goals into executable sub-problems to prevent the agent from becoming overwhelmed.
 
 
</details>


---

### **Agent Development**

### 5. What is the primary purpose of Chain-of-Thought (CoT) prompting in Large Language Models?

- [ ] **A)** Increase context window size
- [ ] **B)** Improve reasoning via intermediate steps
- [ ] **C)** Speed up raw token generation
- [ ] **D)** Reduce the need for tool calls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> CoT improves reasoning by prompting the model to generate a sequence of intermediate reasoning steps.
 
 
</details>

### 6. Which components are part of the ReAct (Reasoning and Acting) framework loop?

- [ ] **A)** Thought
- [ ] **B)** Action
- [ ] **C)** Observation
- [ ] **D)** Manual User Feedback

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The ReAct framework follows an iterative loop of thought, action, and observation.
 
 
</details>

### 7. Identify the error in this few-shot reasoning pattern implementation.

```text
Example 1:
Input: Calculate tax for $100
Output: $10

Example 2:
Input: Calculate tax for $200
Output: $20
```

- [ ] **A)** Missing tool names
- [ ] **B)** Missing reasoning steps
- [ ] **C)** Too many examples
- [ ] **D)** Incorrect output format

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Providing only Input/Output without Thought/Action fails to teach the underlying logic needed for generalization.
 
 
</details>

### 8. What does task decomposition involve in agent development?

- [ ] **A)** Combining multiple agents
- [ ] **B)** Splitting goals into sub-problems
- [ ] **C)** Increasing token importance
- [ ] **D)** Automating tool selection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Task decomposition is the strategic instruction to break a high-level goal into smaller, executable sub-problems.
 
 
</details>


---

### **Cognition, Planning, and Memory**

### 9. Which technique involves prompting an LLM to generate intermediate reasoning steps to solve complex problems?

- [ ] **A)** Chain-of-Thought
- [ ] **B)** Task Decomposition
- [ ] **C)** Few-Shot Prompting
- [ ] **D)** Self-Reflection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Chain-of-Thought (CoT) prompting specifically requires the model to generate a sequence of intermediate reasoning steps.
 
 
</details>

### 10. In the ReAct framework, which three components form the iterative loop used by an agent?

- [ ] **A)** Thought
- [ ] **B)** Action
- [ ] **C)** Observation
- [ ] **D)** Instruction

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The ReAct framework consists of a 'thought' (reasoning), an 'action' (tool call), and an 'observation' (result).
 
 
</details>

### 11. Review the following few-shot example pattern. Is this pattern correctly designed for teaching reasoning logic?

```text
Example 1:
Input: What is the weather?
Output: It is sunny.
```

- [ ] **A)** Yes, it includes Thought/Action/Output
- [ ] **B)** No, it only provides Input/Output
- [ ] **C)** No, it lacks tool definitions
- [ ] **D)** Yes, it uses simple instructions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Effective few-shot reasoning for agents must include (Input/Thought/Action/Output) rather than just (Input/Output).
 
 
</details>


---

### **Deployment and Scaling**

### 12. Which technique involves prompting an LLM to generate intermediate reasoning steps to break down complex problems?

- [ ] **A)** Chain-of-Thought (CoT)
- [ ] **B)** Simple Instruction
- [ ] **C)** Task Decomposition
- [ ] **D)** Few-Shot Learning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Chain-of-Thought (CoT) prompting improves reasoning by generating intermediate steps for complex problems.
 
 
</details>

### 13. In the ReAct framework, which components make up the iterative reasoning and acting loop?

- [ ] **A)** Thought
- [ ] **B)** Action
- [ ] **C)** Observation
- [ ] **D)** User Input

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> ReAct combines reasoning traces (thought), task-specific actions (action), and results (observation).
 
 
</details>

### 14. Review the few-shot example provided in the code and identify why it might fail to teach complex logic.

```text
Example 1:
Input: 'What is 5 + 5?'
Output: '10'
```

- [ ] **A)** Lacks reasoning steps
- [ ] **B)** Too many examples
- [ ] **C)** Incorrect tool names
- [ ] **D)** Missing observations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Providing only Input/Output without Thought/Action steps fails to teach the underlying logic.
 
 
</details>

### 15. What is the purpose of Self-Reflection and Self-Correction in autonomous agents?

- [ ] **A)** To recover from errors
- [ ] **B)** To increase context window
- [ ] **C)** To select tools faster
- [ ] **D)** To reduce token usage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Self-reflection allows agents to review reasoning for inconsistencies and recover from failures.
 
 
</details>


---

### **Evaluation and Tuning**

### 16. Which technique involves prompting an LLM to generate a sequence of intermediate reasoning steps to solve complex problems?

- [ ] **A)** Few-Shot Prompting
- [ ] **B)** Chain-of-Thought (CoT)
- [ ] **C)** Task Decomposition
- [ ] **D)** Self-Reflection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Chain-of-Thought (CoT) prompting improves reasoning by forcing the model to generate intermediate steps.
 
 
</details>

### 17. In the ReAct framework, which three components form the iterative loop used by the agent?

- [ ] **A)** Thought
- [ ] **B)** Action
- [ ] **C)** Observation
- [ ] **D)** Instruction

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The ReAct framework combines reasoning (thought), task-specific actions, and observations from the environment.
 
 
</details>

### 18. Review the following few-shot example pattern. Is this pattern sufficient for teaching an agent complex logic?

```text
Example 1:
Input: 'What is the weather in NYC?'
Output: 'The weather is 72 degrees.'
```

- [ ] **A)** Yes, it includes Thought/Action/Output
- [ ] **B)** No, it only provides Input/Output
- [ ] **C)** Yes, it uses simple instruction
- [ ] **D)** No, it lacks task decomposition

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Providing only Input/Output fails to teach the agent the underlying logic; it needs Thought/Action/Output steps.
 
 
</details>

### 19. What is the primary purpose of task decomposition in agentic workflows?

- [ ] **A)** To increase the context window size
- [ ] **B)** To prevent the agent from being overwhelmed
- [ ] **C)** To replace the need for CoT prompting
- [ ] **D)** To automate tool selection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Task decomposition prevents agents from being overwhelmed and ensures focus on verifiable objectives.
 
 
</details>


---

### **Human-AI Interaction and Oversight**

### 20. What is the primary purpose of the Chain-of-Thought (CoT) prompting technique in Large Language Models?

- [ ] **A)** Increasing context window size
- [ ] **B)** Generating intermediate reasoning steps
- [ ] **C)** Providing tool execution results
- [ ] **D)** Reducing total token usage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> CoT improves reasoning by prompting the model to generate a sequence of intermediate steps to break down complex problems.
 
 
</details>

### 21. Which components are part of the iterative ReAct (Reasoning and Acting) framework loop?

- [ ] **A)** Thought
- [ ] **B)** Action
- [ ] **C)** Observation
- [ ] **D)** Instruction

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The ReAct framework combines reasoning traces (thought), task-specific actions (action), and external results (observation).
 
 
</details>


---

### **Knowledge Integration and Data Handling**

### 22. What is the primary goal of using Chain-of-Thought (CoT) prompting in large language models?

- [ ] **A)** Generate faster responses
- [ ] **B)** Provide immediate final answers
- [ ] **C)** Break problems into manageable sub-tasks
- [ ] **D)** Increase the context window size

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> CoT allows the agent to break down complex problems into manageable sub-tasks via intermediate reasoning steps.
 
 
</details>

### 23. Which components are part of the ReAct (Reasoning and Acting) framework iterative loop?

- [ ] **A)** Thought
- [ ] **B)** Action
- [ ] **C)** Observation
- [ ] **D)** Instruction

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The ReAct framework consists of a loop of thought (reasoning), action (tool call), and observation (result).
 
 
</details>

### 24. Review the few-shot example provided below and determine if it follows the correct reasoning pattern.

```text
Example 1:
Input: What is the weather in NYC?
Output: It is 75 degrees.

Example 2:
Input: What is the weather in NYC?
Thought: I need to call the weather tool.
Action: get_weather(location='NYC')
Observation: 75 degrees
Output: The weather is 75 degrees.
```

- [ ] **A)** Correct: Includes Thought/Action
- [ ] **B)** Incorrect: Missing Reasoning
- [ ] **C)** Incorrect: Only uses Input/Output
- [ ] **D)** Correct: Uses only Tool Results

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Few-shotting for agents must include reasoning steps (Input/Thought/Action/Output) rather than just Input/Output.
 
 
</details>


---

### **NVIDIA Platform Implementation**

### 25. Which statement best describes the primary purpose of Chain-of-Thought (CoT) prompting in Large Language Models?

- [ ] **A)** Increasing context window size
- [ ] **B)** Enhancing reasoning via intermediate steps
- [ ] **C)** Speeding up tool execution time
- [ ] **D)** Reducing the number of required tokens

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> CoT improves reasoning by prompting the model to generate a sequence of intermediate reasoning steps for complex problems.
 
 
</details>

### 26. In this scenario, which components are part of the ReAct (Reasoning and Acting) framework loop?

- [ ] **A)** Thought
- [ ] **B)** Action
- [ ] **C)** Observation
- [ ] **D)** Instruction

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The ReAct framework combines reasoning traces and actions through a loop of thought, action, and observation.
 
 
</details>


---

### **Run, Monitor, and Maintain**

### 27. Which framework uses an iterative loop of thought, action, and observation to allow an agent to adapt?

- [ ] **A)** Chain-of-Thought
- [ ] **B)** ReAct Framework
- [ ] **C)** Task Decomposition
- [ ] **D)** Few-Shot Reasoning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The ReAct framework combines reasoning (thought) and acting (action) in an iterative loop with observations.
 
 
</details>

### 28. Which of the following are considered key reasoning techniques for improving LLM agent capabilities?

- [ ] **A)** Chain-of-Thought
- [ ] **B)** Self-Reflection
- [ ] **C)** FIFO Token Management
- [ ] **D)** Simple Instruction Following

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Chain-of-Thought and Self-Reflection are core techniques for improving reasoning and error recovery in agents.
 
 
</details>


---

### **Safety, Ethics, and Compliance**

### 29. In the ReAct framework, what is the specific definition of an 'observation'?

- [ ] **A)** User input
- [ ] **B)** Tool output
- [ ] **C)** Model reasoning
- [ ] **D)** Action plan

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In the ReAct framework, the observation is the result of a tool call being fed back into the model's reasoning loop.
 
 
</details>

### 30. Which techniques help an agent recover from errors without manual human intervention?

- [ ] **A)** Self-Reflection
- [ ] **B)** Self-Correction
- [ ] **C)** Simple Instruction
- [ ] **D)** FIFO Token Management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Self-reflection and self-correction are closed-loop reasoning techniques that allow agents to recover from failures autonomously.
 
 
</details>

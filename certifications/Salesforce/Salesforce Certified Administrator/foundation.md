<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Salesforce/Salesforce%20Certified%20Administrator.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Salesforce Certified Administrator</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Agentforce](#agentforce) (2 questions)
- [Automation](#automation) (4 questions)
- [Configuration and setup](#configuration-and-setup) (5 questions)
- [Data and analytics management](#data-and-analytics-management) (5 questions)
- [Object Manager and Lightning App Builder](#object-manager-and-lightning-app-builder) (5 questions)
- [Productivity and collaboration](#productivity-and-collaboration) (3 questions)
- [Sales and marketing applications](#sales-and-marketing-applications) (3 questions)
- [Service and support applications](#service-and-support-applications) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:47:06.958Z |
| Domains | 8 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Agentforce | 2 |
| Automation | 4 |
| Configuration and setup | 5 |
| Data and analytics management | 5 |
| Object Manager and Lightning App Builder | 5 |
| Productivity and collaboration | 3 |
| Sales and marketing applications | 3 |
| Service and support applications | 3 |

---

### **Agentforce**

### 1. Why should an administrator configure an Agentforce agent to focus on a specific business domain such as Service or Sales?

- [ ] **A)** To prevent the agent from attempting tasks outside its intended boundaries
- [ ] **B)** To make the agent automatically access all Salesforce data
- [ ] **C)** To remove the need for agent-specific permission sets
- [ ] **D)** To allow the agent to work without any instructions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The agent role and purpose must be scoped to specific business domains so the agent does not attempt tasks outside its intended operational boundaries.
 
 
</details>

### 2. Which items must be explicitly configured when grounding an Agentforce agent to CRM data?

- [ ] **A)** Specific objects
- [ ] **B)** Specific fields
- [ ] **C)** Knowledge articles
- [ ] **D)** Automatic access to all CRM data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Administrators must define the objects, fields, and Knowledge articles the agent can use. The agent does not automatically receive access to all data.
 
 
</details>


---

### **Automation**

### 3. Which configuration element defines the specific persona and scope of an agent?

- [ ] **A)** Agent Role & Purpose
- [ ] **B)** Actions & Tooling
- [ ] **C)** Reasoning Engine
- [ ] **D)** Data Grounding

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Agent Role & Purpose defines the persona and scope of the agent, preventing it from acting outside its intended business domain.
 
 
</details>

### 4. Which two components execute logic as Actions, rather than merely generate text?

- [ ] **A)** Apex classes
- [ ] **B)** Flow Builder flows
- [ ] **C)** Prompt Templates
- [ ] **D)** Knowledge Articles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Flow Builder flows and Apex classes execute logic, while Prompt Templates only generate text and Knowledge Articles are data sources.
 
 
</details>

### 5. The configuration snippet in the code block represents which key concept?

```json
{
  "grounding": {
    "objects": ["Case", "Contact"],
    "fields": ["Case.Status", "Case.Subject", "Contact.Email"],
    "knowledge": ["Installation_Guide"]
  }
}
```

- [ ] **A)** Data Grounding
- [ ] **B)** Agent Role & Purpose
- [ ] **C)** Actions & Tooling
- [ ] **D)** Einstein Trust Layer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Data Grounding connects the agent to CRM objects, fields, and Knowledge articles so it can answer using real customer data.
 
 
</details>

### 6. What is the purpose of the Einstein Trust Layer integration in an agent configuration?

- [ ] **A)** Masking sensitive PII before sending to the LLM
- [ ] **B)** Replacing the reasoning engine
- [ ] **C)** Granting the agent access to all CRM data
- [ ] **D)** Creating flowcharts for the agent

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Einstein Trust Layer masks PII before data is sent to the LLM and helps enforce the organization's data-sharing rules.
 
 
</details>


---

### **Configuration and setup**

### 7. What is the primary purpose of defining an Agent's Role and Purpose during configuration?

- [ ] **A)** It defines the specific persona and operational boundaries of the agent.
- [ ] **B)** It automatically grants the agent access to all Salesforce data.
- [ ] **C)** It replaces the need for instructions and guardrails.
- [ ] **D)** It generates Apex code for the agent.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Defining the role and purpose sets the agent's persona and scope, ensuring it focuses on intended business domains like Service or Sales.
 
 
</details>

### 8. Which of the following are considered Agentic Actions or Tools in Agentforce?

- [ ] **A)** Flow Builder flows
- [ ] **B)** Apex classes
- [ ] **C)** Prompt Templates
- [ ] **D)** Knowledge article records

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Agentic actions include Flow Builder flows, Apex classes, and Prompt Templates. Knowledge articles are data used for grounding, not actions.
 
 
</details>

### 9. Based on the code snippet, what type of Agentic Action is being configured for the agent?

```json
{
  "actionName": "UpdateCasePriority",
  "implementationType": "Flow",
  "flowApiName": "Update_Case_Priority_Flow",
  "description": "Updates case priority based on user input"
}
```

- [ ] **A)** Apex class
- [ ] **B)** Flow
- [ ] **C)** Prompt Template
- [ ] **D)** Data grounding

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The implementationType is set to Flow and the flowApiName references a Flow Builder flow, so this is a Flow action.
 
 
</details>

### 10. What is dynamic context injection in Agentforce?

- [ ] **A)** Pulling relevant record data into the agent's reasoning process
- [ ] **B)** Generating text using Prompt Templates
- [ ] **C)** Masking sensitive PII before sending data to the LLM
- [ ] **D)** Creating a visual flowchart for the agent's conversation path

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Dynamic context injection pulls record data like Case details into reasoning, allowing personalized, data-driven responses rather than generic replies.
 
 
</details>

### 11. Which configuration settings are part of Einstein Trust Layer Integration?

- [ ] **A)** Masking PII before data is sent to the LLM
- [ ] **B)** Adhering to the organization's data sharing rules
- [ ] **C)** Giving the agent access to every Salesforce object
- [ ] **D)** Requiring a flowchart for every agent conversation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Einstein Trust Layer Integration masks sensitive PII and follows org data sharing rules. It does not grant universal data access.
 
 
</details>


---

### **Data and analytics management**

### 12. In an Agentforce deployment, what is the main purpose of defining the agent’s role and persona?

- [ ] **A)** Keeps agent within its intended operational boundaries
- [ ] **B)** Guarantees a 100% task completion rate
- [ ] **C)** Automatically creates Flows and Apex classes
- [ ] **D)** Replaces Salesforce security permissions entirely

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Defining a persona and scope prevents the agent from attempting work outside its designated business domain, such as using Service actions for Sales tasks.
 
 
</details>

### 13. Which of the following components should be classified as agentic actions rather than as governance settings when configuring an Agentforce agent?

- [ ] **A)** Flow Builder flow
- [ ] **B)** Apex class
- [ ] **C)** Prompt Template
- [ ] **D)** Reasoning engine

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Agentic actions are executable capabilities like Flows, Apex, or Prompt Templates. The reasoning engine makes decisions rather than being a tool the agent invokes.
 
 
</details>

### 14. Based on the configuration snippet provided, which action is intended to perform a business operation instead of generating text?

```json
{
  "agent": {
    "name": "Case Support Agent",
    "actions": [
      { "type": "PromptTemplate", "name": "Summarize Case", "enabled": true },
      { "type": "Flow", "name": "UpdateCaseStatus", "enabled": true }
    ],
    "dataAccess": ["Case", "Contact"]
  }
}
```

- [ ] **A)** Flow named UpdateCaseStatus
- [ ] **B)** Prompt Template named Summarize Case
- [ ] **C)** Data access for Case
- [ ] **D)** Agent name

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Prompt Templates generate text; a Flow is an action that executes logic in the agent. Data access is grounding, not an executable action.
 
 
</details>

### 15. What does the process of data grounding accomplish when an administrator configures an Agentforce agent?

- [ ] **A)** Provides contextually accurate responses using real-time data
- [ ] **B)** Generates Apex classes for every object
- [ ] **C)** Creates a flowchart for agent conversations
- [ ] **D)** Removes all security on the selected objects

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Data grounding connects the agent to the right objects, fields, and Knowledge articles so answers are based on real-time CRM data and are contextually accurate.
 
 
</details>

### 16. Which of the following settings are examples of guardrails that control an Agentforce agent's behavior and data access?

- [ ] **A)** Restricting objects and fields accessible to the agent
- [ ] **B)** Setting explicit allowed actions for the agent
- [ ] **C)** Requiring human approval for high-risk processes
- [ ] **D)** Granting unrestricted access to all Salesforce data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Guardrails include boundaries on data access, action permissions, autonomy, and human-in-the-loop approval to prevent unauthorized or unsafe agent behavior.
 
 
</details>


---

### **Object Manager and Lightning App Builder**

### 17. What is the primary purpose of defining an agent's role and purpose in Agentforce?

- [ ] **A)** It keeps the agent focused on specific business domains and prevents out-of-scope tasks.
- [ ] **B)** It gives the agent automatic access to all Salesforce data.
- [ ] **C)** It creates a step-by-step flowchart for every interaction.
- [ ] **D)** It removes the need to configure actions and tooling.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Configuring the agent's role and purpose defines its persona and operational scope, preventing it from attempting tasks outside its intended business domain.
 
 
</details>

### 18. Which of the following must an administrator configure when setting up an agent? Select all that apply.

- [ ] **A)** Actions and Tooling
- [ ] **B)** Data Grounding
- [ ] **C)** Einstein Trust Layer Integration
- [ ] **D)** A visual flowchart for all user requests

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Actions and Tooling, Data Grounding, and Einstein Trust Layer Integration are core configuration areas. A flowchart is not required because flows are tools the agent uses, not the map it follows.
 
 
</details>

### 19. The provided configuration snippet defines an agent with a specific domain and assigned actions. What concept is represented by the actions section?

```yaml
agent:
  name: Service Agent
  domain: Service
  actions:
    - Flow: Update Case Status
    - Apex: Validate Warranty
```

- [ ] **A)** Agentic Actions
- [ ] **B)** Reasoning Engine
- [ ] **C)** Dynamic Context Injection
- [ ] **D)** Einstein Trust Layer Integration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The action list contains specific assigned capabilities such as Flow and Apex, which are Agentic Actions.
 
 
</details>

### 20. What is the main function of the reasoning engine in an agent?

- [ ] **A)** It interprets the input and decides which Salesforce actions are required.
- [ ] **B)** It automatically approves all high-stakes actions without review.
- [ ] **C)** It masks all sensitive data before the LLM processes it.
- [ ] **D)** It generates a visual flowchart for the conversation.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The reasoning engine analyzes the user's goal, interprets natural language, and decides which Salesforce actions are needed using available metadata.
 
 
</details>

### 21. Which statements about agent data access are true? Select all that apply.

- [ ] **A)** Agent data access must be explicitly configured through grounding and permissions.
- [ ] **B)** An agent can access data only if it has been granted specific action permissions.
- [ ] **C)** An agent operates within the context of the user's permissions and its own security settings.
- [ ] **D)** An agent automatically inherits access to all objects and fields.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Administrators must explicitly configure an agent's data access through grounding and action permissions, and the agent operates under both user and agent-level security settings.
 
 
</details>


---

### **Productivity and collaboration**

### 22. What is the primary purpose of configuring an Agent Role & Purpose in Salesforce Agentforce?

- [ ] **A)** Defines the specific persona and scope of the agent
- [ ] **B)** Creates a linear flow for the agent to follow
- [ ] **C)** Masks sensitive PII before sending data to the LLM
- [ ] **D)** Assigns the agent a permission set for all data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Agent Role & Purpose defines the specific persona and business scope, preventing the agent from attempting tasks outside its intended domain.
 
 
</details>

### 23. Which of the following are examples of Agentic Actions, or the tools an agent can use? Select all that apply.

- [ ] **A)** Flow Builder flows
- [ ] **B)** Apex classes
- [ ] **C)** Prompt Templates
- [ ] **D)** Reasoning Engine context

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Agentic Actions are the tools assigned to an agent: Flow Builder flows, Apex classes, and Prompt Templates. The Reasoning Engine is the logic layer, not an action.
 
 
</details>

### 24. Review the configuration excerpt below. Which type of agent capability does the component named UpdateCaseStatus represent?

```json
{
  "name": "UpdateCaseStatus",
  "resourceType": "Apex",
  "class": "CaseStatusUpdater",
  "description": "Updates case status"
}
```

- [ ] **A)** Agentic Action
- [ ] **B)** Prompt Template
- [ ] **C)** Data Grounding
- [ ] **D)** Guardrail

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The excerpt describes an Apex class invocation, which is an Agentic Action. Prompt Templates generate text, while grounding and guardrails serve different purposes.
 
 
</details>


---

### **Sales and marketing applications**

### 25. What is the main purpose of defining an agent role in Agentforce configurations for a Sales team?

- [ ] **A)** Restrict to specific business domains.
- [ ] **B)** Grant access to all Salesforce data.
- [ ] **C)** Set chat window branding.
- [ ] **D)** Provide a fixed decision flowchart.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An agent role defines its persona and scope, preventing it from handling tasks outside its intended business domain.
 
 
</details>

### 26. Which two Agentic Actions execute business logic rather than simply generate text for an Agentforce agent?

- [ ] **A)** Flow Builder flows
- [ ] **B)** Apex classes
- [ ] **C)** Prompt Templates
- [ ] **D)** Knowledge article layouts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Flows and Apex classes execute business logic, while Prompt Templates only generate text and do not perform system changes.
 
 
</details>

### 27. An administrator configures the access settings shown in the code block below. Which key Agentforce concept is being configured?

```text
Agent Configuration:
  Access Level: Explicit
  Objects: Opportunity, Lead
  Fields: Amount, Status
  Knowledge Articles: Sales Playbooks
```

- [ ] **A)** Data Grounding
- [ ] **B)** Human-in-the-Loop
- [ ] **C)** Einstein Trust Layer
- [ ] **D)** Reasoning Engine

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Data Grounding connects the agent to specific Salesforce objects, fields, and Knowledge articles for accurate responses.
 
 
</details>


---

### **Service and support applications**

### 28. Which configuration element in an Agentforce agent defines the specific persona and operational scope of the agent?

- [ ] **A)** Agent Role & Purpose
- [ ] **B)** Actions & Tooling
- [ ] **C)** Data Grounding
- [ ] **D)** Einstein Trust Layer Integration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Agent Role & Purpose is the configuration element that defines the agent's persona and scope. This keeps the agent focused on specific business domains and prevents tasks outside its intended boundaries.
 
 
</details>

### 29. Which two statements correctly describe the role of Actions and Tooling when an administrator configures an Agentforce agent?

- [ ] **A)** They execute specific capabilities such as updating Cases or querying Knowledge.
- [ ] **B)** They are the reasoning layer that interprets user intent.
- [ ] **C)** They are the same as Prompt Templates in the agent runtime.
- [ ] **D)** They are configured to call Flows or Apex classes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Actions execute logic, not text generation. They are configured by mapping natural language instructions to Apex classes or Flows and provide capabilities like updating a Case or querying Knowledge. Prompt Templates are not Actions.
 
 
</details>

### 30. Examine the JSON snippet from an Agentforce agent configuration. Based on the value shown for the action type, which statement correctly describes the capability being added?

```json
{
  "agent_config": {
    "name": "ServiceAgent",
    "action": {
      "type": "Flow",
      "name": "CaseStatusUpdateFlow",
      "input": {
        "caseId": "%from context%",
        "newStatus": "Escalated"
      }
    }
  }
}
```

- [ ] **A)** It calls a Flow to update a Case status.
- [ ] **B)** It uses a Prompt Template to generate a response instead of executing logic.
- [ ] **C)** It prevents the agent from updating any record.
- [ ] **D)** It masks sensitive data before LLM processing.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The JSON action type is 'Flow' with a case status update path. Therefore the agent capability is implemented by invoking a Flow rather than by Prompt Template, restrictions, or Trust Layer.
 
 
</details>

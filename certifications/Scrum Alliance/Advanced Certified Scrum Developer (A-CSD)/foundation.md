<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Scrum%20Alliance/Advanced%20Certified%20Scrum%20Developer%20(A-CSD).png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Advanced Certified Scrum Developer (A-CSD)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Agile Engineering Practices](#agile-engineering-practices) (6 questions)
- [Scrum Artifacts](#scrum-artifacts) (5 questions)
- [Scrum Events](#scrum-events) (6 questions)
- [Scrum Roles](#scrum-roles) (5 questions)
- [Scrum Theory and Values](#scrum-theory-and-values) (4 questions)
- [Team Collaboration and Technical Practices](#team-collaboration-and-technical-practices) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:47:45.322Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Agile Engineering Practices | 6 |
| Scrum Artifacts | 5 |
| Scrum Events | 6 |
| Scrum Roles | 5 |
| Scrum Theory and Values | 4 |
| Team Collaboration and Technical Practices | 4 |

---

### **Agile Engineering Practices**

### 1. In the A-CSD context, what does the principle of Collective Ownership of the Increment primarily mean?

- [ ] **A)** Each developer is solely accountable for their assigned code modules.
- [ ] **B)** The whole development group is collectively accountable for quality and seamless integration.
- [ ] **C)** The Product Owner is accountable for the quality of every Increment.
- [ ] **D)** The Scrum Master must ensure that every code change is personally reviewed.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Collective ownership means no single person is responsible for a piece of code; the entire team ensures every item meets the Definition of Done and integrates seamlessly.
 
 
</details>

### 2. Which two behaviors reflect Developer self-management and task autonomy in the A-CSD framework?

- [ ] **A)** Waiting for the Project Manager to assign each task.
- [ ] **B)** Deciding how to turn Product Backlog items into Increments of value.
- [ ] **C)** Managing their own workload and identifying dependencies.
- [ ] **D)** Escalating every technical adjustment to the Product Owner for approval.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Advanced Developers decide how to turn Backlog items into value, manage their own workload, and adjust their technical approach without waiting for manager assignments.
 
 
</details>

### 3. Based on the code block, which A-CSD engineering accountability is most directly threatened for the development team?

```java
class PaymentProcessor {
    // TODO: This method is coupled to the database schema.
    // Only Alice knows why this fallback value is hard-coded.
    public void charge(Customer c) {
        if (c.getBalance() > 100) {
            // ...
        }
    }
}
```

- [ ] **A)** Collective ownership of the Increment
- [ ] **B)** Adherence to the Definition of Done
- [ ] **C)** Negotiating technical debt
- [ ] **D)** Architectural runway management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The comment shows that only one developer understands the logic, creating a knowledge silo and a single point of failure, so collective ownership is violated.
 
 
</details>

### 4. What does the Managerial Fallacy refer to in the A-CSD material?

- [ ] **A)** Assuming a Project Manager or Scrum Master is responsible for ensuring developers follow technical standards.
- [ ] **B)** Believing that developers should not manage their own workload.
- [ ] **C)** Thinking the Product Owner should define the Definition of Done.
- [ ] **D)** Assuming all technical decisions require business approval.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Managerial Fallacy is assuming that a Project Manager or Scrum Master enforces technical standards and task completion instead of the Developers themselves.
 
 
</details>

### 5. Which three activities are part of Technical Backlog Refinement according to the playbook?

- [ ] **A)** Collaborating with the Product Owner to decompose complex stories
- [ ] **B)** Identifying dependencies and clarifying technical constraints
- [ ] **C)** Ensuring the Definition of Ready is met
- [ ] **D)** Replacing the Product Owner's priorities with technical preferences

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Technical Backlog Refinement is a collaboration with the PO to decompose stories, identify dependencies, clarify constraints, and meet the Definition of Ready before the Sprint.
 
 
</details>

### 6. If a developer proposes the database change in the code block without informing the Product Owner, which trap is being committed?

```sql
ALTER TABLE users DROP COLUMN legacy_role;
```

- [ ] **A)** The Silo Fallacy
- [ ] **B)** The Translator Gap
- [ ] **C)** Ownership Confusion
- [ ] **D)** The Task-Oriented Trap

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Silo Fallacy is the assumption that technical decisions such as schema changes have no business impact and require no Product Owner awareness.
 
 
</details>


---

### **Scrum Artifacts**

### 7. In the context of Scrum, what does collective ownership of the Increment mean for the development team?

- [ ] **A)** Everyone is accountable for overall quality
- [ ] **B)** Each developer owns one module
- [ ] **C)** The Product Owner owns quality
- [ ] **D)** The Scrum Master fixes defects

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Collective ownership means all developers share accountability for the quality of the whole Increment, not for isolated pieces.
 
 
</details>

### 8. Which two actions reflect self-management for an advanced Scrum developer when delivering value during a Sprint?

- [ ] **A)** Deciding how to turn Product Backlog items into Increments
- [ ] **B)** Waiting for a manager to assign tasks
- [ ] **C)** Managing workload and identifying dependencies
- [ ] **D)** Escalating all decisions to the Product Owner

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Advanced developers decide how to build Increments, manage their workload, identify dependencies, and adjust their technical approach during the Sprint.
 
 
</details>

### 9. Review the code block and identify which Scrum accountability principle is violated by the logic shown.

```python
if not all([criterion.met for criterion in definition_of_done]):
    story.status = 'Done'
```

- [ ] **A)** Adherence to the Definition of Done
- [ ] **B)** Collective ownership
- [ ] **C)** Technical refactoring
- [ ] **D)** NFR integration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code marks an item as Done without satisfying all Definition of Done criteria, violating the primary measure of team accountability.
 
 
</details>

### 10. According to Scrum, what is the primary measure of accountability for a Scrum team's Increment?

- [ ] **A)** The Definition of Done
- [ ] **B)** The Sprint velocity
- [ ] **C)** The Product Owner's approval
- [ ] **D)** Number of automated tests

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Definition of Done is the primary measure; no item is Done unless every DoD criterion is met.
 
 
</details>

### 11. Which two practices help prevent technical knowledge from being siloed in a Scrum team of developers?

- [ ] **A)** Conducting rigorous peer reviews
- [ ] **B)** Mentoring teammates
- [ ] **C)** Keeping code knowledge within each specialty
- [ ] **D)** Avoiding collaboration to save time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Peer reviews and mentoring spread knowledge, reduce silos, and prevent single points of failure within the team.
 
 
</details>


---

### **Scrum Events**

### 12. According to the playbook, in the context of the Advanced Certified Scrum Developer, what is the primary measure of developer accountability?

- [ ] **A)** The Definition of Done
- [ ] **B)** The number of completed tasks
- [ ] **C)** The Product Owner's satisfaction
- [ ] **D)** The Sprint burndown chart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Definition of Done is the primary measure of accountability. Developers must ensure every criterion is met before any item is considered Done.
 
 
</details>

### 13. Which of the following are presented in the playbook as accountability traps that developers should avoid? Select all that apply.

- [ ] **A)** Managerial Fallacy
- [ ] **B)** Task-Oriented Trap
- [ ] **C)** Silo Assumption
- [ ] **D)** Collective Ownership

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The Managerial Fallacy, Task-Oriented Trap, and Silo Assumption are the accountability traps listed in the playbook. Collective Ownership is a positive practice, not a trap.
 
 
</details>

### 14. Read the developer comment in the code block. Which accountability principle from the playbook is contradicted by the comment?

```plaintext
// I only write my own module; the rest of the system is someone else's problem.

```

- [ ] **A)** Collective ownership of the Increment
- [ ] **B)** Adherence to Definition of Done
- [ ] **C)** NFR Integration
- [ ] **D)** Architectural Runway Management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The comment reflects a siloed mindset, which violates the principle of collective ownership of the whole Increment.
 
 
</details>

### 15. When collaborating with the Product Owner in a Scrum event, how should an A-CSD developer communicate technical debt?

- [ ] **A)** Translate technical risks into business terms
- [ ] **B)** Use detailed technical jargon only
- [ ] **C)** Avoid mentioning debt until it blocks work
- [ ] **D)** Ask the Scrum Master to fix the debt

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A-CSD developers translate technical debt into business terms so the Product Owner can prioritize maintenance and refactoring alongside new features.
 
 
</details>

### 16. According to the playbook, which activities are part of Technical Backlog Refinement? Select all that apply.

- [ ] **A)** Collaborating with the PO to decompose user stories
- [ ] **B)** Identifying dependencies among technical tasks
- [ ] **C)** Ensuring the Definition of Ready is met
- [ ] **D)** Assigning work by the manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Technical Backlog Refinement includes decomposing user stories, identifying dependencies, and ensuring Definition of Ready. Assigning work by a manager is not part of it.
 
 
</details>

### 17. Review the code block. Which two practices would help the developer communicate this performance issue effectively to the Product Owner? Select all that apply.

```plaintext
// The database index on the transactional table is missing, causing a full table scan that will affect the API latency requirements.

```

- [ ] **A)** Translate the issue into business terms
- [ ] **B)** Ignore the performance concern
- [ ] **C)** Include NFRs like latency in the Product Backlog
- [ ] **D)** Ask the Project Manager to assign the work

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Developers should turn performance issues into business impact and ensure NFRs such as latency are represented in the Product Backlog. Ignoring or delegating the issue is not advised.
 
 
</details>


---

### **Scrum Roles**

### 18. What is the core meaning of collective ownership of the Increment in Scrum?

- [ ] **A)** Each developer owns a specific module
- [ ] **B)** The team collectively ensures Increment quality
- [ ] **C)** The Scrum Master owns integration quality
- [ ] **D)** Only senior developers guarantee quality

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Collective ownership means no single person owns a code area; the whole team is accountable for Increment quality and Definition of Done adherence.
 
 
</details>

### 19. Which accountabilities are part of self-management for Advanced Scrum Developers?

- [ ] **A)** Deciding how to deliver Product Backlog value
- [ ] **B)** Waiting for a manager to assign tasks
- [ ] **C)** Managing workload and identifying dependencies
- [ ] **D)** Adjusting technical approach during the Sprint

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Self-management includes deciding how to deliver value, managing workload, identifying dependencies, and adjusting technical approach without waiting for manager assignment.
 
 
</details>

### 20. Review the provided code snippet. What accountability violation is represented?

```javascript
function markItemAsDone(item) { if (item.someChecksPassed) { return 'Done'; } return 'Not Done'; }
```

- [ ] **A)** Failing to adhere to the Definition of Done
- [ ] **B)** Delaying the Sprint Retrospective
- [ ] **C)** Assigning work to the Product Owner
- [ ] **D)** Hiding technical debt from stakeholders

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code marks an item Done based on some checks rather than every Definition of Done criterion, violating the primary measure of accountability.
 
 
</details>

### 21. What is the managerial fallacy in Scrum?

- [ ] **A)** Assuming a manager ensures technical quality
- [ ] **B)** Developers deciding how to accomplish Sprint work
- [ ] **C)** The Product Owner prioritizing the Product Backlog
- [ ] **D)** The team conducting peer reviews

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The managerial fallacy incorrectly places responsibility for developer task completion and technical standards on a Scrum Master or Project Manager.
 
 
</details>

### 22. Which activities are part of Technical Backlog Refinement with the Product Owner?

- [ ] **A)** Decomposing user stories into technical tasks
- [ ] **B)** Identifying dependencies and ensuring Definition of Ready
- [ ] **C)** Clarifying technical constraints early
- [ ] **D)** Assigning story points to the Product Owner

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Developers collaborate with the Product Owner to decompose stories, identify dependencies, meet Definition of Ready, and clarify technical constraints.
 
 
</details>


---

### **Scrum Theory and Values**

### 23. In Scrum, what is the primary measure of a team's accountability for the quality of the Increment?

- [ ] **A)** Definition of Done
- [ ] **B)** Sprint Review feedback
- [ ] **C)** Product Owner approval
- [ ] **D)** Number of completed tasks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Definition of Done is the primary measure of accountability; developers must satisfy every criterion before an item can be considered Done.
 
 
</details>

### 24. Which practices help a team build collective ownership of the Increment rather than relying on individual specialists?

- [ ] **A)** Performing rigorous peer reviews
- [ ] **B)** Coaching one another to prevent knowledge silos
- [ ] **C)** Avoiding review of code outside your specialty
- [ ] **D)** Escalating every defect to a single senior developer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Collective ownership requires peer reviews and mentoring across the team so technical knowledge is not siloed and no single point of failure remains.
 
 
</details>

### 25. Using the doneCriteria list in the code_block, if a feature satisfies only three of the four criteria, what action should the team take?

```javascript
const doneCriteria = ['Code reviewed', 'Unit tests pass', 'Deployed to staging', 'Documentation updated'];
```

- [ ] **A)** Refuse to call it Done until all criteria are met
- [ ] **B)** Mark it Done if the Product Owner agrees
- [ ] **C)** Mark it Done because most criteria are satisfied
- [ ] **D)** Move the unmet criterion to the next Sprint and still call it Done

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Definition of Done is binary; a team must meet every criterion before an item can be transparently marked as Done.
 
 
</details>

### 26. What is the mistake called when a team measures success by completing tickets instead of producing a high-quality, usable Increment?

- [ ] **A)** The Task-Oriented Trap
- [ ] **B)** The Managerial Fallacy
- [ ] **C)** The Silo Assumption
- [ ] **D)** Ownership Confusion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Task-Oriented Trap occurs when the team focuses on completing specific tickets rather than delivering a high-quality Increment that meets the Definition of Done.
 
 
</details>


---

### **Team Collaboration and Technical Practices**

### 27. According to the Scrum Alliance, which group is collectively accountable for the quality of the Increment?

- [ ] **A)** The Product Owner
- [ ] **B)** The Scrum Master
- [ ] **C)** The Developers
- [ ] **D)** The Stakeholders

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Developers are collectively accountable for the quality of the Increment; the whole group ensures every item meets the Definition of Done and integrates seamlessly into the product.
 
 
</details>

### 28. Which responsibilities reflect the developers' commitment to technical excellence and team growth? Select all that apply.

- [ ] **A)** Proactively manage technical debt by refactoring the codebase
- [ ] **B)** Ensure the Definition of Done is met for all completed items
- [ ] **C)** Wait for a project manager to assign technical tasks
- [ ] **D)** Conduct rigorous peer reviews and mentor colleagues

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Advanced Developers are accountable for technical practices, DoD adherence, peer reviews, and knowledge sharing. Waiting for a project manager would reflect the Managerial Fallacy.
 
 
</details>

### 29. Review the developer comment in the code block. Which accountability misconception is being demonstrated?

```python
# This module is my territory. I only check quality in my own files; other modules' issues are not my concern.
```

- [ ] **A)** Collective Ownership
- [ ] **B)** Managerial Fallacy
- [ ] **C)** Silo Assumption
- [ ] **D)** Task-Oriented Trap

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The statement reflects the Silo Assumption: believing a specialist is only accountable for their specific module instead of recognizing collective accountability for the whole system.
 
 
</details>

### 30. What is the primary measure of accountability for Developers in Scrum?

- [ ] **A)** The Sprint Backlog
- [ ] **B)** The Product Owner's request
- [ ] **C)** The Definition of Done
- [ ] **D)** The number of story points completed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Definition of Done is the primary measure of accountability. Developers must ensure no item is marked Done unless it meets every single criterion in the DoD.
 
 
</details>

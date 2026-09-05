<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Salesforce/Salesforce%20Certified%20Business%20Analyst.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Salesforce Certified Business Analyst</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Business Process Mapping](#business-process-mapping) (3 questions)
- [Collaboration with Stakeholders](#collaboration-with-stakeholders) (7 questions)
- [Customer Discovery](#customer-discovery) (5 questions)
- [Requirements](#requirements) (5 questions)
- [User Acceptance](#user-acceptance) (4 questions)
- [User Stories](#user-stories) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:47:14.606Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Business Process Mapping | 3 |
| Collaboration with Stakeholders | 7 |
| Customer Discovery | 5 |
| Requirements | 5 |
| User Acceptance | 4 |
| User Stories | 6 |

---

### **Business Process Mapping**

### 1. In the MoSCoW method, which category represents requirements that are critical for a project's success?

- [ ] **A)** Must have
- [ ] **B)** Should have
- [ ] **C)** Could have
- [ ] **D)** Won't have

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Must-have requirements are critical to a project's success; omitting them means the project cannot launch.
 
 
</details>

### 2. According to the playbook, which of the following options are recognized prioritization traps that should be avoided?

- [ ] **A)** Prioritizing by Technical Ease
- [ ] **B)** Ignoring Dependencies
- [ ] **C)** Static Prioritization
- [ ] **D)** Weighted Scoring Model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Technical ease, ignored dependencies, and static priorities are traps; weighted scoring is a structured prioritization technique.
 
 
</details>

### 3. Review the requirement in the code block. Which MoSCoW category does it match?

```json
{
  "requirement": "The login system is mandatory and without it the product cannot be released."
}
```

- [ ] **A)** Must have
- [ ] **B)** Should have
- [ ] **C)** Could have
- [ ] **D)** Won't have

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The requirement is mandatory for release, so it is a Must have item in the MoSCoW method.
 
 
</details>


---

### **Collaboration with Stakeholders**

### 4. In the MoSCoW method, which category is used for requirements that are critical for project success?

- [ ] **A)** Must have
- [ ] **B)** Should have
- [ ] **C)** Could have
- [ ] **D)** Won't have

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MoSCoW defines 'Must have' as requirements that are critical for success. The other categories represent less critical or out-of-scope items.
 
 
</details>

### 5. Which of the following statements accurately describe the Weighted Scoring Model? Select all that apply.

- [ ] **A)** Stakeholders assign numerical weights to criteria
- [ ] **B)** It reduces subjective bias with final priority scores
- [ ] **C)** It plots value and effort in a quadrant
- [ ] **D)** It quantifies lost opportunity from delay

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Weighted scoring uses numerical weights to reduce subjective bias. Quadrant plotting belongs to Value vs. Effort, and delay costing belongs to Cost of Delay.
 
 
</details>

### 6. Review the dependency mapping in the code. Which requirement should be high priority despite low standalone value?

```json
{
  "dependencies": {
    "R2": ["R1"],
    "R3": ["R1"],
    "R4": ["R1"]
  }
}
```

- [ ] **A)** R1
- [ ] **B)** R2
- [ ] **C)** R3
- [ ] **D)** R4

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> R1 is a prerequisite for R2, R3, and R4, making it a foundational blocker. Dependency mapping says a low-value requirement can be high priority when it enables multiple high-value features.
 
 
</details>

### 7. According to the Value vs. Effort Matrix, which quadrant represents requirements known as 'Quick Wins'?

- [ ] **A)** High business value and low technical effort
- [ ] **B)** High business value and high technical effort
- [ ] **C)** Low business value and low technical effort
- [ ] **D)** Low business value and high technical effort

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The playbook defines 'Quick Wins' as requirements with high business value and low effort in the Value vs. Effort Matrix.
 
 
</details>

### 8. Which of the following are explicitly identified as prioritization traps in the playbook? Select all that apply.

- [ ] **A)** Prioritizing by technical ease
- [ ] **B)** Ignoring dependencies
- [ ] **C)** Static prioritization
- [ ] **D)** Using weighted scoring

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The playbook lists prioritizing by technical ease, ignoring dependencies, and static prioritization as traps. Weighted scoring is a recommended technique, not a trap.
 
 
</details>

### 9. Review the Cost of Delay estimates in the code. Based on the Cost of Delay concept, which feature should be prioritized first?

```json
{
  "Feature_A": 12000,
  "Feature_B": 8500,
  "Feature_C": 15000,
  "Feature_D": 3000
}
```

- [ ] **A)** Feature A
- [ ] **B)** Feature B
- [ ] **C)** Feature C
- [ ] **D)** Feature D

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Cost of Delay quantifies lost opportunity or increased risk. Feature C has the highest estimated cost of delay, so postponing it has the greatest negative impact.
 
 
</details>

### 10. In economic terms, what does the Cost of Delay concept help a Business Analyst quantify?

- [ ] **A)** Lost opportunity or increased risk from delay
- [ ] **B)** The technical effort needed to build a feature
- [ ] **C)** The number of stakeholders needed for approval
- [ ] **D)** The dependency between two requirements

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cost of Delay is an economic concept that quantifies the lost opportunity or increased risk associated with postponing a specific feature.
 
 
</details>


---

### **Customer Discovery**

### 11. In the MoSCoW method, what does the 'Must have' category represent in terms of project success and release scope?

- [ ] **A)** Must have
- [ ] **B)** Should have
- [ ] **C)** Could have
- [ ] **D)** Won't have

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Must have category includes requirements that are critical for project success. MoSCoW uses these non-negotiable items to define the minimum release scope and manage scope creep.
 
 
</details>

### 12. Which of the following are recognized prioritization traps in requirements management that a business analyst should avoid? Select all that apply.

- [ ] **A)** Prioritizing by technical ease
- [ ] **B)** Ignoring dependencies
- [ ] **C)** Static prioritization
- [ ] **D)** Using weighted scoring

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The materials list prioritizing by technical ease, ignoring dependencies, and static prioritization as traps. Weighted scoring is a valid quantitative prioritization technique and is not a trap.
 
 
</details>

### 13. Examine the code block containing value and effort scores, then identify which requirement should be classified as a Quick Win.

```json
[
  { "id": "Req-A", "value": 8, "effort": 2 },
  { "id": "Req-B", "value": 9, "effort": 9 },
  { "id": "Req-C", "value": 3, "effort": 8 },
  { "id": "Req-D", "value": 2, "effort": 2 }
]
```

- [ ] **A)** Req-A
- [ ] **B)** Req-B
- [ ] **C)** Req-C
- [ ] **D)** Req-D

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Quick Win has high business value and low technical effort. Req-A scores value 8 and effort 2, while Req-B is high effort and Req-C/Req-D are low value.
 
 
</details>

### 14. How does the Weighted Scoring Model help business analysts reduce subjective bias during requirements prioritization?

- [ ] **A)** Assigns numerical weights and calculates scores
- [ ] **B)** Plots requirements by value and effort
- [ ] **C)** Sorts requirements into four MoSCoW categories
- [ ] **D)** Measures urgency through lost opportunity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Weighted scoring assigns numerical weights to criteria such as revenue impact and risk reduction, then calculates a score. This structured approach reduces subjective bias.
 
 
</details>

### 15. Which two outcomes does Cost of Delay help a business analyst quantify when a requirement is postponed? Select all that apply.

- [ ] **A)** Lost opportunity
- [ ] **B)** Increased risk
- [ ] **C)** User satisfaction
- [ ] **D)** Technical effort

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Cost of Delay quantifies the lost opportunity and increased risk caused by postponing a feature, helping analysts justify urgency in economic terms.
 
 
</details>


---

### **Requirements**

### 16. In the MoSCoW method, which category is reserved for requirements that are critical to the success of the solution?

- [ ] **A)** Must have
- [ ] **B)** Should have
- [ ] **C)** Could have
- [ ] **D)** Won't have

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Must have requirements are critical for success and cannot be omitted from the release.
 
 
</details>

### 17. Which statements about MoSCoW categories are correct?

- [ ] **A)** Should have requirements are important but not vital.
- [ ] **B)** Could have requirements are desirable but can be omitted.
- [ ] **C)** Won't have requirements are excluded from this release.
- [ ] **D)** Must have requirements are optional if time is short.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> MoSCoW distinguishes critical must-haves, important should-haves, optional could-haves, and items explicitly out of scope.
 
 
</details>

### 18. Refer to the matrix in the block. Which quadrant represents \"Quick Wins\"?

```plaintext
Value vs Effort Matrix:
High Value / Low Effort -> Quick Wins
High Value / High Effort -> Major Projects
Low Value / Low Effort -> Fill-ins
Low Value / High Effort -> Money Pit
```

- [ ] **A)** High Value, Low Effort
- [ ] **B)** High Value, High Effort
- [ ] **C)** Low Value, Low Effort
- [ ] **D)** Low Value, High Effort

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Quick Wins are high business value and low implementation effort, making them attractive first priorities.
 
 
</details>

### 19. What is the main purpose of a weighted scoring model in requirements prioritization?

- [ ] **A)** It reduces subjective bias by using numerical weights and scores.
- [ ] **B)** It replaces all stakeholder judgment with technical analysis.
- [ ] **C)** It ranks requirements only by implementation sequence.
- [ ] **D)** It identifies dependencies between requirements.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Weighted scoring assigns numerical weights to criteria such as revenue impact, risk reduction, or UX to produce a final priority score and reduce bias.
 
 
</details>

### 20. Which of the following are quantitative approaches used to prioritize requirements?

- [ ] **A)** Value vs Effort Matrix
- [ ] **B)** Weighted Scoring Model
- [ ] **C)** Cost of Delay
- [ ] **D)** MoSCoW Method

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Value vs Effort, weighted scoring, and cost of delay are quantitative approaches; MoSCoW is a qualitative categorization.
 
 
</details>


---

### **User Acceptance**

### 21. In the MoSCoW method, what is the meaning of 'Should have'?

- [ ] **A)** Critical for success and cannot be omitted
- [ ] **B)** Important but not vital for the release
- [ ] **C)** Desirable but can be omitted
- [ ] **D)** Not included in this release

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In MoSCoW, 'Should have' means important but not vital, so the solution can still launch without it.
 
 
</details>

### 22. Which of the following are prioritization techniques described in the playbook? Select all that apply.

- [ ] **A)** MoSCoW Method
- [ ] **B)** Value vs. Effort Matrix
- [ ] **C)** Dependency Mapping
- [ ] **D)** Scope Creep Analysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The playbook describes MoSCoW, Value vs. Effort Matrix, Weighted Scoring, Cost of Delay, and Dependency Mapping. Scope Creep Analysis is not one of them.
 
 
</details>

### 23. Based on the Weighted Scoring Model results in the code block, which requirement should receive the highest priority?

```json
[
  {"requirement": "A", "score": 72},
  {"requirement": "B", "score": 84},
  {"requirement": "C", "score": 91},
  {"requirement": "D", "score": 68}
]
```

- [ ] **A)** Requirement A
- [ ] **B)** Requirement B
- [ ] **C)** Requirement C
- [ ] **D)** Requirement D

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Requirement C has the highest score (91), so it should be prioritized first under the Weighted Scoring Model.
 
 
</details>

### 24. In the Value vs. Effort Matrix, how are 'Quick Wins' defined?

- [ ] **A)** High business value and low effort
- [ ] **B)** High business value and high effort
- [ ] **C)** Low business value and low effort
- [ ] **D)** Low business value and high effort

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> 'Quick Wins' are requirements plotted as High Value and Low Effort in the Value vs. Effort Matrix.
 
 
</details>


---

### **User Stories**

### 25. What does the MoSCoW method primarily help a business analyst do?

- [ ] **A)** Categorize requirements into four priority groups
- [ ] **B)** Calculate the return on investment of a project
- [ ] **C)** Identify all technical dependencies
- [ ] **D)** Assign monetary values to user stories

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MoSCoW categorizes requirements as Must have, Should have, Could have, or Won't have to establish priority boundaries.
 
 
</details>

### 26. Which statements about the Value vs. Effort Matrix are correct?

- [ ] **A)** High value and low effort is a Quick Win
- [ ] **B)** High value and high effort is a Major Project
- [ ] **C)** Low value and low effort should always be avoided
- [ ] **D)** It plots business value against implementation effort

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> The Value vs. Effort Matrix plots business value against effort, with Quick Wins being high value/low effort and Major Projects being high value/high effort.
 
 
</details>

### 27. Review the four requirements in the code block. Which one should be classified as a Must have using MoSCoW?

```text
Requirement 1: The system cannot launch without this feature.
Requirement 2: The feature is important but a workaround exists.
Requirement 3: The feature is desirable but optional.
Requirement 4: The feature is explicitly out of scope for this release.
```

- [ ] **A)** The requirement the system cannot launch without
- [ ] **B)** The requirement that is important but has a workaround
- [ ] **C)** The requirement that is desirable but optional
- [ ] **D)** The requirement that is explicitly out of scope

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Must have is critical for success, so the requirement without which the system cannot launch belongs in that category.
 
 
</details>

### 28. What does Cost of Delay quantify in requirement prioritization?

- [ ] **A)** The lost opportunity or risk caused by postponing a feature
- [ ] **B)** The total monetary cost to build the feature
- [ ] **C)** The amount of effort needed to develop the requirement
- [ ] **D)** The number of dependencies blocked by the feature

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cost of Delay helps business analysts justify urgency by quantifying lost opportunity or increased risk from postponing a requirement.
 
 
</details>

### 29. Which of the following are prioritization traps described in the playbook?

- [ ] **A)** Choosing tasks based on technical ease
- [ ] **B)** Treating requirements as independent units
- [ ] **C)** Assuming the backlog never changes
- [ ] **D)** Applying a weighted scoring model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The traps are prioritizing by technical ease, ignoring dependencies, and static prioritization. Weighted scoring is a valid prioritization method.
 
 
</details>

### 30. Review the dependency relationships in the code block. Why should the low-value feature be considered a high priority?

```text
Feature A: Low value on its own.
Feature B: Depends on Feature A.
Feature C: Depends on Feature A.
Feature D: High value and independent.
```

- [ ] **A)** It is a prerequisite for multiple features
- [ ] **B)** It has the lowest implementation effort
- [ ] **C)** It is a Must have by definition
- [ ] **D)** It reduces the cost of delay

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Dependency mapping shows that a low-value requirement becomes high priority when it blocks multiple high-value features.
 
 
</details>

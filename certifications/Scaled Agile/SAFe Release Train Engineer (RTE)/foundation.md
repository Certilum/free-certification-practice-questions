<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/SAFe%20by%20Scaled%20Agile%2C%20Inc./SAFe%20Release%20Train%20Engineer%20(RTE).png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>SAFe Release Train Engineer (RTE)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Applying AI to the RTE Role](#applying-ai-to-the-rte-role) (4 questions)
- [Coaching the ART](#coaching-the-art) (4 questions)
- [Exploring the RTE Role and Responsibilities](#exploring-the-rte-role-and-responsibilities) (5 questions)
- [Facilitating PI Planning](#facilitating-pi-planning) (3 questions)
- [Fostering Relentless Improvement](#fostering-relentless-improvement) (5 questions)
- [Optimizing Flow](#optimizing-flow) (2 questions)
- [Organizing the ART](#organizing-the-art) (3 questions)
- [Supporting PI Execution](#supporting-pi-execution) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:47:42.768Z |
| Domains | 8 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Applying AI to the RTE Role | 4 |
| Coaching the ART | 4 |
| Exploring the RTE Role and Responsibilities | 5 |
| Facilitating PI Planning | 3 |
| Fostering Relentless Improvement | 5 |
| Optimizing Flow | 2 |
| Organizing the ART | 3 |
| Supporting PI Execution | 4 |

---

### **Applying AI to the RTE Role**

### 1. Which visualization is the primary tool for an RTE to identify bottlenecks?

- [ ] **A)** Cumulative Flow Diagram (CFD)
- [ ] **B)** Kanban Board
- [ ] **C)** Velocity Chart
- [ ] **D)** Burndown Chart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CFD is the primary visual tool for identifying bottlenecks; a widening band indicates accumulating work in a specific state.
 
 
</details>

### 2. Which metrics should an RTE monitor to quantitatively evaluate ART flow? Select all that apply.

- [ ] **A)** Lead Time
- [ ] **B)** Cycle Time
- [ ] **C)** Throughput
- [ ] **D)** Team Velocity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The flow metrics are Lead Time, Cycle Time, and Throughput. Team velocity is not a flow metric and can mislead ART-level analysis.
 
 
</details>

### 3. Inspect the CFD data provided in the JSON block. Which stage shows a widening band over time?

```json
{
  "weeks": ["W1", "W2", "W3"],
  "backlog": [20, 22, 24],
  "analysis": [8, 8, 9],
  "testing": [2, 8, 15],
  "done": [5, 6, 6]
}
```

- [ ] **A)** Backlog
- [ ] **B)** Analysis
- [ ] **C)** Testing
- [ ] **D)** Done

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Testing band grows from 2 to 15 while Done stays flat, indicating work is accumulating in Testing and creating a bottleneck.
 
 
</details>

### 4. In a Cumulative Flow Diagram, what does a widening band signal?

- [ ] **A)** Work accumulating in a state and a capacity constraint
- [ ] **B)** Throughput increasing across the ART
- [ ] **C)** Team velocity improving
- [ ] **D)** WIP limits being reduced

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A widening CFD band indicates work is accumulating in a specific state, signaling a capacity constraint that throttles throughput.
 
 
</details>


---

### **Coaching the ART**

### 5. What is the primary visual tool an RTE uses to identify bottlenecks in the ART flow?

- [ ] **A)** Cumulative Flow Diagram (CFD)
- [ ] **B)** Velocity Chart
- [ ] **C)** Sprint Burndown Chart
- [ ] **D)** Gantt Chart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CFD is the primary visual tool because widening bands reveal accumulating work and capacity constraints.
 
 
</details>

### 6. Which of the following are common traps that an RTE must avoid? Select all that apply.

- [ ] **A)** Assuming that a high-performing team is the solution to bottleneck issues
- [ ] **B)** Confusing a delay with a systemic bottleneck
- [ ] **C)** Focusing on individual productivity instead of system flow
- [ ] **D)** Limiting WIP to increase predictability

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> All three listed traps are real: high-performing teams don't fix constraints, delays differ from bottlenecks, and individual focus ignores system flow. Limiting WIP is healthy.
 
 
</details>

### 7. Based on the calculation shown in the code block, which flow metric is being computed?

```python
active_time = 120
total_lead_time = 480
metric = active_time / total_lead_time
```

- [ ] **A)** Cycle Time
- [ ] **B)** Lead Time
- [ ] **C)** Flow Efficiency
- [ ] **D)** Throughput

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Flow efficiency is active work time divided by total lead time; the code calculates that ratio.
 
 
</details>

### 8. Where should an RTE focus improvement efforts according to the Theory of Constraints?

- [ ] **A)** The bottleneck stage
- [ ] **B)** The fastest team
- [ ] **C)** The most expensive resource
- [ ] **D)** The stage with the most automated tests

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Improvements made anywhere other than the bottleneck are illusory, so the RTE must target the constraint.
 
 
</details>


---

### **Exploring the RTE Role and Responsibilities**

### 9. What is the main visual tool an RTE uses to identify bottlenecks in the ART flow?

- [ ] **A)** Cumulative Flow Diagram (CFD)
- [ ] **B)** Team velocity chart
- [ ] **C)** Resource utilization heatmap
- [ ] **D)** Project milestone list

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A CFD is the primary visual tool for spotting bottlenecks. A widening band indicates accumulating work in a specific state, throttling ART throughput.
 
 
</details>

### 10. Which two statements correctly identify common traps that an RTE must avoid when managing ART flow?

- [ ] **A)** Confusing a delay with a bottleneck
- [ ] **B)** Focusing on individual team productivity instead of system flow
- [ ] **C)** Applying the Theory of Constraints to the bottleneck
- [ ] **D)** Using a Kanban board as a live management tool

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Common traps include confusing a moment-in-time delay with a systemic bottleneck and focusing on individual productivity. The RTE must focus on system flow and use boards as active management tools.
 
 
</details>

### 11. Examine the stage cycle times in the code block. Which stage is showing a leading indicator of a localized bottleneck?

```json
{
  "stages": [
    {"name": "Development", "cycle_time_days": 3},
    {"name": "Testing", "cycle_time_days": 12},
    {"name": "Deployment", "cycle_time_days": 2}
  ]
}
```

- [ ] **A)** Testing
- [ ] **B)** Development
- [ ] **C)** Deployment
- [ ] **D)** No stage can be inferred

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cycle time increasing or much longer in a specific phase is a leading indicator of a bottleneck. Testing has the highest cycle time in the data.
 
 
</details>

### 12. According to the Theory of Constraints, where should an RTE focus improvement efforts to optimize the ART?

- [ ] **A)** The specific stage that limits total system throughput
- [ ] **B)** The non-bottleneck stage with the highest efficiency
- [ ] **C)** The stage with the most available capacity
- [ ] **D)** The team with the highest velocity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Theory of Constraints says improvement anywhere other than the bottleneck is an illusion. The RTE must focus on the stage limiting total throughput.
 
 
</details>

### 13. Which flow metrics should an RTE monitor to provide quantitative evidence of ART health during PI execution?

- [ ] **A)** Lead Time
- [ ] **B)** Cycle Time
- [ ] **C)** Throughput
- [ ] **D)** Resource Utilization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The RTE monitors Lead Time, Cycle Time, and Throughput. These metrics provide empirical evidence to evaluate ART health and predict delivery timelines.
 
 
</details>


---

### **Facilitating PI Planning**

### 14. Which visualization is the primary tool for an RTE to identify bottlenecks in an Agile Release Train?

- [ ] **A)** Cumulative Flow Diagram (CFD)
- [ ] **B)** Burndown Chart
- [ ] **C)** Feature Dependency Diagram
- [ ] **D)** Velocity Chart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A CFD is the primary visual tool for an RTE because a widening band reveals work accumulating in a state, signaling a bottleneck.
 
 
</details>

### 15. Why does an RTE promote strict WIP limits on the ART Kanban? Select two.

- [ ] **A)** They reveal constraints when a stage reaches its limit.
- [ ] **B)** They prevent multitasking and cognitive overload.
- [ ] **C)** They are used to evaluate individual developer productivity.
- [ ] **D)** They put pressure on teams to increase their local velocity.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> WIP limits reveal constraints when a stage is full and prevent multitasking. They do not measure individual productivity or encourage local velocity.
 
 
</details>

### 16. Review the ART Kanban data in the code block. Which stage is the bottleneck?

```plaintext
ART Kanban snapshot:
Funnel: 4 items
Analysis: 3 items
Development: 5 items
Testing: 8 items (WIP limit: 5)
Done: 2 items
Testing cycle time: 7 days (ART average: 3 days)
```

- [ ] **A)** Development
- [ ] **B)** Testing
- [ ] **C)** Funnel
- [ ] **D)** Done

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Testing has 8 items against a WIP limit of 5, and its cycle time is well above average, indicating it is the clogged stage.
 
 
</details>


---

### **Fostering Relentless Improvement**

### 17. Which visual tool is the primary one an RTE uses to identify bottlenecks?

- [ ] **A)** Cumulative Flow Diagram
- [ ] **B)** Team Board
- [ ] **C)** Program Board
- [ ] **D)** Value Stream Map

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CFD is the primary visual tool for an RTE to identify bottlenecks by revealing where work accumulates.
 
 
</details>

### 18. Which statements about WIP limits are correct?

- [ ] **A)** They make constraints visible when a stage reaches its limit.
- [ ] **B)** They are only needed after a bottleneck is fixed.
- [ ] **C)** They prevent hidden accumulation of unfinished work.
- [ ] **D)** They help maintain a predictable cadence.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> WIP limits expose constraints, prevent hidden work, and support cadence. They are not needed only after a bottleneck is fixed.
 
 
</details>

### 19. Review the SQL output in the code block. Which stage is most likely the bottleneck?

```sql
SELECT 'Development' AS stage, 18 AS work_items, 30 AS wip_limit
UNION ALL SELECT 'Testing', 35, 20
UNION ALL SELECT 'Review', 15, 20
UNION ALL SELECT 'Done', 10, 15
```

- [ ] **A)** Development
- [ ] **B)** Testing
- [ ] **C)** Review
- [ ] **D)** Done

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Testing has 35 work items against a WIP limit of 20, showing accumulated work beyond the agreed constraint.
 
 
</details>

### 20. According to the Theory of Constraints, where should improvement efforts be focused?

- [ ] **A)** The fastest team
- [ ] **B)** The system bottleneck
- [ ] **C)** The first step in the flow
- [ ] **D)** The most expensive resource

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Theory of Constraints states that improvement anywhere other than the bottleneck is an illusion, so the RTE focuses on the bottleneck.
 
 
</details>

### 21. Which of the following are flow metrics monitored by an RTE?

- [ ] **A)** Lead Time
- [ ] **B)** Cycle Time
- [ ] **C)** Throughput
- [ ] **D)** Story Point Velocity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Lead Time, Cycle Time, and Throughput are flow metrics. Team velocity is not a flow metric for predicting ART delivery.
 
 
</details>


---

### **Optimizing Flow**

### 22. Which visualization is the primary tool an RTE uses to identify bottlenecks on an ART?

- [ ] **A)** Cumulative Flow Diagram (CFD)
- [ ] **B)** Team velocity chart
- [ ] **C)** Program increment burndown chart
- [ ] **D)** Detailed Gantt schedule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CFD is the primary visual tool for an RTE. A widening band in a CFD shows where work is accumulating, which directly reveals bottlenecks.
 
 
</details>

### 23. Which quantitative flow metrics give the RTE evidence of ART health and support delivery predictions? Select all that apply.

- [ ] **A)** Lead Time
- [ ] **B)** Cycle Time
- [ ] **C)** Throughput
- [ ] **D)** Resource Utilization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Lead Time, Cycle Time, and Throughput are the flow metrics the RTE monitors. High resource utilization can be misleading because it often increases WIP and wait times.
 
 
</details>


---

### **Organizing the ART**

### 24. Which statement best describes the primary visual tool an RTE uses to identify bottlenecks in the ART flow?

- [ ] **A)** Cumulative Flow Diagram (CFD)
- [ ] **B)** Team burndown chart
- [ ] **C)** Program Predictability Measure
- [ ] **D)** Sprint board for a high-performing team

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CFD is the primary visual tool for identifying bottlenecks. A widening band indicates work is accumulating in a specific state, such as Testing or Review, which signals a capacity constraint throttling ART throughput. Local team tools do not provide system-level flow visibility.
 
 
</details>

### 25. Which two practices are aligned with an RTE's responsibility to optimize ART-level flow?

- [ ] **A)** Increasing the speed of every stage so each stage operates at maximum possible throughput
- [ ] **B)** Applying WIP limits and investigating when a stage reaches its limit
- [ ] **C)** Focusing improvement on the process bottleneck even if upstream teams appear fast
- [ ] **D)** Reassigning people to maximize individual productivity at every stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> The RTE applies WIP limits to make constraints visible and investigates stalling work when limits are exceeded. The Theory of Constraints states that improvement anywhere except the bottleneck is an illusion, so the RTE must focus on the true system constraint. Maximizing every stage or individual productivity creates excessive WIP and defeats healthy system flow.
 
 
</details>

### 26. Based on the cumulative flow data in the code block below, which stage is most likely the bottleneck?

```plaintext
WIP by Stage per Week
Stage: Backlog | Analysis | Development | Testing | Done
Week 1:   20    |    8     |     12      |   4    |   2
Week 2:   22    |   10     |     15      |   8    |   4
Week 3:   24    |   12     |     17      |  16    |   7
Week 4:   26    |   14     |     18      |  28    |   9
```

- [ ] **A)** Development
- [ ] **B)** Testing
- [ ] **C)** Backlog
- [ ] **D)** Done

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Testing WIP grows from 4 to 28 items over four weeks, while other stages grow more slowly. The widening band for Testing indicates a systemic capacity constraint and is the clearest bottleneck signal in the data.
 
 
</details>


---

### **Supporting PI Execution**

### 27. Which visual tool is the RTE's primary instrument for identifying bottlenecks in the ART?

- [ ] **A)** Cumulative Flow Diagram (CFD)
- [ ] **B)** Team Burndown Chart
- [ ] **C)** Program Board
- [ ] **D)** Value Stream Map

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CFD is the primary visual tool for an RTE to identify bottlenecks and observe process stability over time.
 
 
</details>

### 28. Which metrics does an RTE monitor to empirically evaluate the health of the ART? (Select all that apply)

- [ ] **A)** Lead Time
- [ ] **B)** Cycle Time
- [ ] **C)** Throughput
- [ ] **D)** Velocity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The RTE monitors Lead Time, Cycle Time, and Throughput as flow metrics. Velocity is a team-based story-point measure, not an ART flow metric.
 
 
</details>

### 29. Examine the dataset in the code block. Which stage shows a growing accumulation of work?

```python
cfd_data = {
    "Backlog": [10, 12, 15],
    "Development": [8, 9, 8],
    "Testing": [5, 9, 14],
    "Done": [3, 4, 5]
}
```

- [ ] **A)** Testing
- [ ] **B)** Backlog
- [ ] **C)** Development
- [ ] **D)** Done

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Testing grows from 5 to 14, widening significantly while other stages remain stable, signaling a bottleneck in that state.
 
 
</details>

### 30. What does a widening band in a Cumulative Flow Diagram signal?

- [ ] **A)** Work is accumulating in a specific state
- [ ] **B)** Throughput is increasing
- [ ] **C)** WIP is decreasing
- [ ] **D)** The process is becoming more stable

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A widening band in a CFD indicates work is accumulating in a state, often revealing a capacity constraint that throttles throughput.
 
 
</details>

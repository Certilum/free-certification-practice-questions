<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/FinOps%20Foundation/FinOps%20Certified%20Practitioner.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>FinOps Certified Practitioner</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Cloud Cost Management Concepts](#cloud-cost-management-concepts) (4 questions)
- [Commitment-based Discounts](#commitment-based-discounts) (3 questions)
- [Cost Allocation and Tagging](#cost-allocation-and-tagging) (4 questions)
- [FinOps Lifecycle](#finops-lifecycle) (8 questions)
- [FinOps Principles and Personas](#finops-principles-and-personas) (6 questions)
- [Organizational Adoption](#organizational-adoption) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:37.680Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Cloud Cost Management Concepts | 4 |
| Commitment-based Discounts | 3 |
| Cost Allocation and Tagging | 4 |
| FinOps Lifecycle | 8 |
| FinOps Principles and Personas | 6 |
| Organizational Adoption | 5 |

---

### **Cloud Cost Management Concepts**

### 1. In which phase of the FinOps lifecycle would a team purchase a Reserved Instance to reduce committed cloud spend?

- [ ] **A)** Inform
- [ ] **B)** Optimize
- [ ] **C)** Operate
- [ ] **D)** Data Collection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Purchasing Reserved Instances is an optimization action. The Inform phase focuses on visibility and allocation, not procurement decisions.
 
 
</details>

### 2. Which statements about cloud tagging in a FinOps practice are correct? Select all that apply.

- [ ] **A)** Tagging is primarily a technical task for cloud engineers.
- [ ] **B)** Tagging is a cross-functional governance requirement.
- [ ] **C)** Tagging must support cost allocation and accountability.
- [ ] **D)** Tagging is a one-time activity performed when a resource is created.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Tagging is not purely technical; it is a governance practice that requires collaboration and must support cost allocation and accountability.
 
 
</details>

### 3. Examine the cost item shown below. In which FinOps phase should this unallocated spend be resolved?

```json
{
  "cost_item": "shared-cloud-services",
  "allocated_owner": "unassigned",
  "amount": 4800
}
```

- [ ] **A)** Inform
- [ ] **B)** Optimize
- [ ] **C)** Operate
- [ ] **D)** Data Collection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Unallocated spend is addressed in the Inform phase by improving cost visibility and allocation; it is not an Operate phase activity.
 
 
</details>

### 4. In a FinOps context, what is the difference between rightsizing a resource and purchasing Reserved Instances?

- [ ] **A)** Rightsizing changes the resource type or size; Reserved Instances change payment.
- [ ] **B)** Rightsizing changes the payment plan, while Reserved Instances change the resource type.
- [ ] **C)** Rightsizing only applies to storage, while Reserved Instances apply only to compute.
- [ ] **D)** Rightsizing is an Inform activity, while Reserved Instances are an Operate activity.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Rightsizing adjusts the type or size of a cloud resource to match workload demand, whereas a Reserved Instance is a commitment-based pricing method.
 
 
</details>


---

### **Commitment-based Discounts**

### 5. Which common trap is shown when someone purchases commitment-based discounts during the Inform phase?

- [ ] **A)** Confusing Inform with Optimize
- [ ] **B)** Treating tagging as purely technical
- [ ] **C)** Relying on unallocated spend
- [ ] **D)** Falling into the latency trap

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Purchasing commitment-based discounts is an Optimize action, so assigning it to Inform reflects the trap of confusing Inform with Optimize.
 
 
</details>

### 6. Based on the playbook, which two statements about tagging in FinOps are correct?

- [ ] **A)** It is a purely technical task
- [ ] **B)** It is a cross-functional governance requirement
- [ ] **C)** It should be managed by a single team
- [ ] **D)** It is not purely technical

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Tagging in FinOps is cross-functional governance, so it is neither purely technical nor managed by one team.
 
 
</details>

### 7. Review the snippet below. Which common trap does this phase-action pairing represent?

```json
{
  "phase": "Inform",
  "action": "Purchase Reserved Instances"
}
```

- [ ] **A)** Confusing Inform with Optimize
- [ ] **B)** Equating Optimization with cost reduction
- [ ] **C)** Treating Operate as the final phase
- [ ] **D)** Assuming FinOps is centralized

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet assigns a commitment purchase to Inform, but commitment purchases belong to Optimize, so the trap is phase confusion.
 
 
</details>


---

### **Cost Allocation and Tagging**

### 8. In FinOps, purchasing a Reserved Instance is an activity in which phase?

- [ ] **A)** Inform phase
- [ ] **B)** Optimize phase
- [ ] **C)** Operate phase
- [ ] **D)** Tagging phase

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Purchasing Reserved Instances is a cost optimization action; it changes the payment model, not an Inform-phase reporting activity.
 
 
</details>

### 9. Which statements correctly describe tagging in FinOps?

- [ ] **A)** It is purely a technical task
- [ ] **B)** It is a cross-functional governance requirement
- [ ] **C)** It should be managed only by engineering
- [ ] **D)** It requires coordination across finance, engineering, and operations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Tagging is a cross-functional governance requirement, not a purely technical task. Effective tagging requires coordinated decisions from finance, engineering, and operations.
 
 
</details>

### 10. The query shown in the code block finds resources without a cost-center tag. In which phase should the resulting unallocated spend be addressed?

```sql
SELECT resource_id
FROM resources
WHERE tags NOT LIKE '%cost_center=%';
```

- [ ] **A)** Inform phase
- [ ] **B)** Optimize phase
- [ ] **C)** Operate phase
- [ ] **D)** Tagging phase

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Unallocated spend is identified and made visible in the Inform phase; it is not a problem to be solved in the Operate phase.
 
 
</details>

### 11. In FinOps, what does rightsizing change?

- [ ] **A)** The type or size of the resource
- [ ] **B)** The payment commitment or discount
- [ ] **C)** The tags applied to the resource
- [ ] **D)** The cloud provider being used

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Rightsizing changes the type or size of a resource, while Reserved Instances change how you pay. They are distinct optimization actions.
 
 
</details>


---

### **FinOps Lifecycle**

### 12. In the FinOps lifecycle, which activity is performed during the Inform phase rather than during the Optimize phase?

- [ ] **A)** Purchasing Reserved Instances
- [ ] **B)** Rightsizing compute resources
- [ ] **C)** Allocating cloud costs to teams
- [ ] **D)** Negotiating discounts with providers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Inform focuses on visibility, accountability, and cost allocation. Reserved Instances, rightsizing, and rate negotiation belong to Optimize.
 
 
</details>

### 13. Which statements about tagging in FinOps are correct when the practice is implemented by multiple teams? Select all that apply.

- [ ] **A)** A purely technical task
- [ ] **B)** A cross-functional governance requirement
- [ ] **C)** Needed to support cost allocation
- [ ] **D)** Irrelevant to finance teams

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Tagging is a cross-functional governance requirement, not purely technical. It supports cost allocation and must involve finance, engineering, and operations.
 
 
</details>

### 14. Review the SQL query in the code block. Which phase of the FinOps lifecycle is directly supported by grouping cost data by cost center?

```sql
SELECT cost_center,
       SUM(billed_cost) AS total_cost
FROM cloud_billing
GROUP BY cost_center;
```

- [ ] **A)** Optimize
- [ ] **B)** Inform
- [ ] **C)** Operate
- [ ] **D)** Procurement

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Grouping billing data by cost center increases cost visibility and allocation, which are core goals of the Inform phase.
 
 
</details>

### 15. Compared with Reserved Instances, which resource attribute does rightsizing change in a cloud workload to better match demand?

- [ ] **A)** The payment commitment
- [ ] **B)** The resource type or size
- [ ] **C)** The cloud provider region
- [ ] **D)** The billing owner

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Rightsizing changes the type or size of a resource. Reserved Instances change payment commitment and rate, not the resource itself.
 
 
</details>

### 16. Which two statements correctly describe optimization in the FinOps lifecycle rather than as a one-time cost-cutting exercise?

- [ ] **A)** It is a one-time cleanup project.
- [ ] **B)** It is a continuous improvement loop.
- [ ] **C)** It focuses exclusively on cutting costs.
- [ ] **D)** It seeks to maximize business value.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Optimization is a continuous, value-driven process. Cost reduction is part of it, but not the exclusive objective.
 
 
</details>

### 17. The command in the code block changes an EC2 instance type. Which FinOps optimization action does this represent?

```bash
aws ec2 modify-instance-attribute --instance-id i-1234567890abcdef0 --instance-type t3.small
```

- [ ] **A)** Purchasing a Savings Plan
- [ ] **B)** Rightsizing
- [ ] **C)** Data collection
- [ ] **D)** Budgeting

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Changing an instance type or size is rightsizing. Purchasing plans and savings plans address payment commitments.
 
 
</details>

### 18. In which FinOps phase should unallocated spend be addressed so it does not create hidden costs or blind spots?

- [ ] **A)** Operate
- [ ] **B)** Optimize
- [ ] **C)** Inform
- [ ] **D)** Procurement

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Unallocated spend is a visibility and allocation challenge, addressed in Inform by defining allocation policies for shared costs.
 
 
</details>

### 19. Which statements accurately describe the Operate phase of the FinOps lifecycle when considering phase interactions? Select all that apply.

- [ ] **A)** It encourages decentralized accountability
- [ ] **B)** It is a one-time final step
- [ ] **C)** It involves continuous operational improvement
- [ ] **D)** It centralizes all decision-making

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Operate emphasizes decentralized accountability and continuous improvement. It is part of a loop, not a final or centralized stage.
 
 
</details>


---

### **FinOps Principles and Personas**

### 20. Which statement correctly distinguishes the Inform phase from the Optimize phase?

- [ ] **A)** Purchasing Reserved Instances is an Inform-phase activity.
- [ ] **B)** Purchasing Reserved Instances belongs to the Optimize phase, not the Inform phase.
- [ ] **C)** Collecting usage data is an Optimize-phase activity.
- [ ] **D)** Tagging is a purely technical Inform-phase task.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Purchasing Reserved Instances is a rate optimization action and belongs in the Optimize phase. The Inform phase focuses on visibility, allocation, and data collection, so confusing these two phases is a common trap.
 
 
</details>

### 21. Select two statements that correctly describe tagging in FinOps.

- [ ] **A)** Tagging is only a technical responsibility of the cloud engineering team.
- [ ] **B)** Tagging is a cross-functional governance requirement.
- [ ] **C)** Tagging requires alignment among finance, engineering, and business stakeholders.
- [ ] **D)** Tagging is only relevant during the Operate phase.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Tagging is not purely technical; it is a cross-functional governance requirement that requires alignment among finance, engineering, and business stakeholders to support allocation and accountability.
 
 
</details>

### 22. Review the code excerpt. Which activity has been assigned to the wrong phase?

```python
phase_assignment = {
    "reserved_instance_purchase": "Optimize",
    "rightsizing_instance": "Optimize",
    "identify_savings_opportunities": "Operate",
    "collect_usage_data": "Inform"
}
```

- [ ] **A)** reserved_instance_purchase
- [ ] **B)** rightsizing_instance
- [ ] **C)** identify_savings_opportunities
- [ ] **D)** collect_usage_data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Identifying savings opportunities is an optimization activity, not an Operate phase activity. The code incorrectly places it in Operate, reflecting the trap of confusing Optimization with Operation.
 
 
</details>

### 23. In which phase should the problem of unallocated spend be handled?

- [ ] **A)** Operate phase, as an operational cleanup task.
- [ ] **B)** Inform phase, because it is a visibility and allocation problem.
- [ ] **C)** Optimize phase, because it is a rate discount problem.
- [ ] **D)** It should never be analyzed after initial allocation.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Unallocated spend is an allocation and visibility challenge, so it belongs in the Inform phase. Treating it as an Operate phase cleanup task is a common trap.
 
 
</details>

### 24. Select two statements that correctly describe FinOps optimization concepts.

- [ ] **A)** Optimization focuses on value, not only on cost reduction.
- [ ] **B)** Rightsizing changes the type or size of a resource.
- [ ] **C)** Reserved Instances change the type or size of a resource.
- [ ] **D)** Optimization is a destination that stops when a cost target is met.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> True optimization focuses on value, and rightsizing changes the type or size of a resource. Reserved Instances change pricing and discounting, not the resource type or size, and optimization is a continuous loop, not a destination.
 
 
</details>

### 25. Review the code excerpt. Which action is incorrectly labeled as an optimization activity?

```python
actions = {
    "collect_cloud_logs": "optimization",
    "resize_underutilized_instance": "optimization",
    "purchase_reserved_capacity": "optimization",
    "adjust_instance_type": "optimization"
}
```

- [ ] **A)** collect_cloud_logs
- [ ] **B)** resize_underutilized_instance
- [ ] **C)** purchase_reserved_capacity
- [ ] **D)** adjust_instance_type

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Collecting cloud logs is data collection, a prerequisite for optimization, but it is not an optimization action by itself. The other actions are usage or rate optimization.
 
 
</details>


---

### **Organizational Adoption**

### 26. To which phase of the FinOps lifecycle does purchasing Reserved Instances belong?

- [ ] **A)** Inform
- [ ] **B)** Optimize
- [ ] **C)** Operate
- [ ] **D)** Allocate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Purchasing Reserved Instances is an Optimize-phase action because it changes commitment and discounts rather than providing visibility or operational accountability.
 
 
</details>

### 27. Why is tagging considered a cross-functional governance requirement rather than a purely technical task? Select all that apply.

- [ ] **A)** Requires alignment across finance, engineering, and product teams
- [ ] **B)** Enables cost allocation and accountability
- [ ] **C)** Can be delegated to one technical team
- [ ] **D)** Is only relevant during the Optimize phase

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Tagging is cross-functional because it requires stakeholder alignment and supports cost allocation. A single team or a single phase cannot make tagging effective.
 
 
</details>

### 28. Review the instance configuration change in the code block. Which FinOps optimization type does it represent?

```yaml
instances:
  web-server:
    previous_type: t3.medium
    current_type: m5.large
```

- [ ] **A)** Rightsizing
- [ ] **B)** Reserved Instance purchase
- [ ] **C)** Data collection
- [ ] **D)** Unallocated cost allocation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Changing an instance from t3.medium to m5.large alters the resource type and size, which is rightsizing. Reserved Instances change commitment and discount, not the resource specification.
 
 
</details>

### 29. Why is optimization a continuous loop rather than a one-time event?

- [ ] **A)** Cloud usage changes and creates new opportunities
- [ ] **B)** Cost goals stay met after a single pass
- [ ] **C)** The Optimize phase occurs only once
- [ ] **D)** Operate is the final, disconnected phase

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Optimization is recurring because new cloud usage, changing workloads, and evolving requirements continually create new opportunities to improve value.
 
 
</details>

### 30. Which two statements correctly describe optimization in FinOps?

- [ ] **A)** Focuses on business value, not just cost reduction
- [ ] **B)** Recurs when cloud usage changes
- [ ] **C)** Aims only at lower cost
- [ ] **D)** Is owned by a central FinOps team

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> FinOps optimization balances value and cost, and it is continuous. It is not limited to cost cutting or to a centralized team.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Blue%20Prism/SS&C%20|%20Blue%20Prism®%20Chorus%20Foundation%20Certification" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Chorus Foundation</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Chorus Orchestration and Case Management](#chorus-orchestration-and-case-management) (9 questions)
- [Chorus Overview and Architecture](#chorus-overview-and-architecture) (6 questions)
- [Deployment and Maintenance](#deployment-and-maintenance) (4 questions)
- [Monitoring, Reporting, and Analytics](#monitoring-reporting-and-analytics) (6 questions)
- [User Interface and Interaction Management](#user-interface-and-interaction-management) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:34.998Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Chorus Orchestration and Case Management | 9 |
| Chorus Overview and Architecture | 6 |
| Deployment and Maintenance | 4 |
| Monitoring, Reporting, and Analytics | 6 |
| User Interface and Interaction Management | 5 |

---

### **Chorus Orchestration and Case Management**

### 1. What is the primary purpose of a case type in Blue Prism Chorus?

- [ ] **A)** To execute automated processes without human intervention.
- [ ] **B)** To define the structure, lifecycle, and behavior of a unit of work.
- [ ] **C)** To store user credentials and manage system access.
- [ ] **D)** To manage system logs and audit trails.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A case type acts as a blueprint for managing a business process from initiation to resolution, including stages, data fields, and SLA rules.
 
 
</details>

### 2. Which of the following statements about work queues are correct? (Select two.)

- [ ] **A)** A work queue can contain cases from multiple case types.
- [ ] **B)** Work queues hold individual cases that are awaiting human or digital worker action.
- [ ] **C)** A single case type can have multiple work queues.
- [ ] **D)** Work queues are defined at the system level and shared across all case types.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Work queues are per case type and act as containers for cases at specific stages. A case type can have several queues, but a queue belongs to exactly one case type.
 
 
</details>

### 3. Based on the decision table shown, what is the outcome for a case with Age=25 and Country='US'?

```text
Condition: Age > 18 | Condition: Country = 'US' | Outcome: Route to Stage A
Condition: Age <= 18 | Condition: Country = 'US' | Outcome: Route to Stage B
Condition: * | Condition: * | Outcome: Route to Stage C
```

- [ ] **A)** Route to Stage A
- [ ] **B)** Route to Stage B
- [ ] **C)** Route to Stage C
- [ ] **D)** No matching rule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The first row (Age > 18 and Country = 'US') matches, so the outcome is 'Route to Stage A'. The table uses first-hit policy.
 
 
</details>

### 4. In the context of case lifecycle, what is the purpose of an escalation rule?

- [ ] **A)** To automatically complete pending tasks.
- [ ] **B)** To reassign or notify when a stage exceeds its SLA threshold.
- [ ] **C)** To delete stalled cases from the system.
- [ ] **D)** To change the case type of a running case.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Escalation rules respond to SLA breaches on manual or wait stages by notifying or reassigning to ensure timely action.
 
 
</details>

### 5. Which of the following actions can be configured in an exception stage? (Select two.)

- [ ] **A)** Log exception details to the audit trail.
- [ ] **B)** Send notification emails to designated recipients.
- [ ] **C)** Automatically escalate the case to a manager.
- [ ] **D)** Reassign the case to a different user.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Exception stages can log errors and send notifications, but escalation and reassignment are configured via escalation rules, not directly inside exception stages.
 
 
</details>

### 6. Based on the configuration snippet, which SLA setting uses calendar hours?

```text
Stage: Document Verification
SLA: 48 hours (Business Hours)
Escalation: Move to Priority Queue after 40 hours
Queue-Level SLA: 20 hours (Calendar Hours)
```

- [ ] **A)** Stage SLA (48 hours Business Hours)
- [ ] **B)** Queue-Level SLA (20 hours Calendar Hours)
- [ ] **C)** Both use calendar hours
- [ ] **D)** Neither uses calendar hours

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The queue-level SLA explicitly states 'Calendar Hours', meaning it counts real time, while the stage SLA uses business hours.
 
 
</details>

### 7. What is the default hit policy in a Chorus decision table?

- [ ] **A)** All hits
- [ ] **B)** Last hit
- [ ] **C)** First hit
- [ ] **D)** Random

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Chorus uses a first-hit policy, meaning the first row whose conditions are all satisfied determines the outcome.
 
 
</details>

### 8. Which of the following statements about case stages are true? (Select two.)

- [ ] **A)** Stages are optional in a case lifecycle.
- [ ] **B)** Each stage can have multiple work queues attached.
- [ ] **C)** A disabled stage throws an exception when encountered.
- [ ] **D)** Stages can have entry and exit conditions.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Stages can have multiple queues (e.g., urgent/standard) and can define conditions for transitions. Disabled stages are skipped, not errored.
 
 
</details>

### 9. If a case is in 'Document Check' and the reviewer rejects the documents, which transition sends the case back to 'New'?

```text
Stages: New -> Document Check -> Approved -> Completed
Allowed transitions:
  Document Check -> New (rework)
  Document Check -> Approved (standard)
```

- [ ] **A)** Document Check -> Approved
- [ ] **B)** Document Check -> New
- [ ] **C)** New -> Document Check
- [ ] **D)** No transition exists for rework

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The diagram shows 'Document Check -> New' as an allowed transition, enabling the case to return to the New stage for rework.
 
 
</details>


---

### **Chorus Overview and Architecture**

### 10. Which component of the Blue Prism Chorus platform provides a low-code environment for designing automation processes?

- [ ] **A)** Chorus Studio
- [ ] **B)** Chorus Interact
- [ ] **C)** Chorus Control Room
- [ ] **D)** Chorus Hub

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Chorus Studio is the low-code development environment for designing automation processes.
 
 
</details>

### 11. Which two of the following are responsibilities of the Chorus orchestrator?

- [ ] **A)** Managing human-in-the-loop interactions
- [ ] **B)** Dispatching work items to digital workers based on availability
- [ ] **C)** Designing process logic using low-code tools
- [ ] **D)** Handling retry and escalation policies for failed work items

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> The orchestrator dispatches work items and manages retries; human interactions are handled by Interact, and design is done in Studio.
 
 
</details>

### 12. Examine the JSON code block below. Which property indicates the status of a completed work item?

```json
{
  "work_item_id": "123",
  "status": "success",
  "output": {
    "data": "value"
  }
}
```

- [ ] **A)** work_item_id
- [ ] **B)** status
- [ ] **C)** output
- [ ] **D)** message

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 'status' property in the response message indicates the outcome of the work item execution.
 
 
</details>

### 13. Which Chorus component is used to store configuration data, process definitions, and execution logs?

- [ ] **A)** Chorus Database
- [ ] **B)** Chorus Hub
- [ ] **C)** Chorus Control Room
- [ ] **D)** Chorus Interact

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Chorus Database (Microsoft SQL Server) stores all persistent data including process definitions, logs, and configurations.
 
 
</details>

### 14. Which two statements correctly describe the difference between Chorus and Blue Prism's core RPA capabilities?

- [ ] **A)** Core RPA executes processes; Chorus orchestrates them.
- [ ] **B)** Chorus can design process logic; core RPA cannot.
- [ ] **C)** Chorus provides human-in-the-loop capabilities out of the box.
- [ ] **D)** Core RPA includes executive dashboards; Chorus does not.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Chorus orchestrates and adds human-in-the-loop; core RPA executes. Chorus does not design logic and core RPA lacks dashboards.
 
 
</details>

### 15. Refer to the code block which shows a configuration snippet for a queue. What type of queue is being defined?

```yaml
queue:
  name: loan-processing-queue
  type: work queue
  routing_key: worker.assignments
  durable: true
```

- [ ] **A)** Request queue
- [ ] **B)** Work queue
- [ ] **C)** Response queue
- [ ] **D)** Dead letter queue

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The configuration defines a work queue that workers consume from, as indicated by the 'routing_key' pointing to worker assignments.
 
 
</details>


---

### **Deployment and Maintenance**

### 16. What must be completed before importing a solution into a target Chorus environment?

- [ ] **A)** Restart all schedules
- [ ] **B)** Perform a full database backup
- [ ] **C)** Delete the existing solution version
- [ ] **D)** Reduce environment security settings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A full backup ensures the ability to rollback if the import fails or causes issues.
 
 
</details>

### 17. Which statements about release packages in Chorus are correct? (Select two)

- [ ] **A)** They are only used for production deployments
- [ ] **B)** They can be full or delta releases
- [ ] **C)** They become immutable once marked as Released
- [ ] **D)** They are stored exclusively in the Blue Prism database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Release packages can be full or delta, and once Released they become read-only for audit purposes.
 
 
</details>

### 18. What is the purpose of the following PowerShell command?

```powershell
Remove-Item -Path C:\ProgramData\Chorus\Logs\*.log -LastWriteTime -gt (Get-Date).AddDays(-30)
```

- [ ] **A)** Deletes all log files older than 30 days
- [ ] **B)** Moves log files to a backup directory
- [ ] **C)** Compresses log files older than 30 days
- [ ] **D)** Lists log files older than 30 days

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command removes Chorus log files with a last write time older than 30 days.
 
 
</details>

### 19. What is the recommended first step when troubleshooting a Chorus user login failure?

- [ ] **A)** Restart the Chorus Windows service
- [ ] **B)** Clear the browser cache and cookies
- [ ] **C)** Check the database connection string
- [ ] **D)** Reinstall the Chorus application

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A corrupt authentication cookie often causes login failures; clearing the cache is the fastest test.
 
 
</details>


---

### **Monitoring, Reporting, and Analytics**

### 20. Which Chorus dashboard category is specifically designed to show resource utilization and error rates?

- [ ] **A)** Process Performance
- [ ] **B)** Resource Performance
- [ ] **C)** Queue Performance
- [ ] **D)** System Health

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Resource Performance dashboard focuses on utilization and error rates per resource (bot). Process Performance deals with process-level success rates and duration. Queue Performance concerns backlog and SLA. System Health covers server load and licensing.
 
 
</details>

### 21. Which two metrics are essential for measuring SLA compliance in operational reports? (Choose two.)

- [ ] **A)** Average Resolution Time
- [ ] **B)** Cases Resolved per Hour
- [ ] **C)** Percentage of cases completed within target time
- [ ] **D)** Queue Depth

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> SLA compliance is measured by comparing actual cycle times (average resolution time) against targets and by the percentage of cases that meet the SLA. Cases per hour is throughput, not SLA. Queue depth is a queue health metric, not directly SLA.
 
 
</details>

### 22. Examine the following alert rule configuration. What type of alert is being defined?

```json
{
  "condition": "pendingItems > 100",
  "evaluation": "threshold",
  "frequency": "every 5 minutes",
  "channel": "email"
}
```

- [ ] **A)** Static threshold alert
- [ ] **B)** Event-driven notification
- [ ] **C)** Custom event alert
- [ ] **D)** System alert

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The rule uses a fixed threshold ('pendingItems > 100') and evaluates periodically (every 5 minutes). This matches the definition of a static threshold alert. Event-driven notifications fire immediately when an event occurs, not on a timer.
 
 
</details>

### 23. What is the primary purpose of analyzing worker utilization metrics in Chorus?

- [ ] **A)** To measure the number of tasks completed per worker
- [ ] **B)** To optimize resource cost and availability
- [ ] **C)** To calculate the backlog of work queues
- [ ] **D)** To identify individual worker errors

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Worker utilization metrics are designed to optimize resource cost and availability. Throughput and error rates are separate measures. Queue backlog belongs to queue health analysis.
 
 
</details>

### 24. Which two features are critical for compliance-driven logging according to the document? (Choose two.)

- [ ] **A)** Tamper-evident logs
- [ ] **B)** Real-time dashboard integration
- [ ] **C)** Role-based access to logs
- [ ] **D)** Automatic process optimization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Compliance logging requires tamper-evidence (integrity) and role-based access (least privilege). Real-time dashboards are for monitoring, not compliance storage. Automatic optimization is unrelated.
 
 
</details>

### 25. Examine the following panel configuration extracted from a Chorus dashboard. Which dashboard category is this panel most likely from?

```json
{
  "panelTitle": "Process Success",
  "metric": "successRate",
  "groupBy": "processName",
  "aggregation": "avg"
}
```

- [ ] **A)** Process Performance
- [ ] **B)** Resource Performance
- [ ] **C)** Queue Performance
- [ ] **D)** System Health

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The panel groups by process name and shows average success rate. This aligns with the Process Performance dashboard, which focuses on per-process KPIs like success rate and duration.
 
 
</details>


---

### **User Interface and Interaction Management**

### 26. What is the primary purpose of the Chorus Portal compared to the Blue Prism Interactive Client?

- [ ] **A)** Provide a technical development environment for process automation
- [ ] **B)** Offer a role-specific, non-technical view for business stakeholders to monitor and manage digital workers
- [ ] **C)** Serve as the runtime environment for attended automation
- [ ] **D)** Manage Blue Prism database schemas

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Chorus Portal is designed for business stakeholders with a non-technical interface, whereas the Interactive Client targets technical developers and attended automation users.
 
 
</details>

### 27. Which of the following statements about Chorus portal roles are correct?

- [ ] **A)** The Administrator role has full control of portal configuration.
- [ ] **B)** The Manager role can create workspaces and approve exceptions.
- [ ] **C)** The Operator role can modify process definitions.
- [ ] **D)** The Viewer role has read-only access to all objects.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Administrator has full control; Manager can manage workspaces and approvals; Operator cannot modify processes; Viewer is read-only.
 
 
</details>

### 28. Consider the following queue assignment configuration. Which user will receive the next task?

```json
{
  "assignmentType": "RoundRobin",
  "users": [
    {"id": "user1", "capacity": 5, "currentTasks": 5},
    {"id": "user2", "capacity": 5, "currentTasks": 3},
    {"id": "user3", "capacity": 5, "currentTasks": 4}
  ]
}
```

- [ ] **A)** user1
- [ ] **B)** user2
- [ ] **C)** user3
- [ ] **D)** None, the task remains unassigned

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> user1 is at capacity (5/5), user2 has 3 tasks, user3 has 4. Round robin will skip user1 and assign to user2.
 
 
</details>

### 29. Which stage should be used when the automation requires a simple yes/no decision from a human operator?

- [ ] **A)** Interact Stage
- [ ] **B)** Query Stage
- [ ] **C)** Decision Stage
- [ ] **D)** Wait Stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Query Stage returns a single value (e.g., Yes/No), while Interact is for multi-field forms.
 
 
</details>

### 30. Which of the following are true about Chorus Portal dashboard configuration?

- [ ] **A)** Dashboards are shared by default with all users.
- [ ] **B)** Administrators can assign dashboards to specific security roles.
- [ ] **C)** Widgets can be resized and positioned on a grid layout.
- [ ] **D)** Only custom widgets require coding; built-in widgets are no-code.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C, D**
 
> 💡  **Explanation** 
> 
> Dashboards must be published to be shared; admins assign roles; widgets are resizable; built-in widgets need no coding.
 
 
</details>

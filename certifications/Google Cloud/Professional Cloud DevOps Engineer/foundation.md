<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Google%20Cloud/Professional%20Cloud%20DevOps%20Engineer.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Professional Cloud DevOps Engineer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Applying Site Reliability Engineering Practices](#applying-site-reliability-engineering-practices) (5 questions)
- [Bootstrapping and Maintaining a Google Cloud Organization](#bootstrapping-and-maintaining-a-google-cloud-organization) (6 questions)
- [Building and Implementing CI/CD Pipelines](#building-and-implementing-ci-cd-pipelines) (7 questions)
- [Implementing Observability Practices and Troubleshooting](#implementing-observability-practices-and-troubleshooting) (8 questions)
- [Optimizing Performance and Cost](#optimizing-performance-and-cost) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:52:12.540Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Applying Site Reliability Engineering Practices | 5 |
| Bootstrapping and Maintaining a Google Cloud Organization | 6 |
| Building and Implementing CI/CD Pipelines | 7 |
| Implementing Observability Practices and Troubleshooting | 8 |
| Optimizing Performance and Cost | 4 |

---

### **Applying Site Reliability Engineering Practices**

### 1. In the context of Site Reliability Engineering at Google, which statement correctly describes the primary goal of the discipline?

- [ ] **A)** Automate every operational task
- [ ] **B)** Maximize feature velocity without limits
- [ ] **C)** Eliminate all software failures
- [ ] **D)** Balance reliability and feature velocity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> SRE exists to balance the risk of unreliable systems with the need for fast feature development.
 
 
</details>

### 2. Which two measurement types are used together in Site Reliability Engineering to define a service's reliability target?

- [ ] **A)** Service Level Indicator
- [ ] **B)** Service Level Objective
- [ ] **C)** Service Level Agreement
- [ ] **D)** Total Cost of Ownership

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SLIs measure service behavior, and SLOs specify target values for those indicators; SLAs are external contracts.
 
 
</details>

### 3. Based on the SLO configuration shown above, what reliability percentage is defined as the target for the service?

```yaml
apiVersion: monitoring.googleapis.com/v1
kind: Slo
metadata:
  name: payments-service-slo
spec:
  service: payments-service
  goal: 0.99

```

- [ ] **A)** 90 percent
- [ ] **B)** 99 percent
- [ ] **C)** 99.9 percent
- [ ] **D)** 99.99 percent

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The goal value 0.99 expressed as a percentage is 99 percent.
 
 
</details>

### 4. In Site Reliability Engineering, what is the term for the acceptable amount of failure a service can experience?

- [ ] **A)** Error budget
- [ ] **B)** Latency target
- [ ] **C)** Rollback window
- [ ] **D)** Capacity buffer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The error budget is the acceptable amount of failure a service can experience while still meeting its SLO.
 
 
</details>

### 5. Within Site Reliability Engineering, which two characteristics are commonly used to identify toil in operational work?

- [ ] **A)** Manual repetitive tasks with no enduring value
- [ ] **B)** Work that provides no lasting improvement
- [ ] **C)** One-time strategic automation projects
- [ ] **D)** Creative development of new product features

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Toil is manual, repetitive work with no long-term benefit; strategic projects and product development are not toil.
 
 
</details>


---

### **Bootstrapping and Maintaining a Google Cloud Organization**

### 6. What is the highest-level node in the Google Cloud resource hierarchy?

- [ ] **A)** Organization node
- [ ] **B)** Folder
- [ ] **C)** Project
- [ ] **D)** Billing account

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The organization node is the root of the Google Cloud resource hierarchy. It enables centralized administration, IAM policy assignment, and organization policy enforcement across all folders and projects.
 
 
</details>

### 7. Select all items that are part of the Google Cloud resource hierarchy.

- [ ] **A)** Organization node
- [ ] **B)** Folder
- [ ] **C)** Project
- [ ] **D)** Billing account

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The Google Cloud resource hierarchy consists of the organization node, folders, and projects. Billing accounts are important resources but are not part of the resource hierarchy.
 
 
</details>

### 8. A cloud engineer executes the command shown below during initial organization bootstrap. What action does it perform?

```bash
gcloud organizations add-iam-policy-binding 123456789012 --member="user:admin@example.com" --role="roles/organizationAdmin"
```

- [ ] **A)** Grants the Organization Administrator role at the organization level
- [ ] **B)** Grants Project Owner on a project
- [ ] **C)** Creates a new service account key
- [ ] **D)** Assigns the Billing Administrator role at the organization level

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses gcloud organizations add-iam-policy-binding to assign the roles/organizationAdmin role to a user at the organization level.
 
 
</details>

### 9. Which IAM role should be assigned to a user who is responsible for managing the financial aspects of all Google Cloud accounts?

- [ ] **A)** Billing Account Administrator
- [ ] **B)** Project Owner
- [ ] **C)** Organization Administrator
- [ ] **D)** Service Account Admin

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Billing Account Administrator role, roles/billing.admin, allows a user to manage billing accounts, payment methods, and related financial settings.
 
 
</details>

### 10. A consultant is starting to bootstrap a new Google Cloud organization. Which two initial steps should be performed?

- [ ] **A)** Create a Cloud Identity account and verify the domain
- [ ] **B)** Create the organization node associated with the Cloud Identity domain
- [ ] **C)** Create a project for every department
- [ ] **D)** Apply a uniform organization policy to all resources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Bootstrapping starts with a Cloud Identity account and then creates the organization node. Projects and policies can be created later, but the Cloud Identity domain and organization node are foundational.
 
 
</details>

### 11. The following command is used in a bootstrap process. Which resource does it create?

```bash
gcloud resource-manager folders create --display-name="Production" --organization=123456789012
```

- [ ] **A)** A folder named Production under the organization
- [ ] **B)** A project named Production inside the organization
- [ ] **C)** An organization policy called Production
- [ ] **D)** A billing account for Production

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command gcloud resource-manager folders create creates a folder with the display name Production under the specified organization node.
 
 
</details>


---

### **Building and Implementing CI/CD Pipelines**

### 12. In Google Cloud, which fully managed service is designed for building, testing, and deploying artifacts in a CI/CD pipeline?

- [ ] **A)** Cloud Build
- [ ] **B)** Cloud Run
- [ ] **C)** Cloud Deploy
- [ ] **D)** Artifact Registry

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Build is Google Cloud's fully managed CI/CD service. Cloud Run is a compute platform, Cloud Deploy orchestrates delivery, and Artifact Registry stores artifacts.
 
 
</details>

### 13. Which of the following are considered core stages in a CI/CD pipeline? Select all that apply.

- [ ] **A)** Executing unit tests
- [ ] **B)** Compiling source code
- [ ] **C)** Deploying to an environment
- [ ] **D)** Opening a support ticket

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A CI/CD pipeline includes source checkout, build or compile, test, and deploy. Opening a support ticket is not a pipeline stage.
 
 
</details>

### 14. In the Cloud Build config snippet, what does the 'name' field in a build step define?

```yaml
steps:
- name: 'gcr.io/cloud-builders/docker'
  args: ['build', '-t', 'gcr.io/$PROJECT_ID/my-image', '.']
```

- [ ] **A)** The container image used to execute the step
- [ ] **B)** The name of the build result
- [ ] **C)** The Google Cloud project ID
- [ ] **D)** The file path to the Dockerfile

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In Cloud Build, each step uses a container image specified in the 'name' field to run the defined arguments and commands.
 
 
</details>

### 15. Which Google Cloud service is a fully managed artifact registry for storing container images and software packages?

- [ ] **A)** Artifact Registry
- [ ] **B)** Cloud Functions
- [ ] **C)** Cloud Source Repositories
- [ ] **D)** Cloud Run

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Artifact Registry stores Docker images, Maven packages, and other artifacts. Cloud Source Repositories hosts git repositories, and Cloud Functions is a compute service.
 
 
</details>

### 16. Which of the following can be used to trigger a Cloud Build? Select all that apply.

- [ ] **A)** A push to a Cloud Source Repository
- [ ] **B)** A Pub/Sub message
- [ ] **C)** Submitting a build with the gcloud command
- [ ] **D)** Creating a Compute Engine VM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Cloud Build supports triggers from repository events, Pub/Sub messages, manual gcloud builds, and webhooks. Creating a Compute Engine VM does not trigger a build.
 
 
</details>

### 17. When the following Cloud Build step runs, what output is written to the build log?

```yaml
steps:
- name: 'ubuntu'
  args: ['echo', 'Hello, Cloud Build']
```

- [ ] **A)** Hello, Cloud Build
- [ ] **B)** ubuntu
- [ ] **C)** echo
- [ ] **D)** Build success

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The step runs the 'ubuntu' image with arguments 'echo' and 'Hello, Cloud Build', so the log displays the text 'Hello, Cloud Build'.
 
 
</details>

### 18. Which IAM role is required to submit builds in Cloud Build?

- [ ] **A)** roles/cloudbuild.builds.editor
- [ ] **B)** roles/storage.objectViewer
- [ ] **C)** roles/cloudfunctions.developer
- [ ] **D)** roles/iam.serviceAccountAdmin

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Build uses IAM roles to control permissions. The roles/cloudbuild.builds.editor role grants permission to create and run builds.
 
 
</details>


---

### **Implementing Observability Practices and Troubleshooting**

### 19. Which Google Cloud service provides dashboards, alerting, and monitoring for applications and infrastructure?

- [ ] **A)** Centralized metrics, dashboards, and alerting
- [ ] **B)** Long-term storage and querying of logs
- [ ] **C)** Profiling application code and memory use
- [ ] **D)** Tracing requests across distributed services

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Monitoring collects metrics, builds dashboards, and sends alerts; Cloud Logging handles logs, Cloud Profiler profiles resources, and Cloud Trace measures request latency.
 
 
</details>

### 20. Which services are included in the Google Cloud operations suite?

- [ ] **A)** Cloud Monitoring
- [ ] **B)** Cloud Logging
- [ ] **C)** Cloud Trace
- [ ] **D)** Cloud Composer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Cloud Monitoring, Cloud Logging, and Cloud Trace are core operations suite components. Cloud Composer orchestrates workflows and is not an observability service.
 
 
</details>

### 21. Look at the Cloud Logging filter in the code block. What log entries does it select?

```text
severity>=ERROR AND resource.type="k8s_container" AND resource.labels.namespace_name="payments"
```

- [ ] **A)** Payments namespace logs with severity ERROR or higher
- [ ] **B)** Error logs from all Kubernetes namespaces
- [ ] **C)** All logs from the payments cluster
- [ ] **D)** Info and ERROR logs in the payments namespace

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The filter requires a k8s container in the payments namespace and severity greater than or equal to ERROR, so only matching errors or worse entries are selected.
 
 
</details>

### 22. What does Cloud Trace primarily analyze for a request?

- [ ] **A)** Latency across the request call path and its spans
- [ ] **B)** Number of log entries generated per service
- [ ] **C)** Disk usage of each application instance
- [ ] **D)** HTTP status codes returned by load balancers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Trace samples requests and records latency for the full path and individual spans, helping locate performance bottlenecks.
 
 
</details>

### 23. Which practices are recommended when designing Cloud Monitoring alert policies?

- [ ] **A)** Alert on user-visible symptoms rather than every internal fluctuation.
- [ ] **B)** Use SLO burn-rate alerts to detect imminent reliability issues.
- [ ] **C)** Page engineers for every warning-level condition.
- [ ] **D)** Route all alerts through a single communication channel.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Good alerting focuses on symptoms and SLO burn rates. Paging on every warning creates alert fatigue, and a single channel is fragile.
 
 
</details>

### 24. A log-based counter metric is created with the filter in the code block. What events will it count?

```text
resource.type="global"
severity>=ERROR
```

- [ ] **A)** Global log entries with severity ERROR or higher
- [ ] **B)** Only log entries that contain an error message
- [ ] **C)** All log entries from every resource type
- [ ] **D)** Global logs with WARNING severity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The filter selects global log entries with severity ERROR or above, so the counter metric increments only for those matching entries.
 
 
</details>

### 25. What is an uptime check in Google Cloud Monitoring?

- [ ] **A)** A synthetic request that verifies availability and response
- [ ] **B)** A policy that auto-scales managed instance groups
- [ ] **C)** A method for storing monitoring time series data
- [ ] **D)** A log sink that exports health data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Uptime checks send synthetic requests to a public endpoint and verify that it is reachable and responding, supporting availability monitoring.
 
 
</details>

### 26. Which capabilities are provided by Cloud Logging?

- [ ] **A)** Ingest logs from applications and Google Cloud services
- [ ] **B)** Query logs with Logs Explorer
- [ ] **C)** Export logs to Cloud Storage
- [ ] **D)** Restart unhealthy virtual machines

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Cloud Logging ingests, stores, queries, and exports logs. It does not execute recovery actions on resources.
 
 
</details>


---

### **Optimizing Performance and Cost**

### 27. In the context of Google Cloud cost management, what is the primary purpose of setting a Cloud Billing budget?

- [ ] **A)** Get alerts before spending exceeds the budget
- [ ] **B)** Automatically scale down compute resources
- [ ] **C)** Create a new billing account
- [ ] **D)** Apply committed use discounts to invoices

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Cloud Billing budget tracks actual and forecast costs. Alerts help DevOps teams keep spending aligned with expected operating costs.
 
 
</details>

### 28. As a DevOps engineer, which two practices are most effective for reducing compute costs in Google Cloud workloads?

- [ ] **A)** Right-size machine types to fit application demand
- [ ] **B)** Use preemptible VMs for fault-tolerant batch jobs
- [ ] **C)** Keep all VMs running constantly
- [ ] **D)** Always choose the largest machine type available

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Right-sizing matches capacity to actual utilization, and preemptible VMs cut costs for interruptible batch work. Keeping all VMs running constantly increases idle cost.
 
 
</details>

### 29. A DevOps Engineer runs the command shown in the code block. What outcome should they expect?

```bash
gcloud billing budgets create --billing-account=012345-6789AB-CDEF01 --display-name=Monthly-budget --budget-amount=500 --threshold-rule=percent=0.5 --threshold-rule=percent=0.9
```

- [ ] **A)** Sets $500 budget with 50% and 90% alerts
- [ ] **B)** Enables automatic shutdown after $500 are spent
- [ ] **C)** Creates two separate budgets for 50% and 90%
- [ ] **D)** Renames the billing account to Monthly-budget

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> gcloud billing budgets create defines a budget amount and threshold rules. Alerts are sent when forecast or actual spend reaches 50% and 90%.
 
 
</details>

### 30. In Google Cloud, what does a Committed Use Discount provide to customers who commit to steady baseline usage for one or three years?

- [ ] **A)** Discounted price for committed resource use
- [ ] **B)** Monthly credits for early payments
- [ ] **C)** Automatically converts all VMs to spot VMs
- [ ] **D)** Applies only to Cloud Storage transfer operations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Committed Use Discounts offer lower prices when you commit to a minimum level of vCPU, memory, or GPU in return for predictable savings.
 
 
</details>

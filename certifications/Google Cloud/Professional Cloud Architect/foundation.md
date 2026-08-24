<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Google%20Cloud/Professional%20Cloud%20Architect%20Certification" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Professional Cloud Architect</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Analyzing and optimizing technical and business processes](#analyzing-and-optimizing-technical-and-business-processes) (5 questions)
- [Designing and planning a cloud solution architecture](#designing-and-planning-a-cloud-solution-architecture) (7 questions)
- [Designing for security and compliance](#designing-for-security-and-compliance) (5 questions)
- [Ensuring solution and operations reliability](#ensuring-solution-and-operations-reliability) (4 questions)
- [Managing and provisioning cloud solution infrastructure](#managing-and-provisioning-cloud-solution-infrastructure) (5 questions)
- [Managing implementation](#managing-implementation) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:52:05.478Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Analyzing and optimizing technical and business processes | 5 |
| Designing and planning a cloud solution architecture | 7 |
| Designing for security and compliance | 5 |
| Ensuring solution and operations reliability | 4 |
| Managing and provisioning cloud solution infrastructure | 5 |
| Managing implementation | 4 |

---

### **Analyzing and optimizing technical and business processes**

### 1. What is the primary purpose of analyzing technical processes when designing an enterprise cloud architecture?

- [ ] **A)** Identifying optimization opportunities
- [ ] **B)** Increasing infrastructure costs
- [ ] **C)** Reducing system redundancy
- [ ] **D)** Eliminating all documentation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Analyzing technical processes helps identify inefficiencies and optimization opportunities, enabling better cost, performance, and reliability outcomes.
 
 
</details>

### 2. Which activities are part of optimizing business processes on Google Cloud? Select all that apply.

- [ ] **A)** Automating manual workflows
- [ ] **B)** Right-sizing cloud resources
- [ ] **C)** Increasing manual approvals
- [ ] **D)** Ignoring customer metrics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Automating workflows and right-sizing resources improve efficiency and reduce waste, while manual approvals and ignoring metrics hinder optimization.
 
 
</details>

### 3. Given the following command, what does it help you analyze during resource optimization in Google Cloud?

```bash
gcloud compute instances list --filter="status=RUNNING" --format="table(name,zone,status)"
```

- [ ] **A)** Discover running instances for potential right-sizing
- [ ] **B)** Review IAM policy bindings
- [ ] **C)** Create new virtual machines
- [ ] **D)** Monitor network firewall rules

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command lists running compute instances, supporting analysis of resource usage and opportunities for right-sizing or cleanup.
 
 
</details>

### 4. Which Google Cloud service provides recommendations for reducing cost and improving performance of cloud resources?

- [ ] **A)** Recommender
- [ ] **B)** Cloud Scheduler
- [ ] **C)** Cloud Debugger
- [ ] **D)** Cloud Armor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Recommender analyzes usage patterns and provides actionable recommendations to optimize cost, performance, and reliability in Google Cloud.
 
 
</details>

### 5. Which key metrics should be monitored when optimizing a technical process in Google Cloud? Select all that apply.

- [ ] **A)** CPU utilization
- [ ] **B)** Memory usage
- [ ] **C)** Network latency
- [ ] **D)** Git star count

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> CPU, memory, and network latency directly affect process performance, while unrelated repository metrics do not support optimization decisions.
 
 
</details>


---

### **Designing and planning a cloud solution architecture**

### 6. In Google Cloud, what is the scope of a Virtual Private Cloud (VPC) network?

- [ ] **A)** Global
- [ ] **B)** Regional
- [ ] **C)** Zonal
- [ ] **D)** Multi-regional but limited to one continent

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A VPC network is a global resource that spans all regions. Its subnets, firewall rules, and routes can be used across the Google Cloud global network.
 
 
</details>

### 7. Which two statements are true about managed instance groups (MIGs) in Google Cloud?

- [ ] **A)** MIGs can automatically heal unhealthy instances.
- [ ] **B)** MIGs provide autoscaling based on load metrics.
- [ ] **C)** MIGs can only contain instances in different projects.
- [ ] **D)** MIGs require manual replacement of failed instances.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Managed instance groups support autoscaling and automatic healing so failed instances are recreated without manual intervention. Group instances are normally in the same project.
 
 
</details>

### 8. Review the provided Terraform code block and identify the Google Cloud resource being created.

```hcl
resource "google_storage_bucket" "archive" {
  name          = "my-archive-bucket"
  location      = "US"
  force_destroy = true
}

```

- [ ] **A)** Cloud Storage bucket
- [ ] **B)** Compute Engine instance
- [ ] **C)** Kubernetes cluster
- [ ] **D)** Cloud SQL instance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Terraform block declares resource \"google_storage_bucket\", so it creates a Cloud Storage bucket.
 
 
</details>

### 9. Which Google Cloud service enables declarative provisioning of infrastructure through YAML and Python templates?

- [ ] **A)** Cloud Deployment Manager
- [ ] **B)** Cloud Functions
- [ ] **C)** Cloud Run
- [ ] **D)** App Engine

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Deployment Manager is Google Cloud's infrastructure deployment tool, using YAML, Python, or Jinja2 templates.
 
 
</details>

### 10. Which two factors should have the greatest influence on region selection for a highly available Google Cloud architecture?

- [ ] **A)** Deploying across multiple zones or regions to avoid correlated failure.
- [ ] **B)** Using regions that meet data residency or compliance requirements.
- [ ] **C)** Choosing the cheapest region without considering latency or resilience.
- [ ] **D)** Placing all resources in one zone to reduce complexity.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A highly available regional plan should minimize correlated failure and honor data residency or compliance constraints. A single zone increases risk.
 
 
</details>

### 11. In the provided Kubernetes manifest, which type of workload resource is declared?

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: web-server
spec:
  replicas: 3
  selector:
    matchLabels:
      app: web
  template:
    metadata:
      labels:
        app: web
    spec:
      containers:
      - name: nginx
        image: nginx:latest

```

- [ ] **A)** Deployment
- [ ] **B)** Service
- [ ] **C)** ConfigMap
- [ ] **D)** Namespace

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The manifest has apiVersion apps/v1 and kind Deployment, so it defines a Deployment managing a set of replicated Pods.
 
 
</details>

### 12. Which statement best describes global external HTTPS load balancing in Google Cloud?

- [ ] **A)** It uses a single anycast IPv4 or IPv6 address to distribute traffic globally.
- [ ] **B)** It is limited to a single region and zone.
- [ ] **C)** It requires one load balancer per backend service.
- [ ] **D)** It can only balance traffic between Cloud Run services.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Global external HTTP(S) load balancing uses a single global anycast IP address and forwards traffic to the nearest available backend across regions.
 
 
</details>


---

### **Designing for security and compliance**

### 13. Which Google Cloud service is used to define and enforce fine-grained access control on resources?

- [ ] **A)** Cloud Identity and Access Management (Cloud IAM)
- [ ] **B)** Cloud Audit Logs
- [ ] **C)** Cloud Key Management Service (Cloud KMS)
- [ ] **D)** Virtual Private Cloud (VPC) Service Controls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud IAM authorizes who can act on specific Google Cloud resources. It defines members, roles, and policies to enforce access control.
 
 
</details>

### 14. Which items are core components of an IAM policy? (Select all that apply.)

- [ ] **A)** Members
- [ ] **B)** Roles
- [ ] **C)** IAM bindings
- [ ] **D)** Billing accounts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> An IAM policy is composed of bindings that attach one or more members to a role. Billing accounts are not part of the IAM policy structure.
 
 
</details>

### 15. Refer to the IAM policy in the code block. Which role is granted to sara@example.com?

```json
{
  "bindings": [
    {
      "role": "roles/storage.objectViewer",
      "members": ["user:sara@example.com"]
    }
  ]
}
```

- [ ] **A)** roles/storage.objectViewer
- [ ] **B)** roles/storage.objectAdmin
- [ ] **C)** roles/iam.serviceAccountUser
- [ ] **D)** roles/viewer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The IAM policy binds user:sara@example.com to roles/storage.objectViewer, granting read-only access to Cloud Storage objects.
 
 
</details>

### 16. Which Google Cloud service records user activity such as resource changes, access attempts, and administrative actions?

- [ ] **A)** Cloud Audit Logs
- [ ] **B)** Cloud Monitoring
- [ ] **C)** Cloud Profiler
- [ ] **D)** Cloud Trace

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Audit Logs record administrative activity, data access, and system events to help answer who did what, where, and when.
 
 
</details>

### 17. Which of the following are valid types of Cloud Audit Logs? (Select all that apply.)

- [ ] **A)** Admin Activity
- [ ] **B)** Data Access
- [ ] **C)** System Event
- [ ] **D)** Access Transparency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Cloud Audit Logs categories include Admin Activity, Data Access, System Event, and Policy Denied. Access Transparency is a separate feature that logs actions taken by Google staff.
 
 
</details>


---

### **Ensuring solution and operations reliability**

### 18. Which Google Cloud service is used to visualize performance metrics and set up custom monitoring dashboards?

- [ ] **A)** Cloud Monitoring
- [ ] **B)** Cloud Logging
- [ ] **C)** Cloud Trace
- [ ] **D)** Cloud Profiler

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Monitoring is the Google Cloud service for metrics, uptime checks, and dashboards; Cloud Logging stores logs, Cloud Trace analyzes latency, and Cloud Profiler analyzes performance.
 
 
</details>

### 19. Which three services are part of Google Cloud's operations suite commonly used for application reliability?

- [ ] **A)** Cloud Monitoring
- [ ] **B)** Cloud Logging
- [ ] **C)** Cloud Trace
- [ ] **D)** Cloud Storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Cloud Monitoring, Cloud Logging, and Cloud Trace are central Google Cloud operations tools. Cloud Storage is object storage, not an observability service.
 
 
</details>

### 20. Review the gcloud command in the code block. What is the primary purpose of this command?

```bash
gcloud logging read 'resource.type=gce_instance AND severity>=ERROR' --limit=10
```

- [ ] **A)** It reads recent ERROR or higher severity log entries from Compute Engine instances.
- [ ] **B)** It creates a Cloud Logging sink for Compute Engine ERROR logs.
- [ ] **C)** It creates an alerting policy for all Compute Engine ERROR logs.
- [ ] **D)** It deletes log entries with severity ERROR from Compute Engine instances.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses gcloud logging read to retrieve log entries filtered by resource type and minimum severity.
 
 
</details>

### 21. What is a service level objective (SLO) in the context of cloud service reliability?

- [ ] **A)** A target value or range of values for a service level indicator
- [ ] **B)** A legal agreement that specifies penalties for downtime
- [ ] **C)** A log-based metric that counts all user requests
- [ ] **D)** A postmortem document used after a production incident

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An SLO is the target level for an SLI, for example 99.9% availability. It is not a legal contract, log metric, or postmortem.
 
 
</details>


---

### **Managing and provisioning cloud solution infrastructure**

### 22. What is the primary role of a Virtual Private Cloud (VPC) in Google Cloud?

- [ ] **A)** It provides isolated networking resources
- [ ] **B)** It stores unstructured object data
- [ ] **C)** It executes code in response to events
- [ ] **D)** It manages user identities and access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A VPC provides isolated networking resources, such as subnets, routes, and firewalls, for Google Cloud resources.
 
 
</details>

### 23. Which of the following are Google Cloud compute services?

- [ ] **A)** Cloud Storage
- [ ] **B)** Compute Engine
- [ ] **C)** Cloud Run
- [ ] **D)** Cloud SQL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Compute Engine and Cloud Run are compute services. Cloud Storage is object storage and Cloud SQL is a managed database service.
 
 
</details>

### 24. What resource is declared in the provided Terraform configuration?

```terraform
resource "google_compute_network" "vpc" {
  name                    = "example-vpc"
  auto_create_subnetworks = false
}

```

- [ ] **A)** A VPC network
- [ ] **B)** A firewall rule
- [ ] **C)** A Cloud Router
- [ ] **D)** A subnetwork

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The configuration uses google_compute_network, which declares a VPC network resource with automatic subnetwork creation disabled. This means subnets must be created separately.
 
 
</details>

### 25. What is a service account used for in Google Cloud?

- [ ] **A)** To provide a secure identity for applications and services
- [ ] **B)** To store secrets and encryption keys
- [ ] **C)** To create and manage virtual machines
- [ ] **D)** To assign static IP addresses to resources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A service account provides an identity that applications and services use to authenticate and access Google Cloud resources.
 
 
</details>

### 26. Which of the following can be used to manage Google Cloud infrastructure as code?

- [ ] **A)** Cloud Deployment Manager
- [ ] **B)** Terraform
- [ ] **C)** Cloud Console
- [ ] **D)** Cloud Shell

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Cloud Deployment Manager and Terraform allow you to define and provision Google Cloud resources as code. Console and Shell are interfaces, not infrastructure-as-code tools.
 
 
</details>


---

### **Managing implementation**

### 27. Which Google Cloud service provisions resources from declarative YAML configuration files and is a native Infrastructure-as-Code option?

- [ ] **A)** Cloud Deployment Manager
- [ ] **B)** Cloud Build
- [ ] **C)** Kubernetes Engine
- [ ] **D)** App Engine

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Deployment Manager is Google Cloud’s native Infrastructure-as-Code service, which creates resources from YAML declarative configuration files.
 
 
</details>

### 28. What are valid benefits of using Cloud Deployment Manager to manage implementation? Select two.

- [ ] **A)** Deployments can be repeated in multiple projects
- [ ] **B)** Resources can be updated by editing the configuration
- [ ] **C)** The service replaces IAM policies automatically
- [ ] **D)** It runs inside every GKE node

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Deployment Manager provides repeatable, declarative deployments and supports update operations; it does not automatically replace IAM policies nor run in GKE nodes.
 
 
</details>

### 29. The provided Deployment manifest specifies an update strategy. What is the name of this upgrade method?

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: app
spec:
  replicas: 5
  strategy:
    type: RollingUpdate
  selector:
    matchLabels:
      app: web
  template:
    metadata:
      labels:
        app: web
    spec:
      containers:
      - name: web
        image: gcr.io/project/web:v2
```

- [ ] **A)** RollingUpdate
- [ ] **B)** Recreate
- [ ] **C)** Blue/green
- [ ] **D)** Canary

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The `strategy` field with `type: RollingUpdate` instructs Kubernetes to replace pods incrementally with minimal downtime.
 
 
</details>

### 30. Which command sends the local source tree to Cloud Build using an existing build config file?

- [ ] **A)** gcloud builds submit --config cloudbuild.yaml .
- [ ] **B)** gcloud app deploy cloudbuild.yaml
- [ ] **C)** kubectl apply -f cloudbuild.yaml
- [ ] **D)** gsutil cp cloudbuild.yaml gs://bucket

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> `gcloud builds submit --config cloudbuild.yaml` uploads source code and the build configuration to Cloud Build for execution.
 
 
</details>

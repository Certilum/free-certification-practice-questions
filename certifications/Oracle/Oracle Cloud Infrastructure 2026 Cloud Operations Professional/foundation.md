<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Oracle%20Cloud%20Infrastructure%202026%20Cloud%20Operations%20Professional.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Oracle Cloud Infrastructure 2026 Cloud Operations Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Configuration Management Tools](#configuration-management-tools) (6 questions)
- [Cost and Performance Optimization](#cost-and-performance-optimization) (5 questions)
- [Deploying and Managing Resources](#deploying-and-managing-resources) (3 questions)
- [Identity and Security](#identity-and-security) (7 questions)
- [Observability](#observability) (6 questions)
- [Reliability and Business Continuity](#reliability-and-business-continuity) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:46:02.876Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Configuration Management Tools | 6 |
| Cost and Performance Optimization | 5 |
| Deploying and Managing Resources | 3 |
| Identity and Security | 7 |
| Observability | 6 |
| Reliability and Business Continuity | 3 |

---

### **Configuration Management Tools**

### 1. Which Oracle Cloud Infrastructure service is the managed Terraform service used to automate the deployment and lifecycle of cloud resources?

- [ ] **A)** Resource Manager
- [ ] **B)** Cloud Shell
- [ ] **C)** Cloud Advisor
- [ ] **D)** Virtual Cloud Network

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI Resource Manager is the managed Terraform service that provisions and updates resources from Terraform configuration files.
 
 
</details>

### 2. Which functions are provided by the Oracle Cloud Infrastructure Resource Manager service for Terraform-based configuration management?

- [ ] **A)** Creating Terraform plans
- [ ] **B)** Applying Terraform configurations
- [ ] **C)** Detecting drift in deployed resources
- [ ] **D)** Managing user authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Resource Manager runs plan and apply jobs, and drift detection compares the last successful job with the current state of resources. Identity and access tasks are handled by IAM.
 
 
</details>

### 3. Review the displayed OCI CLI command and identify the flag that provides the path to the Terraform configuration directory.

```bash
oci resource-manager stack create \
--compartment-id ocid1.compartment.oc1.. \
--display-name "Production Web Stack" \
--config-source ./terraform/config \
--terraform-version "1.3.x"
```

- [ ] **A)** --compartment-id
- [ ] **B)** --display-name
- [ ] **C)** --config-source
- [ ] **D)** --terraform-version

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The --config-source flag defines the Terraform configuration location. The other flags identify the compartment, service label, and Terraform version.
 
 
</details>

### 4. Which type of file maintains metadata about Oracle Cloud resources after a Terraform configuration has been applied?

- [ ] **A)** Terraform state file
- [ ] **B)** Provider configuration file
- [ ] **C)** IAM policy file
- [ ] **D)** OCI CLI config file

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Terraform state file stores resource metadata and is used to plan changes. The other listed files are not used to store state.
 
 
</details>

### 5. Which of the following source locations can Resource Manager use to obtain the Terraform configuration for a new stack?

- [ ] **A)** GitHub repository
- [ ] **B)** GitLab repository
- [ ] **C)** Object Storage bucket
- [ ] **D)** Autonomous Database table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Resource Manager can load configurations from supported Git providers and Object Storage buckets. A database table is not a configuration source.
 
 
</details>

### 6. Which language is used in the displayed configuration excerpt to declare Oracle Cloud Infrastructure resources?

```hcl
resource "oci_core_vcn" "production_vcn" {
  cidr_block       = "10.0.0.0/16"
  compartment_id   = var.compartment_id
  display_name     = "production-vcn"
  dns_label        = "prod"
}
```

- [ ] **A)** HCL
- [ ] **B)** JSON
- [ ] **C)** YAML
- [ ] **D)** Python

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Terraform configurations are normally written in HCL, the HashiCorp Configuration Language. Resource Manager reads HCL to create the resources described.
 
 
</details>


---

### **Cost and Performance Optimization**

### 7. What is the primary purpose of Cost Analysis in Oracle Cloud Infrastructure?

- [ ] **A)** To explore OCI costs and usage trends
- [ ] **B)** To deploy compute resources automatically
- [ ] **C)** To configure network security rules
- [ ] **D)** To create user access policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cost Analysis provides visibility into OCI spending and usage, allowing teams to identify optimization opportunities and manage cloud costs.
 
 
</details>

### 8. Which two Oracle Cloud Infrastructure capabilities are used to manage cloud costs?

- [ ] **A)** Budgets
- [ ] **B)** Cost Analysis
- [ ] **C)** Virtual Cloud Network (VCN)
- [ ] **D)** OCI Identity and Access Management (IAM)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Budgets and Cost Analysis are cost management services. VCN and IAM provide networking and access control, not cost monitoring.
 
 
</details>

### 9. What action does the OCI CLI command in the code block perform?

```bash
oci budgets budget create --compartment-id ocid1.compartment.oc1..example --amount 500 --reset-period MONTHLY --description MonthlyBudget
```

- [ ] **A)** It creates a new monthly budget
- [ ] **B)** It lists all budgets in the compartment
- [ ] **C)** It removes the existing monthly budget
- [ ] **D)** It generates a cost and usage report

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The budget create command creates a new budget in the specified compartment; it does not list, delete, or report budgets.
 
 
</details>

### 10. What is a primary benefit of enabling Compute autoscaling for an OCI workload?

- [ ] **A)** It automatically adjusts compute capacity to match demand
- [ ] **B)** It applies security rules to compute instances
- [ ] **C)** It backs up every application database
- [ ] **D)** It removes the need for performance monitoring

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Autoscaling adjusts compute capacity according to workload demand, reducing overprovisioning and supporting performance targets.
 
 
</details>

### 11. Which two practices help optimize costs while protecting workload performance?

- [ ] **A)** Stopping unused compute instances
- [ ] **B)** Rightsizing underutilized resources
- [ ] **C)** Deploying workloads on the largest available shapes
- [ ] **D)** Removing all cost tracking tags from resources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Stopping unused resources and right-sizing shapes reduce waste while maintaining the capacity required for application performance.
 
 
</details>


---

### **Deploying and Managing Resources**

### 12. In Oracle Cloud Infrastructure, which element is used as the primary logical container for organizing and isolating resources?

- [ ] **A)** Compartment
- [ ] **B)** Region
- [ ] **C)** Availability Domain
- [ ] **D)** Virtual Cloud Network

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A compartment is a primary logical container in OCI for organizing and isolating cloud resources. Regions, availability domains, and VCNs describe physical or network boundaries, not resource organization containers.
 
 
</details>

### 13. Which two statements about OCI compartments are correct?

- [ ] **A)** Compartments can be nested to create a hierarchy.
- [ ] **B)** Each new cloud resource is created inside a compartment.
- [ ] **C)** Compartments replace the need for network security lists.
- [ ] **D)** Compartments automatically replicate resources across all global regions.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OCI compartments can be nested, and all cloud resources belong to a compartment. Compartments do not replace network security or automatically replicate resources across regions.
 
 
</details>

### 14. Review the OCI command in the code block. What does this command do?

```bash
oci compute instance list \
  --compartment-id ocid1.compartment.oc1..example \
  --availability-domain "AD-1"
```

- [ ] **A)** It lists compute instances in the specified compartment and availability domain.
- [ ] **B)** It launches a new compute instance in the given compartment.
- [ ] **C)** It terminates all compute instances that are currently running.
- [ ] **D)** It displays the service limits for the tenancy.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses the OCI CLI compute instance list operation with compartment and availability domain parameters. Therefore, it retrieves and lists the matching compute instances.
 
 
</details>


---

### **Identity and Security**

### 15. In the context of Oracle Cloud Infrastructure identity and security, what is the primary purpose of an IAM policy?

- [ ] **A)** Determines permitted resource operations
- [ ] **B)** Provides physical data center security
- [ ] **C)** Creates virtual cloud networks
- [ ] **D)** Designs database schemas

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI IAM policies determine which groups can act on which resources. The policy grants authorization after the user or service principal is authenticated.
 
 
</details>

### 16. Which of the following OCI entities are used by IAM to control access to cloud resources? Select all that apply.

- [ ] **A)** Users
- [ ] **B)** Groups
- [ ] **C)** Virtual cloud networks
- [ ] **D)** Fault domains

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Users and groups identify principals in IAM policies. VCNs and fault domains are infrastructure constructs, not identity and access control entities.
 
 
</details>

### 17. Refer to the OCI IAM policy statement displayed in the code block. Which access result does it produce for the named group?

```plaintext
Allow group NetworkAdmins to manage virtual-network-family in compartment Network
```

- [ ] **A)** Manage network resources in the Network compartment
- [ ] **B)** Read compute instances in the Network compartment
- [ ] **C)** Manage users across the tenancy
- [ ] **D)** Delete object storage buckets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This IAM policy allows the NetworkAdmins group to perform management actions on the virtual-network-family inside the Network compartment.
 
 
</details>

### 18. What is an OCI compartment and what role does it play when cloud resources are deployed?

- [ ] **A)** Logical isolation container for cloud resources
- [ ] **B)** Dedicated physical server
- [ ] **C)** Load balancer configuration
- [ ] **D)** Database backup repository

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Compartments are logical containers for cloud resources. They support security by allowing policies and administrators to organize and isolate deployments.
 
 
</details>

### 19. Which security practices should be implemented when managing users and resources in an OCI tenancy? Select all that apply.

- [ ] **A)** Enable MFA for administrator users
- [ ] **B)** Grant unrestricted access to every user
- [ ] **C)** Use least-privilege policies for groups
- [ ] **D)** Use root user for daily administration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> MFA and least-privilege policies restrict the impact of stolen credentials. The root user and tenancy-wide grants should be avoided for everyday operations.
 
 
</details>

### 20. Based on the policy shown in the code block, what access does the group receive in the specified compartment?

```plaintext
Allow group SecurityAnalysts to read all-resources in compartment Security
```

- [ ] **A)** Read all resources in the Security compartment
- [ ] **B)** Manage all resources in the tenancy
- [ ] **C)** Create resources in the Security compartment
- [ ] **D)** Read resources only in the root compartment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This statement gives SecurityAnalysts read access to all resources in the Security compartment. It does not grant manage, create, or delete rights.
 
 
</details>

### 21. Which sentence correctly describes a dynamic group in Oracle Cloud Infrastructure IAM and its typical use for running workloads?

- [ ] **A)** Resources matched by membership rules
- [ ] **B)** Static list of human users
- [ ] **C)** Virtual network group
- [ ] **D)** Storage replication set

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI dynamic groups allow service resources to obtain IAM permissions without a static user account. Membership is rule-based.
 
 
</details>


---

### **Observability**

### 22. Which OCI service stores metric data and can raise alarms when a threshold is crossed?

- [ ] **A)** Monitoring
- [ ] **B)** Logging
- [ ] **C)** Audit
- [ ] **D)** Resource Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI Monitoring stores metrics, evaluates metric queries against thresholds, and raises alarms when conditions are met.
 
 
</details>

### 23. Which options describe valid uses of the OCI Logging service? (Choose all that apply.)

- [ ] **A)** Collect request and error logs from custom applications through an agent.
- [ ] **B)** Access audit and service logs from supported OCI resources.
- [ ] **C)** Graph infrastructure utilization as a metric time series.
- [ ] **D)** Evaluate tag-based cost tracking rules.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OCI Logging centralizes custom, service, and audit logs; it does not graph metrics or evaluate cost tracking rules.
 
 
</details>

### 24. Review the code block. Which OCI service does this CLI command interact with?

```bash
oci monitoring alarm list --compartment-id ocid1.compartment.oc1..example --all
```

- [ ] **A)** OCI Monitoring
- [ ] **B)** OCI Logging
- [ ] **C)** OCI Audit
- [ ] **D)** OCI Notifications

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses the 'monitoring' service prefix and lists alarms, so it targets OCI Monitoring.
 
 
</details>

### 25. Which OCI resource is a logical container for organizing and isolating cloud resources?

- [ ] **A)** Compartment
- [ ] **B)** Cloud region
- [ ] **C)** Availability domain
- [ ] **D)** Service gateway

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A compartment is a logical container that isolates resources and controls access through IAM policies.
 
 
</details>

### 26. Which OCI services are used to collect observability data? (Choose all that apply.)

- [ ] **A)** OCI Monitoring
- [ ] **B)** OCI Logging
- [ ] **C)** OCI Audit
- [ ] **D)** OCI Object Storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Monitoring, Logging, and Audit provide metrics, logs, and event records for observability; Object Storage is a data storage service.
 
 
</details>

### 27. Read the code block. Which OCI service is accessed by this CLI command?

```bash
oci logging log-group list --compartment-id ocid1.compartment.oc1..example --region us-ashburn-1
```

- [ ] **A)** OCI Logging
- [ ] **B)** OCI Monitoring
- [ ] **C)** OCI Notifications
- [ ] **D)** OCI Audit

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses the 'logging' service prefix and lists log groups, so it targets OCI Logging.
 
 
</details>


---

### **Reliability and Business Continuity**

### 28. Which boundary provides physical isolation against hardware failures within a single Availability Domain?

- [ ] **A)** Fault Domain
- [ ] **B)** Region
- [ ] **C)** Compartment
- [ ] **D)** Tenancy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Fault Domain is a logical data center boundary within an Availability Domain. It limits the impact of hardware failures and supports resilient resource placement.
 
 
</details>

### 29. Which two actions support business continuity when you manage cloud-deployed resources and need to recover from an outage?

- [ ] **A)** Perform automated backups
- [ ] **B)** Establish a disaster recovery site
- [ ] **C)** Disable monitoring alerts
- [ ] **D)** Delete archived configurations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Automated backups preserve data, and a disaster recovery site enables restoration after an outage. Disabling monitoring alerts or deleting archives increases operational risk and reduces continuity.
 
 
</details>

### 30. What is the intended outcome of the OCI CLI command shown in the code block?

```bash
oci resource-manager stack create --compartment-id ocid1.compartment.oc1..example --config-source https://example.com/config.zip --terraform-version 1.2.x --display-name ProductionStack
```

- [ ] **A)** Create a Resource Manager stack
- [ ] **B)** Start a container cluster
- [ ] **C)** Trigger a database backup
- [ ] **D)** Modify a network security list

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Resource Manager stack create registers a Terraform configuration as a stack in OCI Resource Manager. After creation, the stack can be used to plan and apply the described infrastructure.
 
 
</details>

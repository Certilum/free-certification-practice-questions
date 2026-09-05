<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Oracle%20Cloud%20Infrastructure%202026%20for%20Sunbird%20Ed%20Specialty.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Oracle Cloud Infrastructure 2026 for Sunbird Ed Specialty</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Design and Implementation](#design-and-implementation) (9 questions)
- [OCI Overview for Sunbird](#oci-overview-for-sunbird) (7 questions)
- [Operation and Management](#operation-and-management) (6 questions)
- [Sunbird ED Building Blocks](#sunbird-ed-building-blocks) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:46:23.512Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Design and Implementation | 9 |
| OCI Overview for Sunbird | 7 |
| Operation and Management | 6 |
| Sunbird ED Building Blocks | 8 |

---

### **Design and Implementation**

### 1. Which OCI resource is a logical container used to isolate and control access to the resources supporting Sunbird?

- [ ] **A)** Compartment
- [ ] **B)** Region
- [ ] **C)** Availability domain
- [ ] **D)** Dynamic group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A compartment is a logical collection of OCI resources and the primary mechanism for organizing resources and controlling access through IAM policies.
 
 
</details>

### 2. Which two statements about Oracle Cloud Infrastructure regions and availability domains are correct for multi-Availability-Domain deployments?

- [ ] **A)** A region can contain multiple availability domains.
- [ ] **B)** Availability domains provide isolation from data center failures.
- [ ] **C)** A region is always smaller than an availability domain.
- [ ] **D)** Availability domains can only be used for storage.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OCI regions are broad geographic areas and contain one or more availability domains. Availability domains are isolated data centers, so failures in one do not affect other availability domains.
 
 
</details>

### 3. Review the code block. Which first-time configuration must be completed before the OCI CLI command can work?

```bash
oci iam compartment create --compartment-id ocid1.compartment.oc1..test --name SunbirdProduction --description Production
```

- [ ] **A)** Configure an API signing key
- [ ] **B)** Create a compute instance
- [ ] **C)** Add a network security group
- [ ] **D)** Mount a block volume

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An OCI CLI installation must have an API signing key, user OCID, tenancy OCID, and fingerprint configured before it can call OCI IAM APIs.
 
 
</details>

### 4. Which Oracle Cloud Infrastructure service stores unstructured media objects such as Sunbird course videos and assessment content?

- [ ] **A)** Object Storage
- [ ] **B)** Block Volume
- [ ] **C)** File Storage
- [ ] **D)** Oracle Database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Object Storage is the OCI service for durable, scalable, and secure storage of files, images, videos, and other unstructured content.
 
 
</details>

### 5. During Sunbird networking setup, which two components are configured directly in a Virtual Cloud Network?

- [ ] **A)** Subnets
- [ ] **B)** Route tables
- [ ] **C)** Object storage buckets
- [ ] **D)** Resource Manager stacks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A VCN contains virtual network components such as subnets and route tables. Buckets are part of Object Storage, while Resource Manager stacks are used for Terraform-based infrastructure.
 
 
</details>

### 6. Review the Terraform code block for a new Sunbird VCN. How many route table resources are declared in the configuration?

```hcl
resource "oci_core_vcn" "sunbird_vcn" {
  compartment_id = var.compartment_ocid
  cidr_block     = "10.0.0.0/16"
  dns_label      = "sunbird"
}

resource "oci_core_route_table" "sunbird_route" {
  compartment_id = var.compartment_ocid
  vcn_id         = oci_core_vcn.sunbird_vcn.id
}
```

- [ ] **A)** One
- [ ] **B)** Two
- [ ] **C)** Zero
- [ ] **D)** Five

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The configuration declares exactly one route table resource, and it is associated with the VCN after Terraform applies the code.
 
 
</details>

### 7. Which OCI authentication mechanism allows a Sunbird compute instance to call OCI APIs without storing user keys?

- [ ] **A)** Instance principal
- [ ] **B)** Customer secret key
- [ ] **C)** Console password
- [ ] **D)** Network security group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An instance principal gives a compute instance an identity, so it can call OCI APIs without embedding user keys or passwords in code.
 
 
</details>

### 8. Which two Oracle Cloud database services can support operational data storage for a Sunbird deployment?

- [ ] **A)** Oracle Autonomous Database
- [ ] **B)** MySQL HeatWave
- [ ] **C)** OCI Object Storage
- [ ] **D)** OCI Data Transfer Service

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OCI offers fully managed database services such as Oracle Autonomous Database and MySQL HeatWave; the other two options are storage and transfer services.
 
 
</details>

### 9. The code block shows two successive OCI CLI commands for configuring a Sunbird load balancer. Which final backend-set policy is applied?

```bash
oci lb backend-set update --backend-set-name sunbird-backends --load-balancer-id ocid1.loadbalancer.oc1..example --policy ROUND_ROBIN
oci lb backend-set update --backend-set-name sunbird-backends --load-balancer-id ocid1.loadbalancer.oc1..example --policy LEAST_CONNECTIONS
```

- [ ] **A)** ROUND_ROBIN
- [ ] **B)** LEAST_CONNECTIONS
- [ ] **C)** IP HASH
- [ ] **D)** RANDOM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The second command updates the backend set policy to LEAST_CONNECTIONS and therefore replaces the prior ROUND_ROBIN value.
 
 
</details>


---

### **OCI Overview for Sunbird**

### 10. In Oracle Cloud Infrastructure, which statement correctly defines a region?

- [ ] **A)** A localized geographic area that contains one or more availability domains
- [ ] **B)** A group of fault domains used for compute placement
- [ ] **C)** A physical cluster dedicated to database workloads
- [ ] **D)** A billing boundary between two different tenancies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An OCI region is a localized geographic area that contains one or more availability domains. Regions are independent from each other and are usually paired for disaster recovery.
 
 
</details>

### 11. Which of the following are core IAM components in Oracle Cloud Infrastructure?

- [ ] **A)** Users
- [ ] **B)** Policies
- [ ] **C)** Groups
- [ ] **D)** Virtual Cloud Networks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Users, groups, policies, and compartments are IAM resources used to control access. Virtual cloud networks are network resources managed outside IAM.
 
 
</details>

### 12. The command in the code block is an OCI CLI instruction. Which OCI service is it associated with?

```bash
oci iam region list
```

- [ ] **A)** Identity and Access Management
- [ ] **B)** Virtual Cloud Networking
- [ ] **C)** Object Storage
- [ ] **D)** Block Volume

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The `oci iam region list` command targets the Identity and Access Management service and lists the regions subscribed for the tenancy.
 
 
</details>

### 13. Which type of data is best suited for the Standard tier of OCI Object Storage?

- [ ] **A)** Frequently accessed or hot data
- [ ] **B)** Cold data retained for legal compliance
- [ ] **C)** Data that is not used and can be deleted
- [ ] **D)** Data stored on premises in the customer data center

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Standard tier in OCI Object Storage is optimized for frequently accessed data, often called hot data. Archive storage is intended for cold data.
 
 
</details>

### 14. Which elements are normally defined as part of an OCI Virtual Cloud Network (VCN)?

- [ ] **A)** Subnets
- [ ] **B)** Route tables
- [ ] **C)** Security lists
- [ ] **D)** Object Storage buckets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A VCN contains subnets, route tables, and security lists. Object Storage is a separate service and is not defined inside a VCN.
 
 
</details>

### 15. Consider the CLI command in the code block. Which OCI service does it interact with?

```bash
oci os object list --namespace sunbirded --bucket-name sunbird-assets
```

- [ ] **A)** Object Storage
- [ ] **B)** Block Volume
- [ ] **C)** File Storage
- [ ] **D)** Virtual Cloud Networking

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The `oci os` portion of the command is the CLI namespace for Object Storage. Therefore, the command interacts with the Object Storage service.
 
 
</details>

### 16. Which option correctly describes an availability domain in OCI?

- [ ] **A)** One or more isolated data centers within a region
- [ ] **B)** A grouping of compute instances across a fleet
- [ ] **C)** A geographic district used for billing
- [ ] **D)** A dedicated private network connection from a customer data center

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An availability domain is one or more isolated data centers inside an OCI region. Availability domains are designed to reduce the effect of hardware failures.
 
 
</details>


---

### **Operation and Management**

### 17. Which OCI resource-management entity is commonly used to isolate SunbirdEd production and development environments and to control access to their resources?

- [ ] **A)** Compartments
- [ ] **B)** Subnets
- [ ] **C)** Availability domains
- [ ] **D)** Object namespaces

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A compartment is a logical container for OCI resources. Policies control access to compartments, whereas subnets and availability domains have different infrastructure purposes.
 
 
</details>

### 18. Which two OCI services should be used together to warn SunbirdEd administrators when a compute instance CPU utilization exceeds a specified threshold?

- [ ] **A)** OCI Monitoring
- [ ] **B)** OCI Notifications
- [ ] **C)** OCI Object Storage
- [ ] **D)** OCI DNS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Monitoring evaluates metrics and raises alarms; Notifications delivers alert messages through topics and subscriptions. Object Storage stores data, and DNS resolves domain names.
 
 
</details>

### 19. Examine the OCI CLI command shown in the code block. What does this command accomplish?

```bash
oci compute instance list --compartment-id ocid1.compartment.oc1..example

```

- [ ] **A)** List compute instances in the specified compartment
- [ ] **B)** Create a new compute instance
- [ ] **C)** Delete all stopped compute instances
- [ ] **D)** Start a compute instance in the compartment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The list command returns all compute instance resources in the supplied compartment. It does not create, delete, or change the lifecycle state of instances.
 
 
</details>

### 20. Which OCI feature can be applied to SunbirdEd resources to record metadata such as environment, cost center, or business owner?

- [ ] **A)** Tagging
- [ ] **B)** Subnetting
- [ ] **C)** Autoscaling
- [ ] **D)** Data masking

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Tags are key-value metadata used for organization and cost tracking. They do not change resource configuration; subnetting, autoscaling, and data masking are different operational mechanisms.
 
 
</details>

### 21. Which two OCI services provide historical event and log data used to investigate operational changes in a SunbirdEd environment?

- [ ] **A)** OCI Audit
- [ ] **B)** OCI Logging
- [ ] **C)** OCI Notifications
- [ ] **D)** OCI DNS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OCI Audit records API activity in the tenancy. OCI Logging collects and stores logs. Notifications only routes alerts, and DNS handles domain-name resolution.
 
 
</details>

### 22. Review the IAM policy statement shown in the code block. What access will SunbirdOperators group members receive?

```plaintext
Allow group SunbirdOperators to read all-resources in compartment SunbirdProd

```

- [ ] **A)** Read information about resources in compartment SunbirdProd
- [ ] **B)** Create and terminate resources in compartment SunbirdProd
- [ ] **C)** Read information about resources in every compartment in the tenancy
- [ ] **D)** Manage users and groups in the tenancy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy uses the read verb and scopes access to SunbirdProd, so members can only view resources in that compartment and cannot manage resources or access other compartments.
 
 
</details>


---

### **Sunbird ED Building Blocks**

### 23. In an Oracle Cloud Infrastructure overview for Sunbird ED, what does the abbreviation OCI stand for?

- [ ] **A)** Oracle Cloud Infrastructure
- [ ] **B)** Open Cloud Instance
- [ ] **C)** Oracle Certified Interface
- [ ] **D)** Online Cloud Integration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI stands for Oracle Cloud Infrastructure. It is Oracle's cloud platform used to build and run workloads such as Sunbird ED.
 
 
</details>

### 24. Which two OCI building blocks are most directly required to create the network foundation and identity boundary for a Sunbird ED deployment?

- [ ] **A)** Virtual Cloud Network (VCN)
- [ ] **B)** OCI Identity and Access Management (IAM)
- [ ] **C)** Oracle Analytics Cloud
- [ ] **D)** Oracle Blockchain Platform

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A VCN provides the isolated network foundation, while IAM provides authentication and authorization. Together they establish the security and connectivity foundation for Sunbird ED.
 
 
</details>

### 25. Refer to the OCI CLI command in the code block. What is displayed when this command is run during a Sunbird ED environment assessment?

```bash
oci iam availability-domain list
```

- [ ] **A)** All availability domains available to the current tenancy
- [ ] **B)** All compute instances running in the region
- [ ] **C)** All compartments with active resources
- [ ] **D)** All identity users in the tenancy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command lists availability domains in the tenancy. Availability domains are isolated data centers that can host Sunbird ED resources for high availability.
 
 
</details>

### 26. What is the primary purpose of OCI Identity and Access Management (IAM) within a Sunbird ED environment?

- [ ] **A)** It defines which users or groups can perform actions on resources and under what conditions
- [ ] **B)** It runs the Sunbird ED backend as a managed container service
- [ ] **C)** It stores education content in highly durable object storage
- [ ] **D)** It balances traffic between Sunbird ED application instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI IAM manages user identities, groups, policies, and access controls. It determines who can access Sunbird ED cloud resources and what actions they can perform.
 
 
</details>

### 27. Which two OCI services are most commonly used to persist and distribute educational content for a Sunbird ED solution?

- [ ] **A)** OCI Object Storage
- [ ] **B)** OCI Content Delivery Network (CDN)
- [ ] **C)** OCI Container Engine for Kubernetes
- [ ] **D)** OCI Data Safe

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Object Storage provides durable, scalable storage for content, while CDN helps deliver that content quickly to learners across multiple geographic regions.
 
 
</details>

### 28. The code block shows an OCI CLI command used to inspect a Sunbird ED content bucket. What information is returned by the command?

```bash
oci os object list --bucket-name sunbird-content --namespace sunbirdedu
```

- [ ] **A)** A list of objects stored in the bucket
- [ ] **B)** The current bucket access policy
- [ ] **C)** The network security list for the bucket
- [ ] **D)** The identity users with read access to the bucket

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The OCI CLI object list command returns the names and metadata of objects contained in the target Object Storage bucket.
 
 
</details>

### 29. Which OCI service should be used to host the main Sunbird ED application server instances?

- [ ] **A)** OCI Compute
- [ ] **B)** OCI Object Storage
- [ ] **C)** OCI Data Flow
- [ ] **D)** OCI NoSQL Database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI Compute provides virtual machines, also called compute instances, that can run the Sunbird ED application stack.
 
 
</details>

### 30. Why would a Sunbird ED architecture use separate OCI compartments for development, testing, and production?

- [ ] **A)** It creates isolated resource boundaries for different environments
- [ ] **B)** It lets IAM policies grant access at a granular level
- [ ] **C)** It automatically scales compute instances
- [ ] **D)** It globally replicates content to every region

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Compartments group related resources and enforce isolation. They also provide the scope for more granular IAM policies across different Sunbird ED environments.
 
 
</details>

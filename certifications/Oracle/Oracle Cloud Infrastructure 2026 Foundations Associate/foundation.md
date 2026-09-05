<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Oracle%20Cloud%20Infrastructure%202026%20Foundations%20Associate.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Oracle Cloud Infrastructure 2026 Foundations Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Core OCI Services](#core-oci-services) (15 questions)
- [Getting Started with OCI](#getting-started-with-oci) (4 questions)
- [Governance and Administration](#governance-and-administration) (3 questions)
- [Security Services](#security-services) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:46:13.192Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Core OCI Services | 15 |
| Getting Started with OCI | 4 |
| Governance and Administration | 3 |
| Security Services | 8 |

---

### **Core OCI Services**

### 1. When studying Oracle Cloud Infrastructure, what does the acronym OCI stand for in Oracle's cloud offerings?

- [ ] **A)** Oracle Cloud Infrastructure
- [ ] **B)** Oracle Compute Instance
- [ ] **C)** Oracle Cloud Integration
- [ ] **D)** Oracle Customer Interface

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI stands for Oracle Cloud Infrastructure, which is Oracle's platform for delivering cloud computing services.
 
 
</details>

### 2. When designing a deployment on Oracle Cloud Infrastructure, which two concepts define its global geographic and fault-tolerant foundation?

- [ ] **A)** Regions
- [ ] **B)** Availability Domains
- [ ] **C)** Object Storage buckets
- [ ] **D)** Virtual Cloud Networks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OCI uses regions and availability domains to provide geographic distribution and fault tolerance. Object Storage and VCNs are services, not global architecture concepts.
 
 
</details>

### 3. An OCI administrator runs the command shown in the code block. What kind of information does this command return?

```shell
oci iam region list
```

- [ ] **A)** List of OCI regions
- [ ] **B)** List of IAM users
- [ ] **C)** List of compute instances
- [ ] **D)** List of availability domains

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command oci iam region list returns region information, helping administrators see the regions available to their tenancy.
 
 
</details>

### 4. In the Oracle Cloud Infrastructure operating model, what is the best definition of a tenancy for a customer?

- [ ] **A)** A secure and isolated OCI partition for resources
- [ ] **B)** A single virtual machine
- [ ] **C)** A type of object storage bucket
- [ ] **D)** A network firewall service

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A tenancy is a secure and isolated partition within Oracle Cloud Infrastructure where a customer creates and manages cloud resources.
 
 
</details>

### 5. Which two OCI IAM resources are commonly used together to control access to cloud resources?

- [ ] **A)** Users
- [ ] **B)** Groups
- [ ] **C)** Virtual Cloud Networks
- [ ] **D)** Object Storage buckets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OCI IAM uses users and groups to manage identities and permissions. VCNs and Object Storage buckets are not IAM resources.
 
 
</details>

### 6. An administrator executes the OCI CLI command shown in the code block. What is the direct result of this action?

```shell
oci iam compartment create --compartment-id <root> --name "Finance" --description "Finance department resources"
```

- [ ] **A)** A new compartment named Finance is created
- [ ] **B)** The Finance compartment is deleted
- [ ] **C)** A list of existing compartments is displayed
- [ ] **D)** The Finance compartment is renamed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command creates an IAM compartment called Finance inside the specified parent compartment.
 
 
</details>

### 7. Within the Oracle Cloud Infrastructure resource hierarchy, what role does a compartment play for organizing resources?

- [ ] **A)** A logical container for OCI resources
- [ ] **B)** A physical data center
- [ ] **C)** A virtual network gateway
- [ ] **D)** A compute instance shape

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A compartment is a logical container for organizing and isolating Oracle Cloud Infrastructure resources.
 
 
</details>

### 8. Which two services in Oracle Cloud Infrastructure are designed specifically for running compute workloads?

- [ ] **A)** Compute
- [ ] **B)** Container Engine for Kubernetes
- [ ] **C)** Object Storage
- [ ] **D)** Identity and Access Management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OCI Compute provides virtual machines and bare metal instances, while OKE runs containerized workloads. Object Storage and IAM are not compute services.
 
 
</details>

### 9. The OCI CLI command in the code block is used to create which type of networking resource?

```shell
oci network vcn create --compartment-id ocid1.compartment.oc1.. --cidr-blocks 10.0.0.0/16 --display-name my-vcn
```

- [ ] **A)** Virtual Cloud Network
- [ ] **B)** Subnet
- [ ] **C)** Internet Gateway
- [ ] **D)** Route Table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The oci network vcn create command creates a Virtual Cloud Network in the specified compartment.
 
 
</details>

### 10. Within Oracle Cloud Infrastructure regional architecture, what is an Availability Domain designed to provide?

- [ ] **A)** Fault-tolerant data center isolation
- [ ] **B)** A single physical server
- [ ] **C)** A logical IAM policy container
- [ ] **D)** A globally unique storage namespace

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An Availability Domain is one or more data centers within a region. ADs are isolated from each other to prevent correlated failures.
 
 
</details>

### 11. Which two statements accurately describe Oracle Cloud Infrastructure regions and their relationship to availability domains?

- [ ] **A)** A region is a localized geographic area
- [ ] **B)** A region contains one or more availability domains
- [ ] **C)** Every region has exactly one availability domain
- [ ] **D)** A region is the smallest OCI resource unit

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A region is a localized geographic area that contains one or more availability domains. Regions are large-scale architecture components, not small resource units.
 
 
</details>

### 12. What type of information does the OCI CLI command displayed in the code block retrieve from the tenancy?

```shell
oci os ns get
```

- [ ] **A)** Object Storage namespace
- [ ] **B)** List of buckets
- [ ] **C)** List of objects in a bucket
- [ ] **D)** Availability Domain name

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The oci os ns get command returns the Object Storage namespace associated with the tenancy.
 
 
</details>

### 13. Which OCI storage service is intended for storing large amounts of unstructured data such as images and backups?

- [ ] **A)** Object Storage
- [ ] **B)** Block Volume
- [ ] **C)** File Storage
- [ ] **D)** Local NVMe storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI Object Storage is designed for storing and retrieving unstructured data, including images, backups, and other object-based content.
 
 
</details>

### 14. Which two common methods can be used by an administrator to interact with and manage Oracle Cloud Infrastructure resources?

- [ ] **A)** Oracle Cloud Console
- [ ] **B)** OCI Command Line Interface
- [ ] **C)** On-premises physical server
- [ ] **D)** Telephone support

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The Console and CLI are common ways to manage OCI resources. Physical servers and telephone support are not resource management interfaces.
 
 
</details>

### 15. The command in the code block is used to interact with which Oracle Cloud Infrastructure service?

```shell
oci compute instance list --compartment-id ocid1.compartment.oc1.. --availability-domain AD-1
```

- [ ] **A)** Compute
- [ ] **B)** Object Storage
- [ ] **C)** Networking
- [ ] **D)** Identity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The oci compute instance list command belongs to the Compute service and returns information about compute instances.
 
 
</details>


---

### **Getting Started with OCI**

### 16. In Oracle Cloud Infrastructure, what does the term 'tenancy' refer to?

- [ ] **A)** The physical data center within a region
- [ ] **B)** A secure, logically isolated partition of OCI resources
- [ ] **C)** A network gateway for internet connectivity
- [ ] **D)** A command used to manage OCI resources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A tenancy in OCI is a secure and isolated partition of resources created when you sign up for Oracle Cloud Infrastructure.
 
 
</details>

### 17. Which of the following are considered core OCI Identity and Access Management (IAM) components?

- [ ] **A)** Users
- [ ] **B)** Groups
- [ ] **C)** Compartments
- [ ] **D)** Cloud Shell

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> OCI IAM includes users, groups, and compartments to manage access to resources. Cloud Shell is a separate tool.
 
 
</details>

### 18. Review the command in the code block. Which OCI service is the command associated with?

```shell
oci compute instance list --availability-domain AD1 --compartment-id ocid1.compartment.oc1..example
```

- [ ] **A)** Compute
- [ ] **B)** Networking
- [ ] **C)** Database
- [ ] **D)** Identity and Access Management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses 'oci compute instance list', so it interacts with the OCI Compute service.
 
 
</details>

### 19. After creating your Oracle Cloud Infrastructure account, what is the immediate next step to start managing resources?

- [ ] **A)** Sign in to the OCI Console
- [ ] **B)** Create a virtual cloud network
- [ ] **C)** Create a compartment
- [ ] **D)** Launch a compute instance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The first step after account creation is to sign in to the OCI Console, where you can manage all OCI resources.
 
 
</details>


---

### **Governance and Administration**

### 20. In Oracle Cloud Infrastructure, what is the top-level container that holds all resources and is created when you sign up?

- [ ] **A)** Tenancy
- [ ] **B)** Region
- [ ] **C)** Compartment
- [ ] **D)** Availability domain

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The tenancy is the root container for all OCI resources and is created when you register for Oracle Cloud Infrastructure.
 
 
</details>

### 21. In Oracle Cloud Infrastructure, compartments are used to organize and manage resources. Which statements about compartments are correct? Select all that apply.

- [ ] **A)** A compartment is a logical container for resources.
- [ ] **B)** Compartments can be nested inside other compartments.
- [ ] **C)** Compartments provide an access-control boundary.
- [ ] **D)** A compartment can span multiple tenancies.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Compartments are logical containers that organize resources, can be nested, and provide access control boundaries. A compartment cannot span multiple tenancies.
 
 
</details>

### 22. Review the Oracle Cloud Infrastructure command-line interface command shown in the code block. What administrative task does it perform?

```bash
oci iam compartment list --compartment-id ocid1.tenancy.oc1..example --access-level ACCESSIBLE
```

- [ ] **A)** It lists compartments accessible to the user.
- [ ] **B)** It deletes a compartment.
- [ ] **C)** It creates a new user.
- [ ] **D)** It assigns a policy to a compartment.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command lists compartments accessible to the current user in the specified tenancy, which helps administrators review governance structure.
 
 
</details>


---

### **Security Services**

### 23. What is the primary purpose of the Oracle Cloud Infrastructure Identity and Access Management (IAM) service?

- [ ] **A)** Manage compute instances
- [ ] **B)** Control access to OCI resources
- [ ] **C)** Store encryption keys
- [ ] **D)** Monitor security threats

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> OCI IAM is the service used to manage identities and control access to OCI resources by defining who can take action on specific resources.
 
 
</details>

### 24. Which of the following are Oracle Cloud Infrastructure security services?

- [ ] **A)** Cloud Guard
- [ ] **B)** Vault
- [ ] **C)** Object Storage
- [ ] **D)** Security Zones

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Cloud Guard, Vault, and Security Zones are OCI security services, while Object Storage is a data storage service rather than a security service.
 
 
</details>

### 25. What does the following OCI policy statement permit the group CompartmentAdmins to do?

```plaintext
Allow group CompartmentAdmins to manage virtual-network-family in compartment Networking
```

- [ ] **A)** Manage all resources in the tenancy
- [ ] **B)** Manage virtual network resources in the Networking compartment
- [ ] **C)** View all security policies
- [ ] **D)** Only manage compute instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The policy grants the manage permission on the virtual-network-family specifically within the Networking compartment.
 
 
</details>

### 26. Which Oracle Cloud Infrastructure service is used to store and manage sensitive data such as encryption keys and secrets?

- [ ] **A)** Cloud Guard
- [ ] **B)** Vault
- [ ] **C)** IAM
- [ ] **D)** Security Zones

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> OCI Vault is a managed service that securely stores and manages encryption keys and secrets for use in OCI services and applications.
 
 
</details>

### 27. Which capabilities are provided by Oracle Cloud Guard?

- [ ] **A)** Detects security misconfigurations
- [ ] **B)** Monitors and responds to threats
- [ ] **C)** Automates investigation and remediation
- [ ] **D)** Manages user passwords

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Cloud Guard detects security misconfigurations, monitors for threats, and automates investigation and remediation, but it does not manage user passwords.
 
 
</details>

### 28. What does the following OCI CLI command do?

```bash
oci network security-list list --compartment-id ocid1.compartment.oc1..example
```

- [ ] **A)** Lists all security lists in the specified compartment
- [ ] **B)** Creates a new security list
- [ ] **C)** Deletes a security list
- [ ] **D)** Displays details of a single security list

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses the OCI CLI to list all security lists in the compartment identified by the given OCID.
 
 
</details>

### 29. Which Oracle Cloud Infrastructure feature provides a logical collection of related resources and serves as a boundary for access policies?

- [ ] **A)** Compartments
- [ ] **B)** Vaults
- [ ] **C)** Regions
- [ ] **D)** Security Lists

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Compartments are logical collections of related OCI resources and are used as policy boundaries to control access for those resources.
 
 
</details>

### 30. Which statements about Oracle Cloud Infrastructure Security Zones are correct?

- [ ] **A)** They create a compartment with increased security controls
- [ ] **B)** They enforce policies that prevent insecure resource configurations
- [ ] **C)** They eliminate the need for all other security services
- [ ] **D)** They help ensure resources are deployed in a secure environment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Security Zones create secure compartments that enforce policies to prevent insecure configurations, but they do not eliminate the need for other security services.
 
 
</details>

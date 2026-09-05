<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Oracle%20Cloud%20Infrastructure%202026%20Architect%20Associate.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Oracle Cloud Infrastructure 2026 Architect Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Compute](#compute) (4 questions)
- [Database](#database) (4 questions)
- [Identity and Access Management](#identity-and-access-management) (6 questions)
- [Networking](#networking) (7 questions)
- [Observability and Management](#observability-and-management) (3 questions)
- [Storage](#storage) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:57.750Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Compute | 4 |
| Database | 4 |
| Identity and Access Management | 6 |
| Networking | 7 |
| Observability and Management | 3 |
| Storage | 6 |

---

### **Compute**

### 1. In Oracle Cloud Infrastructure, what is the primary purpose of the Identity and Access Management service?

- [ ] **A)** Controlling access to OCI resources
- [ ] **B)** Launching compute instances
- [ ] **C)** Monitoring network traffic
- [ ] **D)** Creating block volume backups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI IAM controls who can access resources and what actions they can perform, across users, groups, and compartments.
 
 
</details>

### 2. Which of the following items are core components of the Oracle Cloud Infrastructure Identity and Access Management service?

- [ ] **A)** IAM users
- [ ] **B)** IAM policies
- [ ] **C)** Compartments
- [ ] **D)** Subnets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> IAM includes users, groups, compartments, and policies as core elements; subnets are networking components, not IAM elements.
 
 
</details>

### 3. Review the IAM policy statement shown in the code block. What level of access is granted to the InstanceAdmins group?

```plaintext
Allow group InstanceAdmins to manage compute-family in compartment Development
```

- [ ] **A)** Manage compute resources in the Development compartment
- [ ] **B)** Read-only access to compute resources
- [ ] **C)** Manage all resources in the tenancy
- [ ] **D)** Delete compute resources only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy allows the group to manage compute-family resources inside the Development compartment, granting full management permissions.
 
 
</details>

### 4. Within the OCI Identity and Access Management model, what exactly is a compartment used for?

- [ ] **A)** A logical container for organizing and isolating resources
- [ ] **B)** A physical server in an OCI data center
- [ ] **C)** A collection of IAM users
- [ ] **D)** A network security rule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A compartment is a logical partition used to organize and isolate OCI resources and control access through policies.
 
 
</details>


---

### **Database**

### 5. What does IAM stand for in Oracle Cloud Infrastructure?

- [ ] **A)** Identity and Access Management
- [ ] **B)** Integrated Application Monitoring
- [ ] **C)** Internet Access Management
- [ ] **D)** Information Asset Management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IAM stands for Identity and Access Management, the OCI service that controls access to resources.
 
 
</details>

### 6. Which two components are fundamental elements of OCI Identity and Access Management?

- [ ] **A)** Users and groups
- [ ] **B)** Access policies
- [ ] **C)** Virtual cloud networks
- [ ] **D)** Block volumes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OCI IAM manages principals such as users and groups, and uses policies to grant access. Networks and block volumes are resources, not IAM constructs.
 
 
</details>

### 7. Review the IAM policy in the code block. What access does it grant?

```oci-policy
allow group NetworkAdmins to manage virtual-network-family in compartment Network
```

- [ ] **A)** Manage virtual network resources in Network compartment
- [ ] **B)** Manage all resources in the tenancy
- [ ] **C)** Read virtual network resources in Network compartment
- [ ] **D)** Create users in Network compartment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The statement uses 'manage virtual-network-family in compartment Network', which grants management of virtual network resources in that compartment.
 
 
</details>

### 8. Which statement about an OCI IAM user is true?

- [ ] **A)** An entity that can be granted access through policies
- [ ] **B)** Another name for an IAM group
- [ ] **C)** A resource that can only exist in the root compartment
- [ ] **D)** A service that monitors user activity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A user is a principal in OCI IAM; policies define the access that the user has to resources.
 
 
</details>


---

### **Identity and Access Management**

### 9. What is the main purpose of a compartment in OCI IAM?

- [ ] **A)** Organizing and isolating cloud resources
- [ ] **B)** Storing user passwords
- [ ] **C)** Encrypting network traffic
- [ ] **D)** Creating backup policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A compartment is a logical container that helps you organize and control access to OCI resources while providing isolation between workloads.
 
 
</details>

### 10. Which two elements must be present to create an OCI IAM policy?

- [ ] **A)** A policy statement
- [ ] **B)** A compartment
- [ ] **C)** A dynamic group
- [ ] **D)** An API key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> An OCI IAM policy is composed of one or more policy statements, and it must be placed in a compartment such as the tenancy root compartment.
 
 
</details>

### 11. Given this IAM policy statement, what access do members of the NetworkAdmins group receive?

```plaintext
Allow group NetworkAdmins to manage virtual-network-family in compartment Network
```

- [ ] **A)** Full management of virtual network resources
- [ ] **B)** Read-only access to virtual networks
- [ ] **C)** Only permission to view compartments
- [ ] **D)** Administrative access to all tenancy resources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy grants the manage verb for the virtual-network-family, allowing full management of virtual network resources in the specified compartment.
 
 
</details>

### 12. Which IAM resource is a collection of users that can be assigned permissions through policies?

- [ ] **A)** Group
- [ ] **B)** Compartment
- [ ] **C)** Policy
- [ ] **D)** Fault domain

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An IAM group is a collection of users that can be referenced together in policies to grant the same permissions to all members.
 
 
</details>

### 13. Which two credentials are commonly used by OCI IAM users to authenticate API requests?

- [ ] **A)** API signing keys
- [ ] **B)** Auth tokens
- [ ] **C)** CIDR blocks
- [ ] **D)** Availability domains

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> API signing keys and auth tokens are both IAM credentials used to authenticate API requests. CIDR blocks and availability domains are not credentials.
 
 
</details>

### 14. Given this dynamic group matching rule, which statements are true?

```plaintext
ALL {instance.compartment.id = 'ocid1.compartment.oc1..example'}
```

- [ ] **A)** It applies only to instances in the specified compartment
- [ ] **B)** It is evaluated automatically based on resource attributes
- [ ] **C)** It assigns users to the dynamic group manually
- [ ] **D)** It directly grants network access privileges

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A dynamic group rule is evaluated automatically using matching criteria based on resource attributes. The rule shown includes only instances in the specified compartment.
 
 
</details>


---

### **Networking**

### 15. In Oracle Cloud Infrastructure, what is the primary purpose of IAM?

- [ ] **A)** Controlling access to cloud resources
- [ ] **B)** Providing network connectivity
- [ ] **C)** Storing backup data
- [ ] **D)** Monitoring server performance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI IAM controls who can access cloud resources and what actions they can perform.
 
 
</details>

### 16. Which two resources are managed by IAM to grant access to Oracle Cloud Infrastructure resources?

- [ ] **A)** Users
- [ ] **B)** Groups
- [ ] **C)** VCNs
- [ ] **D)** Subnets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> IAM uses users and groups as principals, then policies grant access to resources.
 
 
</details>

### 17. Review the policy in the code block. Which action is explicitly allowed?

```plaintext
Allow group NetworkAuditors to inspect virtual-network-family in compartment Network
```

- [ ] **A)** inspect virtual-network-family
- [ ] **B)** manage virtual-network-family
- [ ] **C)** use virtual-network-family
- [ ] **D)** read virtual-network-family

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy says that the group can inspect, not manage, the virtual network family.
 
 
</details>

### 18. Which IAM resource groups multiple users together for access management?

- [ ] **A)** Group
- [ ] **B)** Policy
- [ ] **C)** Compartment
- [ ] **D)** Region

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A group is an IAM resource that contains users so that policies can be applied more efficiently.
 
 
</details>

### 19. Which two statements about OCI IAM policies are correct?

- [ ] **A)** They are written using Allow statements
- [ ] **B)** They are automatically created for every user
- [ ] **C)** They specify what resources a principal can access
- [ ] **D)** They encrypt all network traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> IAM policies use Allow statements to grant access to resources; they are not auto-created per user.
 
 
</details>

### 20. Review the code block. Which group is granted the manage permission?

```plaintext
Allow group NetworkAdmins to manage virtual-network-family in compartment Network
```

- [ ] **A)** NetworkAdmins
- [ ] **B)** NetworkAuditors
- [ ] **C)** NetworkViewers
- [ ] **D)** NetworkUsers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy begins with 'Allow group NetworkAdmins', so NetworkAdmins is the principal.
 
 
</details>

### 21. An OCI IAM policy statement that begins with 'Allow' is mainly used to do what?

- [ ] **A)** Grant permissions
- [ ] **B)** Deny all actions
- [ ] **C)** Assign tags
- [ ] **D)** Create users

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An Allow statement grants a principal permission to perform actions on specified cloud resources.
 
 
</details>


---

### **Observability and Management**

### 22. What is the primary function of OCI Identity and Access Management (IAM)?

- [ ] **A)** Defining which users and groups can access which OCI resources
- [ ] **B)** Managing physical hardware installation
- [ ] **C)** Creating virtual machines automatically
- [ ] **D)** Monitoring application performance only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IAM controls access to OCI resources by managing users, groups, policies, and permissions.
 
 
</details>

### 23. Which two items are core components of OCI IAM? (Choose two.)

- [ ] **A)** Compartments
- [ ] **B)** Policies
- [ ] **C)** Availability Domains
- [ ] **D)** VCN Flow Logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Compartments help organize resources, and policies define resource access. Availability Domains and VCN Flow Logs are not IAM components.
 
 
</details>

### 24. Review the code block. Which type of IAM resource is being shown?

```plaintext
Allow group NetworkAdmins to manage virtual-network-family in compartment Networking
```

- [ ] **A)** A policy statement
- [ ] **B)** A group membership
- [ ] **C)** A compartment hierarchy
- [ ] **D)** A user credential

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block shows an IAM policy statement that grants a group permission to manage resources in a compartment.
 
 
</details>


---

### **Storage**

### 25. In Oracle Cloud Infrastructure, what does the service abbreviation IAM stand for in the context of governance and security?

- [ ] **A)** Identity and Access Management
- [ ] **B)** Infrastructure and Availability Management
- [ ] **C)** Information Asset Management
- [ ] **D)** Integrated Access Monitoring

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IAM stands for Identity and Access Management. It controls access to OCI resources by defining users, groups, policies, and compartments.
 
 
</details>

### 26. Which of the following are core components of Oracle Cloud Infrastructure Identity and Access Management?

- [ ] **A)** Users
- [ ] **B)** Groups
- [ ] **C)** Policies
- [ ] **D)** Object Storage buckets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Core IAM components include users, groups, policies, compartments, and dynamic groups. Object Storage buckets are a storage service resource, not an IAM component.
 
 
</details>

### 27. Look at the IAM policy in the code block. What privilege does the group have over object-family resources?

```plaintext
Allow group StorageAdmins to manage object-family in tenancy
```

- [ ] **A)** Full management
- [ ] **B)** Read-only access
- [ ] **C)** Metadata inspection only
- [ ] **D)** Access to logs only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The manage verb grants full control over the specified resource family. StorageAdmins can create, read, update, delete, and otherwise manage object-family resources in the tenancy.
 
 
</details>

### 28. Which IAM element represents the root container for all of an organization's Oracle Cloud Infrastructure resources?

- [ ] **A)** Tenancy
- [ ] **B)** Compartment
- [ ] **C)** Group
- [ ] **D)** Policy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The tenancy is the root container that includes all compartments and resources. IAM policies and compartments live inside it.
 
 
</details>

### 29. Which of the following are valid verbs that can be used in an OCI IAM policy statement?

- [ ] **A)** inspect
- [ ] **B)** read
- [ ] **C)** use
- [ ] **D)** delete

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> OCI IAM policy statements use the verbs inspect, read, use, and manage. Delete is not a top-level policy verb; it is covered by higher-level verbs.
 
 
</details>

### 30. Based on the IAM policy in the code block, which access level can the group perform on bucket resources in the compartment?

```plaintext
Allow group StorageAuditors to read buckets in compartment Data
```

- [ ] **A)** inspect
- [ ] **B)** read
- [ ] **C)** use
- [ ] **D)** manage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The policy includes the read verb, so the group can read bucket resources but not modify them. Read access is broader than inspect but narrower than use or manage.
 
 
</details>

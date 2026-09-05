<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Oracle%20Cloud%20Infrastructure%202026%20Security%20Professional.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Oracle Cloud Infrastructure 2026 Security Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Improving Cloud Security Posture](#improving-cloud-security-posture) (5 questions)
- [Managing Identity and Access](#managing-identity-and-access) (7 questions)
- [Managing Security Operations](#managing-security-operations) (3 questions)
- [Network, Platform, and Infrastructure Security](#network-platform-and-infrastructure-security) (7 questions)
- [Securing Applications and Data](#securing-applications-and-data) (6 questions)
- [Understanding OCI Security Services](#understanding-oci-security-services) (2 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:46:20.890Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Improving Cloud Security Posture | 5 |
| Managing Identity and Access | 7 |
| Managing Security Operations | 3 |
| Network, Platform, and Infrastructure Security | 7 |
| Securing Applications and Data | 6 |
| Understanding OCI Security Services | 2 |

---

### **Improving Cloud Security Posture**

### 1. Why is learning about OCI security services important for professionals who want to improve their cloud security posture?

- [ ] **A)** They provide capabilities for protecting cloud resources.
- [ ] **B)** They entirely remove cloud security risks.
- [ ] **C)** They only increase OCI workload costs.
- [ ] **D)** They are used only after an incident occurs.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Understanding OCI security services is foundational because these services are the capabilities used to secure Oracle Cloud Infrastructure resources.
 
 
</details>

### 2. Which statements about OCI security services are true? Select all that apply.

- [ ] **A)** They help secure OCI resources.
- [ ] **B)** They can improve cloud security posture.
- [ ] **C)** They are the focus of the playbook title.
- [ ] **D)** They are designed for payroll management.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> OCI security services support securing cloud resources, improving cloud security posture, and are the main topic indicated by the source title.
 
 
</details>

### 3. Refer to the source heading in the code block. What is the primary subject introduced by that heading?

```markdown
# Understanding OCI Security Services
```

- [ ] **A)** Oracle Cloud Infrastructure security services
- [ ] **B)** Oracle Cloud Infrastructure billing processes
- [ ] **C)** Oracle Cloud Infrastructure compute pricing
- [ ] **D)** Oracle Cloud Infrastructure network cabling specifications

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The heading explicitly introduces OCI security services as the document subject, which aligns with the playbook title.
 
 
</details>

### 4. What would a new OCI learner most reasonably expect from a guide called Understanding OCI Security Services?

- [ ] **A)** An introduction to Oracle Cloud Infrastructure security services
- [ ] **B)** Instructions for configuring Oracle Cloud billing groups
- [ ] **C)** Guidance for choosing OCI data center locations
- [ ] **D)** Procedures for applying on-premises firewall patches

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The title clearly signals an introduction to OCI security services; the other choices refer to unrelated operational or billing topics.
 
 
</details>

### 5. Which purposes are indicated by the document title Understanding OCI Security Services? Select all that apply.

- [ ] **A)** Explain available OCI security services
- [ ] **B)** Support foundational security posture learning
- [ ] **C)** Introduce controls for protecting cloud workloads
- [ ] **D)** Remove security controls from OCI environments

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The source title and target domain indicate learning about OCI security services and improving security posture, not eliminating security controls.
 
 
</details>


---

### **Managing Identity and Access**

### 6. Which Oracle Cloud Infrastructure service is responsible for controlling access to OCI resources?

- [ ] **A)** Identity and Access Management
- [ ] **B)** Cloud Guard
- [ ] **C)** OCI Vault
- [ ] **D)** Web Application Firewall

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Identity and Access Management (IAM) is the OCI service used to control access to cloud resources through users, groups, and policies.
 
 
</details>

### 7. Which of the following are core elements managed by OCI Identity and Access Management? Select all that apply.

- [ ] **A)** IAM users
- [ ] **B)** IAM groups
- [ ] **C)** IAM policies
- [ ] **D)** Virtual cloud networks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> IAM manages users, groups, policies, dynamic groups, and compartments. VCNs are network resources handled by OCI Networking.
 
 
</details>

### 8. Refer to the command shown in the code block. What action will the command perform?

```bash
oci iam user list --compartment-id ocid1.compartment.oc1..example
```

- [ ] **A)** Lists users in a compartment
- [ ] **B)** Creates a new IAM user
- [ ] **C)** Deletes an existing IAM group
- [ ] **D)** Assigns a policy to a group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CLI command uses the list action for IAM users and a compartment ID, so it returns user records for that compartment.
 
 
</details>

### 9. In OCI, what is the main purpose of an IAM policy?

- [ ] **A)** They define access to resources
- [ ] **B)** They store encryption keys
- [ ] **C)** They collect security events
- [ ] **D)** They isolate network traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IAM policies state who may perform which actions on which OCI resources, making them the main access-control mechanism.
 
 
</details>

### 10. Which statements accurately describe compartments in OCI IAM? Select all that apply.

- [ ] **A)** They organize and isolate resources
- [ ] **B)** They help control resource access
- [ ] **C)** They can be nested hierarchically
- [ ] **D)** They are equivalent to regions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> OCI compartments are logical containers for organizing resources and applying access policies. They can be nested and are not the same as regions.
 
 
</details>

### 11. Review the IAM policy statement shown in the code block. What access does it grant?

```text
Allow group Engineers to manage instance-family in compartment ProjectA
```

- [ ] **A)** Engineers can manage compute resources in ProjectA
- [ ] **B)** Engineers can manage resources in all compartments
- [ ] **C)** All users can manage ProjectA resources
- [ ] **D)** Engineers can delete IAM policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy allows only members of the Engineers group to manage instance resources inside ProjectA, matching the group, action, and location.
 
 
</details>

### 12. In OCI, to whom should an IAM policy statement normally grant access?

- [ ] **A)** IAM groups
- [ ] **B)** API keys
- [ ] **C)** Subnet CIDR blocks
- [ ] **D)** User email lists

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Applying policies to groups is an IAM best practice because permissions are easier to manage as users join or leave the group.
 
 
</details>


---

### **Managing Security Operations**

### 13. What is the primary purpose of Oracle Cloud Infrastructure (OCI) Security Services?

- [ ] **A)** To protect OCI resources and workloads
- [ ] **B)** To increase network latency
- [ ] **C)** To manage database indexes
- [ ] **D)** To create compute instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI Security Services exist to protect resources and workloads running in Oracle Cloud Infrastructure.
 
 
</details>

### 14. Which of the following are typical capabilities included in OCI Security Services? (Select all that apply.)

- [ ] **A)** Identity and access management
- [ ] **B)** Threat monitoring and detection
- [ ] **C)** Encryption and key management
- [ ] **D)** Predictive data mining

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> OCI Security Services include identity and access management, threat monitoring, and encryption and key management. Predictive data mining is not a core security service capability.
 
 
</details>

### 15. Complete the list of OCI security services by selecting the missing element.

```python
security_services = ["IAM", "Cloud Guard", "Security Zones", "____"]
```

- [ ] **A)** Vulnerability Scanning Service
- [ ] **B)** Load Balancer
- [ ] **C)** Autonomous Database
- [ ] **D)** Object Storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Vulnerability Scanning Service is a recognized OCI security service that helps identify security vulnerabilities in cloud resources.
 
 
</details>


---

### **Network, Platform, and Infrastructure Security**

### 16. Which statement accurately describes a Network Security Group (NSG) in Oracle Cloud Infrastructure?

- [ ] **A)** Virtual firewall for a set of VNICs
- [ ] **B)** Physical appliance in the data center
- [ ] **C)** DNS resolver for all OCI domains
- [ ] **D)** Backup scheduler for block volumes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An NSG is a virtual firewall applied to selected VNICs, providing stateful security rules for the associated resources in a VCN.
 
 
</details>

### 17. Which statements about OCI Security Lists and Network Security Groups are true?

- [ ] **A)** Security Lists apply to all VNICs in the associated subnet.
- [ ] **B)** NSGs can be scoped to one resource or a selected group of VNICs.
- [ ] **C)** Security Lists replace the IAM policy engine.
- [ ] **D)** NSGs block outbound traffic only.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Security Lists filter traffic for every VNIC in a subnet, while NSGs provide more granular rules for specific resources or VNICs. Neither replaces OCI IAM.
 
 
</details>

### 18. After the OCI CLI command shown in the code block is executed, what type of resource is listed?

```bash
oci network nsg list --compartment-id ocid1.compartment.oc1..example --vcn-id ocid1.vcn.oc1..example
```

- [ ] **A)** Network Security Groups in the specified VCN
- [ ] **B)** Security Lists assigned to the VCN subnets
- [ ] **C)** Route tables for the VCN
- [ ] **D)** Virtual Cloud Networks in the tenancy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The oci network nsg list command lists the Network Security Groups that exist in the specified compartment and VCN.
 
 
</details>

### 19. Which OCI service continuously monitors cloud resources for misconfigurations, threats, and suspicious activity?

- [ ] **A)** Cloud Guard
- [ ] **B)** Bastion
- [ ] **C)** Vault
- [ ] **D)** Network Security Group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Guard continuously monitors OCI resources and workloads for security misconfigurations, suspicious activities, and threat indicators.
 
 
</details>

### 20. Which OCI network components can act as virtual firewalls inside a VCN?

- [ ] **A)** Security Lists
- [ ] **B)** Network Security Groups
- [ ] **C)** Internet Gateway
- [ ] **D)** Route Table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Security Lists and Network Security Groups are virtual firewall components. Route tables and internet gateways direct or extend network connectivity but do not act as firewalls.
 
 
</details>

### 21. What is the result of running the OCI CLI command shown in the code block?

```bash
oci network security-list create --compartment-id ocid1.compartment.oc1..example --vcn-id ocid1.vcn.oc1..example --display-name SecurityListProd
```

- [ ] **A)** New security list in the target VCN
- [ ] **B)** New public subnet in the target VCN
- [ ] **C)** New VCN with no subnets
- [ ] **D)** New IAM group for network administrators

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The oci network security-list create command creates a new Security List in the specified VCN and compartment.
 
 
</details>

### 22. Which OCI service provides a managed, private SSH path to compute resources that do not have public endpoints?

- [ ] **A)** Bastion service
- [ ] **B)** Vault service
- [ ] **C)** Object Storage service
- [ ] **D)** Cloud Guard

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI Bastion is a managed service that provides secure and monitored access to private compute resources without requiring a public endpoint.
 
 
</details>


---

### **Securing Applications and Data**

### 23. Which Oracle Cloud Infrastructure service controls who can sign in to and use cloud resources?

- [ ] **A)** OCI Identity and Access Management
- [ ] **B)** OCI Compute
- [ ] **C)** OCI Object Storage
- [ ] **D)** OCI Virtual Cloud Network

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI IAM manages users, groups, and policies and defines who can access OCI resources and how.
 
 
</details>

### 24. Which two options are core OCI Identity and Access Management building blocks? Select two.

- [ ] **A)** IAM users
- [ ] **B)** IAM groups
- [ ] **C)** OCI Compute instances
- [ ] **D)** OCI Object Storage buckets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> IAM users and groups are basic identity constructs; compute instances and storage buckets are infrastructure resources that IAM policies protect.
 
 
</details>

### 25. An administrator runs the OCI CLI command shown in the code block. What resource is being retrieved?

```bash
oci iam user get --user-id ocid1.user.oc1..exampleuniqueid
```

- [ ] **A)** IAM user
- [ ] **B)** IAM group
- [ ] **C)** Dynamic group
- [ ] **D)** Identity provider

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses oci iam user get with a user OCID, so it retrieves details for a specific IAM user.
 
 
</details>

### 26. What is the main purpose of a security list in an OCI VCN?

- [ ] **A)** It controls network traffic at the subnet level
- [ ] **B)** It provides authentication for API access
- [ ] **C)** It encrypts data at rest
- [ ] **D)** It manages IAM user passwords

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A security list applies allow and deny rules to network traffic entering and leaving subnets.
 
 
</details>

### 27. Which two services help detect security threats and vulnerabilities across OCI? Select two.

- [ ] **A)** OCI Cloud Guard
- [ ] **B)** OCI Vulnerability Scanning Service
- [ ] **C)** OCI Compute
- [ ] **D)** OCI Object Storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Cloud Guard detects risky configurations, and Vulnerability Scanning Service reports vulnerabilities in hosts and containers.
 
 
</details>

### 28. The OCI CLI command in the code block requests a key operation on a customer-managed key. What is the operation?

```bash
oci kms crypto encrypt --key-id ocid1.key.oc1..exampleuniqueid --plaintext 'dG8tYmUtZW5jcnlwdGVk' --endpoint https://example-crypto-endpoint
```

- [ ] **A)** Encrypt
- [ ] **B)** Decrypt
- [ ] **C)** Generate a data encryption key
- [ ] **D)** Create a vault

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The oci kms crypto encrypt command encrypts the supplied plaintext with a customer-managed key in OCI Vault.
 
 
</details>


---

### **Understanding OCI Security Services**

### 29. Which Oracle Cloud Infrastructure (OCI) service centrally manages users, groups, and authorization rules?

- [ ] **A)** OCI Identity and Access Management (IAM)
- [ ] **B)** OCI Vault
- [ ] **C)** OCI Cloud Guard
- [ ] **D)** OCI Security Zones

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI Identity and Access Management (IAM) is the central service for managing identities, groups, roles, and policies.
 
 
</details>

### 30. Which of the following are OCI services that provide security capabilities? Select all that apply.

- [ ] **A)** Cloud Guard
- [ ] **B)** Vault
- [ ] **C)** Security Zones
- [ ] **D)** OCI Object Storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Cloud Guard, Vault, and Security Zones represent OCI security services. Object Storage is a storage service, although it supports encryption.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/ISC2/Certified%20Cloud%20Security%20Professional%20(CCSP)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>ISC2 CCSP</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Cloud Application Security](#cloud-application-security) (5 questions)
- [Cloud Concepts, Architecture and Design](#cloud-concepts-architecture-and-design) (5 questions)
- [Cloud Data Security](#cloud-data-security) (6 questions)
- [Cloud Platform and Infrastructure Security](#cloud-platform-and-infrastructure-security) (5 questions)
- [Cloud Security Operations](#cloud-security-operations) (5 questions)
- [Legal, Risk and Compliance](#legal-risk-and-compliance) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-11T02:42:06.416Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Cloud Application Security | 5 |
| Cloud Concepts, Architecture and Design | 5 |
| Cloud Data Security | 6 |
| Cloud Platform and Infrastructure Security | 5 |
| Cloud Security Operations | 5 |
| Legal, Risk and Compliance | 4 |

---

### **Cloud Application Security**

### 1. What does a secure software development lifecycle embed into every phase of the software engineering process?

- [ ] **A)** Security activities and checkpoints
- [ ] **B)** Network firewalls only
- [ ] **C)** Final penetration tests
- [ ] **D)** Compliance audits only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SSDLC embeds security activities and checkpoints into every phase, shifting security left and making it continuous rather than an isolated add-on.
 
 
</details>

### 2. Which are recognized benefits of shifting security left in the secure software development lifecycle for cloud application delivery?

- [ ] **A)** Lower cost of remediation
- [ ] **B)** Earlier vulnerability identification
- [ ] **C)** Eliminates the need for runtime monitoring
- [ ] **D)** Continuous security feedback

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Early security reduces cost, finds flaws sooner, and creates continuous feedback. Runtime monitoring remains necessary for defense-in-depth.
 
 
</details>

### 3. Review the pipeline declaration in the code block. Which security testing tool is executed during the Commit stage?

```groovy
pipeline {
    agent any
    stages {
        stage('Commit') {
            steps { runSastScan() }
        }
        stage('Build') {
            steps { buildImage() }
        }
    }
}
```

- [ ] **A)** SAST
- [ ] **B)** DAST
- [ ] **C)** RASP
- [ ] **D)** WAF

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SAST runs on committed source code before compilation, providing fast feedback on static vulnerabilities in the CI pipeline.
 
 
</details>

### 4. What does static application security testing (SAST) analyze without executing the application?

- [ ] **A)** Source code and binaries
- [ ] **B)** Live network traffic
- [ ] **C)** Runtime user sessions
- [ ] **D)** Production log files

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SAST is a white-box technique that inspects source, bytecode, or binary artifacts without executing the application.
 
 
</details>

### 5. Which components are foundational elements of secure application design for cloud-native architectures?

- [ ] **A)** Identity-centric access controls
- [ ] **B)** Data classification and encryption
- [ ] **C)** A single edge firewall
- [ ] **D)** Threat modeling with STRIDE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Secure cloud design includes identity, data protection, and threat modeling. A single edge firewall is insufficient because cloud architecture assumes no trusted network.
 
 
</details>


---

### **Cloud Concepts, Architecture and Design**

### 6. According to NIST SP 800-145, what is the definition of cloud computing?

- [ ] **A)** On-demand access to shared configurable resources
- [ ] **B)** Virtualized servers in a data center
- [ ] **C)** Outsourced IT infrastructure with fixed capacity
- [ ] **D)** Pay-per-use billing for hosted services

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NIST defines cloud computing as a model for enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable computing resources.
 
 
</details>

### 7. Which two are essential characteristics of cloud computing per NIST?

- [ ] **A)** Rapid elasticity
- [ ] **B)** Measured service
- [ ] **C)** Multi-tenancy
- [ ] **D)** Hybrid deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Rapid elasticity and measured service are NIST essential characteristics; multi-tenancy and hybrid deployment are not listed as essential characteristics.
 
 
</details>

### 8. Based on the provisioning configuration shown, which essential characteristic is not satisfied?

```json
{
  "provision": "requires helpdesk ticket",
  "network_access": "HTTPS and SSH",
  "tenancy": "multi-tenant",
  "scaling": "automatic",
  "metering": "enabled"
}
```

- [ ] **A)** On-demand self-service
- [ ] **B)** Broad network access
- [ ] **C)** Resource pooling
- [ ] **D)** Rapid elasticity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Requiring a helpdesk ticket means the consumer cannot provision without human interaction, so on-demand self-service is not met.
 
 
</details>

### 9. What does on-demand self-service allow a cloud consumer to do?

- [ ] **A)** Provision resources without provider interaction
- [ ] **B)** Access resources through any proprietary protocol
- [ ] **C)** Reserve dedicated physical servers
- [ ] **D)** Eliminate all identity controls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> On-demand self-service lets consumers unilaterally provision computing capabilities without human interaction with the provider.
 
 
</details>

### 10. Which two statements describe rapid elasticity?

- [ ] **A)** Scales outward and inward automatically
- [ ] **B)** Resources may appear unlimited
- [ ] **C)** Requires manual capacity planning
- [ ] **D)** Provides fixed, non-reversible capacity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Rapid elasticity means automatic, reversible scaling and resources often appear unlimited to the consumer.
 
 
</details>


---

### **Cloud Data Security**

### 11. During which cloud data lifecycle phase must data classification and labeling be performed to enable later security controls?

- [ ] **A)** Data creation
- [ ] **B)** Data archival
- [ ] **C)** Data destruction
- [ ] **D)** Data sharing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Classification and labeling are applied when data is created because later retention, encryption, and access policies depend on these initial attributes.
 
 
</details>

### 12. Which techniques are commonly used to implement data dispersion in cloud storage? Select all that apply.

- [ ] **A)** Erasure coding
- [ ] **B)** Sharding
- [ ] **C)** Cryptographic splitting
- [ ] **D)** Identical replication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Data dispersion uses erasure coding, sharding, or cryptographic splitting to distribute fragments so a single fragment reveals no usable information.
 
 
</details>

### 13. Refer to the provided JSON snippet. Which cloud data lifecycle phase does this event represent?

```json
{
  "event": "file_upload",
  "object": "financial_report.xlsx",
  "metadata": {
    "classification": "Confidential",
    "owner": "finance"
  }
}
```

- [ ] **A)** Data creation
- [ ] **B)** Data storage
- [ ] **C)** Data sharing
- [ ] **D)** Data archival

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet shows a file upload event with classification metadata, which corresponds to data creation and classification in the lifecycle.
 
 
</details>

### 14. Which primary control is typically applied to protect data during the cloud storage phase?

- [ ] **A)** Encryption at rest
- [ ] **B)** Data masking on query
- [ ] **C)** DLP inline scanning
- [ ] **D)** Legal hold suspension

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The storage phase focuses on persisted data, so encryption at rest is the primary control; masking and DLP apply during use or sharing.
 
 
</details>

### 15. Which controls should be implemented during the data sharing phase to prevent unauthorized exposure? Select all that apply.

- [ ] **A)** Data loss prevention scanning
- [ ] **B)** Access revocation capability
- [ ] **C)** Shared link expiry policies
- [ ] **D)** Erasure coding on every object

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Sharing requires DLP scanning, access revocation, and expiry policies. Dispersion is a storage architecture control, not a sharing control.
 
 
</details>

### 16. Based on the JSON snippet, how many fragments are required to reconstruct the original data?

```json
{
  "algorithm": "Reed-Solomon",
  "fragments": 6,
  "reconstruction_threshold": 4
}
```

- [ ] **A)** 4
- [ ] **B)** 6
- [ ] **C)** 2
- [ ] **D)** 10

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The reconstruction_threshold value of 4 means any four of the six fragments can rebuild the original data.
 
 
</details>


---

### **Cloud Platform and Infrastructure Security**

### 17. In the shared responsibility model for a public cloud IaaS environment, which party is responsible for installing and managing biometric access controls at the data center?

- [ ] **A)** Cloud service provider
- [ ] **B)** Cloud customer
- [ ] **C)** Customer and provider jointly
- [ ] **D)** Facility landlord

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CSP owns physical data center security, including biometric access controls. The customer's responsibilities begin above the hypervisor and virtual network layers.
 
 
</details>

### 18. Which tasks are typically customer responsibilities in an IaaS deployment? Select all that apply.

- [ ] **A)** Patching guest operating systems
- [ ] **B)** Configuring virtual network firewall rules
- [ ] **C)** Managing application-level identity and access
- [ ] **D)** Hardening the hypervisor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> In IaaS, the customer patches guest OSes, configures virtual network security, and manages application access. The CSP hardens the hypervisor and physical infrastructure.
 
 
</details>

### 19. Review the code block. Which hypervisor type is being configured?

```python
# Cloud hypervisor configuration
hypervisor.mode = "native"
hypervisor.host_os = "none"
hypervisor.start()
```

- [ ] **A)** Type 1 native hypervisor
- [ ] **B)** Type 2 hosted hypervisor
- [ ] **C)** Container runtime
- [ ] **D)** Application-based emulator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A hypervisor that runs directly on host hardware without a host operating system is a Type 1 native hypervisor, the standard for production cloud environments.
 
 
</details>

### 20. In a cloud environment, who retains ultimate accountability for the protection of customer data, even when a CSP provides physical and virtualization security?

- [ ] **A)** Cloud customer
- [ ] **B)** Cloud service provider
- [ ] **C)** Both parties equally
- [ ] **D)** Regulatory authority

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Accountability for customer data cannot be delegated. The CSP operates controls, but the customer retains ultimate accountability for data protection.
 
 
</details>

### 21. Which controls are physical environmental controls in a cloud data center? Select all that apply.

- [ ] **A)** Video surveillance cameras
- [ ] **B)** Biometric access readers
- [ ] **C)** Mantrap entry vestibules
- [ ] **D)** Virtual private cloud subnets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Cameras, biometric readers, and mantraps are physical access and monitoring controls. VPC subnets are logical network constructs, not physical controls.
 
 
</details>


---

### **Cloud Security Operations**

### 22. Under the shared responsibility model for IaaS, who normally patches the guest operating system and applications on a VM?

- [ ] **A)** The cloud customer
- [ ] **B)** The cloud provider
- [ ] **C)** Both parties equally
- [ ] **D)** The software vendor only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In IaaS, the provider secures the physical host and hypervisor, but the customer manages the guest OS and applications.
 
 
</details>

### 23. Which two options are logical infrastructure components in cloud computing?

- [ ] **A)** Virtual networks
- [ ] **B)** Containers
- [ ] **C)** Server racks
- [ ] **D)** Power and cooling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Logical infrastructure includes virtual networks, containers, VMs, and identity resources, while racks and cooling are physical.
 
 
</details>

### 24. Examine the provided code snippet. What type of cloud resource is being defined?

```hcl
resource "aws_instance" "web" {
  ami           = "ami-0abcdef1234567890"
  instance_type = "t3.micro"
  tags = {
    Name = "web-server"
  }
}

```

- [ ] **A)** Virtual machine
- [ ] **B)** Storage bucket
- [ ] **C)** IAM role
- [ ] **D)** Load balancer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Terraform snippet defines an AWS EC2 instance, which is a virtual machine in the cloud.
 
 
</details>

### 25. What is the primary purpose of establishing a secure baseline configuration for cloud components?

- [ ] **A)** Consistency and reduced configuration drift
- [ ] **B)** Increased network bandwidth
- [ ] **C)** Elimination of all security monitoring
- [ ] **D)** Automatic removal of audit logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Secure baselines ensure every component is deployed consistently and prevent configuration drift that can introduce vulnerabilities.
 
 
</details>

### 26. Which two processes are essential for maintaining cloud physical and logical infrastructure?

- [ ] **A)** Change management and version control
- [ ] **B)** Patch and vulnerability management
- [ ] **C)** Disabling all security logging
- [ ] **D)** Removing network security groups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Change management and patch management are core maintenance processes that prevent and remediate security issues.
 
 
</details>


---

### **Legal, Risk and Compliance**

### 27. What does data sovereignty mean?

- [ ] **A)** Laws of the residence country
- [ ] **B)** Customer's home-country laws
- [ ] **C)** Only data owner access
- [ ] **D)** Provider's contract terms

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Data sovereignty means stored data is subject to the laws of the country where it physically resides, linking location with legal authority.
 
 
</details>

### 28. Which two mechanisms are recognized EU cross-border data transfer mechanisms?

- [ ] **A)** Standard Contractual Clauses
- [ ] **B)** Binding Corporate Rules
- [ ] **C)** US Privacy Shield
- [ ] **D)** Verbal consent

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SCCs and BCRs are recognized GDPR transfer mechanisms; the Privacy Shield is no longer valid, and verbal consent does not satisfy transfer requirements.
 
 
</details>

### 29. Review the clause in the code block. Which concept does it best illustrate?

```plaintext
Data will be stored only in the European Union region. Customer acknowledges that storage location does not change the legal jurisdiction to which data is subject.
```

- [ ] **A)** Data sovereignty
- [ ] **B)** Data minimization
- [ ] **C)** Breach notification
- [ ] **D)** Vendor lock-in

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The clause says storage location does not change the legal jurisdiction applying to data, which is the core concept of data sovereignty.
 
 
</details>

### 30. Under GDPR, who must evaluate a data subject's deletion request?

- [ ] **A)** Data controller
- [ ] **B)** Cloud provider
- [ ] **C)** Sub-processor
- [ ] **D)** DPO only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> GDPR data subject rights are exercised against the controller, who evaluates the request; the processor must follow the controller's instructions.
 
 
</details>

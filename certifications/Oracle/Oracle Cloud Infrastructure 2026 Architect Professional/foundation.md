<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Oracle%20Cloud%20Infrastructure%202026%20Architect%20Professional.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Oracle Cloud Infrastructure 2026 Architect Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Cloud-Native Solutions](#cloud-native-solutions) (5 questions)
- [Databases and Storage Operations](#databases-and-storage-operations) (4 questions)
- [High Availability and Disaster Recovery](#high-availability-and-disaster-recovery) (6 questions)
- [Hybrid, Multicloud, and Migration](#hybrid-multicloud-and-migration) (4 questions)
- [Observability and Management](#observability-and-management) (3 questions)
- [Security](#security) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:46:00.323Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Cloud-Native Solutions | 5 |
| Databases and Storage Operations | 4 |
| High Availability and Disaster Recovery | 6 |
| Hybrid, Multicloud, and Migration | 4 |
| Observability and Management | 3 |
| Security | 8 |

---

### **Cloud-Native Solutions**

### 1. What is Oracle Cloud Guard's primary function?

- [ ] **A)** Configuration and activity monitor
- [ ] **B)** Web application firewall
- [ ] **C)** Network firewall service
- [ ] **D)** Identity policy manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Guard is a configuration and activity monitor, not a firewall or WAF.
 
 
</details>

### 2. Which two statements are correct about NSGs and Security Lists?

- [ ] **A)** They are mutually exclusive.
- [ ] **B)** They are additive.
- [ ] **C)** Security Lists are applied at the subnet level.
- [ ] **D)** NSGs are applied at the subnet level.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> NSGs and Security Lists are additive. Security Lists apply to subnets, while NSG rules apply to VNICs.
 
 
</details>

### 3. The code block shows a Security Zone resource and a Cloud Guard target. What must be considered when choosing resources for a Security Zone?

```hcl
resource "oci_security_zone" "prod_zone" {
  compartment_id = "ocid1.compartment.oc1..example"
  display_name   = "prod-security-zone"
}

resource "oci_cloud_guard_target" "prod_target" {
  compartment_id      = oci_security_zone.prod_zone.compartment_id
  target_resource_type = "COMPARTMENT"
}
```

- [ ] **A)** Only a specific set of resources is supported.
- [ ] **B)** Any OCI resource can be placed in a Security Zone.
- [ ] **C)** Security Zones are attached directly to subnets.
- [ ] **D)** Security Zones replace IAM policies.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Security Zones support a specific set of resources, and not every resource can be placed inside one.
 
 
</details>

### 4. When a key is rotated in OCI Vault, what is created?

- [ ] **A)** A new key version
- [ ] **B)** Re-encryption of all existing data
- [ ] **C)** Deletion of the current key
- [ ] **D)** Creation of a new Vault

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Rotating a key in OCI Vault creates a new key version for new data encryption.
 
 
</details>

### 5. Which two practices prevent over-provisioning IAM permissions?

- [ ] **A)** Grant manage permission to every application.
- [ ] **B)** Use resource-specific permissions instead of broad manage.
- [ ] **C)** Apply least privilege to IAM grants.
- [ ] **D)** Store IAM policies inside OCI Vault.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Over-provisioning IAM permissions is risky. Resource-specific policies and least privilege reduce access risk.
 
 
</details>


---

### **Databases and Storage Operations**

### 6. According to the playbook, which of the following statements best describes the primary role of Oracle Cloud Guard in OCI security?

- [ ] **A)** A configuration and activity monitor
- [ ] **B)** A firewall that filters VCN traffic
- [ ] **C)** A Web Application Firewall for HTTP requests
- [ ] **D)** A tool that patches database systems

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Guard is a monitoring service that detects configuration risks and activity; it does not replace network-layer or application-layer protections.
 
 
</details>

### 7. According to the OCI security playbook, which of the following are common security traps that architects should avoid? Select all that apply.

- [ ] **A)** Cloud Guard can replace a WAF
- [ ] **B)** Security Zones can protect every resource
- [ ] **C)** Cloud Guard remediation is always safe
- [ ] **D)** NSGs and Security Lists are additive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The playbook calls out Cloud Guard/WAF confusion, excessive Security Zone scope, and automated remediation as traps. NSGs and Security Lists can be used together.
 
 
</details>

### 8. Review the key rotation command shown in the exhibit. Which outcome will occur after the command is successfully executed in OCI Vault?

```bash
oci kms management key rotate --key-id ocid1.key.oc1..example --compartment-id ocid1.compartment.oc1..example
```

- [ ] **A)** A new key version is created
- [ ] **B)** All encrypted data is rewritten immediately
- [ ] **C)** The existing key is deleted before rotation
- [ ] **D)** The key is replicated to another region

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Key rotation creates a new key version for future encryption and decryption operations; existing data remains usable without being rewritten.
 
 
</details>

### 9. Based on the common traps in the OCI security playbook, which statement is accurate about the resources supported by Security Zones?

- [ ] **A)** Only a specific set of supported resources
- [ ] **B)** Every OCI resource can be included
- [ ] **C)** Security Zones replace NSGs and Security Lists
- [ ] **D)** Security Zones filter web traffic at Layer 7

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Security Zones can be applied to a defined set of OCI resource types; they are not a substitute for network or web application security.
 
 
</details>


---

### **High Availability and Disaster Recovery**

### 10. What is the primary function of Oracle Cloud Infrastructure Cloud Guard when monitoring resource configuration and account activity?

- [ ] **A)** Configuration and activity monitor
- [ ] **B)** Perimeter firewall
- [ ] **C)** Web application firewall
- [ ] **D)** DDoS mitigation service

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Guard is a security posture management service that monitors resource configuration and account activity. It is not a network firewall or WAF.
 
 
</details>

### 11. Which statements are true about OCI Security Zones and their supported resource types? Select all that apply.

- [ ] **A)** Support only certain resource types
- [ ] **B)** Apply to every resource automatically
- [ ] **C)** Enforce policies on contained resources
- [ ] **D)** Act as a Cloud Guard replacement

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Security Zones include selected compartments and protect supported resources with security policies. They cannot be applied to every resource and do not replace Cloud Guard.
 
 
</details>

### 12. Review the Cloud Guard responder configuration in the code block. What should the team consider before enabling automated response in production?

```json
{
  "name": "auto-remediate-production",
  "mode": "automated",
  "isEnabled": true,
  "target": "production-compartment"
}
```

- [ ] **A)** Unexpected changes to live resources
- [ ] **B)** Improved performance for all workloads
- [ ] **C)** Permanent deletion of security policies
- [ ] **D)** Elimination of human security reviews

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Automated responder actions can modify live resources. You should validate responder rules and understand production impact before enabling automation.
 
 
</details>

### 13. In OCI Vault, what is the direct effect of rotating an encryption key instead of re-encrypting data?

- [ ] **A)** Creates a new key version
- [ ] **B)** Re-encrypts all stored objects
- [ ] **C)** Deletes the current key version
- [ ] **D)** Requires a new Vault endpoint

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Rotating a key creates another version of the key. Existing data encrypted with older versions remains readable and is not automatically re-encrypted.
 
 
</details>

### 14. Which practices help prevent over-provisioning of IAM permissions in Oracle Cloud Infrastructure? Select all that apply.

- [ ] **A)** Grant manage only when needed
- [ ] **B)** Use broad manage for every app
- [ ] **C)** Scope policies to resource types
- [ ] **D)** Assign maximum privilege roles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Avoid granting manage by default. Scope policies to required resources and lifecycles, reducing blast radius and accidental changes.
 
 
</details>

### 15. Examine the code snippet that defines a subnet security list and a VNIC NSG. How do these two constructs work together?

```yaml
# Subnet-level security list
security_list:
  ingress:
    - source: "10.0.0.0/16"

# VNIC-level network security group
nsg:
  ingress:
    - source: "192.0.2.0/24"
```

- [ ] **A)** Their rules are additive
- [ ] **B)** Only the NSG rules apply
- [ ] **C)** Only the security list rules apply
- [ ] **D)** They cannot be combined

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Security lists and NSGs are not mutually exclusive. When both apply, their security rules are evaluated together in an additive manner.
 
 
</details>


---

### **Hybrid, Multicloud, and Migration**

### 16. What is the primary role of Cloud Guard in Oracle Cloud Infrastructure?

- [ ] **A)** Monitors configuration and user activity.
- [ ] **B)** Filters traffic between subnets.
- [ ] **C)** Replaces IAM for access management.
- [ ] **D)** Encrypts data in object storage.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Guard is a security monitoring service in OCI; it detects configuration risks and activity anomalies. It is not a firewall, IAM service, or encryption service.
 
 
</details>

### 17. Which statements about OCI Security Zones and resource support are accurate?

- [ ] **A)** They can be applied to any OCI resource.
- [ ] **B)** They support a specific set of OCI resource types.
- [ ] **C)** They can be extended to non-OCI resources.
- [ ] **D)** They enforce stricter policies on the resources they support.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Security Zones are not blanket protections for all resources. They have a defined supported resource set and do not extend to non-OCI resources.
 
 
</details>

### 18. A Vault key is processed with the command in the code block. What is the effect on the key?

```shell
oci kms management key rotate --key-id ocid1.key.oc1..example --endpoint https://example.kms.us-ashburn-1.oraclecloud.com
```

- [ ] **A)** Creates a new key version for future encryption.
- [ ] **B)** Re-encrypts all data using a new key.
- [ ] **C)** Permanently deletes the old key.
- [ ] **D)** Disables the key for all future use.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI Vault key rotation creates a new key version. Existing data is not re-encrypted, and the previous key is not deleted; re-encryption is a separate operation.
 
 
</details>

### 19. An application receives the Manage permission but only needs to read objects. Why should this be corrected?

- [ ] **A)** It prevents the workload from reading objects.
- [ ] **B)** It violates least privilege and grants excessive control.
- [ ] **C)** It creates a new Vault key automatically.
- [ ] **D)** It disables encryption on the bucket.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Manage permission grants full control over the service. Read-only workloads should receive only read permissions. Over-provisioning increases risk of accidental or malicious changes.
 
 
</details>


---

### **Observability and Management**

### 20. Which statement most accurately describes Oracle Cloud Infrastructure Cloud Guard?

- [ ] **A)** A network firewall that filters traffic between VCNs.
- [ ] **B)** A configuration and activity monitor that identifies insecure configurations and suspicious activity.
- [ ] **C)** A web application firewall that protects HTTP endpoints.
- [ ] **D)** A service that stores secrets and rotates keys.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Cloud Guard is a configuration and activity monitoring service, not a firewall, WAF, or key management service.
 
 
</details>

### 21. Which two statements are true about OCI Cloud Guard and Security Zones?

- [ ] **A)** Cloud Guard is an activity and configuration monitoring service.
- [ ] **B)** A Security Zone can be applied to any OCI resource, including unsupported services.
- [ ] **C)** Enabling an automated Cloud Guard responder is always safe in production.
- [ ] **D)** A Security Zone supports only a specific set of OCI resources.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Cloud Guard monitors configuration and activity, while Security Zones support a defined set of resources. Automated remediation is not always safe in production.
 
 
</details>

### 22. The code block shows a command used by an administrator. What is the result of running this command?

```bash
oci kms management key rotate --key-id <key_ocid>
```

- [ ] **A)** It deletes the current key and all data encrypted with it.
- [ ] **B)** It re-encrypts existing ciphertext with a new cryptographic key.
- [ ] **C)** It creates a new version of the existing key for future encryption and decryption.
- [ ] **D)** It permanently disables the key for all future use.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Rotating a key in OCI Vault creates a new version of the key. It does not immediately re-encrypt existing data or delete the previous version.
 
 
</details>


---

### **Security**

### 23. Which statement best describes Oracle Cloud Infrastructure Cloud Guard?

- [ ] **A)** Monitors configuration and activity for security risks.
- [ ] **B)** Filters network traffic as a stateful firewall.
- [ ] **C)** Blocks SQL injection at the application layer.
- [ ] **D)** Provides DNS resolution for private zones.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Guard is a security monitoring service for configuration and activity. It is not a firewall, WAF, or DNS service.
 
 
</details>

### 24. Which two statements about Security Zones and supported resources are true?

- [ ] **A)** Any OCI resource can be added.
- [ ] **B)** Only specific resource types are supported.
- [ ] **C)** Every resource is in a zone by default.
- [ ] **D)** Resource type support must be verified first.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Security Zones do not apply to every OCI resource; only supported resource types can be members. Compatibility should be verified first.
 
 
</details>

### 25. A Cloud Guard responder in a production environment completes successfully. What should the security team conclude?

```json
{
  "responderExecution": {
    "autoRemediation": true,
    "executionStatus": "SUCCEEDED",
    "environment": "production"
  }
}
```

- [ ] **A)** No further action is required.
- [ ] **B)** Manual validation and monitoring are still required.
- [ ] **C)** Run the same responder in every compartment.
- [ ] **D)** Remove the responder execution rules.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Even a successful automated remediation can have unintended effects, especially in production. Review and monitor the result before closing the issue.
 
 
</details>

### 26. What occurs when an OCI Vault key is rotated?

- [ ] **A)** Old key deleted immediately after rotation.
- [ ] **B)** New key version created; old versions still available.
- [ ] **C)** All existing data is automatically re-encrypted.
- [ ] **D)** Rotation changes the key algorithm to AES.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Key rotation creates a new key version and does not replace re-encryption. Previous versions are retained so existing data can still be decrypted.
 
 
</details>

### 27. Which two actions avoid over-provisioning OCI IAM permissions?

- [ ] **A)** Grant manage access to all users.
- [ ] **B)** Grant the minimum access required.
- [ ] **C)** Add broad permissions by default.
- [ ] **D)** Group users and policies by job function.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Least privilege and job-based groups prevent over-broad grants. A default of manage-level access is an over-provisioning risk.
 
 
</details>

### 28. A compute instance is protected by both the NSG and the security list in the code block. How should their rules be applied?

```hcl
resource "oci_core_network_security_group" "web_nsg" {
  compartment_id = "ocid1.compartment.oc1.."
  vcn_id         = "ocid1.vcn.oc1.."
}

resource "oci_core_security_list" "web_subnet_sl" {
  compartment_id = "ocid1.compartment.oc1.."
  vcn_id         = "ocid1.vcn.oc1.."
}

```

- [ ] **A)** They are mutually exclusive; only one can apply.
- [ ] **B)** They are additive; both rule sets apply.
- [ ] **C)** The NSG overrides the security list.
- [ ] **D)** The security list makes the NSG unnecessary.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> NSGs and security lists are additive, not mutually exclusive. Both sets of rules can apply, so effective access is a combination.
 
 
</details>

### 29. What is the correct attachment model for network security groups and security lists?

- [ ] **A)** NSGs target subnets, security lists target VNICs.
- [ ] **B)** NSGs target VNICs, security lists target subnets.
- [ ] **C)** Both target route tables.
- [ ] **D)** Both target internet gateways.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> NSG rules are applied to VNICs while security list rules apply at the subnet level. Confusing these attachment points is common.
 
 
</details>

### 30. Which statements about NSG-to-NSG rules are correct?

- [ ] **A)** Another NSG can be a source or destination.
- [ ] **B)** References must cross to another VCN.
- [ ] **C)** NSG membership defines traffic scope in these rules.
- [ ] **D)** NSG references are disabled by default.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> An NSG rule can use another NSG as source or destination, and the referenced resources are those in that NSG. It is not restricted to a single subnet.
 
 
</details>

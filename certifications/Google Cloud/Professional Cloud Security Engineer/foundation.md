<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Google%20Cloud/Professional%20Cloud%20Security%20Engineer.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Professional Cloud Security Engineer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Configure access](#configure-access) (7 questions)
- [Ensure data protection](#ensure-data-protection) (7 questions)
- [Manage operations](#manage-operations) (5 questions)
- [Secure communications and establish boundary protection](#secure-communications-and-establish-boundary-protection) (7 questions)
- [Support compliance requirements](#support-compliance-requirements) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:52:19.252Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Configure access | 7 |
| Ensure data protection | 7 |
| Manage operations | 5 |
| Secure communications and establish boundary protection | 7 |
| Support compliance requirements | 4 |

---

### **Configure access**

### 1. Which component of an IAM policy directly associates a principal with a role?

- [ ] **A)** Policy binding
- [ ] **B)** Resource hierarchy
- [ ] **C)** Audit log
- [ ] **D)** Organization policy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An IAM policy is made of bindings; each binding associates members with a role.
 
 
</details>

### 2. Which two statements about IAM role types are correct?

- [ ] **A)** Primitive roles grant broad access across an entire project.
- [ ] **B)** Predefined roles are Google-managed and service-specific.
- [ ] **C)** Custom roles are automatically created by Google Cloud.
- [ ] **D)** Primitive roles are recommended for least privilege.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Primitive roles are broad and legacy; predefined roles are granular and Google-managed. Custom roles are user-defined.
 
 
</details>

### 3. In the policy binding represented in the code block, what kind of principal is assigned to the role?

```json
{
  "bindings": [
    {
      "role": "roles/storage.objectViewer",
      "members": ["user:alice@example.com"]
    }
  ]
}
```

- [ ] **A)** A user identity
- [ ] **B)** A service account
- [ ] **C)** A group lifecycle
- [ ] **D)** An API key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'user:' prefix indicates a Google user identity. Service accounts use 'serviceAccount:' and groups use 'group:'.
 
 
</details>

### 4. What is the default setting for Data Access audit logs for most Google Cloud services?

- [ ] **A)** They are disabled by default
- [ ] **B)** They are enabled by default
- [ ] **C)** They require no configuration
- [ ] **D)** They cannot be enabled

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Data Access logs are disabled by default for most services because of volume and cost, and must be explicitly enabled.
 
 
</details>

### 5. Which two audit log categories are associated with reading user data and explicit denial of access?

- [ ] **A)** Data Access
- [ ] **B)** Policy Deny
- [ ] **C)** Admin Activity
- [ ] **D)** System Event

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Data Access logs record read/write to user data; Policy Deny logs record explicit deny-policy blocks.
 
 
</details>

### 6. According to the constraint shown in the code block, which two outcomes will occur?

```yaml
constraint: constraints/compute.vmExternalIpAccess
listPolicy:
  allValues: DENY
```

- [ ] **A)** Compute Engine instances cannot be assigned external IP addresses.
- [ ] **B)** VMs will be denied public internet IPs.
- [ ] **C)** Service account key creation is blocked.
- [ ] **D)** All IAM policy bindings are denied.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> This list constraint denies external IPs on VMs; it does not affect service account keys or IAM bindings.
 
 
</details>

### 7. Which IAM role type is considered a legacy broad role and violates least privilege?

- [ ] **A)** Primitive roles
- [ ] **B)** Predefined roles
- [ ] **C)** Custom roles
- [ ] **D)** Conditional roles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Primitive roles Owner, Editor, and Viewer grant broad legacy access across projects, conflicting with least privilege.
 
 
</details>


---

### **Ensure data protection**

### 8. What is the main purpose of Cloud Key Management Service on Google Cloud for protecting sensitive data?

- [ ] **A)** Monitor network traffic for threats
- [ ] **B)** Manage cryptographic keys for encryption
- [ ] **C)** Store application logs for compliance
- [ ] **D)** Enforce physical data center security

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Cloud KMS is a cloud-hosted cryptographic key management service used to generate, use, rotate, and destroy keys for encrypting sensitive data.
 
 
</details>

### 9. Which key management service tiers does Google Cloud offer through Cloud KMS for encryption of sensitive data?

- [ ] **A)** Cloud External Key Manager
- [ ] **B)** Cloud Data Loss Prevention
- [ ] **C)** Cloud KMS
- [ ] **D)** Cloud HSM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Cloud KMS includes software-backed Cloud KMS, FIPS 140-2 Level 3 Cloud HSM, and Cloud EKM for externally managed keys.
 
 
</details>

### 10. An engineer runs the command shown. What is the effect of this IAM binding on the service account?

```bash
gcloud kms keys add-iam-policy-binding \
  projects/prod-project/locations/global/keyRings/app-keys/cryptoKeys/db-key \
  --member serviceAccount:app-sa@prod-project.iam.gserviceaccount.com \
  --role roles/cloudkms.cryptoKeyEncrypterDecrypter
```

- [ ] **A)** Create new key versions in the key ring
- [ ] **B)** Encrypt and decrypt data with the specified key
- [ ] **C)** Delete the key ring and all its versions
- [ ] **D)** View metadata for all keys in the project

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The roles/cloudkms.cryptoKeyEncrypterDecrypter role allows the service account to encrypt and decrypt data using the referenced crypto key.
 
 
</details>

### 11. What is a key ring in Cloud Key Management Service on Google Cloud for organizing keys?

- [ ] **A)** A hardware security module device
- [ ] **B)** A logical grouping of cryptographic keys
- [ ] **C)** A single encryption algorithm
- [ ] **D)** A type of access transparency log

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A key ring is a logical grouping of cryptographic keys that helps organize keys and assign access control policies.
 
 
</details>

### 12. Which statements accurately describe Customer-Supplied Encryption Keys (CSEK) for data protection on Google Cloud workloads?

- [ ] **A)** Google automatically rotates CSEK keys
- [ ] **B)** The customer generates and supplies the AES-256 key
- [ ] **C)** Google never stores the raw key material
- [ ] **D)** The key is transmitted with each API call

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C, D**
 
> 💡  **Explanation** 
> 
> CSEK requires the customer to supply and manage AES-256 keys. Google uses them transiently and never persists key material, and no automated rotation exists.
 
 
</details>

### 13. An engineer runs the command shown. What access does this IAM binding grant to the service account?

```bash
gcloud secrets add-iam-policy-binding projects/my-project/secrets/db-pass \
  --member serviceAccount:app@my-project.iam.gserviceaccount.com \
  --role roles/secretmanager.secretAccessor
```

- [ ] **A)** Create new secret versions
- [ ] **B)** Access secret payload values
- [ ] **C)** Delete the secret resource
- [ ] **D)** Set IAM policies on secrets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The secretAccessor role is scoped to reading the secret payload, not managing secret resources or versions.
 
 
</details>

### 14. What is the maximum payload size allowed for a Secret Manager secret version on Google Cloud?

- [ ] **A)** 10 MiB
- [ ] **B)** 64 KiB
- [ ] **C)** 128 KiB
- [ ] **D)** 1 MiB

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Secret Manager accommodates payloads up to 64 KiB per secret version.
 
 
</details>


---

### **Manage operations**

### 15. Which Cloud Audit Log category is enabled by default in Google Cloud?

- [ ] **A)** Admin Activity
- [ ] **B)** Data Access
- [ ] **C)** System Event
- [ ] **D)** Policy Denied

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Admin Activity logs are always enabled and record API calls that modify resource configuration or metadata.
 
 
</details>

### 16. Which statements accurately describe Data Access audit logs? Select all that apply.

- [ ] **A)** They are enabled by default for every Google Cloud service.
- [ ] **B)** They record API calls that create, modify, or read user-provided resource data.
- [ ] **C)** They are disabled by default for most services to control ingestion volume and cost.
- [ ] **D)** They primarily track administrative actions that modify resource configuration.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Data Access logs are off by default for most services and record reads and writes of actual resource data, not administrative configuration changes.
 
 
</details>

### 17. What does the gcloud command shown in the code block accomplish?

```bash
gcloud logging sinks create security-log-sink \
  --organization=123456789 \
  --log-filter='logName:"cloudaudit.googleapis.com/activity"' \
  --destination=bigquery.googleapis.com/projects/security-proj/datasets/audit_logs \
  --include-children
```

- [ ] **A)** Creates an organization-level aggregated sink that exports Admin Activity logs to BigQuery
- [ ] **B)** Creates a project-level sink that exports Data Access logs to Cloud Storage
- [ ] **C)** Enables Data Access logs for all child projects in the organization
- [ ] **D)** Exports Policy Denied logs to a Pub/Sub topic for real-time alerting

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses --organization and --include-children, so it creates an aggregated sink that routes Admin Activity logs to BigQuery.
 
 
</details>

### 18. Which destination is NOT supported for a Cloud Logging log sink?

- [ ] **A)** Cloud Storage bucket
- [ ] **B)** BigQuery dataset
- [ ] **C)** Pub/Sub topic
- [ ] **D)** Cloud Functions function

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> Log sinks can route to Cloud Storage, BigQuery, Pub/Sub, or external logging systems, but Cloud Functions is not a direct sink destination.
 
 
</details>

### 19. Which of the following are common traps when working with Cloud Audit Logs and log sinks? Select all that apply.

- [ ] **A)** Assuming Data Access logs are enabled by default across all services
- [ ] **B)** Configuring a project-level sink when centralized organization-wide aggregation is required
- [ ] **C)** Enabling Data Access logs for all services without considering storage costs and data volume
- [ ] **D)** Using an aggregated sink at the organization level to export security logs to a centralized project

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> These are explicitly called out as common traps; organization-level aggregation with native sinks is the recommended practice.
 
 
</details>


---

### **Secure communications and establish boundary protection**

### 20. What is the primary benefit of using Shared VPC in Google Cloud?

- [ ] **A)** Centralized network administration and shared subnets
- [ ] **B)** Independent VPC management with peering
- [ ] **C)** Public internet connectivity for private instances
- [ ] **D)** Non-transitive private connectivity between VPCs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Shared VPC centralizes network management in a host project and lets service projects use its subnets. This is the key enterprise benefit.
 
 
</details>

### 21. Which two statements correctly describe VPC Network Peering?

- [ ] **A)** Uses private internal IP addresses for communication
- [ ] **B)** Is non-transitive between peered networks
- [ ] **C)** Requires traffic to traverse the public internet
- [ ] **D)** Provides centralized billing across projects

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Peering uses internal IPs and is non-transitive, so peered networks cannot relay traffic. It does not use the internet or centralize billing.
 
 
</details>

### 22. The displayed command creates a VPC firewall rule. What is true about its evaluation order?

```bash
gcloud compute firewall-rules create allow-https --network=prod-vpc --priority=100 --allow=tcp:443 --target-tags=web
```

- [ ] **A)** Higher precedence than a priority 1000 rule
- [ ] **B)** Lower precedence than a priority 1000 rule
- [ ] **C)** Rules are evaluated alphabetically by name
- [ ] **D)** Deny rules always override allow rules

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Within Cloud VPC firewalls, lower priority values are evaluated first. A priority 100 rule takes precedence over a priority 1000 rule.
 
 
</details>

### 23. Which service allows private instances without external IP addresses to initiate outbound internet connections?

- [ ] **A)** Cloud NAT
- [ ] **B)** Cloud VPN
- [ ] **C)** VPC Network Peering
- [ ] **D)** Shared VPC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud NAT translates private source IPs and ports to external IP addresses for outbound-only traffic. It does not allow inbound connections.
 
 
</details>

### 24. Which two statements correctly describe Dedicated Interconnect?

- [ ] **A)** Direct physical connection bypassing the public internet
- [ ] **B)** Is encrypted by default without extra setup
- [ ] **C)** Requires a third-party service provider
- [ ] **D)** Can use MACsec to encrypt the physical link

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Dedicated Interconnect bypasses the internet, but encryption is not automatic. Organizations can enable MACsec at Layer 2 or IPsec at Layer 3.
 
 
</details>

### 25. Review the Cloud Armor command shown. What is the immediate effect of this rule?

```bash
gcloud compute security-policies create edge-policy && gcloud compute security-policies rules create 1000 --security-policy=edge-policy --expression="origin.ip in ['203.0.113.0/24']" --action=deny-403
```

- [ ] **A)** Blocks matching traffic with HTTP 403
- [ ] **B)** Allows all traffic to the backend
- [ ] **C)** Applies encryption to matching requests
- [ ] **D)** Redirects matching traffic to another backend

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The rule denies HTTP 403 for requests originating from 203.0.113.0/24. It is a Layer 7 Cloud Armor security policy rule.
 
 
</details>

### 26. Which Cloud DNS feature prevents cache poisoning by authenticating DNS responses?

- [ ] **A)** DNSSEC
- [ ] **B)** Cloud VPN
- [ ] **C)** Response Policy Zones
- [ ] **D)** VPC Service Controls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> DNSSEC adds cryptographic signatures to DNS records, enabling resolvers to validate authenticity and integrity and preventing poisoning.
 
 
</details>


---

### **Support compliance requirements**

### 27. According to Google Cloud's shared responsibility model, which layer of the cloud stack is managed exclusively by Google?

- [ ] **A)** Customer IAM policy configuration
- [ ] **B)** Physical data center security
- [ ] **C)** Application vulnerability management
- [ ] **D)** Virtual machine operating system patching

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Google secures the cloud, including physical data centers, hardware, software, networking, and facilities. Customers oversee data and access controls.
 
 
</details>

### 28. According to Google Cloud's shared responsibility model, which two security controls are specifically customer-managed?

- [ ] **A)** Physical security of data centers
- [ ] **B)** Data classification and identity management
- [ ] **C)** Application-level security controls
- [ ] **D)** Hypervisor maintenance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Customers handle security in the cloud, including data classification, identity management, VM patching, network configuration, and application-level controls.
 
 
</details>

### 29. A security engineer creates the following IAM resource to let a group authorize Google support access requests. Which pre-defined role is being assigned?

```hcl
resource "google_project_iam_binding" "access_approval" {
  project = "my-project"
  role    = "roles/accessapproval.approver"
  members = ["group:security-approvers@example.com"]
}
```

- [ ] **A)** roles/logging.viewer
- [ ] **B)** roles/accessapproval.viewer
- [ ] **C)** roles/accessapproval.approver
- [ ] **D)** roles/iam.securityReviewer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> roles/accessapproval.approver authorizes users to review, approve, or deny explicit Google access requests. It is assigned to designated security operations personnel for Access Approval workflows.
 
 
</details>

### 30. Which Google Cloud console interface provides customers with direct access to SOC reports and ISO certifications?

- [ ] **A)** Cloud Shell
- [ ] **B)** Security Command Center
- [ ] **C)** Cloud Logging
- [ ] **D)** Compliance Reports Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> Compliance Reports Manager is the dedicated console interface for accessing independent audit reports, certifications, and regulatory evaluations.
 
 
</details>

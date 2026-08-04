<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Amazon%20Web%20Services%20Training%20and%20Certification/AWS%20Certified%20Security%20–%20Specialty" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>AWS Certified Security – Specialty</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Data Protection](#data-protection) (6 questions)
- [Identity and Access Management](#identity-and-access-management) (6 questions)
- [Infrastructure Security](#infrastructure-security) (8 questions)
- [Security Logging and Monitoring](#security-logging-and-monitoring) (6 questions)
- [Threat Detection and Incident Response](#threat-detection-and-incident-response) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:34.129Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Data Protection | 6 |
| Identity and Access Management | 6 |
| Infrastructure Security | 8 |
| Security Logging and Monitoring | 6 |
| Threat Detection and Incident Response | 4 |

---

### **Data Protection**

### 1. Which AWS service provides fully managed key management and envelope encryption for data at rest?

- [ ] **A)** AWS CloudHSM
- [ ] **B)** AWS KMS
- [ ] **C)** AWS Secrets Manager
- [ ] **D)** AWS Certificate Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AWS KMS is the managed service for key management and envelope encryption.
 
 
</details>

### 2. Which two encryption options can be set as default encryption on an S3 bucket? (Choose two.)

- [ ] **A)** SSE-S3
- [ ] **B)** SSE-C
- [ ] **C)** SSE-KMS
- [ ] **D)** SSE-D

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> S3 default encryption supports SSE-S3 and SSE-KMS, not SSE-C.
 
 
</details>

### 3. In the KMS policy snippet, which line grants the s3 service principal permission to use the key for GenerateDataKey?

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Principal": {"Service": "s3.amazonaws.com"},
      "Action": ["kms:GenerateDataKey", "kms:Decrypt"],
      "Resource": "*"
    }
  ]
}
```

- [ ] **A)** The Effect line specifying 'Allow'
- [ ] **B)** The Principal line specifying 's3.amazonaws.com'
- [ ] **C)** The Action line containing 'kms:GenerateDataKey'
- [ ] **D)** The Resource line with '*'

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Action line specifies the permissions granted, including GenerateDataKey.
 
 
</details>

### 4. What does TLS termination at an Application Load Balancer mean?

- [ ] **A)** The load balancer forwards traffic encrypted to the backend.
- [ ] **B)** The load balancer decrypts traffic and sends plaintext to the backend.
- [ ] **C)** The backend encrypts all traffic.
- [ ] **D)** The client must provide a certificate.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> TLS termination means the ALB decrypts incoming TLS and forwards plaintext.
 
 
</details>

### 5. Which two AWS services can automatically renew public TLS certificates? (Choose two.)

- [ ] **A)** AWS Certificate Manager
- [ ] **B)** AWS CloudHSM
- [ ] **C)** AWS Private Certificate Authority
- [ ] **D)** ACM with public CA

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> ACM automatically renews public certificates and ACM PCA renews private certificates.
 
 
</details>

### 6. Examine the VPN configuration: AWS tunnel endpoint IP and pre-shared key. Which protocol is used to establish the encrypted tunnel?

```plaintext
IKEv2
```

- [ ] **A)** TLS
- [ ] **B)** IPsec
- [ ] **C)** SSH
- [ ] **D)** DTLS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Site-to-Site VPN uses IPsec with IKEv2 for encrypted tunnels.
 
 
</details>


---

### **Identity and Access Management**

### 7. Which AWS service provides short-lived credentials for IAM roles?

- [ ] **A)** AWS Security Token Service (STS)
- [ ] **B)** AWS Identity and Access Management (IAM)
- [ ] **C)** Amazon Cognito
- [ ] **D)** AWS Key Management Service (KMS)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> STS is the service that issues temporary, limited-privilege credentials for IAM roles or federated users.
 
 
</details>

### 8. Which two are benefits of using IAM roles instead of IAM users for EC2 instances?

- [ ] **A)** Automatic credential rotation
- [ ] **B)** Reduced management overhead
- [ ] **C)** Ability to assign a static public IP
- [ ] **D)** Better integration with CloudWatch logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Roles provide automatic, short-lived credentials and eliminate the need to manage and rotate access keys.
 
 
</details>

### 9. What does the following IAM trust policy allow?

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Principal": {
        "AWS": "arn:aws:iam::123456789012:user/John"
      },
      "Action": "sts:AssumeRole"
    }
  ]
}
```

- [ ] **A)** A specific IAM user (John) can assume this role.
- [ ] **B)** Any IAM user in the account can assume this role.
- [ ] **C)** The role can be assumed by any AWS service.
- [ ] **D)** John can create a new role with the same permissions.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The trust policy's Principal is an IAM user ARN, and Action is sts:AssumeRole, so only that user can assume the role.
 
 
</details>

### 10. Which IAM feature sets a maximum permissions ceiling for an IAM role?

- [ ] **A)** Permission boundary
- [ ] **B)** Service control policy (SCP)
- [ ] **C)** Trust policy
- [ ] **D)** Identity-based policy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A permission boundary is a managed policy that defines the maximum permissions an IAM entity can have.
 
 
</details>

### 11. Which two identity protocols are supported for federation with AWS IAM?

- [ ] **A)** SAML 2.0
- [ ] **B)** OpenID Connect (OIDC)
- [ ] **C)** LDAP
- [ ] **D)** RADIUS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> AWS IAM supports SAML 2.0 and OIDC as identity federation protocols to grant temporary access.
 
 
</details>

### 12. What type of access control is demonstrated by this IAM policy?

```json
{
  "Effect": "Allow",
  "Action": "ec2:*",
  "Resource": "*",
  "Condition": {
    "StringEquals": {
      "ec2:ResourceTag/Environment": "dev"
    }
  }
}
```

- [ ] **A)** Attribute-based access control (ABAC)
- [ ] **B)** Role-based access control (RBAC)
- [ ] **C)** Discretionary access control (DAC)
- [ ] **D)** Mandatory access control (MAC)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy uses a condition on resource tags (Environment=dev), which is characteristic of ABAC.
 
 
</details>


---

### **Infrastructure Security**

### 13. Which AWS service acts as a stateful virtual firewall for an EC2 instance?

- [ ] **A)** Security Group
- [ ] **B)** Network ACL
- [ ] **C)** AWS WAF
- [ ] **D)** AWS Shield

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Security Groups are stateful and act as a virtual firewall for EC2 instances, only allowing inbound and outbound traffic based on rules.
 
 
</details>

### 14. Which two statements about Network ACLs (NACLs) are correct? (Select two.)

- [ ] **A)** They are stateless and require explicit inbound and outbound rules.
- [ ] **B)** They are stateful and automatically allow return traffic.
- [ ] **C)** They support both allow and deny rules evaluated in numeric order.
- [ ] **D)** They can be attached directly to an EC2 instance.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> NACLs are stateless, operate at the subnet level, and support both allow and deny rules evaluated in numerical order (lowest first).
 
 
</details>

### 15. Review the security group inbound rule below. What access does it permit?

```plaintext
Type: Inbound
Protocol: TCP
Port Range: 22
Source: 0.0.0.0/0
```

- [ ] **A)** SSH access from any IP address
- [ ] **B)** HTTP access from any IP address
- [ ] **C)** HTTPS access from any IP address
- [ ] **D)** RDP access from any IP address

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The rule allows TCP port 22 from 0.0.0.0/0, which corresponds to SSH access from any IP.
 
 
</details>

### 16. Which AWS service is used to automatically patch EC2 instances with security updates?

- [ ] **A)** AWS Systems Manager Patch Manager
- [ ] **B)** Amazon Inspector
- [ ] **C)** AWS Config
- [ ] **D)** Amazon GuardDuty

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AWS Systems Manager Patch Manager automates the process of patching managed nodes with security and other updates.
 
 
</details>

### 17. Which two resources can Amazon Inspector scan for vulnerabilities? (Select two.)

- [ ] **A)** EC2 instances
- [ ] **B)** Container images in ECR
- [ ] **C)** RDS databases
- [ ] **D)** S3 buckets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Amazon Inspector can scan EC2 instances for OS vulnerabilities and container images in ECR for software vulnerabilities.
 
 
</details>

### 18. Given the SSM document command below, what operation will be performed on the target instances?

```json
{
  "documentName": "AWS-RunPatchBaseline",
  "parameters": {
    "operation": "Scan"
  }
}
```

- [ ] **A)** It will only report missing patches (Scan mode).
- [ ] **B)** It will apply all missing patches (Install mode).
- [ ] **C)** It will reboot the instances after patching.
- [ ] **D)** It will remove non-compliant patches.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses 'operation': 'Scan', which instructs Patch Manager to report compliance without applying patches.
 
 
</details>

### 19. Which AWS service provides a content delivery network with integrated security features like WAF and Shield?

- [ ] **A)** Amazon CloudFront
- [ ] **B)** AWS Global Accelerator
- [ ] **C)** Amazon Route 53
- [ ] **D)** AWS WAF

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Amazon CloudFront is a global content delivery network that integrates with AWS WAF and Shield for edge security.
 
 
</details>

### 20. Which two benefits does Origin Access Control (OAC) provide when used with CloudFront and S3? (Select two.)

- [ ] **A)** It allows CloudFront to securely access S3 without making the bucket public.
- [ ] **B)** It uses signed requests to authenticate CloudFront to S3.
- [ ] **C)** It enables static website hosting on S3.
- [ ] **D)** It provides automatic SSL/TLS termination at the edge.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OAC allows CloudFront to authenticate using a signed header, so the S3 bucket can remain private while still being accessed by CloudFront.
 
 
</details>


---

### **Security Logging and Monitoring**

### 21. Which AWS service provides centralized log storage and real-time metric extraction from log streams?

- [ ] **A)** AWS CloudTrail
- [ ] **B)** Amazon CloudWatch Logs
- [ ] **C)** Amazon GuardDuty
- [ ] **D)** AWS Config

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Amazon CloudWatch Logs centralizes log data and uses metric filters to extract patterns and trigger CloudWatch alarms.
 
 
</details>

### 22. Which two AWS services are directly integrated with AWS Security Hub as finding sources?

- [ ] **A)** Amazon GuardDuty
- [ ] **B)** AWS CloudTrail
- [ ] **C)** Amazon Inspector
- [ ] **D)** Amazon VPC Flow Logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> GuardDuty and Inspector generate findings that are ingested by Security Hub; CloudTrail and VPC Flow Logs are data sources for GuardDuty, not direct providers.
 
 
</details>

### 23. What CloudWatch Logs Insights query extracts ERROR messages and counts them per log stream?

```sql
fields @timestamp, @message | filter @message like /ERROR/ | stats count() by @logStream
```

- [ ] **A)** fields @timestamp, @message | filter @message like /ERROR/ | stats count() by @logStream
- [ ] **B)** fields @timestamp, @message | filter @message = 'ERROR' | stats count() by @logStream
- [ ] **C)** fields @timestamp, @message | stats count() by @logStream | filter @message like /ERROR/
- [ ] **D)** fields @timestamp, @message | filter @message != /ERROR/ | stats count() by @logStream

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The correct syntax uses 'like /ERROR/' for pattern matching and groups by @logStream. The other options have incorrect order or pattern syntax.
 
 
</details>

### 24. What VPC Flow Logs aggregation interval provides near-real-time visibility?

- [ ] **A)** 1 minute
- [ ] **B)** 5 minutes
- [ ] **C)** 10 minutes
- [ ] **D)** 15 minutes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> VPC Flow Logs support a 1-minute aggregation interval (max) for near-real-time data; default is 10 minutes.
 
 
</details>

### 25. Which two AWS services are essential for centralized logging across multiple accounts using AWS Organizations?

- [ ] **A)** AWS CloudTrail
- [ ] **B)** Amazon Security Hub
- [ ] **C)** AWS Config
- [ ] **D)** AWS Organizations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> CloudTrail delivers logs to S3; AWS Organizations provides the mechanism to create an organization trail that covers all accounts.
 
 
</details>

### 26. What Athena file format minimizes query cost and improves performance?

```sql
CREATE TABLE logs_parquet WITH (format='PARQUET') AS SELECT * FROM logs_raw;
```

- [ ] **A)** JSON
- [ ] **B)** CSV
- [ ] **C)** Parquet
- [ ] **D)** Avro

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Parquet is a columnar format that compresses data and reduces the amount scanned per query, lowering cost and speeding up performance.
 
 
</details>


---

### **Threat Detection and Incident Response**

### 27. Which CloudTrail event type captures object-level API operations like S3 GetObject?

- [ ] **A)** Management events
- [ ] **B)** Data events
- [ ] **C)** Insight events
- [ ] **D)** Control events

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Data events must be explicitly enabled in CloudTrail to capture object-level API calls such as S3 GetObject and PutObject.
 
 
</details>

### 28. Which three AWS services are primarily used for threat detection and analysis, excluding CloudTrail?

- [ ] **A)** Amazon GuardDuty
- [ ] **B)** AWS Security Hub
- [ ] **C)** Amazon Detective
- [ ] **D)** AWS CloudTrail

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> GuardDuty, Security Hub, and Detective are detection and investigation services; CloudTrail provides audit logging.
 
 
</details>

### 29. Based on the GuardDuty finding snippet provided, which finding type is detected?

```json
{
  "type": "UnauthorizedAccess:EC2/SSHBruteForce",
  "severity": 7,
  "resource": { "instanceDetails": { "instanceId": "i-1234567890abcdef0" } }
}
```

- [ ] **A)** UnauthorizedAccess:EC2/SSHBruteForce
- [ ] **B)** Backdoor:EC2/C&CActivity.B!DNS
- [ ] **C)** Recon:EC2/PortProbeUnprotected
- [ ] **D)** Persistence:IAMUser/UserPermissions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The finding type is explicitly stated in the 'type' field of the JSON as UnauthorizedAccess:EC2/SSHBruteForce.
 
 
</details>

### 30. What is the initial step in cloud incident response upon suspecting a breach?

- [ ] **A)** Isolate the compromised instance
- [ ] **B)** Preserve evidence by taking snapshots
- [ ] **C)** Notify the incident response team
- [ ] **D)** Terminate the affected resource

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Preserving evidence (e.g., EBS snapshots) is critical to avoid losing volatile data before containment actions.
 
 
</details>

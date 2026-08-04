<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Avaya/AXP%20Public%20Cloud%20Administrator" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>AXP Public Cloud Administrator</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Cloud Architecture and Design](#cloud-architecture-and-design) (8 questions)
- [Operations and Monitoring](#operations-and-monitoring) (7 questions)
- [Provisioning and Configuration](#provisioning-and-configuration) (9 questions)
- [Security and Compliance](#security-and-compliance) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:11.648Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Cloud Architecture and Design | 8 |
| Operations and Monitoring | 7 |
| Provisioning and Configuration | 9 |
| Security and Compliance | 6 |

---

### **Cloud Architecture and Design**

### 1. Which Avaya AXP component is responsible for secure SIP trunking and NAT traversal?

- [ ] **A)** AXP Core
- [ ] **B)** Avaya Aura Communication Manager
- [ ] **C)** Avaya Session Border Controller (SBC)
- [ ] **D)** Avaya Aura Media Server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The SBC secures SIP sessions, performs NAT traversal, and enforces call admission control.
 
 
</details>

### 2. Which two statements about multi-tenancy in Avaya AXP are correct? (Select two)

- [ ] **A)** A tenant can contain multiple projects
- [ ] **B)** Traffic between tenants is allowed by default
- [ ] **C)** Identity federation can be configured per tenant
- [ ] **D)** All tenants share the same media resources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Tenants can have multiple projects, and identity federation is per tenant. Traffic between tenants is blocked by default, and media resources are logically separated.
 
 
</details>

### 3. Review the following configuration snippet from an Avaya SBC. Which protocol does the highlighted line permit?

```plaintext
security-policy
 allow sip from any to any
 allow rtp from media-subnet to any

```

- [ ] **A)** SIP
- [ ] **B)** RTP
- [ ] **C)** HTTPS
- [ ] **D)** ICMP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The line 'allow sip from any to any' explicitly permits SIP traffic.
 
 
</details>

### 4. Which AWS storage service is best suited for long-term archival of Avaya call recordings?

- [ ] **A)** S3 Standard
- [ ] **B)** S3 Glacier
- [ ] **C)** Amazon EBS
- [ ] **D)** Amazon EFS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> S3 Glacier is designed for long-term archival with low cost, suitable for call recordings older than 90 days.
 
 
</details>

### 5. Which two characteristics apply to the Bring Your Own License (BYOL) model in Avaya AXP? (Select two)

- [ ] **A)** Requires existing Avaya license entitlements
- [ ] **B)** Billing is based on per-minute consumption
- [ ] **C)** Includes annual maintenance fees
- [ ] **D)** No upfront capital expense required

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> BYOL uses existing licenses and still requires maintenance fees. It is not consumption-based and involves upfront capital.
 
 
</details>

### 6. The following entry appears in the Avaya License Manager. Based on the procedure, what is the next step to apply this license to an AXP tenant?

```plaintext
License ID: 12345
Type: BYOL
Status: Active
Product: Avaya AXP Core
Quantity: 100 concurrent agents
```

- [ ] **A)** Generate a cloud activation code
- [ ] **B)** Decommission the on-premises system
- [ ] **C)** Enable PAYG billing
- [ ] **D)** Change the license type to subscription

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> After verifying the license, the administrator must generate a cloud activation code in the ALM portal, then apply it to the tenant.
 
 
</details>

### 7. In which Avaya AXP deployment model does the customer have full control over the underlying virtual machines?

- [ ] **A)** Public Cloud (SaaS)
- [ ] **B)** Private Cloud (IaaS)
- [ ] **C)** Hybrid Cloud
- [ ] **D)** Multi-Cloud

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In Private Cloud (IaaS), the customer controls VMs, networking, and OS. Public cloud is managed by Avaya.
 
 
</details>

### 8. Which two advantages does Direct Connect offer over a Site-to-Site VPN for Avaya workloads? (Select two)

- [ ] **A)** Lower and consistent latency
- [ ] **B)** Lower monthly cost
- [ ] **C)** Dedicated bandwidth with no internet variability
- [ ] **D)** Faster provisioning time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Direct Connect provides dedicated, low-latency connectivity. VPN is cheaper but has variable performance and slower provisioning.
 
 
</details>


---

### **Operations and Monitoring**

### 9. What does a CloudWatch Alarm evaluate to trigger an action?

- [ ] **A)** CloudWatch Metric
- [ ] **B)** CloudWatch Alarm
- [ ] **C)** CloudWatch Logs
- [ ] **D)** AWS Config Rule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> CloudWatch Alarms evaluate metric thresholds and trigger actions like SNS notifications or Lambda functions.
 
 
</details>

### 10. Which two are key metrics for AXP-specific monitoring beyond CPU? (Choose two.)

- [ ] **A)** CallAttemptCount
- [ ] **B)** MediaQualityScore
- [ ] **C)** NetworkIn
- [ ] **D)** CPUUtilization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CallAttemptCount and MediaQualityScore are custom AXP metrics; NetworkIn and CPU are general infrastructure metrics.
 
 
</details>

### 11. Examine the CloudWatch Logs Insights query. What operation does the filter perform?

```cloudwatch-logs-insights
filter @logStream like /media-/ | fields @timestamp, @message | filter @message like /(ERROR|CRITICAL)/ | sort @timestamp desc
```

- [ ] **A)** It filters logs with ERROR or CRITICAL level
- [ ] **B)** It counts all log entries
- [ ] **C)** It sorts logs by session ID
- [ ] **D)** It limits results to the last 5 minutes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The filter `@message like /(ERROR|CRITICAL)/` selects only log entries containing those severity levels.
 
 
</details>

### 12. Which pricing model offers the highest discount for steady-state AXP workloads?

- [ ] **A)** On-Demand
- [ ] **B)** Reserved Instances
- [ ] **C)** Spot Instances
- [ ] **D)** Savings Plans

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Reserved Instances with 1- or 3-year terms can reduce costs by up to 72% for steady-state workloads.
 
 
</details>

### 13. Which two are required for routine maintenance of Avaya cloud solutions? (Choose two.)

- [ ] **A)** Applying security patches
- [ ] **B)** Rotating TLS certificates
- [ ] **C)** Updating agent software on endpoints
- [ ] **D)** Replacing hypervisor firmware

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Patch management and certificate rotation are cloud-side tasks; endpoint agent updates are client-side; hypervisor is provider's responsibility.
 
 
</details>

### 14. This AWS CLI command creates a resource for cost management. What kind of resource is it?

```bash
aws budgets create-budget --account-id 123456789012 --budget file://budget.json --notifications-with-subscribers file://subscribers.json
```

- [ ] **A)** A budget with an alert
- [ ] **B)** A CloudWatch alarm
- [ ] **C)** A cost allocation tag
- [ ] **D)** An S3 bucket for logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The `aws budgets create-budget` command creates a budget; `NotificationThreshold` sets the alert trigger.
 
 
</details>

### 15. What is the purpose of cross-region snapshot copy for Avaya disaster recovery?

- [ ] **A)** Reduce recovery time objective (RTO)
- [ ] **B)** Protect against a regional cloud failure
- [ ] **C)** Lower storage costs
- [ ] **D)** Comply with license terms

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Cross-region copies ensure backups survive a full region outage, which is critical for disaster recovery.
 
 
</details>


---

### **Provisioning and Configuration**

### 16. Which AWS instance family is recommended for Avaya AXP Media Servers handling heavy transcoding?

- [ ] **A)** T2
- [ ] **B)** C5
- [ ] **C)** R5
- [ ] **D)** M5

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Compute-optimized instances like C5 provide high network throughput and CPU performance required for media transcoding.
 
 
</details>

### 17. Which of the following correctly describes security groups in AWS? (Choose two.)

- [ ] **A)** Stateful
- [ ] **B)** Stateless
- [ ] **C)** Apply at subnet level
- [ ] **D)** Apply at instance level

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Security groups are stateful and apply to instances (or ENIs), not subnets.
 
 
</details>

### 18. Review the IAM trust policy snippet. Which element must be added to prevent the confused deputy problem?

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Principal": {
        "AWS": "arn:aws:iam::123456789012:role/AxpService"
      },
      "Action": "sts:AssumeRole",
      "Condition": {}
    }
  ]
}
```

- [ ] **A)** ExternalId
- [ ] **B)** SourceIp
- [ ] **C)** MfaAuth
- [ ] **D)** ResourceArn

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An external ID is required to prevent the confused deputy problem in cross-account role assumption.
 
 
</details>

### 19. Which deployment strategy involves maintaining two identical environments and switching traffic between them?

- [ ] **A)** Rolling update
- [ ] **B)** Blue-green
- [ ] **C)** Canary
- [ ] **D)** In-place

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Blue-green deployment uses two environments (blue=current, green=updated) and switches traffic after validation.
 
 
</details>

### 20. Which tools can be used for Infrastructure as Code to provision AXP cloud resources? (Choose two.)

- [ ] **A)** Ansible
- [ ] **B)** CloudFormation
- [ ] **C)** ARM templates
- [ ] **D)** AWS CLI

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> CloudFormation (AWS) and ARM templates (Azure) are declarative IaC tools for provisioning resources.
 
 
</details>

### 21. Based on the security group rule snippet, what Avaya protocol is permitted?

```json
{
  "IpProtocol": "tcp",
  "FromPort": 5061,
  "ToPort": 5061,
  "IpRanges": [
    {
      "CidrIp": "10.0.0.0/8"
    }
  ]
}
```

- [ ] **A)** SIP over TLS
- [ ] **B)** RTP
- [ ] **C)** HTTPS
- [ ] **D)** SSH

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Port 5061 is used for SIP over TLS (SIP-TLS).
 
 
</details>

### 22. Which protocol uses XML-based assertions for identity federation in Avaya AXP?

- [ ] **A)** OIDC
- [ ] **B)** SAML 2.0
- [ ] **C)** LDAP
- [ ] **D)** OAuth

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SAML 2.0 uses XML assertions for federated authentication.
 
 
</details>

### 23. Which steps should be taken before applying an AXP update in the cloud? (Choose two.)

- [ ] **A)** Take snapshots of all instances
- [ ] **B)** Apply patch immediately
- [ ] **C)** Back up tenant configurations
- [ ] **D)** Disable all health checks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Backups and snapshots ensure recoverability; tenant configurations must be backed up separately.
 
 
</details>

### 24. What is the purpose of 'changed_when: false' in the Ansible task?

```yaml
---
- name: Deploy config
  copy:
    src: /configs/axp.yml
    dest: /etc/axp/axp.yml
  changed_when: false
```

- [ ] **A)** Force the task to always report changed
- [ ] **B)** Prevent the task from reporting changes
- [ ] **C)** Only run the task when file changes
- [ ] **D)** Ensure idempotency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> changed_when: false makes the task always report 'ok' rather than 'changed', useful for tasks that might not be idempotent.
 
 
</details>


---

### **Security and Compliance**

### 25. What is the key difference between a Security Group and a Network ACL?

- [ ] **A)** SGs are stateful; NACLs are stateless
- [ ] **B)** SGs are stateless; NACLs are stateful
- [ ] **C)** Both are stateful
- [ ] **D)** Both are stateless

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Security Groups automatically allow return traffic (stateful), while NACLs require explicit rules in both directions (stateless).
 
 
</details>

### 26. Which two protocols are used to encrypt signaling and media in Avaya AXP?

- [ ] **A)** TLS
- [ ] **B)** SRTP
- [ ] **C)** SSH
- [ ] **D)** SSL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SIP signaling is encrypted using TLS, while media streams are encrypted using SRTP. SSH is for management, and SSL is outdated.
 
 
</details>

### 27. Examine the CloudTrail configuration below. Which compliance requirement does it address?

```json
{
  "enableLogFileValidation": true,
  "s3BucketName": "avaya-logs",
  "includeGlobalServiceEvents": true,
  "isMultiRegionTrail": true
}
```

- [ ] **A)** PCI-DSS Requirement 10.5 (log integrity)
- [ ] **B)** HIPAA 164.312(b) (audit controls)
- [ ] **C)** GDPR Article 30 (records of processing)
- [ ] **D)** SOC 2 CC6.1 (logical and physical access)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Log file validation ensures tamper-proof logs, directly addressing PCI-DSS Requirement 10.5 for integrity of audit trails.
 
 
</details>

### 28. What is the purpose of a permission boundary in cloud IAM for Avaya AXP?

- [ ] **A)** Sets the maximum permissions a role can have
- [ ] **B)** Allows all actions for the role
- [ ] **C)** Replaces the need for an IAM policy
- [ ] **D)** Grants full admin access to the role

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A permission boundary defines the upper limit of permissions an IAM entity can have, preventing privilege escalation.
 
 
</details>

### 29. Which two actions must be taken to ensure CloudTrail logs are tamper-proof?

- [ ] **A)** Enable log file validation
- [ ] **B)** Encrypt logs with KMS CMK
- [ ] **C)** Enable multi-region trail
- [ ] **D)** Use default S3 encryption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Log file validation generates digests for integrity verification, and KMS encryption protects against unauthorized access and tampering.
 
 
</details>

### 30. Review the IAM policy below. Which principle does it implement for Avaya AXP tenant isolation?

```json
{
  "Version": "2012-10-17",
  "Statement": [{
    "Effect": "Allow",
    "Action": ["avaya-axp:*"],
    "Resource": "*",
    "Condition": {
      "StringEquals": {
        "aws:ResourceTag/axp-tenant-id": "Gamma"
      }
    }
  }]
}
```

- [ ] **A)** Attribute-Based Access Control (ABAC) with tags
- [ ] **B)** Role-Based Access Control (RBAC) with groups
- [ ] **C)** Implicit allow, explicit deny
- [ ] **D)** Resource-based policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy uses a condition on the resource tag 'axp-tenant-id' to enforce tenant-specific access, which is ABAC.
 
 
</details>

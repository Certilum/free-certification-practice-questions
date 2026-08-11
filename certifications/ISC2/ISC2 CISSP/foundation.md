<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/ISC2/Certified%20Information%20Systems%20Security%20Professional%20(CISSP)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>ISC2 CISSP</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Asset Security](#asset-security) (3 questions)
- [Communication and Network Security](#communication-and-network-security) (4 questions)
- [Identity and Access Management (IAM)](#identity-and-access-management-iam) (4 questions)
- [Security Architecture and Engineering](#security-architecture-and-engineering) (4 questions)
- [Security Assessment and Testing](#security-assessment-and-testing) (3 questions)
- [Security Operations](#security-operations) (4 questions)
- [Security and Risk Management](#security-and-risk-management) (5 questions)
- [Software Development Security](#software-development-security) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-11T02:42:11.849Z |
| Domains | 8 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Asset Security | 3 |
| Communication and Network Security | 4 |
| Identity and Access Management (IAM) | 4 |
| Security Architecture and Engineering | 4 |
| Security Assessment and Testing | 3 |
| Security Operations | 4 |
| Security and Risk Management | 5 |
| Software Development Security | 3 |

---

### **Asset Security**

### 1. Who bears ultimate accountability for the classification of an organization's information assets?

- [ ] **A)** Data owner
- [ ] **B)** Data custodian
- [ ] **C)** System administrator
- [ ] **D)** Data auditor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The data owner is the senior business leader accountable for classification and protection decisions. Custodians implement controls but do not own classification decisions.
 
 
</details>

### 2. Select the two correct statements about data ownership and custodianship.

- [ ] **A)** The data owner defines classification and access policy.
- [ ] **B)** The data custodian implements and maintains technical controls.
- [ ] **C)** The data custodian determines the final classification level.
- [ ] **D)** The system administrator is ultimately accountable for the data set.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The owner decides classification and policy; the custodian implements controls. Custodians do not classify, and administrators are not accountable owners.
 
 
</details>

### 3. Based on the record metadata shown in the code block, which role should implement encryption and backup controls for this asset?

```plaintext
[Record: Customer_Report]
classification: "Confidential"
owner: "Marketing Director"
```

- [ ] **A)** Data custodian
- [ ] **B)** Data owner
- [ ] **C)** End user
- [ ] **D)** Internal auditor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The custodian executes the owner's directives by applying encryption, backups, and access controls. The owner remains accountable and sets the label.
 
 
</details>


---

### **Communication and Network Security**

### 4. Which protocol is the secure replacement for Telnet for remote administration?

- [ ] **A)** SSH
- [ ] **B)** FTP
- [ ] **C)** HTTP
- [ ] **D)** SNMPv2c

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Telnet sends data in cleartext. SSH encrypts remote administration sessions and is the secure alternative.
 
 
</details>

### 5. Which of the following are secure design principles for network protocols? Select all that apply.

- [ ] **A)** Defense in depth with layered security controls
- [ ] **B)** Disabling unneeded protocols, ports, and services
- [ ] **C)** Fail-safe defaults that deny access by default
- [ ] **D)** Allowing all traffic and logging anomalies for later review

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Secure design combines layered defense, least privilege, and fail-safe defaults. Allowing all traffic and logging anomalies violates these principles.
 
 
</details>

### 6. Refer to the enabled_protocols list in the code block. Which protocols are insecure and should be disabled under least privilege? Select all that apply.

```python
enabled_protocols = ['TELNET', 'FTP', 'SNMPv3', 'HTTPS']
```

- [ ] **A)** TELNET
- [ ] **B)** FTP
- [ ] **C)** SNMPv3
- [ ] **D)** HTTPS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> TELNET and FTP transmit data and credentials in cleartext. SNMPv3 and HTTPS are modern secure protocols and should not be disabled for being insecure.
 
 
</details>

### 7. At which OSI layer does IPsec operate to secure IP communications?

- [ ] **A)** Layer 2
- [ ] **B)** Layer 3
- [ ] **C)** Layer 4
- [ ] **D)** Layer 7

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> IPsec operates at Layer 3, the network layer, protecting IP packets in transit.
 
 
</details>


---

### **Identity and Access Management (IAM)**

### 8. In access control, what is the act of a subject claiming an identity, such as presenting a username or email address?

- [ ] **A)** Identification
- [ ] **B)** Authentication
- [ ] **C)** Authorization
- [ ] **D)** Accountability

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Identification is the subject's claim of identity; authentication verifies that claim through credentials or factors.
 
 
</details>

### 9. Select all that apply. Which of the following are recognized authentication factor categories used to verify an identity claim?

- [ ] **A)** Something you know
- [ ] **B)** Something you have
- [ ] **C)** Something you are
- [ ] **D)** Something you remember

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Knowledge, possession, and inherence are factor categories; 'something you remember' is another form of knowledge, not a distinct category.
 
 
</details>

### 10. Based on the code snippet, which IAM lifecycle action is executed when a user status is terminated?

```python
if user.status == 'Terminated':
    revoke_all_access(user)
else:
    grant_default_access(user)
```

- [ ] **A)** Deprovisioning
- [ ] **B)** Provisioning
- [ ] **C)** Authentication
- [ ] **D)** Authorization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code revokes all access after termination, which is the deprovisioning stage of the identity and access lifecycle.
 
 
</details>

### 11. In the IAM model, which access control stage verifies a subject's identity claim using credentials or factors?

- [ ] **A)** Authentication
- [ ] **B)** Identification
- [ ] **C)** Authorization
- [ ] **D)** Accountability

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Authentication verifies an identity claim by requiring a credential or authentication factor, while authorization decisions happen afterward.
 
 
</details>


---

### **Security Architecture and Engineering**

### 12. Which secure design principle is characterized by deploying multiple, overlapping security controls so that failure of one layer does not compromise the entire system?

- [ ] **A)** Defense in depth
- [ ] **B)** Least privilege
- [ ] **C)** Open design
- [ ] **D)** Fail secure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Defense in depth, also called layered security, uses multiple overlapping controls so that defeating one layer does not compromise the entire system.
 
 
</details>

### 13. Which of the following are required properties of a reference monitor? (Select all that apply)

- [ ] **A)** Tamper-proof
- [ ] **B)** Always invoked
- [ ] **C)** Verifiable
- [ ] **D)** Support caching of authorization decisions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A reference monitor must be tamper-proof, always invoked, and verifiable. Caching prior decisions without rechecking violates complete mediation.
 
 
</details>

### 14. Review the pseudocode. What security model property does this access control logic enforce?

```python
def read_allowed(subject, object):
    if subject.clearance >= object.classification:
        return True
    return False

def write_allowed(subject, object):
    if subject.clearance <= object.classification:
        return True
    return False
```

- [ ] **A)** Bell-LaPadula
- [ ] **B)** Biba
- [ ] **C)** Clark-Wilson
- [ ] **D)** Brewer-Nash

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code allows read when clearance is higher and write only when classification is not lower, matching Bell-LaPadula's No Read Up and No Write Down rules.
 
 
</details>

### 15. Which security model is primarily concerned with preserving data integrity by preventing subjects from writing to higher integrity levels?

- [ ] **A)** Biba
- [ ] **B)** Bell-LaPadula
- [ ] **C)** Clark-Wilson
- [ ] **D)** Brewer-Nash

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Biba model protects integrity by preventing lower-integrity subjects from writing to higher-integrity objects, known as No Write Up.
 
 
</details>


---

### **Security Assessment and Testing**

### 16. What does a vulnerability assessment primarily do?

- [ ] **A)** Identifies and reports known weaknesses without exploitation
- [ ] **B)** Exploits weaknesses to demonstrate business impact
- [ ] **C)** Reviews documents to verify regulatory compliance
- [ ] **D)** Simulates an attacker to gain unauthorized access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A vulnerability assessment uses automated tools to identify known vulnerabilities and does not attempt exploitation. Exploitation is part of penetration testing.
 
 
</details>

### 17. Which two statements about penetration testing are correct?

- [ ] **A)** Actively exploits vulnerabilities to determine impact
- [ ] **B)** Must have signed rules of engagement before starting
- [ ] **C)** Uses automated scanning only, without manual techniques
- [ ] **D)** Is guaranteed to find every vulnerability in scope

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Penetration testing actively exploits vulnerabilities and requires signed rules of engagement. It cannot guarantee finding every vulnerability and is not limited to automated scanning.
 
 
</details>

### 18. Review the testing configuration snippet. What type of assessment is described?

```python
scan_targets = ["10.1.0.0/24"]
check_patches = True
try_exploit = False
report_severity = True
```

- [ ] **A)** Vulnerability assessment
- [ ] **B)** Penetration test
- [ ] **C)** Security audit
- [ ] **D)** Red team exercise

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet enables patch checking and severity reporting but disables exploitation, matching vulnerability assessment.
 
 
</details>


---

### **Security Operations**

### 19. When an unexpected security event is identified, which document should provide the authoritative framework for guiding the organization's response?

- [ ] **A)** Incident Response Plan
- [ ] **B)** Disaster Recovery Plan
- [ ] **C)** Business Impact Analysis
- [ ] **D)** Network diagram

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Incident Response Plan is the authoritative set of procedures for responding to unexpected security events and aligns actions with policy and risk tolerance.
 
 
</details>

### 20. Which of the following options are legitimate stages in the NIST SP 800-61 incident response process model?

- [ ] **A)** Preparation
- [ ] **B)** Containment
- [ ] **C)** Baselining
- [ ] **D)** Capacity planning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> NIST SP 800-61 defines Preparation, Detection and Analysis, Containment, Eradication, Recovery, and Post-Incident Activity; baselining and capacity planning are not process stages.
 
 
</details>

### 21. Review the severity value in the code block. Based on typical escalation principles, what action should the analyst take for this alert?

```plaintext
Alert: severity=high, source=workstation, event=multiple_failed_logins
```

- [ ] **A)** Escalate to the SOC manager
- [ ] **B)** Ignore the alert
- [ ] **C)** Delete the log
- [ ] **D)** Run a port scan

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> High-severity alerts require escalation to the appropriate level of response rather than being ignored, deleted, or investigated with unrelated tools.
 
 
</details>

### 22. In the NIST incident response process, which stage directly follows the containment stage once the threat has been isolated?

- [ ] **A)** Eradication
- [ ] **B)** Recovery
- [ ] **C)** Preparation
- [ ] **D)** Detection and Analysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The linear sequence is Preparation, Detection and Analysis, Containment, Eradication, Recovery, and Post-Incident Activity; containment precedes eradication.
 
 
</details>


---

### **Security and Risk Management**

### 23. Under security governance principles, who is ultimately accountable for an organization's security program and its outcomes?

- [ ] **A)** Board of Directors
- [ ] **B)** Chief Information Security Officer
- [ ] **C)** IT Director
- [ ] **D)** Security Steering Committee

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Ultimate accountability rests with the board of directors; accountability cannot be delegated to implementers such as the CISO.
 
 
</details>

### 24. Which of the following options are considered core components of security governance in the CISSP framework?

- [ ] **A)** Strategic alignment with business goals
- [ ] **B)** Board and senior management oversight
- [ ] **C)** Defining risk appetite
- [ ] **D)** Configuring network firewalls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Governance focuses on strategic alignment, executive oversight, and risk appetite; firewall configuration is operational management.
 
 
</details>

### 25. Review the JSON structure in the code block. Who holds the approval authority for these governance actions?

```json
{
  "decision": "Approve enterprise risk appetite",
  "document": "Information Security Policy",
  "approval_authority": "???",
  "accountability_type": "ultimate"
}
```

- [ ] **A)** Board of Directors
- [ ] **B)** Security Analyst
- [ ] **C)** Network Engineer
- [ ] **D)** Help Desk Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Board and senior management approve enterprise policies and risk appetite; staff roles implement, not approve.
 
 
</details>

### 26. Which statement most accurately distinguishes security governance from regulatory compliance in the CISSP governance framework?

- [ ] **A)** Governance includes strategic alignment; compliance is one output.
- [ ] **B)** Compliance is the ultimate goal of governance.
- [ ] **C)** Governance and compliance are identical.
- [ ] **D)** Governance is a one-time audit exercise.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Compliance is a necessary output of governance, but governance is a strategic, continuous enterprise-wide process.
 
 
</details>

### 27. Which of the following are mandatory legal or regulatory instruments in a security governance context?

- [ ] **A)** GDPR regulation
- [ ] **B)** HIPAA legislation
- [ ] **C)** ISO/IEC 27001 standard
- [ ] **D)** NIST SP 800-53 framework

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> GDPR and HIPAA are laws; ISO 27001 and NIST are voluntary frameworks unless incorporated by contracts.
 
 
</details>


---

### **Software Development Security**

### 28. What does application security in the SDLC emphasize most?

- [ ] **A)** Adding security testing only before release
- [ ] **B)** Integrating security controls and verification into every phase of development
- [ ] **C)** Deploying a web application firewall after deployment
- [ ] **D)** Outsourcing all security activities to an external vendor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Application security is a continuous, proactive effort embedded in each SDLC phase, not a final inspection or standalone tool.
 
 
</details>

### 29. Which activities are performed during the design phase of a secure SDLC? (Select all that apply)

- [ ] **A)** Threat modeling
- [ ] **B)** Applying secure design principles
- [ ] **C)** Deploying the application to production
- [ ] **D)** Executing DAST against a running instance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Threat modeling and secure design principles are performed before code is written. Deployment and DAST occur later in the lifecycle.
 
 
</details>

### 30. The code block constructs a database query by concatenating user input. Which control most effectively eliminates the injection risk?

```CHECK
CHECK
```

- [ ] **A)** Parameterized queries or prepared statements
- [ ] **B)** Blocklisting SQL keywords
- [ ] **C)** Adding a Web Application Firewall
- [ ] **D)** Encrypting the database connection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Parameterized prepared statements separate SQL code from data, preventing injection. Blacklists and firewalls can be bypassed.
 
 
</details>

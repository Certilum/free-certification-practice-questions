<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CompTIA/CompTIA%20Security%2B%20Certification" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>CompTIA Security+</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [General Security Concepts](#general-security-concepts) (4 questions)
- [Security Architecture](#security-architecture) (5 questions)
- [Security Operations](#security-operations) (8 questions)
- [Security Program Management and Oversight](#security-program-management-and-oversight) (6 questions)
- [Threats, Vulnerabilities, and Mitigations](#threats-vulnerabilities-and-mitigations) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:51:48.288Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| General Security Concepts | 4 |
| Security Architecture | 5 |
| Security Operations | 8 |
| Security Program Management and Oversight | 6 |
| Threats, Vulnerabilities, and Mitigations | 7 |

---

### **General Security Concepts**

### 1. Which security control type is specifically designed to discourage potential attackers from attempting a violation?

- [ ] **A)** Preventative
- [ ] **B)** Detective
- [ ] **C)** Deterrent
- [ ] **D)** Corrective

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Deterrent controls, such as warning banners or surveillance cameras, are designed to discourage individuals from attempting attacks or policy violations.
 
 
</details>

### 2. Which of the following are considered components of the AAA framework?

- [ ] **A)** Authentication
- [ ] **B)** Authorization
- [ ] **C)** Accounting
- [ ] **D)** Availability

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The AAA framework consists of Authentication (verifying identity), Authorization (determining access rights), and Accounting (tracking actions).
 
 
</details>

### 3. Review the following configuration and identify which security principle is being violated.

```javascript
user_account = {
  "id": "intern_01",
  "role": "intern",
  "permissions": ["read", "write", "delete", "admin_all"]
}

function perform_task(user, task) {
  if (user.permissions.includes(task)) {
    execute(task);
  }
}
```

- [ ] **A)** Confidentiality
- [ ] **B)** Integrity
- [ ] **C)** Availability
- [ ] **D)** Least Privilege

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> The code shows a user account with 'admin_all' permissions being used for a simple 'read_only' task, violating the principle of least privilege.
 
 
</details>

### 4. What is the primary purpose of a hashing algorithm in cryptography?

- [ ] **A)** Confidentiality
- [ ] **B)** Integrity
- [ ] **C)** Non-repudiation
- [ ] **D)** Availability

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Hashing is a one-way function used to ensure integrity by verifying that data has not been altered.
 
 
</details>


---

### **Security Architecture**

### 5. Which security model is based on the principle of 'never trust, always verify'?

- [ ] **A)** Defense in Depth
- [ ] **B)** Zero Trust Architecture
- [ ] **C)** Perimeter-based Security
- [ ] **D)** Implicit Trust Model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Zero Trust Architecture (ZTA) is defined by the principle of 'never trust, always verify,' eliminating implicit trust regardless of network location.
 
 
</details>

### 6. Which of the following are components of a Zero Trust Architecture?

- [ ] **A)** Identity Provider (IdP) integration
- [ ] **B)** Microsegmentation
- [ ] **C)** Implicit trust zones
- [ ] **D)** Perimeter-only firewalls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Zero Trust includes identity provider integration, microsegmentation, device health checks, and least privilege access policies.
 
 
</details>

### 7. Review the following deployment model configuration and identify the correct ownership type.

```json
{
  "device_ownership": "Organization",
  "usage_policy": "Business-only",
  "management_level": "Full lockdown"
}
```

- [ ] **A)** BYOD
- [ ] **B)** COBO
- [ ] **C)** CYOD
- [ ] **D)** COPE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> COBO (Corporate-Owned, Business-Only) is characterized by organization ownership and strict lockdown for business use only.
 
 
</details>

### 8. What is the primary goal of network segmentation?

- [ ] **A)** To increase network speed
- [ ] **B)** To limit lateral movement
- [ ] **C)** To eliminate the need for firewalls
- [ ] **D)** To provide universal access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Network segmentation aims to divide networks into zones to limit the ability of an attacker to move laterally if a host is compromised.
 
 
</details>

### 9. Which of the following are considered cloud-specific security tools?

- [ ] **A)** Cloud Security Posture Management (CSPM)
- [ ] **B)** Cloud Workload Protection Platforms (CWPP)
- [ ] **C)** Hardware Security Modules (HSM)
- [ ] **D)** Physical perimeter fences

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CSPM and CWPP are specific to cloud security architecture for managing configurations and workloads.
 
 
</details>


---

### **Security Operations**

### 10. Which phase of the incident response lifecycle involves isolating affected systems to prevent the spread of malware?

- [ ] **A)** Preparation
- [ ] **B)** Detection and Analysis
- [ ] **C)** Containment
- [ ] **D)** Eradication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Containment is the phase dedicated to isolating affected systems to prevent the lateral spread of malware or attackers.
 
 
</details>

### 11. Which of the following are considered highly volatile data types in digital forensics?

- [ ] **A)** RAM
- [ ] **B)** CPU Cache
- [ ] **C)** Hard Drive
- [ ] **D)** USB Media

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> RAM and CPU cache are highly volatile and can be lost in milliseconds when power is removed, unlike persistent storage like hard drives.
 
 
</details>

### 12. Review the following sequence of forensic actions and identify which step is missing from the standard acquisition process.

```text
1. Capture volatile RAM
2. Perform hard power-off
3. Connect drive to hardware write blocker
4. Create bit-for-bit forensic image
```

- [ ] **A)** Capture RAM
- [ ] **B)** Create Forensic Image
- [ ] **C)** Verify Hash Integrity
- [ ] **D)** Document Chain of Custody

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> After creating an image, a forensic examiner must calculate and verify hashes to ensure the integrity of the copy.
 
 
</details>

### 13. What is the primary purpose of a SIEM system in a Security Operations Center?

- [ ] **A)** Automated response execution
- [ ] **B)** Log aggregation and correlation
- [ ] **C)** Endpoint malware prevention
- [ ] **D)** Vulnerability scanning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SIEM systems perform aggregation, normalization, and correlation to transform raw logs into actionable security intelligence.
 
 
</details>

### 14. Which of the following are key responsibilities of a SOAR platform?

- [ ] **A)** Executing automated playbooks
- [ ] **B)** Integrating disparate security tools
- [ ] **C)** Storing raw log files for compliance
- [ ] **D)** Performing initial asset discovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SOAR platforms focus on orchestration (integrating tools) and automation (executing playbooks) to respond to alerts.
 
 
</details>

### 15. Based on the provided configuration, which security tool is being described?

```text
Feature: Continuous behavioral telemetry
Focus: Endpoint monitoring
Capability: Detects fileless malware and zero-day attacks
```

- [ ] **A)** SIEM
- [ ] **B)** EDR
- [ ] **C)** HIPS
- [ ] **D)** Firewall

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> EDR is characterized by continuous behavioral monitoring and telemetry recording on endpoints to detect advanced threats.
 
 
</details>

### 16. What is the main difference between a playbook and a runbook?

- [ ] **A)** Playbooks are manual; runbooks are automated
- [ ] **B)** Playbooks are automated; runbooks are manual
- [ ] **C)** Playbooks are for networks; runbooks are for endpoints
- [ ] **D)** Playbooks are for SIEM; runbooks are for SOAR

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Playbooks are automated, machine-executable workflows, whereas runbooks are manual procedural documents for analysts.
 
 
</details>

### 17. Which of the following are essential components of maintaining a proper chain of custody?

- [ ] **A)** Tamper-evident packaging
- [ ] **B)** Chronological documentation
- [ ] **C)** Immediate deletion of original files
- [ ] **D)** Using software write blockers only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Chain of custody requires chronological records of handling and secure, tamper-evident packaging to ensure evidence integrity.
 
 
</details>


---

### **Security Program Management and Oversight**

### 18. Which risk response strategy involves shifting the financial burden of a potential loss to a third party?

- [ ] **A)** Mitigation
- [ ] **B)** Avoidance
- [ ] **C)** Transference
- [ ] **D)** Acceptance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Transference involves shifting the financial consequences of a risk to a third party, such as through insurance.
 
 
</details>

### 19. Which of the following are considered mandatory organizational security documents?

- [ ] **A)** Policies
- [ ] **B)** Standards
- [ ] **C)** Guidelines
- [ ] **D)** Procedures

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Policies, standards, and procedures are mandatory. Guidelines are recommended but non-mandatory.
 
 
</details>

### 20. Match the recovery metric to its correct definition based on the provided logic.

```javascript
metric_1 = 'max_downtime_allowed';
metric_2 = 'max_data_loss_allowed';
```

- [ ] **A)** RTO = Downtime duration
- [ ] **B)** RPO = Data loss amount
- [ ] **C)** MTTR = System reliability
- [ ] **D)** MTBF = Repair time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> RTO is the time to restore operations; RPO is the maximum acceptable data loss measured in time.
 
 
</details>

### 21. What is the primary purpose of a Business Impact Analysis (BIA)?

- [ ] **A)** Identify vulnerabilities
- [ ] **B)** Determine critical functions
- [ ] **C)** Perform penetration tests
- [ ] **D)** Write security policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> BIA evaluates operational and financial consequences to identify critical functions and recovery metrics.
 
 
</details>

### 22. Which factors are used in a quantitative risk assessment?

- [ ] **A)** Single Loss Expectancy (SLE)
- [ ] **B)** Annual Rate of Occurrence (ARO)
- [ ] **C)** Expert intuition
- [ ] **D)** Subjective scales

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Quantitative assessment uses SLE and ARO to calculate ALE. Intuition and scales are qualitative.
 
 
</details>

### 23. Analyze the risk calculation logic and select the correct formula for ALE.

```javascript
function calculateALE(sle, aro) {
  return sle * aro;
}
```

- [ ] **A)** ALE = SLE * ARO
- [ ] **B)** ALE = SLE / ARO
- [ ] **C)** ALE = SLE + ARO
- [ ] **D)** ALE = ARO - SLE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Annualized Loss Expectancy (ALE) is calculated by multiplying Single Loss Expectancy (SLE) by the Annual Rate of Occurrence (ARO).
 
 
</details>


---

### **Threats, Vulnerabilities, and Mitigations**

### 24. Which term describes the total sum of all vulnerabilities, entry points, and assets exposed to potential exploitation?

- [ ] **A)** Attack vector
- [ ] **B)** Attack surface
- [ ] **C)** Threat actor
- [ ] **D)** Vulnerability assessment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The attack surface represents the total sum of vulnerabilities, entry points, and assets exposed to potential exploitation.
 
 
</details>

### 25. Which of the following are considered types of threat actors?

- [ ] **A)** Nation-states
- [ ] **B)** Insider threats
- [ ] **C)** Attack vectors
- [ ] **D)** Motivations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CompTIA categorizes actors like nation-states and insider threats by skill, resources, and intent.
 
 
</details>

### 26. Analyze the following code snippet and identify the specific application attack being performed.

```sql
SELECT * FROM users WHERE username = '" OR '1'='1' --' AND password = 'password';
```

- [ ] **A)** SQL injection
- [ ] **B)** Cross-site scripting
- [ ] **C)** Buffer overflow
- [ ] **D)** DLL hijacking

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code shows the manipulation of a backend query through unsanitized input, which is SQL injection.
 
 
</details>

### 27. What is the primary difference between a virus and a worm?

- [ ] **A)** A worm requires a host file
- [ ] **B)** A virus self-propagates without user action
- [ ] **C)** A worm self-propagates without user intervention
- [ ] **D)** A virus is always more destructive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> A virus requires a host file and user action, whereas a worm is standalone and self-propagates.
 
 
</details>

### 28. Which of the following are examples of social engineering attacks?

- [ ] **A)** Phishing
- [ ] **B)** Vishing
- [ ] **C)** SQL injection
- [ ] **D)** DDoS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Phishing and vishing are social engineering attacks that manipulate human psychology.
 
 
</details>

### 29. Examine the following configuration and identify the missing security control.

```javascript
system("echo " + user_input);
```

- [ ] **A)** Input validation
- [ ] **B)** Network segmentation
- [ ] **C)** Least privilege
- [ ] **D)** Patch management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code accepts raw user input directly into a command, indicating a lack of input validation.
 
 
</details>

### 30. Which term describes an attacker setting up a rogue access point with a duplicate SSID?

- [ ] **A)** Jamming
- [ ] **B)** Deauthentication
- [ ] **C)** Evil twin
- [ ] **D)** IV attack

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> An evil twin is a rogue access point that uses a duplicate SSID to trick users into connecting.
 
 
</details>

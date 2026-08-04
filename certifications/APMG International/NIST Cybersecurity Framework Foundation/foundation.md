<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/APMG%20International/NIST%20Cybersecurity%20Framework%20Foundation" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>NIST Cybersecurity Framework Foundation</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Applying the Framework and Exam Preparation](#applying-the-framework-and-exam-preparation) (3 questions)
- [Framework Core - Identify Function](#framework-core-identify-function) (6 questions)
- [Framework Core - Protect, Detect, and Respond Functions](#framework-core-protect-detect-and-respond-functions) (10 questions)
- [Framework Core - Recover Function and Overall Framework Governance](#framework-core-recover-function-and-overall-framework-governance) (6 questions)
- [Introduction to the NIST Cybersecurity Framework](#introduction-to-the-nist-cybersecurity-framework) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:24:56.813Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Applying the Framework and Exam Preparation | 3 |
| Framework Core - Identify Function | 6 |
| Framework Core - Protect, Detect, and Respond Functions | 10 |
| Framework Core - Recover Function and Overall Framework Governance | 6 |
| Introduction to the NIST Cybersecurity Framework | 5 |

---

### **Applying the Framework and Exam Preparation**

### 1. What is the very first step in the NIST CSF implementation methodology?

- [ ] **A)** Prioritize and Scope
- [ ] **B)** Create a Current Profile
- [ ] **C)** Conduct a Risk Assessment
- [ ] **D)** Implement an Action Plan

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The methodology begins with Prioritize and Scope, where the organization identifies business objectives and defines the boundaries of the implementation. This step ensures alignment with senior leadership's risk appetite.
 
 
</details>

### 2. Which two steps are part of the NIST CSF seven‑step implementation methodology? (Select two.)

- [ ] **A)** Prioritize and Scope
- [ ] **B)** Orient
- [ ] **C)** Create a Risk Register
- [ ] **D)** Conduct a Compliance Audit

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The methodology consists of seven steps: Prioritize and Scope, Orient, Create a Current Profile, Conduct a Risk Assessment, Create a Target Profile, Determine/Analyze/Prioritize Gaps, and Implement an Action Plan. Creating a risk register and conducting a compliance audit are not standalone steps in the CSF implementation process.
 
 
</details>

### 3. Read the scenario in the code block below. Then select the Implementation Tier that best describes the organization.

```text
The organization has no documented cybersecurity policy. Each department handles security on a case‑by‑case basis. There is no regular risk assessment or communication with external partners.
```

- [ ] **A)** Tier 1 – Partial
- [ ] **B)** Tier 2 – Risk Informed
- [ ] **C)** Tier 3 – Repeatable
- [ ] **D)** Tier 4 – Adaptive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The organization has no formal cybersecurity process and reacts only when an incident occurs. This reactive, ad‑hoc approach matches Tier 1 (Partial).
 
 
</details>


---

### **Framework Core - Identify Function**

### 4. According to the NIST CSF, what is the foundational prerequisite before implementing any cybersecurity controls?

- [ ] **A)** Establishing a complete and accurate asset inventory
- [ ] **B)** Deploying a firewall at the network perimeter
- [ ] **C)** Conducting a vulnerability scan on all systems
- [ ] **D)** Installing endpoint protection software on all workstations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Asset Management (ID.AM) is the foundational discipline under the Identify function. Without knowing what assets exist, their classification, and ownership, no other cybersecurity activity (Protect, Detect, Respond) can be effectively performed. The framework emphasizes that you cannot protect what you do not know.
 
 
</details>

### 5. Which of the following are key components of Asset Management (ID.AM) as defined in the NIST CSF? (Select two answers)

- [ ] **A)** Asset Inventory
- [ ] **B)** Asset Ownership
- [ ] **C)** Threat Identification
- [ ] **D)** Vulnerability Scanning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Asset Management (ID.AM) encompasses asset inventory, classification, and ownership. Threat Identification belongs to Risk Assessment (ID.RA), and vulnerability scanning is part of the Protect or Detect functions, not a core ID.AM component.
 
 
</details>

### 6. Review the following CSV excerpt representing an asset inventory. According to NIST CSF Asset Management (ID.AM), which assets are missing an assigned owner? (Select all that apply)

```csv
Asset Name, Type, Owner
Server1, physical, ITAdmin
Server2, physical, 
Database, logical, DBADept
Contractor John, human, 
```

- [ ] **A)** Server1
- [ ] **B)** Server2
- [ ] **C)** Database
- [ ] **D)** Contractor John

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Asset ownership is a requirement under ID.AM. In the inventory, Server2 and Contractor John have no owner listed, making them non-compliant. Server1 and Database already have designated owners.
 
 
</details>

### 7. Which Business Environment (ID.BE) subcategory requires an organization to define its role and dependencies within the supply chain?

- [ ] **A)** ID.BE-1
- [ ] **B)** ID.BE-2
- [ ] **C)** ID.BE-3
- [ ] **D)** ID.BE-4

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ID.BE-1 is defined as 'Organizational role in supply chain'. ID.BE-2 refers to critical infrastructure place, ID.BE-3 deals with mission objectives, and ID.BE-4 covers dependencies and critical functions. Only ID.BE-1 explicitly addresses supply chain role.
 
 
</details>

### 8. Which of the following activities belong to the Governance (ID.GV) category of the NIST CSF Identify function? (Select two answers)

- [ ] **A)** Approving the cybersecurity policy
- [ ] **B)** Installing network firewalls
- [ ] **C)** Identifying legal and regulatory requirements
- [ ] **D)** Conducting penetration tests

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> ID.GV includes policy approval (board-level governance) and identification of legal/regulatory requirements. Installing firewalls is a Protect function activity, and penetration testing belongs to Risk Assessment (ID.RA) or Detect, not Governance.
 
 
</details>

### 9. Examine the following list of activities. Based on the NIST CSF, which one is NOT part of Risk Assessment (ID.RA)?

```text
Activities:
1. Threat Identification
2. Vulnerability Analysis
3. Control Implementation
4. Impact Analysis
```

- [ ] **A)** Threat Identification
- [ ] **B)** Vulnerability Analysis
- [ ] **C)** Control Implementation
- [ ] **D)** Impact Analysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Risk Assessment (ID.RA) involves threat identification, vulnerability analysis, and impact analysis. Control implementation belongs to the Protect function (PR) and is not part of ID.RA.
 
 
</details>


---

### **Framework Core - Protect, Detect, and Respond Functions**

### 10. Which NIST CSF Protect category ensures that only authorized users, devices, and processes are granted access to assets and data?

- [ ] **A)** PR.AC
- [ ] **B)** PR.AT
- [ ] **C)** PR.DS
- [ ] **D)** PR.IP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PR.AC (Access Control) manages identities, credentials, and physical access to ensure only authorized users and devices can access assets.
 
 
</details>

### 11. Which two categories are part of the NIST CSF Detect Function? (Select two)

- [ ] **A)** DE.AE
- [ ] **B)** DE.CM
- [ ] **C)** RS.RP
- [ ] **D)** PR.AC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DE.AE (Anomalies and Events) and DE.CM (Continuous Monitoring) are the two categories of the Detect Function. RS.RP is Respond, PR.AC is Protect.
 
 
</details>

### 12. Based on the incident response timeline, which Respond category does the action at 10:55 belong to?

```plaintext
[10:45] SOC received alert from SIEM.
[10:46] Triage: severe anomaly.
[10:50] Incident declared.
[10:55] Isolated affected host.
[11:00] Notified legal.
```

- [ ] **A)** RS.RP
- [ ] **B)** RS.CO
- [ ] **C)** RS.AN
- [ ] **D)** RS.MI

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> Isolating a host is a mitigation action (RS.MI) to contain the incident.
 
 
</details>

### 13. Which Protect subcategory focuses on protecting data at rest?

- [ ] **A)** PR.DS-1
- [ ] **B)** PR.DS-2
- [ ] **C)** PR.AC-3
- [ ] **D)** PR.PT-3

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PR.DS-1 specifically addresses protection of data at rest, such as full-disk encryption.
 
 
</details>

### 14. Which two are key elements of the Respond Function? (Select two)

- [ ] **A)** RS.RP
- [ ] **B)** RS.IM
- [ ] **C)** DE.AE
- [ ] **D)** PR.MA

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> RS.RP (Response Planning) and RS.IM (Improvements) are categories of the Respond Function. DE.AE is Detect, PR.MA is Protect.
 
 
</details>

### 15. Refer to the firewall rule snippet. Which Protect subcategory does this configuration support?

```plaintext
firewall rule:
  source: any
  destination: internal_servers
  protocol: tcp
  ports: 443, 8443
  action: allow
```

- [ ] **A)** PR.PT-3
- [ ] **B)** PR.PT-1
- [ ] **C)** PR.AC-4
- [ ] **D)** PR.DS-2

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The rule blocks all but essential ports, implementing least functionality (PR.PT-3).
 
 
</details>

### 16. What is the primary purpose of the Detect Function?

- [ ] **A)** Prevent incidents from occurring
- [ ] **B)** Identify incidents in a timely manner
- [ ] **C)** Restore normal operations after an incident
- [ ] **D)** Develop response plans

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Detect Function is designed to identify the occurrence of a cybersecurity event in a timely manner.
 
 
</details>

### 17. Which two categories are part of the Protect Function? (Select two)

- [ ] **A)** PR.AT
- [ ] **B)** PR.IP
- [ ] **C)** RS.AN
- [ ] **D)** DE.CM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> PR.AT (Awareness and Training) and PR.IP (Information Protection Processes) are categories of the Protect Function. RS.AN is Respond, DE.CM is Detect.
 
 
</details>

### 18. The code block shows a log entry. Which Detect subcategory is most directly relevant to this activity?

```plaintext
12:34:56 Firewall log: src=203.0.113.5 dst=10.0.1.2 port=443 action=allow
```

- [ ] **A)** DE.CM-1
- [ ] **B)** DE.CM-3
- [ ] **C)** DE.AE-1
- [ ] **D)** DE.DP-1

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The log captures network traffic from an external IP, which aligns with network monitoring (DE.CM-1).
 
 
</details>

### 19. Which Respond category involves executing the incident response plan during an incident?

- [ ] **A)** RS.RP
- [ ] **B)** RS.CO
- [ ] **C)** RS.MI
- [ ] **D)** RS.IM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RS.RP (Response Planning) mandates that the organization executes its response plan during and after an incident.
 
 
</details>


---

### **Framework Core - Recover Function and Overall Framework Governance**

### 20. According to the NIST CSF, what is the primary purpose of the Recover Function?

- [ ] **A)** Contain and eradicate threats
- [ ] **B)** Restore capabilities or services impaired by an incident
- [ ] **C)** Detect anomalies in network traffic
- [ ] **D)** Identify assets and risks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Recover Function focuses on restoring normal operations after a cybersecurity incident, distinct from the Respond Function which handles containment and eradication.
 
 
</details>

### 21. Which of the following are categories within the Recover Function? (Select two)

- [ ] **A)** Recovery Planning (RC.RP)
- [ ] **B)** Incident Response (RS.RP)
- [ ] **C)** Improvements (RC.IM)
- [ ] **D)** Detection Processes (DE.DP)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The Recover Function has three categories: Recovery Planning, Improvements, and Communications. Incident Response is part of Respond, Detection is part of Detect.
 
 
</details>

### 22. The IT team executes a script to restore the customer database from a backup. After restoration, they verify integrity. According to the CSF, which step is missing to fully satisfy the Recover Function?

```pseudocode
restore_database('backup_2025-01-01.sql');
verify_integrity();
```

- [ ] **A)** Activate the incident response plan
- [ ] **B)** Conduct a post-incident review and capture lessons learned
- [ ] **C)** Isolate the affected network segment
- [ ] **D)** Notify law enforcement

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Recover Function includes Improvements (RC.IM) which require capturing lessons learned and updating plans. Technical restoration alone is insufficient.
 
 
</details>

### 23. What do the NIST CSF Implementation Tiers primarily describe?

- [ ] **A)** The maturity of an organization's security controls
- [ ] **B)** The degree to which risk management processes are integrated and adaptive
- [ ] **C)** The number of cybersecurity incidents handled
- [ ] **D)** The budget allocated to cybersecurity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Tiers describe the rigor of risk management processes from Partial (ad hoc) to Adaptive (continuous improvement), not control maturity or incident count.
 
 
</details>

### 24. Which statements about Current and Target Profiles are correct? (Select two)

- [ ] **A)** The Current Profile represents the desired cybersecurity state
- [ ] **B)** The Target Profile is based on business requirements and risk appetite
- [ ] **C)** Profiles are static and should not be changed after approval
- [ ] **D)** Gap analysis compares Current and Target Profiles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> The Current Profile is the as-is state; the Target Profile is the to-be state driven by business needs. Profiles are dynamic and updated regularly.
 
 
</details>

### 25. The code below outlines a self-assessment process. According to the CSF, what critical step must occur before creating the Target Profile?

```python
def self_assessment():
    profile = create_current_profile()
    target = create_target_profile()
    gaps = compare(profile, target)
    prioritize(gaps, risk)
```

- [ ] **A)** Conduct a vulnerability scan
- [ ] **B)** Obtain executive approval and input from stakeholders
- [ ] **C)** Develop a disaster recovery plan
- [ ] **D)** Purchase new security tools

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Target Profile requires alignment with business strategy and risk appetite, necessitating stakeholder input and senior leadership approval.
 
 
</details>


---

### **Introduction to the NIST Cybersecurity Framework**

### 26. Which Executive Order led to the creation of the NIST Cybersecurity Framework?

- [ ] **A)** Executive Order 13636
- [ ] **B)** Executive Order 13800
- [ ] **C)** Executive Order 14028
- [ ] **D)** Executive Order 13231

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Executive Order 13636, issued in 2013, directed NIST to develop a voluntary risk-based cybersecurity framework for critical infrastructure.
 
 
</details>

### 27. Which of the following are benefits of adopting the NIST Cybersecurity Framework?

- [ ] **A)** Establishing a common language for cybersecurity risk management
- [ ] **B)** Guaranteeing compliance with all regulations
- [ ] **C)** Enabling risk-based prioritization of security investments
- [ ] **D)** Eliminating all cybersecurity risks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The NIST CSF provides a common language, supports risk-based prioritization, and promotes continuous improvement. It does not guarantee compliance or eliminate all risks.
 
 
</details>

### 28. Based on the subcategory identifier shown, which Framework function does it belong to?

```plaintext
# CSF Subcategory
ID.AM-1
```

- [ ] **A)** Identify
- [ ] **B)** Protect
- [ ] **C)** Detect
- [ ] **D)** Respond

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ID.AM-1 is under the Identify function, specifically the Asset Management category.
 
 
</details>

### 29. In which version of the NIST Cybersecurity Framework was the 'Govern' function introduced?

- [ ] **A)** CSF 1.0
- [ ] **B)** CSF 1.1
- [ ] **C)** CSF 2.0
- [ ] **D)** CSF 1.2

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Govern function was added in CSF 2.0, released in 2024, to emphasize governance and enterprise risk management.
 
 
</details>

### 30. Which of the following are valid Implementation Tiers defined by the NIST Cybersecurity Framework?

- [ ] **A)** Partial
- [ ] **B)** Risk-Informed
- [ ] **C)** Repeatable
- [ ] **D)** Adaptive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> The four Implementation Tiers are Partial (Tier 1), Risk-Informed (Tier 2), Repeatable (Tier 3), and Adaptive (Tier 4).
 
 
</details>

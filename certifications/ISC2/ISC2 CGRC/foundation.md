<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/ISC2/Certified%20in%20Governance%2C%20Risk%20and%20Compliance%20(CGRC)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>ISC2 CGRC</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Assessment/Audit of Security and Privacy Controls](#assessment-audit-of-security-and-privacy-controls) (5 questions)
- [Compliance Maintenance](#compliance-maintenance) (4 questions)
- [Implementation of Security and Privacy Controls](#implementation-of-security-and-privacy-controls) (5 questions)
- [Scope of the System](#scope-of-the-system) (3 questions)
- [Security and Privacy Governance, Risk Management, and Compliance Program](#security-and-privacy-governance-risk-management-and-compliance-program) (5 questions)
- [Selection and Approval of Framework, Security, and Privacy Controls](#selection-and-approval-of-framework-security-and-privacy-controls) (4 questions)
- [System Compliance](#system-compliance) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-11T02:42:09.130Z |
| Domains | 7 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Assessment/Audit of Security and Privacy Controls | 5 |
| Compliance Maintenance | 4 |
| Implementation of Security and Privacy Controls | 5 |
| Scope of the System | 3 |
| Security and Privacy Governance, Risk Management, and Compliance Program | 5 |
| Selection and Approval of Framework, Security, and Privacy Controls | 4 |
| System Compliance | 4 |

---

### **Assessment/Audit of Security and Privacy Controls**

### 1. What document is the primary output of the preparation phase in the RMF Assess step?

- [ ] **A)** Security and Privacy Assessment Plan
- [ ] **B)** Security Assessment Report
- [ ] **C)** Plan of Action and Milestones
- [ ] **D)** System Security and Privacy Plan

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Security and Privacy Assessment Plan is produced during preparation and defines scope, objectives, methods, and logistics for the assessment.
 
 
</details>

### 2. According to NIST SP 800-53A, which three assessment methods are used to evaluate controls?

- [ ] **A)** Examination
- [ ] **B)** Interview
- [ ] **C)** Testing
- [ ] **D)** Implementation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> NIST SP 800-53A defines examination, interview, and testing as the three assessment methods; implementation is not an assessment method.
 
 
</details>

### 3. Given the approval logic in the code snippet, whose approval is required before the assessment plan can be approved?

```python
plan_status = "draft"
if ao.approval:
    plan_status = "approved"
if assessor.approval:
    plan_status = "draft"
```

- [ ] **A)** Authorizing Official
- [ ] **B)** Assessor
- [ ] **C)** System Owner
- [ ] **D)** Control Implementer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Only the Authorizing Official approves the assessment plan; the assessor develops it but cannot approve it.
 
 
</details>

### 4. Which system documentation is explicitly reviewed by the assessor to understand architecture and data flows during preparation?

- [ ] **A)** System Security and Privacy Plan
- [ ] **B)** Security Assessment Report
- [ ] **C)** Plan of Action and Milestones
- [ ] **D)** Continuous Monitoring Strategy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The assessor reviews system documentation including the System Security and Privacy Plan, network diagrams, and architectural models.
 
 
</details>

### 5. Which tasks are part of logistics and coordination when preparing an assessment?

- [ ] **A)** Scheduling assessment activities
- [ ] **B)** Arranging personnel interviews
- [ ] **C)** Preparing test tools
- [ ] **D)** Implementing security controls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Logistics includes scheduling, arranging interviews, and preparing test tools; implementing controls is not part of the assessor's preparation role.
 
 
</details>


---

### **Compliance Maintenance**

### 6. What is the primary purpose of continuous monitoring after a system is authorized?

- [ ] **A)** To continually verify that controls remain effective and aligned with risk tolerance
- [ ] **B)** To replace the initial authorization with a one-time audit
- [ ] **C)** To eliminate every vulnerability in real time
- [ ] **D)** To wait until the next reauthorization before taking action

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Continuous monitoring is an ongoing, evidence-driven process that verifies controls remain effective and aligned with organizational risk tolerance.
 
 
</details>

### 7. Which items should be defined in a continuous monitoring strategy?

- [ ] **A)** The security and privacy controls to be monitored
- [ ] **B)** The frequency and collection methods for monitoring
- [ ] **C)** The roles responsible for monitoring activities
- [ ] **D)** A guarantee that no vulnerabilities will appear

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A continuous monitoring strategy defines controls, frequency, collection methods, and roles; it also covers security and privacy controls. It cannot guarantee absence of vulnerabilities.
 
 
</details>

### 8. Review the monitoring data in the code block. Which control requires POA&M documentation?

```json
{
  "controls": [
    {"id": "AC-2", "status": "failed", "risk": "high"},
    {"id": "MP-4", "status": "passed", "risk": "low"},
    {"id": "RA-5", "status": "passed", "risk": "medium"}
  ]
}
```

- [ ] **A)** AC-2
- [ ] **B)** MP-4
- [ ] **C)** RA-5
- [ ] **D)** None of the controls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The failed high-risk control, AC-2, must be recorded as a weakness in the POA&M. The other controls passed.
 
 
</details>

### 9. Which NIST publication specifically defines continuous monitoring strategy?

- [ ] **A)** NIST SP 800-137
- [ ] **B)** NIST SP 800-53
- [ ] **C)** NIST SP 800-30
- [ ] **D)** NIST SP 800-145

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NIST SP 800-137 is the continuous monitoring publication; SP 800-53, SP 800-30, and SP 800-145 cover other areas.
 
 
</details>


---

### **Implementation of Security and Privacy Controls**

### 10. Which step of the NIST RMF follows the selection of controls?

- [ ] **A)** Implement
- [ ] **B)** Assess
- [ ] **C)** Authorize
- [ ] **D)** Monitor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The RMF sequence is Categorize, Select, Implement, Assess, Authorize, Monitor; so Implement is Step 4 and precedes assessment.
 
 
</details>

### 11. Which activities are part of managing security and privacy control implementation?

- [ ] **A)** Documented configuration management
- [ ] **B)** Change control
- [ ] **C)** Ongoing awareness of control instantiation
- [ ] **D)** Deferring documentation until assessment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Implementation management requires documented configuration management, change control, and ongoing awareness; documentation is required, not deferred.
 
 
</details>

### 12. Based on the code block, which implementation activity is indicated?

```plaintext
Control ID: AC-3
Deployment: Enabled
Baseline: Updated
```

- [ ] **A)** Deployed with updated baseline
- [ ] **B)** Under assessment
- [ ] **C)** Awaiting authorization
- [ ] **D)** In monitoring only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Deployment Enabled and Baseline Updated show the control was implemented and the configuration baseline was revised during Step 4.
 
 
</details>

### 13. Who is responsible for developing, implementing, and assessing common controls?

- [ ] **A)** Common control provider
- [ ] **B)** System owner
- [ ] **C)** ISSO
- [ ] **D)** Authorizing official

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The common control provider develops, implements, and assesses common controls; system owners consume or inherit them.
 
 
</details>

### 14. Which actions are part of implementing privacy controls?

- [ ] **A)** Conducting privacy training
- [ ] **B)** Providing notices and SORNs
- [ ] **C)** Applying encryption and access restrictions
- [ ] **D)** Issuing the authorization decision

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Privacy implementation includes administrative actions such as training and notices plus technical controls like encryption and access restrictions.
 
 
</details>


---

### **Scope of the System**

### 15. Which statement best defines the system boundary within the NIST Risk Management Framework for an information system being authorized?

- [ ] **A)** Explicit logical or physical perimeter defining included components
- [ ] **B)** Entire physical network owned by the organization
- [ ] **C)** Diagram created only after security controls are selected
- [ ] **D)** Hardware and software inventory of the data center

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The boundary is the explicit logical or physical perimeter defining included components. It shapes categorization, control allocation, risk assessment, and the authorization decision.
 
 
</details>

### 16. Which elements must be documented when identifying the system boundary in the system security and privacy plan? Select all that apply.

- [ ] **A)** Trust relationships
- [ ] **B)** Data flows
- [ ] **C)** External services and interconnections
- [ ] **D)** Vendor marketing materials

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Boundary documentation must include trust relationships, data flows, and external services so assessors can identify risk, inherited controls, and interconnections requiring agreements.
 
 
</details>

### 17. Examine the system description in the code block and identify which item must be documented as an interconnection requiring an agreement.

```json
{
  "system": "Case Management",
  "inside": ["web app", "database", "authentication service"],
  "external": ["vendor API"]
}
```

- [ ] **A)** Vendor API
- [ ] **B)** Database
- [ ] **C)** Authentication service
- [ ] **D)** Web application

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The vendor API is an external service crossing the boundary. Interconnections such as APIs require agreements like ISAs, MOUs, or SLAs to define security responsibilities.
 
 
</details>


---

### **Security and Privacy Governance, Risk Management, and Compliance Program**

### 18. In the CGRC context, what is the primary purpose of establishing a governance and risk management program?

- [ ] **A)** Directs and controls risk aligned with business missions
- [ ] **B)** Purchase security tools quickly
- [ ] **C)** Eliminate all risk from information systems
- [ ] **D)** Replace continuous monitoring

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Governance is a structural framework that aligns risk management with strategic objectives; it does not eliminate risk or focus on tooling.
 
 
</details>

### 19. According to NIST SP 800-37, which two items are part of risk framing?

- [ ] **A)** Assumptions, constraints, and risk priorities
- [ ] **B)** System-level vulnerability scan outputs
- [ ] **C)** Credible threats and acceptable uncertainty
- [ ] **D)** Specific security control implementation details

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Risk framing develops the context for risk decisions, including assumptions, constraints, priorities, threats, and uncertainty. Vulnerability scans and control details belong to system-level assessment.
 
 
</details>

### 20. Refer to the code block. Which step must occur first when establishing a governance and risk management program?

```text
POSSIBLE_ACTIONS:
1. Select risk assessment tools
2. Draft security policies
3. Obtain executive sponsorship and formal charter
4. Assess residual risk
```

- [ ] **A)** Select risk assessment tools
- [ ] **B)** Draft security policies
- [ ] **C)** Obtain executive sponsorship and formal charter
- [ ] **D)** Assess residual risk

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The process begins with executive sponsorship and a formal charter; tools, policies, and assessments come after direction and authority are established.
 
 
</details>

### 21. Which role has final accountability for accepting residual risk on an information system?

- [ ] **A)** Authorizing Official
- [ ] **B)** Chief Information Security Officer
- [ ] **C)** System Owner
- [ ] **D)** Common Control Provider

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Authorizing Official evaluates the authorization package and accepts residual risk. The CISO advises, while the System Owner implements and operates controls.
 
 
</details>

### 22. Which two statements correctly distinguish governance from management?

- [ ] **A)** Governance sets direction and policies; management implements controls
- [ ] **B)** Governance is board-owned; management is executed by security managers
- [ ] **C)** Governance focuses on installing technical safeguards
- [ ] **D)** Management approves the enterprise risk appetite

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Governance is strategic and establishes direction, accountability, and policy. Management is operational; it implements and operates controls to achieve that direction.
 
 
</details>


---

### **Selection and Approval of Framework, Security, and Privacy Controls**

### 23. Which publication defines the initial low, moderate, and high control baselines for security and privacy controls?

- [ ] **A)** FIPS 199
- [ ] **B)** NIST SP 800-53B
- [ ] **C)** NIST SP 800-37
- [ ] **D)** FedRAMP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> NIST SP 800-53B supplies the initial security and privacy control baselines; FIPS 199 supports categorization, not baseline content.
 
 
</details>

### 24. Which activities are part of control tailoring? (Select all that apply.)

- [ ] **A)** Scoping
- [ ] **B)** Parameterization
- [ ] **C)** Specifying compensating controls
- [ ] **D)** Issuing the ATO

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Tailoring includes scoping, parameterization, compensating controls, and common or hybrid assignments. ATO issuance is a separate authorization step.
 
 
</details>

### 25. Based on the impact values in the block, which initial control baseline should be selected?

```text
System impact: confidentiality = High, integrity = Moderate, availability = Moderate.
```

- [ ] **A)** High
- [ ] **B)** Moderate
- [ ] **C)** Low
- [ ] **D)** Privacy baseline

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When impacts are mixed, the highest impact across objectives determines the baseline; High confidentiality drives High.
 
 
</details>

### 26. Who must approve the tailored control baseline before implementation can begin?

- [ ] **A)** System Owner
- [ ] **B)** Authorizing Official
- [ ] **C)** Information System Security Officer
- [ ] **D)** Control Assessor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The AO approves the security and privacy plan and accepts risk; the system owner proposes tailoring, not approval.
 
 
</details>


---

### **System Compliance**

### 27. In the CGRC framework, how is failure to comply with an internal policy primarily classified?

- [ ] **A)** Internal governance issue
- [ ] **B)** Legal liability issue
- [ ] **C)** Criminal offense
- [ ] **D)** Regulatory violation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Policy noncompliance is an internal governance issue, while noncompliance with a law or regulation carries legal liability.
 
 
</details>

### 28. Which three documents are core components of the authorization package under the NIST Risk Management Framework?

- [ ] **A)** System Security Plan (SSP)
- [ ] **B)** Security Assessment Report (SAR)
- [ ] **C)** Plan of Action and Milestones (POA&M)
- [ ] **D)** Authorization decision letter

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The authorization package includes the SSP, SAR, and POA&M. The authorization decision letter is issued separately after AO review.
 
 
</details>

### 29. Review the code block. Which compliance concept does the conditional logic illustrate in the CGRC context?

```javascript
if (org.processesEUResidentData) { applyLegalRequirement('GDPR'); }
```

- [ ] **A)** Extraterritorial applicability
- [ ] **B)** Internal policy classification
- [ ] **C)** Control inheritance
- [ ] **D)** Risk acceptance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> GDPR may apply extraterritorially when an organization processes EU residents' personal data, regardless of the organization's location.
 
 
</details>

### 30. Who is accountable for the final authorization decision and for accepting residual risk under RMF?

- [ ] **A)** Authorizing Official
- [ ] **B)** System Owner
- [ ] **C)** Security Assessor
- [ ] **D)** Information System Security Officer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Authorizing Official is accountable for accepting residual risk and issuing the authorization decision; other roles support but do not decide.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CREST/CREST%20Certified%20Incident%20Manager%20(CCIM)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Certified Incident Manager</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Crisis Management and Communication](#crisis-management-and-communication) (4 questions)
- [Incident Detection and Analysis](#incident-detection-and-analysis) (8 questions)
- [Incident Management Strategy and Governance](#incident-management-strategy-and-governance) (6 questions)
- [Incident Response Execution](#incident-response-execution) (9 questions)
- [Team Leadership and Continuous Improvement](#team-leadership-and-continuous-improvement) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:18.945Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Crisis Management and Communication | 4 |
| Incident Detection and Analysis | 8 |
| Incident Management Strategy and Governance | 6 |
| Incident Response Execution | 9 |
| Team Leadership and Continuous Improvement | 3 |

---

### **Crisis Management and Communication**

### 1. According to the CREST CCIM framework, what is the primary focus of crisis management compared to routine incident handling?

- [ ] **A)** Technical containment and restoration
- [ ] **B)** Organisational survival and trust preservation
- [ ] **C)** Immediate deployment of additional security tools
- [ ] **D)** Ensuring all systems are patched within 24 hours

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Crisis management shifts focus from tactical resolution to strategic outcome, stakeholder trust, and leadership, as per the CCIM framework.
 
 
</details>

### 2. Which of the following are key principles of crisis management as outlined in the CREST CCIM framework? (Select two)

- [ ] **A)** Separate strategic decision-making from tactical execution
- [ ] **B)** Maintain communication integrity across internal and external stakeholders
- [ ] **C)** Always prioritise speed over accuracy
- [ ] **D)** Deploy maximum technical resources immediately

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Core principles include establishing a clear command structure, separating strategic from tactical, and maintaining communication integrity.
 
 
</details>

### 3. Referring to the code block above, which phase of the OODA loop was most critical in this rapid decision-making scenario?

```text
The crisis manager observed the unfolding situation, quickly oriented their mental model, decided to activate the crisis response plan, and acted immediately. Which phase of the OODA loop was most critical in this rapid decision-making?
```

- [ ] **A)** Observe
- [ ] **B)** Orient
- [ ] **C)** Decide
- [ ] **D)** Act

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> According to the document, orientation (mental model of the crisis) is the most critical phase of the OODA loop.
 
 
</details>

### 4. According to crisis communication principles, what is the recommended approach for communicating bad news during an incident?

- [ ] **A)** Wait until the investigation is complete before making any statement
- [ ] **B)** Tell it all, tell it early, tell it yourself
- [ ] **C)** Only inform internal stakeholders and avoid external communication
- [ ] **D)** Delay communication to avoid panic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The CCIM emphasises that silence creates a vacuum filled by speculation; the rule is 'Tell it all, tell it early, tell it yourself.'
 
 
</details>


---

### **Incident Detection and Analysis**

### 5. What is the primary function of a Security Information and Event Management (SIEM) system?

- [ ] **A)** Centralised log aggregation and correlation
- [ ] **B)** Inline blocking of malicious network traffic
- [ ] **C)** Behavioural monitoring of endpoints
- [ ] **D)** Signature-based detection on endpoints

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SIEM aggregates and correlates logs from multiple sources; it does not block traffic or monitor endpoints directly.
 
 
</details>

### 6. Which two detection methods are used by Intrusion Detection/Prevention Systems (IDS/IPS)?

- [ ] **A)** Signature-based detection
- [ ] **B)** Anomaly-based detection
- [ ] **C)** Behavioural endpoint monitoring
- [ ] **D)** Log aggregation and correlation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> IDS/IPS use signature-based (known patterns) and anomaly-based (baseline deviations) detection. Log correlation is SIEM; endpoint monitoring is EDR.
 
 
</details>

### 7. Based on the alert shown, which component generated this event?

```plaintext
Alert: Suspicious process tree detected. Parent: winword.exe -> Child: powershell.exe (encoded command) on endpoint HOST-42. Telemetry: process creation, registry, network connections.
```

- [ ] **A)** Endpoint Detection and Response (EDR)
- [ ] **B)** Network Intrusion Detection System (NIDS)
- [ ] **C)** Security Information and Event Management (SIEM)
- [ ] **D)** Intrusion Prevention System (IPS)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The alert includes process execution and parent-child relations, typical of EDR telemetry. NIDS/IPS focus on packets; SIEM correlates logs.
 
 
</details>

### 8. What is the main objective of alert tuning in a SOC?

- [ ] **A)** Reduce false positive rate while maintaining detection fidelity
- [ ] **B)** Increase the number of alerts to ensure coverage
- [ ] **C)** Eliminate all alerts below a certain severity threshold
- [ ] **D)** Replace signature-based detection with anomaly detection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Tuning adjusts thresholds and whitelists to reduce noise (false positives) without missing true threats. Increasing alerts or eliminating all low-severity alerts contradicts effective tuning.
 
 
</details>

### 9. Which two factors are used to assign priority to a security alert during triage?

- [ ] **A)** Asset criticality tier
- [ ] **B)** Alert severity score
- [ ] **C)** Number of previous similar alerts
- [ ] **D)** Threat actor attribution from intel

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Priority is a business decision based on asset criticality and threat context (e.g., APT involvement). Severity alone is technical; alert volume does not directly set priority.
 
 
</details>

### 10. The following is a triage decision step. What is the next action after an alert is enriched with threat intelligence?

```plaintext
Alert ingested. Static exclusion applied (known legitimate IP). Threat intel enrichment: IP matched known C2 server (confidence 90%). Contextual enrichment: asset is Tier 0 domain controller. Composite priority score: 85/100.
```

- [ ] **A)** Human analyst review
- [ ] **B)** Automated response execution
- [ ] **C)** Incident declaration
- [ ] **D)** Rule tuning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> After enrichment, the alert is queued for human review (analyst triage) unless it can be auto-closed. Automated response or incident declaration comes after human confirmation.
 
 
</details>

### 11. What is the purpose of applying MITRE ATT&CK mapping to threat intelligence?

- [ ] **A)** To correlate alerts with specific adversary tactics and techniques
- [ ] **B)** To automatically block all IP addresses from a feed
- [ ] **C)** To reduce the number of false positives
- [ ] **D)** To prioritise incidents by asset criticality

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ATT&CK mapping allows SOC to understand the attack pattern (tactic/technique) and select appropriate response playbooks. It does not directly block IPs, reduce FPs, or set priority.
 
 
</details>

### 12. Which two aspects are essential for maintaining the admissibility of digital evidence?

- [ ] **A)** A documented chain of custody
- [ ] **B)** Evidence collected by any team member
- [ ] **C)** Use of software write-blockers only
- [ ] **D)** Cryptographic hash verification

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Chain of custody and hash verification (integrity) are key. Evidence must be collected by trained examiners; hardware write-blockers are preferred over software.
 
 
</details>


---

### **Incident Management Strategy and Governance**

### 13. What is the primary purpose of an incident management policy?

- [ ] **A)** Define step-by-step containment procedures
- [ ] **B)** Provide a high-level statement of intent and principles
- [ ] **C)** List all technical tools needed for response
- [ ] **D)** Assign individual blame for failures

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A policy is a high-level statement of intent and principles, not a detailed procedure.
 
 
</details>

### 14. Which of the following are mandatory under GDPR breach notification? (Select two)

- [ ] **A)** Notify the supervisory authority within 72 hours
- [ ] **B)** Notify the supervisory authority within 24 hours
- [ ] **C)** Notify only if data was encrypted
- [ ] **D)** Notify the affected data subjects if high risk

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> GDPR Article 33 requires notification to the supervisory authority within 72 hours and to data subjects if high risk.
 
 
</details>

### 15. Based on the RACI matrix shown, which role is Accountable for the overall incident response?

```plaintext
| Role             | Incident Response |
|------------------|------------------|
| SOC Analyst      | Responsible      |
| Incident Manager | Accountable      |
| Technical Lead   | Responsible      |
| Legal Counsel    | Consulted        |
```

- [ ] **A)** SOC Analyst
- [ ] **B)** Incident Manager
- [ ] **C)** Technical Lead
- [ ] **D)** Legal Counsel

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Incident Manager is Accountable for the overall response according to the RACI model.
 
 
</details>

### 16. What should be the initial action in a communication plan during an incident?

- [ ] **A)** Notify all employees via email
- [ ] **B)** Contact the CEO directly
- [ ] **C)** Verify the incident and assign severity
- [ ] **D)** Prepare a press release

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The first step is to verify the incident and assign severity before any communication is sent.
 
 
</details>

### 17. Which are key components of a post-incident review? (Select two)

- [ ] **A)** Assigning blame to individuals
- [ ] **B)** Root cause analysis
- [ ] **C)** Action plan development
- [ ] **D)** Ignoring minor incidents

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Root cause analysis and action plan development are core components; blame assignment is not a goal.
 
 
</details>

### 18. According to the decision tree, what must be done for a breached personal data incident with high risk to data subjects?

```yaml
decision_tree:
  personal_data: yes
  risk_to_subjects: high
  actions:
    - notify_supervisory_authority
    - notify_data_subjects
```

- [ ] **A)** Notify the supervisory authority and the affected data subjects
- [ ] **B)** Only notify the supervisory authority
- [ ] **C)** Only notify law enforcement
- [ ] **D)** Take no action as risk is assumed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> If risk to data subjects is high, both the supervisory authority and data subjects must be notified under GDPR.
 
 
</details>


---

### **Incident Response Execution**

### 19. What are the five phases of the incident response lifecycle according to NIST SP 800-61?

- [ ] **A)** Preparation, Detection, Containment, Eradication, Recovery
- [ ] **B)** Detection, Containment, Eradication, Recovery, Lessons Learned
- [ ] **C)** Preparation, Identification, Isolation, Removal, Restoration
- [ ] **D)** Preparation, Analysis, Containment, Remediation, Post-Incident

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NIST SP 800-61 defines the phases as Preparation, Detection, Containment, Eradication, and Recovery.
 
 
</details>

### 20. Which of the following are examples of short-term containment actions?

- [ ] **A)** Disabling a compromised user account
- [ ] **B)** Blocking a malicious IP at the firewall
- [ ] **C)** Reimaging an infected workstation
- [ ] **D)** Implementing network segmentation across the entire site

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Short-term containment includes immediate actions like disabling accounts and blocking IPs; reimaging and segmentation are long-term.
 
 
</details>

### 21. Review the following script snippet used during eradication. What is the primary purpose of the 'Remove-Item' command?

```powershell
Remove-Item -Path 'HKLM:\Software\Microsoft\Windows\CurrentVersion\Run\MaliciousKey' -Force
```

- [ ] **A)** Deleting malicious registry keys
- [ ] **B)** Creating a system restore point
- [ ] **C)** Initiating a network scan
- [ ] **D)** Backing up log files

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Remove-Item is a PowerShell cmdlet to delete file system objects; here it removes malicious registry persistence.
 
 
</details>

### 22. Which type of incident requires GDPR notification within 72 hours?

- [ ] **A)** Personal data breach
- [ ] **B)** Malware infection without data loss
- [ ] **C)** DDoS attack on a public website
- [ ] **D)** Insider threat policy violation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> GDPR Article 33 requires notification for personal data breaches; other incidents may not involve personal data.
 
 
</details>

### 23. Which teams should the Incident Manager coordinate with during a data breach involving customer PII?

- [ ] **A)** Legal counsel
- [ ] **B)** Public relations
- [ ] **C)** Marketing department
- [ ] **D)** National cybercrime unit

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Legal, PR, and law enforcement are key; marketing is not typically part of immediate incident coordination.
 
 
</details>

### 24. Examine the following log entry. What phase of the incident response lifecycle does this log represent?

```plaintext
ALERT: IDS signature 'ET MALWARE Suspicious User-Agent' triggered on host 10.0.1.45
```

- [ ] **A)** Detection and Analysis
- [ ] **B)** Containment
- [ ] **C)** Eradication
- [ ] **D)** Recovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The log shows an IDS alert being triggered, which is a detection activity requiring analysis.
 
 
</details>

### 25. What is a key deliverable of the Preparation phase?

- [ ] **A)** Incident Response Plan (IRP)
- [ ] **B)** Forensic image of affected systems
- [ ] **C)** Root cause analysis report
- [ ] **D)** Press release

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The IRP is developed in the Preparation phase; forensic imaging occurs later, during detection or containment.
 
 
</details>

### 26. Which factors should the Incident Manager consider when selecting a containment strategy?

- [ ] **A)** Business impact assessment
- [ ] **B)** Preservation of forensic evidence
- [ ] **C)** Ease of reimaging the system
- [ ] **D)** Legal and regulatory obligations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> BIA, evidence preservation, and legal obligations are key; reimaging ease is not a primary containment factor.
 
 
</details>

### 27. The code below is part of a data breach notification script. What does the 'notify_ico' function trigger?

```python
def notify_ico(breach_details):
    # Submit breach report
    ico_api.post(breach_details)
    log_breach_notification(breach_details)
```

- [ ] **A)** Sends a breach report to the Information Commissioner's Office
- [ ] **B)** Initiates a system recovery
- [ ] **C)** Blocks the attacker's IP address
- [ ] **D)** Logs the incident in the SIEM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The function 'notify_ico' is designed to submit the mandatory GDPR breach notification to the ICO.
 
 
</details>


---

### **Team Leadership and Continuous Improvement**

### 28. What is the primary benefit of psychological safety in an incident response team?

- [ ] **A)** It encourages team members to report errors and challenge decisions without fear.
- [ ] **B)** It ensures all team members follow the incident commander's orders without question.
- [ ] **C)** It reduces the need for post-incident reviews.
- [ ] **D)** It allows the team to skip debriefs and focus on technical tasks.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Psychological safety creates an environment where team members feel safe to speak up, reducing risks of groupthink and errors.
 
 
</details>

### 29. Which of the following are key steps in the Continuous Improvement Cycle for incident management? (Select two)

- [ ] **A)** Identify Improvement Opportunity
- [ ] **B)** Assign blame for failures
- [ ] **C)** Implement Improvement
- [ ] **D)** Immediately deploy new tools without testing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The cycle includes identifying opportunities and implementing improvements, not assigning blame or untested tool deployment.
 
 
</details>

### 30. Refer to the code block showing a fragment of an incident report. Which metric is missing from this report to demonstrate continuous improvement?

```text
Incident Report
- Incident ID: INC-2024-045
- Date: 2024-11-15
- Type: Phishing
- Containment Time: 1 hour 20 min
- Recovery Time: 4 hours
- Root Cause: User clicked malicious link
```

- [ ] **A)** Mean Time to Detect (MTTD)
- [ ] **B)** Number of team members involved
- [ ] **C)** Incident severity score
- [ ] **D)** Total cost of incident

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MTTD is a key KPI for continuous improvement; it is missing from the report snippet.
 
 
</details>

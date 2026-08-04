<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CREST/CREST%20Certified%20Red%20Team%20Specialist%20(CCRTS)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Certified Red Team Specialist</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Adversary Emulation and TTPs](#adversary-emulation-and-ttps) (6 questions)
- [Exploitation and Post-Exploitation](#exploitation-and-post-exploitation) (9 questions)
- [Planning, Scoping, and Legal Compliance](#planning-scoping-and-legal-compliance) (4 questions)
- [Reconnaissance and Intelligence Gathering](#reconnaissance-and-intelligence-gathering) (6 questions)
- [Reporting and Communication](#reporting-and-communication) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:24.038Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Adversary Emulation and TTPs | 6 |
| Exploitation and Post-Exploitation | 9 |
| Planning, Scoping, and Legal Compliance | 4 |
| Reconnaissance and Intelligence Gathering | 6 |
| Reporting and Communication | 5 |

---

### **Adversary Emulation and TTPs**

### 1. What is the primary purpose of mapping TTPs from known threat actors?

- [ ] **A)** Replicate indicators of compromise
- [ ] **B)** Validate detection analytics against realistic behaviors
- [ ] **C)** Exploit all vulnerabilities
- [ ] **D)** Automate penetration testing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The primary purpose is to validate detection analytics and response procedures by emulating realistic adversary behavior, not just replicating IOCs.
 
 
</details>

### 2. Which components are part of the MITRE ATT&CK hierarchy?

- [ ] **A)** Tactics
- [ ] **B)** Techniques
- [ ] **C)** Procedures
- [ ] **D)** Indicators of Compromise

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The ATT&CK hierarchy consists of Tactics (why), Techniques (how), and Procedures (specific implementation). IOCs are not part of the hierarchy.
 
 
</details>

### 3. The following C2 profile fragment configures which parameter?

```cobaltstrike
set sleep_time 60000;
set jitter 20;
```

- [ ] **A)** Beacon interval
- [ ] **B)** Connection retries
- [ ] **C)** Encryption key
- [ ] **D)** HTTP method

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The parameters 'set sleep_time 60000' and 'set jitter 20' configure the beacon's sleep interval and jitter, which define how frequently the agent communicates.
 
 
</details>

### 4. What is a key characteristic of APT simulation compared to standard penetration testing?

- [ ] **A)** Speed of exploitation
- [ ] **B)** Use of automated scanners
- [ ] **C)** Emphasis on stealth and persistence
- [ ] **D)** Focus on vulnerability discovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> APT simulation prioritizes stealth and long-term persistence to mimic real advanced actors, unlike penetration tests which are often time-limited and noisy.
 
 
</details>

### 5. Which of the following are valid adaptations after detecting a defensive response?

- [ ] **A)** Change payload hash
- [ ] **B)** Rotate C2 domain
- [ ] **C)** Increase attack speed
- [ ] **D)** Switch to a different lateral movement technique

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Adaptations include rotating hashes and C2 domains, and changing techniques. Speeding up usually increases detection risk, so it is not a valid adaptation.
 
 
</details>

### 6. The techniques shown belong to which MITRE ATT&CK tactic?

```text
T1566, T1190
```

- [ ] **A)** Initial Access
- [ ] **B)** Execution
- [ ] **C)** Persistence
- [ ] **D)** Defense Evasion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> T1566 (Phishing) and T1190 (Exploit Public-Facing Application) are both Initial Access techniques.
 
 
</details>


---

### **Exploitation and Post-Exploitation**

### 7. What is the primary goal of vulnerability identification in red team exploitation?

- [ ] **A)** To assign CVSS scores to all findings
- [ ] **B)** To discover weaknesses across the attack surface
- [ ] **C)** To generate automated scan reports
- [ ] **D)** To patch identified vulnerabilities immediately

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Identification involves systematic reconnaissance to discover weaknesses across operating systems, networks, and applications.
 
 
</details>

### 8. Which factors should be considered when prioritizing vulnerabilities for exploitation? (Select two)

- [ ] **A)** Exploit complexity
- [ ] **B)** CVSS score only
- [ ] **C)** Asset criticality
- [ ] **D)** Number of open ports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Prioritization is risk-based, considering exploit complexity and asset value, not just CVSS.
 
 
</details>

### 9. Examine the following code block. Which type of privilege escalation vulnerability does it demonstrate?

```cmd
sc qc VulnSvc
BINARY_PATH_NAME: C:\Program Files\MyApp\service.exe
```

- [ ] **A)** Unquoted Service Path
- [ ] **B)** Token Impersonation
- [ ] **C)** Kernel Exploit
- [ ] **D)** AlwaysInstallElevated

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code shows a service binary path with spaces and no quotes, indicating unquoted service path vulnerability.
 
 
</details>

### 10. What is the purpose of using a SOCKS proxy in pivoting?

- [ ] **A)** To directly access the target's desktop
- [ ] **B)** To route traffic through a compromised host
- [ ] **C)** To perform vulnerability scanning locally
- [ ] **D)** To bypass antivirus software

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A SOCKS proxy on a compromised host allows the attacker to route traffic to otherwise unreachable segments.
 
 
</details>

### 11. Which of the following are native Windows persistence mechanisms? (Select two)

- [ ] **A)** Scheduled tasks
- [ ] **B)** AppInit_DLLs
- [ ] **C)** SSH authorized_keys
- [ ] **D)** LD_PRELOAD

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Scheduled tasks and AppInit_DLLs are Windows-specific persistence mechanisms; SSH and LD_PRELOAD are Linux.
 
 
</details>

### 12. Analyze the command below. What is the attacker trying to achieve?

```bash
find / -perm -4000 -type f 2>/dev/null
```

- [ ] **A)** Dumping LSASS credentials
- [ ] **B)** Enumerating SUID binaries
- [ ] **C)** Checking sudo privileges
- [ ] **D)** Modifying cron jobs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The find command with -perm -4000 lists files with SUID bit set, used for Linux privilege escalation enumeration.
 
 
</details>

### 13. What does 'living off the land' mean in red team operations?

- [ ] **A)** Using only open-source tools
- [ ] **B)** Leveraging built-in OS tools for malicious purposes
- [ ] **C)** Relying on third-party remote access software
- [ ] **D)** Exploiting zero-day vulnerabilities

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> LotL uses built-in binaries like PowerShell, wmic, or certutil to execute attacks, reducing forensic footprint.
 
 
</details>

### 14. Which of the following are common Linux privilege escalation vectors? (Select two)

- [ ] **A)** SUID binary exploitation
- [ ] **B)** Unquoted service paths
- [ ] **C)** Kernel exploits
- [ ] **D)** Token impersonation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> SUID binaries and kernel exploits are Linux-specific; unquoted service paths and token impersonation apply to Windows.
 
 
</details>

### 15. Examine the snippet of a WMI event subscription. What is the purpose of this code?

```powershell
New-Object System.Management.ManagementClass('root\subscription:__EventFilter')
```

- [ ] **A)** Scheduled task creation
- [ ] **B)** WMI permanent event subscription
- [ ] **C)** Registry run key modification
- [ ] **D)** Service installation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> WMI event subscriptions allow code execution when specific events occur, providing stealthy persistence without file drops.
 
 
</details>


---

### **Planning, Scoping, and Legal Compliance**

### 16. Which law is the primary legislation for unauthorised computer access in the UK?

- [ ] **A)** Computer Misuse Act 1990
- [ ] **B)** CFAA (Computer Fraud and Abuse Act)
- [ ] **C)** GDPR
- [ ] **D)** PCI DSS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Computer Misuse Act 1990 is the primary UK law that criminalises unauthorised access to computer material.
 
 
</details>

### 17. Which items must be explicitly included in a Red Team Rules of Engagement? (Select all that apply.)

- [ ] **A)** Permitted attack techniques and tools
- [ ] **B)** Excluded target systems and assets
- [ ] **C)** Exact start time of the engagement
- [ ] **D)** Data handling and privacy procedures

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> RoE must specify techniques, exclusions, and data handling rules. The exact start time is typically withheld for realism.
 
 
</details>

### 18. Based on the communication protocol shown, what is the primary purpose of having a single point of contact (SPOC) in red team exercises?

```plaintext
Procedure: Upon triggering a detection alert, the red team must notify the SPOC via encrypted chat within 5 minutes. The SPOC will validate whether the alert is part of the exercise and, if not, initiate the incident response plan.
```

- [ ] **A)** To enable rapid deconfliction and prevent false alarms
- [ ] **B)** To provide the blue team with real-time attack details
- [ ] **C)** To bypass legal compliance requirements
- [ ] **D)** To allow the red team to continue without interruption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The SPOC validates whether alerts are from the exercise, allowing quick deconfliction and avoiding unnecessary escalation.
 
 
</details>

### 19. Which risk treatment approach involves formally consenting to proceed with a documented risk?

- [ ] **A)** Avoid
- [ ] **B)** Mitigate
- [ ] **C)** Risk acceptance
- [ ] **D)** Transfer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Risk acceptance is a formal decision to retain the risk, documented and signed off by the client.
 
 
</details>


---

### **Reconnaissance and Intelligence Gathering**

### 20. Which of the following best defines passive reconnaissance?

- [ ] **A)** Interacting directly with target systems
- [ ] **B)** Collecting data from third-party sources without touching target
- [ ] **C)** Performing vulnerability scans
- [ ] **D)** Sending phishing emails

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Passive reconnaissance gathers information from public sources without direct interaction with the target.
 
 
</details>

### 21. Which of the following are considered OSINT tools?

- [ ] **A)** Nmap
- [ ] **B)** Maltego
- [ ] **C)** theHarvester
- [ ] **D)** Metasploit

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Maltego and theHarvester are OSINT tools; Nmap and Metasploit are active reconnaissance or exploitation tools.
 
 
</details>

### 22. Given the following command, what is its primary purpose?

```bash
theHarvester -d example.com -b google
```

- [ ] **A)** Email addresses and subdomains
- [ ] **B)** Open ports
- [ ] **C)** SSL certificates
- [ ] **D)** Social media profiles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The theHarvester command with -b google searches for emails and subdomains from Google indexes.
 
 
</details>

### 23. Which Nmap scan type is stealthy because it does not complete the TCP handshake?

- [ ] **A)** TCP connect scan
- [ ] **B)** SYN scan
- [ ] **C)** UDP scan
- [ ] **D)** ACK scan

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Nmap SYN scan (-sS) sends only SYN packets and does not complete the three-way handshake.
 
 
</details>

### 24. Which of the following are application enumeration techniques?

- [ ] **A)** Directory busting
- [ ] **B)** Service fingerprinting
- [ ] **C)** WHOIS lookup
- [ ] **D)** SNMP walk

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Directory busting and service fingerprinting are application-level; WHOIS and SNMP are network/OSINT.
 
 
</details>

### 25. What does the -sV flag in this Nmap command do?

```bash
nmap -sV -p 80,443 10.0.0.1
```

- [ ] **A)** Enables version detection
- [ ] **B)** Performs SYN scan
- [ ] **C)** Sets timing template
- [ ] **D)** Defines output format

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The -sV flag tells Nmap to probe open ports to determine service version information.
 
 
</details>


---

### **Reporting and Communication**

### 26. What is the primary purpose of the executive summary in a red team report?

- [ ] **A)** Provide detailed exploitation commands and technical evidence
- [ ] **B)** Communicate business risk, top findings, and high-level recommendations to non-technical stakeholders
- [ ] **C)** List all vulnerabilities by CVSS score
- [ ] **D)** Include raw packet captures and full log files

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The executive summary is designed for non-technical stakeholders like executives; it must translate technical findings into business impact and strategic recommendations, avoiding jargon and excessive detail.
 
 
</details>

### 27. Which of the following are essential components of a professional red team report? (Select all that apply)

- [ ] **A)** Executive Summary
- [ ] **B)** Risk Assessment Matrix
- [ ] **C)** Full source code of all exploits used
- [ ] **D)** Technical Annex

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> A red team report includes an Executive Summary (for executives), a Risk Assessment Matrix (for prioritization), and a Technical Annex (for technical teams). Full exploit source code is not typically included unless agreed upon.
 
 
</details>

### 28. Read the following excerpt from a red team report. Which section of the report does it most likely belong to?

```plaintext
The attack began with a phishing email that delivered a malicious macro. Within 2 hours, the attacker gained Domain Admin privileges and accessed the customer database. This represents a critical risk to the organization due to potential regulatory fines and loss of customer trust.
```

- [ ] **A)** Executive Summary
- [ ] **B)** Technical Annex
- [ ] **C)** Risk Assessment Matrix
- [ ] **D)** Remediation Recommendations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The excerpt focuses on business impact and high-level findings without technical depth, which is characteristic of the Executive Summary.
 
 
</details>

### 29. When communicating a technical finding to a non-technical executive, which approach is most appropriate?

- [ ] **A)** We exploited CVE-2023-3434 via a buffer overflow in the web application.
- [ ] **B)** An attacker could gain complete control of your critical systems, leading to significant financial and reputational damage.
- [ ] **C)** The vulnerability has a CVSS score of 9.8 and is remotely exploitable with low complexity.
- [ ] **D)** We used Metasploit module exploit/multi/http/struts2_rest_xstream to achieve code execution.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Executive audiences need business risk context, not technical details. The correct option translates the finding into business impact and uses non-technical language.
 
 
</details>

### 30. Which of the following are examples of appropriate audience-specific communication in a red team engagement? (Select all that apply)

- [ ] **A)** Using MITRE ATT&CK technique IDs when briefing the SOC team
- [ ] **B)** Using business impact language (e.g., financial loss, regulatory fines) when briefing the board
- [ ] **C)** Including full command outputs and raw logs in the executive summary
- [ ] **D)** Providing a step-by-step attack chain with evidence in the technical annex

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> The SOC team appreciates technical details like MITRE ATT&CK IDs; the board needs business impact; the technical annex is for deep technical information. Including raw logs in the executive summary is inappropriate for that audience.
 
 
</details>

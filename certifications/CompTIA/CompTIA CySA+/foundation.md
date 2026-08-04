<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CompTIA/CompTIA%20CySA%2B%20ce%20Certification" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>CompTIA CySA+</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Incident Response and Management](#incident-response-and-management) (7 questions)
- [Reporting and Communication](#reporting-and-communication) (5 questions)
- [Security Operations](#security-operations) (10 questions)
- [Vulnerability Management](#vulnerability-management) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:24.211Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Incident Response and Management | 7 |
| Reporting and Communication | 5 |
| Security Operations | 10 |
| Vulnerability Management | 8 |

---

### **Incident Response and Management**

### 1. Which NIST IR phase involves establishing policies and tools before an incident?

- [ ] **A)** Detection & Analysis
- [ ] **B)** Preparation
- [ ] **C)** Containment/Eradication/Recovery
- [ ] **D)** Post-Incident Activity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Preparation is the initial phase where policies, tools, and training are established before any incident occurs.
 
 
</details>

### 2. Which two phases are unique to the SANS PICERL model compared to NIST?

- [ ] **A)** Identification
- [ ] **B)** Containment
- [ ] **C)** Eradication
- [ ] **D)** Recovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> SANS separates Identification and Eradication, while NIST combines Containment, Eradication, and Recovery into one phase.
 
 
</details>

### 3. The analyst runs the command shown below. Which tool is being used to capture volatile data?

```powershell
winpmem.exe memory.dump
```

- [ ] **A)** FTK Imager
- [ ] **B)** WinPmem
- [ ] **C)** Volatility
- [ ] **D)** dd

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> WinPmem is a tool specifically designed to capture physical memory volatile data from Windows systems.
 
 
</details>

### 4. According to RFC 3227, what is the most volatile data that should be collected first?

- [ ] **A)** CPU registers and cache
- [ ] **B)** Hard drive image
- [ ] **C)** Network traffic logs
- [ ] **D)** Backup tapes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CPU registers and cache are the most volatile and must be captured first before any system state is lost.
 
 
</details>

### 5. Which two items are essential components of a chain of custody document?

- [ ] **A)** Cryptographic hash values
- [ ] **B)** Network topology diagrams
- [ ] **C)** Signatures of each handler
- [ ] **D)** List of affected users

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Chain of custody must include hash values to verify integrity and signatures to track each person who handled the evidence.
 
 
</details>

### 6. An analyst applies the firewall rule shown. What type of incident response action is this?

```bash
iptables -A INPUT -s 192.168.1.100 -j DROP
```

- [ ] **A)** Detection
- [ ] **B)** Containment
- [ ] **C)** Eradication
- [ ] **D)** Recovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Blocking an IP address with a firewall rule is a containment action to stop further malicious traffic.
 
 
</details>

### 7. In the SANS PICERL model, which phase directly follows Containment?

- [ ] **A)** Identification
- [ ] **B)** Eradication
- [ ] **C)** Recovery
- [ ] **D)** Lessons Learned

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SANS order is Preparation, Identification, Containment, Eradication, Recovery, Lessons Learned.
 
 
</details>


---

### **Reporting and Communication**

### 8. What is the primary purpose of an executive summary in security reporting?

- [ ] **A)** To provide a high-level overview of business impact and recommended actions for leadership
- [ ] **B)** To detail every technical finding with log excerpts and packet captures
- [ ] **C)** To serve as a legal document for court proceedings
- [ ] **D)** To list all vulnerabilities with CVSS scores and exploit code

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An executive summary is intended for senior leadership and focuses on business impact, risk, and actionable recommendations, avoiding technical jargon.
 
 
</details>

### 9. Which two of the following are key components of an incident report according to CySA+ best practices?

- [ ] **A)** Timeline of events and actions taken
- [ ] **B)** Executive summary with financial impact
- [ ] **C)** Full disk image of every affected system
- [ ] **D)** Personal opinions of the analyst

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> An incident report should include a chronological timeline and an executive summary focusing on impact. Full disk images are evidence but not always required; personal opinions are not included.
 
 
</details>

### 10. Analyze the code block. Which type of communication channel is most appropriate for the given scenario?

```plaintext
Scenario: A security analyst detects a ransomware outbreak actively encrypting files on the file server. The incident response team must be notified immediately to isolate the server. The CEO needs to be informed within 15 minutes.
```

- [ ] **A)** Email with a full forensic report attachment
- [ ] **B)** Verbal brief or phone call for immediate action
- [ ] **C)** Quarterly written report
- [ ] **D)** Dashboard with historical trends

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code block describes a critical ongoing incident requiring immediate containment. Verbal communication (phone call) is best for urgency, followed by written documentation.
 
 
</details>

### 11. Under GDPR, within how many hours must a breach be reported to the supervisory authority?

- [ ] **A)** 72 hours
- [ ] **B)** 48 hours
- [ ] **C)** 24 hours
- [ ] **D)** 7 days

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> GDPR Article 33 requires breach notification to the supervisory authority within 72 hours of becoming aware of the breach.
 
 
</details>

### 12. Which two regulations require organizations to implement technical safeguards for protecting sensitive data? (Choose two.)

- [ ] **A)** HIPAA
- [ ] **B)** PCI DSS
- [ ] **C)** SOX
- [ ] **D)** GLBA

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> HIPAA requires technical safeguards for ePHI; PCI DSS mandates technical controls for cardholder data. SOX and GLBA focus on financial and consumer data but do not specifically prescribe technical safeguards in the same detailed manner.
 
 
</details>


---

### **Security Operations**

### 13. Which of the following describes passive reconnaissance?

- [ ] **A)** Gathering information through direct interaction with target infrastructure
- [ ] **B)** Collecting data from public sources without directly contacting target systems
- [ ] **C)** Performing port scans to identify open services
- [ ] **D)** Using vulnerability scanners to detect weaknesses

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Passive reconnaissance relies on publicly available data sources and does not involve direct interaction with the target's systems, making it less detectable.
 
 
</details>

### 14. Which of the following are valid open-source intelligence (OSINT) sources for environmental reconnaissance? (Select TWO.)

- [ ] **A)** WHOIS records
- [ ] **B)** Internal network packet captures
- [ ] **C)** Social media platforms
- [ ] **D)** Firewall logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> OSINT uses publicly available information such as WHOIS records and social media. Internal logs are not public.
 
 
</details>

### 15. An analyst sees the following Snort rule in the IDS configuration. What type of detection is this rule implementing?

```snort
alert tcp any any -> any any (msg:"Test Alert"; content:"|01 02 03|"; sid:1000001;)
```

- [ ] **A)** Anomaly-based detection
- [ ] **B)** Signature-based detection
- [ ] **C)** Behavioral analysis
- [ ] **D)** Heuristic detection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Snort rules with specific content patterns are signature-based, matching known attack patterns.
 
 
</details>

### 16. How does an Endpoint Detection and Response (EDR) solution differ from traditional antivirus?

- [ ] **A)** EDR relies solely on signature-based detection
- [ ] **B)** EDR uses behavioral analytics and machine learning
- [ ] **C)** EDR cannot provide retrospective analysis
- [ ] **D)** EDR only monitors network traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> EDR uses behavioral analytics and machine learning to detect unknown threats, unlike signature-based antivirus.
 
 
</details>

### 17. Which of the following are true regarding host firewall configuration? (Select TWO.)

- [ ] **A)** Outbound rules are not important for security
- [ ] **B)** Rules are processed top-down and first match applies
- [ ] **C)** Host firewalls can filter traffic based on application
- [ ] **D)** Host firewalls only filter inbound traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Host firewalls process rules in order and can filter per application based on process or port.
 
 
</details>

### 18. A security analyst executes the following command on a Linux host firewall. What is the immediate effect?

```bash
iptables -A INPUT -p tcp --dport 22 -j DROP
```

- [ ] **A)** Blocks all incoming traffic
- [ ] **B)** Blocks incoming SSH traffic on port 22
- [ ] **C)** Blocks all outgoing traffic
- [ ] **D)** Allows incoming SSH traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The rule drops incoming TCP packets to port 22 (SSH).
 
 
</details>

### 19. Which security technique is most effective in preventing SQL injection attacks?

- [ ] **A)** Output encoding
- [ ] **B)** Input validation with blacklists
- [ ] **C)** Parameterized queries
- [ ] **D)** Using stored procedures without parameterization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Parameterized queries (prepared statements) separate SQL logic from data, preventing injection.
 
 
</details>

### 20. Which of the following are characteristics of Static Application Security Testing (SAST)? (Select TWO.)

- [ ] **A)** It analyzes running applications
- [ ] **B)** It requires access to source code
- [ ] **C)** It can detect runtime configuration issues
- [ ] **D)** It is typically integrated into CI/CD pipelines

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> SAST scans source code without execution and fits well in development pipelines.
 
 
</details>

### 21. The following SIEM query counts failed login events per source IP. What potential threat is it trying to detect?

```splunk
index=main sourcetype=WinEventLog:Security EventCode=4625 | stats count by src_ip
```

- [ ] **A)** Malware infection
- [ ] **B)** Brute-force attack
- [ ] **C)** Data exfiltration
- [ ] **D)** Privilege escalation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Counting failed logins per source can reveal a brute-force password guessing attempt.
 
 
</details>

### 22. Which network traffic pattern is a common indicator of beaconing malware?

- [ ] **A)** Random high-volume data transfers
- [ ] **B)** Periodic connections at consistent intervals
- [ ] **C)** Continuous streaming of packets
- [ ] **D)** Infrequent large file downloads

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Beaconing malware checks in at regular intervals to receive commands.
 
 
</details>


---

### **Vulnerability Management**

### 23. What is the primary purpose of vulnerability scanning?

- [ ] **A)** Exploit vulnerabilities
- [ ] **B)** Identify, categorize, and assess security weaknesses
- [ ] **C)** Automatically patch systems
- [ ] **D)** Monitor network traffic in real time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Vulnerability scanning is a systematic automated process to identify, categorize, and assess security weaknesses in systems.
 
 
</details>

### 24. Which two advantages does authenticated scanning have over unauthenticated scanning? (Select two.)

- [ ] **A)** Require no credentials
- [ ] **B)** Reveal missing patches and misconfigurations
- [ ] **C)** Produce fewer false positives
- [ ] **D)** Can be run without network access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Authenticated scans use credentials to inspect registry, patch levels, and configurations, yielding higher accuracy and deeper results.
 
 
</details>

### 25. Review the Nessus output snippet. What type of scan was likely performed?

```text
Nessus Scan Result:

Port 80: Detected HTTP service
Port 443: TLS certificate valid
No credential failure reported
No missing patches listed
```

- [ ] **A)** Authenticated scan
- [ ] **B)** Unauthenticated scan
- [ ] **C)** Credentialed scan
- [ ] **D)** Agent-based scan

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The output shows only network-level findings without patch status, indicating an unauthenticated scan.
 
 
</details>

### 26. Why are exclusion lists important when planning a vulnerability scan?

- [ ] **A)** Reduce scan duration by skipping all ports
- [ ] **B)** Preclude scanning of sensitive or breakable devices
- [ ] **C)** Increase the number of findings
- [ ] **D)** Allow scanning without authorization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Exclusion lists avoid scanning sensitive systems like printers or legacy controllers that could be disrupted.
 
 
</details>

### 27. Which two factors should be considered when scheduling a vulnerability scan? (Select two.)

- [ ] **A)** Peak business hours
- [ ] **B)** Maintenance windows
- [ ] **C)** System owner coordination
- [ ] **D)** Maximum concurrent hosts without limits

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Scans should be scheduled during maintenance windows and coordinated with system owners to avoid service disruption.
 
 
</details>

### 28. Given the CVSS vector string: AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H. What is the base score range?

```text
CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H
```

- [ ] **A)** Confidentiality impact is low
- [ ] **B)** Confidentiality impact is high
- [ ] **C)** Attack vector is local
- [ ] **D)** User interaction is required

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> C:H indicates high confidentiality impact, meaning the vulnerability could read all data on the system.
 
 
</details>

### 29. What does the Exploit Prediction Scoring System (EPSS) predict?

- [ ] **A)** Severity of the vulnerability
- [ ] **B)** Probability of exploitation in the next 30 days
- [ ] **C)** Number of affected assets
- [ ] **D)** Time required to patch

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> EPSS uses real-world data to predict the likelihood that a vulnerability will be exploited within 30 days.
 
 
</details>

### 30. Which three methods are valid remediation strategies for vulnerabilities? (Select three.)

- [ ] **A)** Patch management
- [ ] **B)** Configuration changes
- [ ] **C)** Compensating controls
- [ ] **D)** Ignoring low-severity findings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The three primary remediation strategies are patch management, configuration changes, and compensating controls.
 
 
</details>

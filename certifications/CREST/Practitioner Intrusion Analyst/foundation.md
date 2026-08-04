<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CREST/CREST%20Practitioner%20Intrusion%20Analyst%20(CPIA)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Practitioner Intrusion Analyst</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Host Based Attacks](#host-based-attacks) (7 questions)
- [Network and Application Attacks](#network-and-application-attacks) (9 questions)
- [Network and Host Based Investigation](#network-and-host-based-investigation) (8 questions)
- [Overview of the Intrusion Analysis Process](#overview-of-the-intrusion-analysis-process) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:34.409Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Host Based Attacks | 7 |
| Network and Application Attacks | 9 |
| Network and Host Based Investigation | 8 |
| Overview of the Intrusion Analysis Process | 6 |

---

### **Host Based Attacks**

### 1. Which Windows Event ID indicates a successful logon?

- [ ] **A)** 4624
- [ ] **B)** 4625
- [ ] **C)** 4688
- [ ] **D)** 7045

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Event ID 4624 is logged for successful authentication in the Windows Security log.
 
 
</details>

### 2. Which Linux log files contain authentication information? (Select two)

- [ ] **A)** /var/log/auth.log
- [ ] **B)** /var/log/syslog
- [ ] **C)** /var/log/secure
- [ ] **D)** /var/log/boot.log

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> On Linux, authentication messages are typically stored in /var/log/auth.log (Debian) or /var/log/secure (RHEL/CentOS).
 
 
</details>

### 3. Run a command to display all running processes and their PIDs.

```powershell
tasklist /v
```

- [ ] **A)** tasklist
- [ ] **B)** netstat
- [ ] **C)** schtasks
- [ ] **D)** wevtutil

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'tasklist' command displays all running processes with their PIDs on Windows.
 
 
</details>

### 4. Which Sysmon Event ID logs process creation?

- [ ] **A)** 1
- [ ] **B)** 3
- [ ] **C)** 11
- [ ] **D)** 7

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Sysmon Event ID 1 (ProcessCreate) logs process creation with command line and parent info.
 
 
</details>

### 5. Which of the following are Windows persistence mechanisms? (Select two)

- [ ] **A)** Registry Run keys
- [ ] **B)** Scheduled tasks
- [ ] **C)** Prefetch files
- [ ] **D)** Event logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Attackers often use Registry Run keys and scheduled tasks to ensure malware runs after reboot.
 
 
</details>

### 6. Use a command to view all scheduled tasks on a Windows system.

```cmd
schtasks /query /v /fo LIST
```

- [ ] **A)** schtasks /query
- [ ] **B)** tasklist /svc
- [ ] **C)** net start
- [ ] **D)** sc query

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'schtasks /query' command displays all scheduled tasks on the system.
 
 
</details>

### 7. Which Windows Event ID indicates the Security log was cleared?

- [ ] **A)** 1102
- [ ] **B)** 104
- [ ] **C)** 4698
- [ ] **D)** 4624

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Event ID 1102 is recorded when the Windows Security log is manually cleared.
 
 
</details>


---

### **Network and Application Attacks**

### 8. What is the primary characteristic of a Denial of Service (DoS) attack?

- [ ] **A)** Attack from multiple distributed sources
- [ ] **B)** Attack from a single source overwhelming resources
- [ ] **C)** Interception of communications between two parties
- [ ] **D)** Corruption of DNS resolver cache

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> DoS originates from a single source, while DDoS uses multiple sources. MITM and DNS spoofing are different attack types.
 
 
</details>

### 9. Which of the following are types of Man-in-the-Middle (MITM) attacks? (Select two)

- [ ] **A)** ARP spoofing
- [ ] **B)** DNS amplification
- [ ] **C)** Session hijacking
- [ ] **D)** SYN flood

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> ARP spoofing and session hijacking are MITM techniques; DNS amplification is a DDoS, SYN flood is a DoS.
 
 
</details>

### 10. Based on the HTTP request shown, what type of attack is being attempted?

```http
GET /products?category=Gifts' OR 1=1-- HTTP/1.1
```

- [ ] **A)** Cross-Site Scripting (XSS)
- [ ] **B)** SQL Injection
- [ ] **C)** Cross-Site Request Forgery (CSRF)
- [ ] **D)** Command Injection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The parameter contains SQL keywords (OR 1=1) and a comment (--), indicating a SQL injection attempt.
 
 
</details>

### 11. What is the key difference between reflected and stored XSS?

- [ ] **A)** Stored XSS is persistent on server; reflected is not
- [ ] **B)** Reflected XSS affects the attacker only
- [ ] **C)** Stored XSS requires no user interaction
- [ ] **D)** Reflected XSS is server-side

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Stored XSS saves payload in database; reflected XSS appears only in the immediate response.
 
 
</details>

### 12. Which of the following are indicators of a SYN flood attack? (Select two)

- [ ] **A)** Many half-open TCP connections
- [ ] **B)** High volume of HTTP requests
- [ ] **C)** SYN-ACK responses with no matching SYN
- [ ] **D)** A single IP sending many SYN packets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> SYN floods cause many half-open connections (SYN_RECEIVED) and originate from one or few IPs.
 
 
</details>

### 13. Examine the database log entry. What type of attack is likely in progress?

```sql
2025-03-15 10:00:02, app_user, SELECT * FROM users WHERE id = 1; WAITFOR DELAY '0:0:5'--
```

- [ ] **A)** Blind SQL injection
- [ ] **B)** Cross-Site Scripting
- [ ] **C)** Command injection
- [ ] **D)** Privilege escalation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The use of WAITFOR DELAY indicates time-based blind SQL injection, delaying response to infer data.
 
 
</details>

### 14. What does DNS spoofing (cache poisoning) typically aim to achieve?

- [ ] **A)** Overwhelm DNS servers with traffic
- [ ] **B)** Redirect users to malicious IP addresses
- [ ] **C)** Steal session cookies from browsers
- [ ] **D)** Encrypt DNS communications

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> DNS spoofing corrupts resolver cache, directing traffic to attacker-controlled IPs.
 
 
</details>

### 15. Which of the following are common application layer attacks? (Select two)

- [ ] **A)** SQL Injection
- [ ] **B)** SYN Flood
- [ ] **C)** Cross-Site Scripting (XSS)
- [ ] **D)** ARP spoofing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> SQLi and XSS are application-layer; SYN flood is transport layer, ARP is data link.
 
 
</details>

### 16. The following PCAP snippet shows an ARP reply. What attack is likely being performed?

```text
192.168.1.1 is at 00:11:22:33:44:55 (gratuitous ARP reply)
```

- [ ] **A)** ARP spoofing (MITM)
- [ ] **B)** DNS poisoning
- [ ] **C)** DHCP starvation
- [ ] **D)** MAC flooding

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Unsolicited ARP replies mapping a gateway IP to a different MAC indicate ARP spoofing.
 
 
</details>


---

### **Network and Host Based Investigation**

### 17. What is the primary role of Snort according to the document?

- [ ] **A)** Signature-based NIDS
- [ ] **B)** Protocol analysis framework
- [ ] **C)** Multi-threaded inline IPS
- [ ] **D)** Application-layer firewall

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Snort is defined as a signature-based NIDS that uses rule files for real-time packet analysis.
 
 
</details>

### 18. Which of the following are features of Suricata as per the document?

- [ ] **A)** Multi-threading
- [ ] **B)** Inline prevention
- [ ] **C)** Signature-based detection only
- [ ] **D)** Native TLS protocol support

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Suricata features multi-threading, inline prevention, and native TLS/HTTP support; it extends Snort-compatible rules.
 
 
</details>

### 19. An analyst runs the command shown. What type of log file does Zeek primarily generate?

```bash
zeek -C -r incident.pcap
```

- [ ] **A)** conn.log
- [ ] **B)** eve.json
- [ ] **C)** fast.log
- [ ] **D)** alert.log

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Zeek's default log is conn.log, which records per-connection metadata, distinct from Suricata's JSON output.
 
 
</details>

### 20. What does Zeek primarily produce according to the document?

- [ ] **A)** High-level protocol logs
- [ ] **B)** Real-time intrusion alerts
- [ ] **C)** Packet-level signatures
- [ ] **D)** Inline blocking decisions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Zeek is a network analysis framework that produces structured logs (e.g., conn.log, http.log), not alerts.
 
 
</details>

### 21. Which alert formats are supported by Snort as mentioned in the document?

- [ ] **A)** unified2
- [ ] **B)** syslog
- [ ] **C)** JSON
- [ ] **D)** CSV

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Snort uses unified2 and syslog formats; JSON is Suricata's output (eve.json). CSV is not standard.
 
 
</details>

### 22. Analyze this Suricata rule header. What action is defined in the rule?

```suricata
alert tcp $HOME_NET any -> $EXTERNAL_NET 80 (msg:"Possible HTTP scan"; sid:1000001;)
```

- [ ] **A)** alert
- [ ] **B)** drop
- [ ] **C)** pass
- [ ] **D)** reject

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The rule starts with 'alert', meaning it only logs the event without dropping traffic.
 
 
</details>

### 23. What is the first step in log correlation according to the document?

- [ ] **A)** Normalize timestamps
- [ ] **B)** Run SIEM rules
- [ ] **C)** Block suspicious IPs
- [ ] **D)** Generate reports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Normalizing timestamps to a common time zone (e.g., UTC) is essential to align events from different sources.
 
 
</details>

### 24. Which are common challenges in log correlation as per the document?

- [ ] **A)** Clock skew between devices
- [ ] **B)** Time zone differences
- [ ] **C)** Missing logs due to rotation
- [ ] **D)** Too many alerts from SIEM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Clock skew, time zones, and missing logs directly affect accurate correlation; alert volume is a separate issue.
 
 
</details>


---

### **Overview of the Intrusion Analysis Process**

### 25. Which phase of the incident response lifecycle involves establishing and maintaining tools, playbooks, and training?

- [ ] **A)** Preparation
- [ ] **B)** Detection
- [ ] **C)** Containment
- [ ] **D)** Recovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Preparation is the phase where incident response capabilities, including tools and playbooks, are established and maintained.
 
 
</details>

### 26. Which of the following are phases in the incident response lifecycle? (Select two)

- [ ] **A)** Preparation
- [ ] **B)** Assessment
- [ ] **C)** Eradication
- [ ] **D)** Evaluation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The incident response lifecycle includes Preparation, Detection & Analysis, Containment, Eradication, Recovery, and Post-Incident Activity.
 
 
</details>

### 27. Based on the code block below, which phase of the incident response lifecycle is most directly associated with the action described?

```plaintext
Alert: Suspicious outbound connection from 10.0.1.5 to 203.0.113.50 at 2025-03-20 14:32:00
```

- [ ] **A)** Detection
- [ ] **B)** Containment
- [ ] **C)** Eradication
- [ ] **D)** Recovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The log entry shows an alert trigger, which is part of detection – identifying potential incidents through monitoring.
 
 
</details>

### 28. In the incident response lifecycle, which phase involves removing the root cause of the incident, such as deleting malware?

- [ ] **A)** Eradication
- [ ] **B)** Recovery
- [ ] **C)** Containment
- [ ] **D)** Analysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Eradication is specifically about removing the root cause, such as malware, backdoors, or compromised accounts.
 
 
</details>

### 29. Which of the following activities are part of the Preparation phase? (Select two)

- [ ] **A)** Creating playbooks
- [ ] **B)** Removing malware
- [ ] **C)** Deploying logging
- [ ] **D)** Restoring backups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Preparation includes establishing response capabilities, creating playbooks, deploying logging, and training. Removing malware is eradication, and restoring backups is recovery.
 
 
</details>

### 30. Based on the action described in the code block, which phase of the incident response lifecycle is being executed?

```plaintext
Action: Isolate host 10.0.1.5 by blocking all inbound/outbound traffic at the switch port.
```

- [ ] **A)** Containment
- [ ] **B)** Recovery
- [ ] **C)** Eradication
- [ ] **D)** Post-Incident

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Isolating a host from the network is a containment action to stop the incident from spreading.
 
 
</details>

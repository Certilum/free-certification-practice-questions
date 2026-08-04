<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CREST/CREST%20Registered%20Intrusion%20Analyst%20(CRIA)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Registered Intrusion Analyst</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Forensic Analysis and Investigation](#forensic-analysis-and-investigation) (8 questions)
- [Incident Response](#incident-response) (8 questions)
- [Malware Analysis](#malware-analysis) (6 questions)
- [Network Security Monitoring](#network-security-monitoring) (4 questions)
- [SOC Processes and Operations](#soc-processes-and-operations) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:42.460Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Forensic Analysis and Investigation | 8 |
| Incident Response | 8 |
| Malware Analysis | 6 |
| Network Security Monitoring | 4 |
| SOC Processes and Operations | 4 |

---

### **Forensic Analysis and Investigation**

### 1. According to RFC 3227, which type of evidence must be collected first during digital forensic acquisition?

- [ ] **A)** CPU registers and cache
- [ ] **B)** Hard drive contents
- [ ] **C)** Network packet captures
- [ ] **D)** Event logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Order of Volatility (OoV) in RFC 3227 states CPU registers and cache are the most volatile and must be captured first.
 
 
</details>

### 2. Which two tools are specifically designed for memory acquisition on Windows systems? (Choose two.)

- [ ] **A)** WinPmem
- [ ] **B)** Magnet RAM Capture
- [ ] **C)** FTK Imager
- [ ] **D)** Autopsy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> WinPmem and Magnet RAM Capture are memory acquisition tools; FTK Imager is for disk imaging, Autopsy is for analysis.
 
 
</details>

### 3. Examine the following command used during live response. What does it capture?

```powershell
netstat -anb
 tasklist /v
 arp -a
```

- [ ] **A)** Network connections and process list
- [ ] **B)** Full memory dump
- [ ] **C)** Disk partition table
- [ ] **D)** Registry hives

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command captures network state and running processes, which are volatile data items.
 
 
</details>

### 4. What is the minimum cryptographic hash standard recommended for verifying forensic image integrity?

- [ ] **A)** SHA-256
- [ ] **B)** MD5
- [ ] **C)** SHA-1
- [ ] **D)** CRC32

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The document specifies SHA-256 as the minimum for cryptographic hashing of forensic images.
 
 
</details>

### 5. Which two items are part of a proper chain of custody for digital evidence? (Choose two.)

- [ ] **A)** Hash values computed at acquisition and verification
- [ ] **B)** Timestamps of each evidence transfer
- [ ] **C)** Network bandwidth used during capture
- [ ] **D)** Antivirus version installed on analysis machine

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Chain of custody requires hash values and timestamps to prove integrity and handling.
 
 
</details>

### 6. The following command is used to capture memory on a Linux server. What is the tool being utilized?

```bash
insmod lime.ko path=/evidence/mem_dump.lime format=lime
```

- [ ] **A)** LiME
- [ ] **B)** dd
- [ ] **C)** MemProcFS
- [ ] **D)** Rekall

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses LiME (Linux Memory Extractor) to acquire memory with a specified output file.
 
 
</details>

### 7. What must be used when acquiring a disk from a suspect drive to prevent any write operations to the source?

- [ ] **A)** Hardware write-blocker
- [ ] **B)** Software write-blocker only
- [ ] **C)** Forensic boot CD
- [ ] **D)** Network share

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A hardware write-blocker physically prevents any write commands from reaching the suspect drive.
 
 
</details>

### 8. Which two are common tools for network packet capture during incident response? (Choose two.)

- [ ] **A)** tcpdump
- [ ] **B)** Wireshark
- [ ] **C)** FTK Imager
- [ ] **D)** RegRipper

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> tcpdump and Wireshark are standard tools for capturing and analyzing network packets.
 
 
</details>


---

### **Incident Response**

### 9. What is the first phase in the SANS PICERL incident response model?

- [ ] **A)** Preparation
- [ ] **B)** Identification
- [ ] **C)** Containment
- [ ] **D)** Lessons Learned

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Preparation is the foundational phase that includes planning, tool acquisition, and training before any incident occurs.
 
 
</details>

### 10. Which phases are explicitly separated in the SANS PICERL model but combined into a single phase in NIST SP 800-61?

- [ ] **A)** Containment
- [ ] **B)** Eradication
- [ ] **C)** Recovery
- [ ] **D)** Preparation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> NIST SP 800-61 combines Containment, Eradication, and Recovery into a single phase, whereas SANS PICERL treats them as three separate phases.
 
 
</details>

### 11. Consider the following action: 'Disconnecting a compromised host from the network.' According to SANS PICERL, which phase does this belong to?

```text
CHECK
```

- [ ] **A)** Identification
- [ ] **B)** Containment
- [ ] **C)** Eradication
- [ ] **D)** Recovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Disconnecting a host is a short-term containment action to prevent the incident from spreading.
 
 
</details>

### 12. What is the primary purpose of the identification phase in incident response?

- [ ] **A)** Recognizing that an incident may be occurring
- [ ] **B)** Removing the root cause of the incident
- [ ] **C)** Restoring systems to normal operation
- [ ] **D)** Documenting lessons learned

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Identification is about detecting and confirming incidents through alerts, logs, or user reports.
 
 
</details>

### 13. Which of the following are key activities performed during the preparation phase of incident response?

- [ ] **A)** Creating an incident response plan
- [ ] **B)** Acquiring forensic imaging kits
- [ ] **C)** Establishing communication channels
- [ ] **D)** Analyzing memory dumps

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Preparation includes planning, tool acquisition, and training; analyzing memory dumps is part of identification or analysis, not preparation.
 
 
</details>

### 14. A security team receives an alert about a potential data exfiltration from a web server. According to triage best practices, what should the analyst do first?

```text
CHECK
```

- [ ] **A)** Isolate the web server from the network
- [ ] **B)** Review the raw logs to verify the alert
- [ ] **C)** Report the incident to the regulatory authority
- [ ] **D)** Rebuild the server from a clean backup

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Initial verification of the alert through log review is the correct first triage step before any containment or reporting.
 
 
</details>

### 15. In incident triage, what does the term 'severity' refer to?

- [ ] **A)** The business-driven ordering of incidents
- [ ] **B)** The intrinsic danger of the alert based on CIA impact
- [ ] **C)** The number of affected systems
- [ ] **D)** The time since the alert was generated

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Severity is determined by the technical impact on confidentiality, integrity, and availability, while priority includes business factors.
 
 
</details>

### 16. Which factors should be considered when prioritizing security incidents during triage?

- [ ] **A)** Criticality of the affected asset
- [ ] **B)** Kill-chain stage of the attack
- [ ] **C)** Regulatory reporting deadlines
- [ ] **D)** Number of false positives from the same rule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Priority is adjusted using asset value, attack phase, and legal obligations; past false positives do not automatically lower priority.
 
 
</details>


---

### **Malware Analysis**

### 17. What is the primary purpose of generating a SHA-256 hash of a malware sample during static analysis?

- [ ] **A)** To uniquely identify the sample
- [ ] **B)** To determine the file type
- [ ] **C)** To extract embedded strings
- [ ] **D)** To detect packers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A SHA-256 hash provides a unique identifier for the file, allowing correlation with threat intelligence feeds. The other options are done with different tools.
 
 
</details>

### 18. Which two of the following are common static analysis techniques for malware? (Select two)

- [ ] **A)** Examining PE headers
- [ ] **B)** Running the sample in a VM
- [ ] **C)** Extracting strings with 'strings'
- [ ] **D)** Monitoring registry changes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> PE header examination and string extraction are static; running in VM is dynamic, and monitoring registry is dynamic analysis.
 
 
</details>

### 19. Examine the code block showing a PE section header. Which section characteristic indicates the code is executable?

```text
Characteristics : 0x60000020
 IMAGE_SCN_CNT_CODE
 IMAGE_SCN_MEM_EXECUTE
 IMAGE_SCN_MEM_READ
```

- [ ] **A)** IMAGE_SCN_MEM_EXECUTE
- [ ] **B)** IMAGE_SCN_MEM_READ
- [ ] **C)** IMAGE_SCN_MEM_WRITE
- [ ] **D)** IMAGE_SCN_CNT_CODE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IMAGE_SCN_MEM_EXECUTE is the characteristic that allows the section to be executed. The other flags control read/write permissions.
 
 
</details>

### 20. What does high entropy (close to 8.0) in the .text section of a PE file typically indicate?

- [ ] **A)** The code is packed or encrypted
- [ ] **B)** The file is a legitimate Windows binary
- [ ] **C)** The section contains only ASCII strings
- [ ] **D)** The file has no imports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> High entropy in a code section often indicates packing or encryption because compressed/encrypted data has high randomness. Normal code has lower entropy.
 
 
</details>

### 21. Which two of the following are examples of persistence mechanisms used by malware? (Select two)

- [ ] **A)** Registry Run keys
- [ ] **B)** Process hollowing
- [ ] **C)** Scheduled tasks
- [ ] **D)** API hooking

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Registry Run keys and scheduled tasks ensure the malware runs automatically after reboot. Process hollowing and API hooking are runtime evasion techniques.
 
 
</details>

### 22. Review the strings output from a malware sample. Which extracted string is most likely a C2 indicator?

```text
http://malicious.com/bot
C:\Windows\System32\kernel32.dll
Microsoft Windows 10
Error: File not found
```

- [ ] **A)** http://malicious.com/bot
- [ ] **B)** C:\\Windows\\System32\\kernel32.dll
- [ ] **C)** Microsoft Windows 10
- [ ] **D)** Error: File not found

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The URL with a suspicious domain and path is a typical C2 indicator. The other strings are benign system references or error messages.
 
 
</details>


---

### **Network Security Monitoring**

### 23. What field is typically recorded in a firewall log to indicate the outcome of a connection attempt?

- [ ] **A)** Action
- [ ] **B)** User-Agent
- [ ] **C)** URL
- [ ] **D)** Payload

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The action field (allow/deny) indicates the firewall decision on a connection.
 
 
</details>

### 24. Which of the following fields are typically found in an IDS/IPS log? (Select two)

- [ ] **A)** Rule ID
- [ ] **B)** Alert severity
- [ ] **C)** HTTP status code
- [ ] **D)** User-Agent string

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> IDS/IPS logs include rule ID and severity; HTTP status and User-Agent are from proxy logs.
 
 
</details>

### 25. Examine the log entry below. What type of network device generated this log?

```plaintext
192.168.1.10 - - [10/Oct/2024:13:55:36 +0000] "GET /index.html HTTP/1.1" 200 2326
```

- [ ] **A)** Firewall
- [ ] **B)** IDS/IPS
- [ ] **C)** Proxy
- [ ] **D)** Router

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The log includes client IP, URL, HTTP method, and status code, typical of a proxy log.
 
 
</details>

### 26. What is the primary function of a Security Information and Event Management (SIEM) system?

- [ ] **A)** Aggregate and correlate log data from multiple sources
- [ ] **B)** Block malicious traffic in real-time
- [ ] **C)** Replace the need for firewall logs
- [ ] **D)** Encrypt all network communications

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A SIEM aggregates, normalises, and correlates log data to produce security alerts.
 
 
</details>


---

### **SOC Processes and Operations**

### 27. What is the primary role of a Tier 1 analyst in a SOC?

- [ ] **A)** Performing deep forensic analysis
- [ ] **B)** Triage and initial response to alerts
- [ ] **C)** Reverse engineering malware samples
- [ ] **D)** Developing custom detection rules

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Tier 1 analysts triage alerts, filter false positives, and escalate confirmed incidents. Deep forensics and reverse engineering are Tier 2/3 roles.
 
 
</details>

### 28. Which of the following are valid escalation triggers from Tier 1 to Tier 2? (Select all that apply)

- [ ] **A)** Confirmed true positive after triage
- [ ] **B)** Alert that can be resolved by a runbook
- [ ] **C)** Incident with moderate/high business impact
- [ ] **D)** Any alert that appears unusual even if unverified

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Escalation is for confirmed incidents beyond runbook resolution or with significant impact. Alerts resolvable by runbook stay at Tier 1; unverified alerts need more analysis.
 
 
</details>

### 29. Review the SIEM query output below. Which Cyber Kill Chain phase is most directly associated with the detected event?

```plaintext
Event: DNS Query for 'evil-c2.example.com' from internal host 10.0.0.45
Time: 2025-03-01 14:32:01 UTC
Source IP: 10.0.0.45
Destination: 8.8.8.8
Query Type: A
Response IP: 198.51.100.99 (known C2 IP in threat feed)
```

- [ ] **A)** Reconnaissance
- [ ] **B)** Delivery
- [ ] **C)** Command & Control
- [ ] **D)** Actions on Objectives

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> A DNS query to a known malicious domain indicates the adversary is maintaining communication with a C2 server, which is the Command & Control phase.
 
 
</details>

### 30. Which Cyber Kill Chain phase involves the attacker delivering the weaponized payload to the target?

- [ ] **A)** Weaponization
- [ ] **B)** Delivery
- [ ] **C)** Exploitation
- [ ] **D)** Installation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Delivery is the phase where the weapon (e.g., phishing email, USB drop) is sent to the target. Weaponization precedes it; Exploitation triggers the payload; Installation follows.
 
 
</details>

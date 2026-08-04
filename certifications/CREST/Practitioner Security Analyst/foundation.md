<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CREST/CREST%20Practitioner%20Security%20Analyst%20(CPSA)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Practitioner Security Analyst</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Information Security and Standards](#information-security-and-standards) (6 questions)
- [Networking and Technologies](#networking-and-technologies) (9 questions)
- [Penetration Testing Methodologies](#penetration-testing-methodologies) (6 questions)
- [Professional Conduct and Ethics](#professional-conduct-and-ethics) (3 questions)
- [Tools and Technical Skills](#tools-and-technical-skills) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:37.084Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Information Security and Standards | 6 |
| Networking and Technologies | 9 |
| Penetration Testing Methodologies | 6 |
| Professional Conduct and Ethics | 3 |
| Tools and Technical Skills | 6 |

---

### **Information Security and Standards**

### 1. Which of the CIA triad objectives ensures that sensitive information is accessible only to authorised individuals?

- [ ] **A)** Availability
- [ ] **B)** Integrity
- [ ] **C)** Confidentiality
- [ ] **D)** Non-repudiation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Confidentiality ensures that information is not disclosed to unauthorised parties. It is protected through encryption, access controls, and the principle of least privilege.
 
 
</details>

### 2. Which of the following are factors of authentication according to the AAA framework? (Select all that apply)

- [ ] **A)** Something you know
- [ ] **B)** Something you have
- [ ] **C)** Something you are
- [ ] **D)** Something you do

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The three authentication factors are knowledge (e.g., password), possession (e.g., token), and inheritance (e.g., fingerprint). 'Something you do' is not a standard factor.
 
 
</details>

### 3. Refer to the code block below. Which security framework is described as having a control catalog of over 1,000 controls?

```json
{
  "ISO 27001": "ISMS requirements",
  "NIST 800-53": "Control catalog of over 1,000 controls",
  "OWASP": "Web application security guidance"
}
```

- [ ] **A)** ISO 27001
- [ ] **B)** NIST 800-53
- [ ] **C)** OWASP
- [ ] **D)** GDPR

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> NIST SP 800-53 provides a comprehensive catalog of over 1,000 security and privacy controls organised into 20 families.
 
 
</details>

### 4. Under GDPR, within how many hours must a data breach be reported to the supervisory authority?

- [ ] **A)** 24 hours
- [ ] **B)** 48 hours
- [ ] **C)** 72 hours
- [ ] **D)** 7 days

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> GDPR Article 33 requires notification to the supervisory authority within 72 hours of becoming aware of the breach, unless the breach is unlikely to result in a risk.
 
 
</details>

### 5. Which of the following are typical classification levels in an information classification policy? (Select all that apply)

- [ ] **A)** Public
- [ ] **B)** Confidential
- [ ] **C)** Restricted
- [ ] **D)** Shared

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Common classification levels include Public, Internal, Confidential, and Restricted. 'Shared' is not a standard classification level.
 
 
</details>

### 6. Refer to the code block showing phases of the incident response lifecycle. Which phase comes immediately after 'Containment'?

```json
[
  "Preparation",
  "Identification",
  "Containment",
  "Eradication",
  "Recovery",
  "Lessons Learned"
]
```

- [ ] **A)** Preparation
- [ ] **B)** Eradication
- [ ] **C)** Recovery
- [ ] **D)** Lessons Learned

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In the SANS PICERL model, the phases are Preparation, Identification, Containment, Eradication, Recovery, Lessons Learned. Eradication follows Containment.
 
 
</details>


---

### **Networking and Technologies**

### 7. Which protocol provides reliable, connection-oriented data delivery?

- [ ] **A)** TCP
- [ ] **B)** UDP
- [ ] **C)** IP
- [ ] **D)** ICMP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TCP uses sequencing and acknowledgements to provide reliable, connection-oriented service at the transport layer.
 
 
</details>

### 8. Which two characteristics apply to IPv6 addressing?

- [ ] **A)** 32-bit address length
- [ ] **B)** 128-bit address length
- [ ] **C)** NAT is mandatory for internet connectivity
- [ ] **D)** Eliminates the need for NAT

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> IPv6 uses 128-bit addresses and removes the necessity for Network Address Translation (NAT).
 
 
</details>

### 9. Analyze the packet capture snippet. Which flag indicates a TCP connection request?

```plaintext
Source: 10.0.0.1, Dest: 10.0.0.2
Protocol: TCP, Flags: SYN
Seq: 1000, Ack: 0
```

- [ ] **A)** SYN
- [ ] **B)** ACK
- [ ] **C)** FIN
- [ ] **D)** RST

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The SYN flag is set in the first packet of the TCP three-way handshake to initiate a connection.
 
 
</details>

### 10. At which OSI layer does a switch operate?

- [ ] **A)** Layer 1
- [ ] **B)** Layer 2
- [ ] **C)** Layer 3
- [ ] **D)** Layer 4

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Switches forward frames based on MAC addresses at the Data Link layer (Layer 2).
 
 
</details>

### 11. Which two vulnerabilities are associated with Layer 2 switching?

- [ ] **A)** ARP spoofing
- [ ] **B)** BGP hijacking
- [ ] **C)** MAC flooding
- [ ] **D)** IP spoofing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> ARP spoofing and MAC flooding are attacks that exploit Layer 2 switching mechanisms.
 
 
</details>

### 12. Examine the STP port state description. Which state prevents frame forwarding but processes BPDUs?

```plaintext
STP Port State: Does not forward frames, receives BPDUs.
```

- [ ] **A)** Blocking
- [ ] **B)** Listening
- [ ] **C)** Learning
- [ ] **D)** Forwarding

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In the STP Blocking state, the port does not forward data frames but still receives and processes BPDUs.
 
 
</details>

### 13. Which type of firewall keeps track of connection state?

- [ ] **A)** Stateless firewall
- [ ] **B)** Stateful firewall
- [ ] **C)** Packet filter
- [ ] **D)** Application gateway

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A stateful firewall keeps track of the state of active connections, using a state table to allow return traffic automatically.
 
 
</details>

### 14. Which two characteristics apply to a stateless firewall?

- [ ] **A)** Maintains a connection state table
- [ ] **B)** Requires explicit rules for return traffic
- [ ] **C)** Inspects each packet independently
- [ ] **D)** Can detect SYN floods automatically

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> A stateless firewall inspects packets independently without context and needs explicit bidirectional rules.
 
 
</details>

### 15. Analyze the firewall rule. What is the purpose of the 'established' keyword in a stateful firewall rule?

```plaintext
allow tcp from any to any established
```

- [ ] **A)** Allows all outbound traffic
- [ ] **B)** Matches packets belonging to an existing session
- [ ] **C)** Matches TCP SYN packets only
- [ ] **D)** Matches packets with any flag set

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 'established' keyword matches packets that are part of an already established connection, used by stateful firewalls.
 
 
</details>


---

### **Penetration Testing Methodologies**

### 16. What is the primary purpose of the Rules of Engagement (RoE) document in a penetration test?

- [ ] **A)** Sets the payment terms
- [ ] **B)** Defines legal and technical boundaries
- [ ] **C)** Lists all vulnerabilities found
- [ ] **D)** Describes the testing team's skills

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The RoE is a legal contract that defines the scope, methods, and constraints of the test. It is the single source of truth for all parties.
 
 
</details>

### 17. Which two elements must be included in a penetration test scoping document?

- [ ] **A)** Target IP addresses
- [ ] **B)** Testers' educational background
- [ ] **C)** Time window for testing
- [ ] **D)** Client's marketing budget

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> A scoping document lists target IP addresses/URLs and the testing time window. It does not include tester backgrounds or client budgets.
 
 
</details>

### 18. Given the nmap command shown, what scan type does it perform?

```bash
nmap -sS -p 80 192.168.1.1
```

- [ ] **A)** SYN stealth scan
- [ ] **B)** TCP connect scan
- [ ] **C)** UDP scan
- [ ] **D)** Ping sweep

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The option -sS indicates a SYN stealth scan, which is the default when run with root privileges.
 
 
</details>

### 19. What is the first step a penetration tester should take after receiving a client request for a test?

- [ ] **A)** Start scanning immediately
- [ ] **B)** Define scope and obtain written authorisation
- [ ] **C)** Send an invoice
- [ ] **D)** Gather OSINT

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The first step is to define a scoping document with clear boundaries and obtain written authorisation before any technical activity.
 
 
</details>

### 20. Which two of the following are considered OSINT (passive reconnaissance) techniques?

- [ ] **A)** Querying certificate transparency logs
- [ ] **B)** Performing a SYN scan on target IP
- [ ] **C)** Using Shodan to find open ports
- [ ] **D)** Exploiting a SQL injection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> CT logs and Shodan are sources that collect public data without sending traffic to the target. SYN scanning is active.
 
 
</details>

### 21. Examine the following command. What task does it perform during OSINT?

```bash
theHarvester -d example.com -b google
```

- [ ] **A)** Enumerating subdomains via CT logs
- [ ] **B)** Searching for emails on public sources
- [ ] **C)** Performing a DNS zone transfer
- [ ] **D)** Scanning for open ports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The command uses theHarvester with a domain to collect email addresses from public sources like search engines.
 
 
</details>


---

### **Professional Conduct and Ethics**

### 22. What is the primary purpose of the CREST Code of Ethics for penetration testers?

- [ ] **A)** To provide guidelines that can be ignored in emergencies
- [ ] **B)** To ensure testers prioritize profit over safety
- [ ] **C)** To uphold integrity, trust, and professionalism in the testing industry
- [ ] **D)** To allow testers to alter reports as requested by clients

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The CREST Code of Ethics is a binding requirement that upholds integrity, trust, and professionalism. It is not aspirational and must be adhered to.
 
 
</details>

### 23. Which of the following are key elements of responsible vulnerability reporting? (Select all that apply)

- [ ] **A)** Coordinated disclosure with the asset owner
- [ ] **B)** Immediate public posting of all findings
- [ ] **C)** Use of encrypted channels for transmission
- [ ] **D)** Including raw PII in the report to prove impact

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Responsible reporting involves coordinated disclosure with the asset owner, using encrypted channels, and avoiding inclusion of raw PII. Immediate public posting can cause harm.
 
 
</details>

### 24. During a penetration test, you discover a vulnerability that allows you to access a database containing personal data of UK residents. According to the legal boundaries described in the playbook, what must you do? Refer to the code snippet below as context.

```sql
-- Example SQL query that retrieved personal data
SELECT * FROM customers WHERE country = 'UK';
```

- [ ] **A)** Continue testing and include the data in the report
- [ ] **B)** Stop testing, secure the evidence, and contact the client immediately
- [ ] **C)** Ignore the data as it is outside the signed scope
- [ ] **D)** Delete the data and proceed as if nothing happened

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Upon discovering personal data outside scope, the analyst must stop testing, secure the evidence, and inform the client immediately to avoid legal violations under UK DPA and CMA.
 
 
</details>


---

### **Tools and Technical Skills**

### 25. Which command is used to execute an auxiliary module in the Metasploit Framework?

- [ ] **A)** run
- [ ] **B)** exploit
- [ ] **C)** execute
- [ ] **D)** start

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Auxiliary modules use the 'run' command; exploit modules use 'exploit'. This distinction is fundamental in MSF usage.
 
 
</details>

### 26. Which of the following are Burp Suite modules? (Select two.)

- [ ] **A)** Repeater
- [ ] **B)** Intruder
- [ ] **C)** Metasploit
- [ ] **D)** Wireshark

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Burp Suite includes Repeater for manual request replay and Intruder for automated fuzzing. Metasploit and Wireshark are separate tools.
 
 
</details>

### 27. In Wireshark, what does the display filter shown below do?

```wireshark-filter
dns.flags.response == 0
```

- [ ] **A)** Shows only HTTP POST requests
- [ ] **B)** Displays only DNS queries (not responses)
- [ ] **C)** Filters all UDP port 53 traffic
- [ ] **D)** Captures only DNS responses from the server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The filter `dns.flags.response == 0` isolates DNS queries (where the response bit is not set). It does not show responses or all UDP/53 traffic.
 
 
</details>

### 28. Which Nmap scan type sends only a SYN packet and does not complete the TCP handshake?

- [ ] **A)** TCP SYN scan (-sS)
- [ ] **B)** TCP Connect scan (-sT)
- [ ] **C)** UDP scan (-sU)
- [ ] **D)** FIN scan (-sF)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SYN scan (-sS) sends a SYN, receives SYN/ACK (open) or RST (closed), and does not send the final ACK. It is the default privileged scan.
 
 
</details>

### 29. Which two attack modes are supported by Hashcat for password cracking? (Select two.)

- [ ] **A)** Dictionary attack (-a 0)
- [ ] **B)** Mask attack (-a 3)
- [ ] **C)** Incremental mode
- [ ] **D)** Single crack mode

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Hashcat uses numeric modes: -a 0 for dictionary and -a 3 for mask. Incremental and single crack are John the Ripper modes.
 
 
</details>

### 30. What does the following Bash one-liner do?

```bash
grep 'failed' /var/log/auth.log | awk '{print $1}' | sort | uniq -c
```

- [ ] **A)** Counts the number of unique IP addresses in a log file
- [ ] **B)** Filters lines containing 'failed' and counts occurrences per day
- [ ] **C)** Deletes log entries older than 24 hours
- [ ] **D)** Extracts all IP addresses that failed authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The command uses grep to select lines with 'failed', awk to extract the date field, sort, and uniq -c to count occurrences per unique date. It shows failed event counts by day.
 
 
</details>

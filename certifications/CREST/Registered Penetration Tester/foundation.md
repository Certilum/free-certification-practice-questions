<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CREST/CREST%20Registered%20Penetration%20Tester%20(CRT)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Registered Penetration Tester</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Exploitation and Post-Exploitation](#exploitation-and-post-exploitation) (10 questions)
- [Information Gathering and Vulnerability Identification](#information-gathering-and-vulnerability-identification) (8 questions)
- [Reporting and Communication](#reporting-and-communication) (6 questions)
- [Web Application and API Security Testing](#web-application-and-api-security-testing) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:45.097Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Exploitation and Post-Exploitation | 10 |
| Information Gathering and Vulnerability Identification | 8 |
| Reporting and Communication | 6 |
| Web Application and API Security Testing | 6 |

---

### **Exploitation and Post-Exploitation**

### 1. What type of XSS stores malicious script permanently on the server?

- [ ] **A)** Stored XSS
- [ ] **B)** Reflected XSS
- [ ] **C)** DOM-based XSS
- [ ] **D)** Blind XSS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Stored (persistent) XSS saves the script on the server, affecting any user viewing the page.
 
 
</details>

### 2. Which two protocols are commonly poisoned by Responder for credential capture?

- [ ] **A)** LLMNR
- [ ] **B)** NBT-NS
- [ ] **C)** DNS
- [ ] **D)** DHCP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Responder poisons LLMNR and NBT-NS (NetBIOS Name Service) to capture authentication attempts.
 
 
</details>

### 3. What does the following Metasploit command achieve?

```metasploit
route add 192.168.1.0 255.255.255.0 1
```

- [ ] **A)** Adds a route to subnet 192.168.1.0/24 through session 1
- [ ] **B)** Removes route to subnet 192.168.1.0/24
- [ ] **C)** Sets the local IP to 192.168.1.0
- [ ] **D)** Changes default gateway to session 1

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'route add' command in Meterpreter instructs MSF to route traffic for the given subnet through the session.
 
 
</details>

### 4. Which vulnerability forces an authenticated user to execute unintended actions?

- [ ] **A)** CSRF
- [ ] **B)** XSS
- [ ] **C)** SSRF
- [ ] **D)** SQL Injection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CSRF (Cross-Site Request Forgery) tricks the victim's browser into sending authenticated requests.
 
 
</details>

### 5. Which two hashes can be extracted from LSASS memory using Mimikatz?

- [ ] **A)** NTLM hash
- [ ] **B)** Kerberos tickets
- [ ] **C)** SHA-512 hash
- [ ] **D)** MD5 hash

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Mimikatz extracts NTLM hashes and Kerberos tickets (e.g., TGT, TGS) from LSASS.
 
 
</details>

### 6. What does this Hashcat command mode indicate?

```bash
hashcat -m 1000 -a 0 hash.txt wordlist.txt
```

- [ ] **A)** NTLM
- [ ] **B)** NetNTLMv2
- [ ] **C)** LM
- [ ] **D)** Kerberos TGS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Hashcat mode 1000 corresponds to NTLM hashes (Windows local hashes).
 
 
</details>

### 7. What does SSRF allow an attacker to do?

- [ ] **A)** Access internal services via the server
- [ ] **B)** Execute arbitrary code on the client
- [ ] **C)** Steal session cookies from users
- [ ] **D)** Inject SQL queries into the database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SSRF (Server-Side Request Forgery) tricks the server into making requests to internal or external resources.
 
 
</details>

### 8. Which two techniques are used for privilege escalation on Windows?

- [ ] **A)** Token impersonation
- [ ] **B)** Unquoted service paths
- [ ] **C)** Pass-the-Hash
- [ ] **D)** LLMNR poisoning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Token impersonation and unquoted service paths are local privilege escalation techniques. Pass-the-Hash is lateral movement; LLMNR poisoning is credential harvesting.
 
 
</details>

### 9. What does the following SSH command accomplish?

```bash
ssh -L 127.0.0.1:8080:10.0.0.5:80 user@pivot-host
```

- [ ] **A)** Forwards local port 8080 to internal host's port 80 via the pivot
- [ ] **B)** Forwards remote port 8080 to attacker's port 80
- [ ] **C)** Creates a SOCKS proxy on port 8080
- [ ] **D)** Starts an SSH server on port 8080

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Local port forwarding (-L) tunnels traffic from the attacker's local port to a target host through the SSH connection.
 
 
</details>

### 10. Which tool is used to forge Kerberos golden tickets?

- [ ] **A)** Mimikatz
- [ ] **B)** Hashcat
- [ ] **C)** John the Ripper
- [ ] **D)** BloodHound

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Mimikatz's kerberos::golden module creates a golden ticket (forged TGT) for persistent domain admin access.
 
 
</details>


---

### **Information Gathering and Vulnerability Identification**

### 11. What is the primary characteristic of passive reconnaissance?

- [ ] **A)** Generating traffic that is detectable by the target
- [ ] **B)** Gathering information without directly interacting with target systems
- [ ] **C)** Performing a full TCP three-way handshake scan
- [ ] **D)** Sending crafted packets to probe for open ports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Passive reconnaissance relies on publicly available information and does not send any packets to the target, making it undetectable.
 
 
</details>

### 12. Which of the following are examples of Open Source Intelligence (OSINT) sources? (Select all that apply)

- [ ] **A)** WHOIS records
- [ ] **B)** Nmap SYN scan results
- [ ] **C)** Social media profiles (LinkedIn, Twitter)
- [ ] **D)** A direct DNS zone transfer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> OSINT involves collecting publicly available data from sources like WHOIS, social media, and search engines without active probing. A DNS zone transfer is an active technique.
 
 
</details>

### 13. Analyze the following command output and determine what type of reconnaissance was performed.

```bash
dig axfr example.com @ns1.example.com
```

- [ ] **A)** Passive DNS enumeration
- [ ] **B)** Active DNS zone transfer
- [ ] **C)** OSINT via Shodan
- [ ] **D)** Passive network scanning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The command attempts a DNS zone transfer using 'dig axfr', which is an active technique that sends a query to the target's DNS server.
 
 
</details>

### 14. Which Nmap scan type sends a SYN packet and does not complete the three-way handshake?

- [ ] **A)** TCP connect scan (-sT)
- [ ] **B)** SYN scan (-sS)
- [ ] **C)** UDP scan (-sU)
- [ ] **D)** FIN scan (-sF)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SYN scan (half-open) sends a SYN packet; if SYN/ACK is received, the port is open, and the scanner sends RST to avoid completing the handshake.
 
 
</details>

### 15. Which of the following are passive reconnaissance techniques? (Select all that apply)

- [ ] **A)** Searching Shodan for target IP history
- [ ] **B)** Performing a DNS zone transfer
- [ ] **C)** Using theHarvester to harvest email addresses from public sources
- [ ] **D)** Running an Nmap ping sweep

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Shodan and theHarvester collect data from public records without sending packets to the target. Zone transfers and ping sweeps are active.
 
 
</details>

### 16. The following output was obtained from a tool. Identify the tool that produced it.

```plaintext
*******************
[*] Target: example.com
[*] Searching Google. found: 10 emails
[*] Searching LinkedIn. found: 5 emails
[*] Subdomains found: www, mail, vpn
*******************
```

- [ ] **A)** Nmap
- [ ] **B)** Masscan
- [ ] **C)** theHarvester
- [ ] **D)** dnsrecon

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The output shows email addresses and subdomains obtained from search engines and social media, typical of theHarvester.
 
 
</details>

### 17. What is the primary purpose of service fingerprinting during a penetration test?

- [ ] **A)** Identify the operating system of the target
- [ ] **B)** Determine the specific software and version running on open ports
- [ ] **C)** Map the network topology
- [ ] **D)** Discover hidden subdomains

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Service fingerprinting identifies the exact application and version, enabling targeted vulnerability searches.
 
 
</details>

### 18. Which of the following statements about DNS enumeration are correct? (Select all that apply)

- [ ] **A)** Passive DNS enumeration queries authoritative DNS servers for cached records.
- [ ] **B)** Active DNS enumeration includes zone transfers and subdomain brute-forcing.
- [ ] **C)** A zone transfer (AXFR) is always allowed by default.
- [ ] **D)** DNS enumeration can reveal mail servers, nameservers, and subdomains.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Active enumeration involves zone transfers and brute-forcing. Zone transfers are usually blocked. DNS enumeration indeed reveals infrastructure details.
 
 
</details>


---

### **Reporting and Communication**

### 19. What is the primary audience for the executive summary of a penetration test report?

- [ ] **A)** Non-technical stakeholders and senior management
- [ ] **B)** System administrators and developers
- [ ] **C)** External auditors only
- [ ] **D)** The penetration testing team itself

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The executive summary is written for non-technical stakeholders to convey business impact and risk without technical jargon.
 
 
</details>

### 20. Which two elements are essential components of a professional penetration test report?

- [ ] **A)** Executive Summary
- [ ] **B)** Raw tool output in the main body
- [ ] **C)** Risk Rating Methodology
- [ ] **D)** Personal opinions about the client's security posture

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> A professional report must include an executive summary and a clear risk rating methodology; raw output belongs in appendices.
 
 
</details>

### 21. Based on the code snippet, which report section should contain this type of content?

```plaintext
The overall security posture is high risk. Three critical vulnerabilities were identified that could lead to a data breach.
```

- [ ] **A)** Executive Summary
- [ ] **B)** Technical Findings Section
- [ ] **C)** Appendices
- [ ] **D)** Scope and Limitations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code shows a high-level risk statement suitable for non-technical readers, which is part of the executive summary.
 
 
</details>

### 22. What does CVSS stand for in the context of vulnerability scoring?

- [ ] **A)** Common Vulnerability Scoring System
- [ ] **B)** Computer Vulnerability Severity Standard
- [ ] **C)** Critical Vulnerability Scoring Scheme
- [ ] **D)** Comprehensive Vulnerability Security Score

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CVSS stands for Common Vulnerability Scoring System, a standard for rating vulnerability severity.
 
 
</details>

### 23. Which two metric groups are part of the CVSS v3.x scoring system?

- [ ] **A)** Base Metrics
- [ ] **B)** Temporal Metrics
- [ ] **C)** Environmental Metrics
- [ ] **D)** Operational Metrics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CVSS v3.x includes Base, Temporal, and Environmental metric groups. Two of these are Base and Temporal.
 
 
</details>

### 24. Given the CVSS vector, what is the Attack Vector (AV) metric value?

```plaintext
CVSS:3.1/AV:N/AC:L/PR:L/UI:N/S:U/C:H/I:H/A:H
```

- [ ] **A)** Network
- [ ] **B)** Adjacent Network
- [ ] **C)** Local
- [ ] **D)** Physical

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In the vector 'AV:N', the Attack Vector is Network (N).
 
 
</details>


---

### **Web Application and API Security Testing**

### 25. Which of the following best describes a SQL Injection vulnerability?

- [ ] **A)** An attacker injects malicious SQL queries through input fields to manipulate a database.
- [ ] **B)** An attacker uses cross-site scripting to steal session cookies.
- [ ] **C)** An attacker modifies HTTP headers to bypass authentication.
- [ ] **D)** An attacker sends crafted XML to cause a denial of service.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SQL Injection occurs when user input is inserted into SQL queries without proper sanitization, allowing database manipulation.
 
 
</details>

### 26. Which of the following are common techniques used in SQL Injection attacks? (Select all that apply.)

- [ ] **A)** Error-based injection
- [ ] **B)** Blind injection (boolean/time-based)
- [ ] **C)** Reflected XSS
- [ ] **D)** CSRF token manipulation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Error-based and blind injection are SQLi techniques; XSS and CSRF are separate attack types.
 
 
</details>

### 27. Analyze the following code snippet and determine the type of vulnerability it demonstrates.

```vb
Dim sql As String = "SELECT * FROM users WHERE username = '" & txtUser.Text & "' AND password = '" & txtPass.Text & "'"
```

- [ ] **A)** SQL Injection
- [ ] **B)** Command Injection
- [ ] **C)** LDAP Injection
- [ ] **D)** Broken Authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code concatenates user input directly into a SQL query, leading to SQL Injection.
 
 
</details>

### 28. Which OWASP Top 10 category does 'Broken Authentication' primarily belong to?

- [ ] **A)** A2 – Broken Authentication
- [ ] **B)** A1 – Injection
- [ ] **C)** A3 – Sensitive Data Exposure
- [ ] **D)** A5 – Broken Access Control

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In the OWASP Top 10, Broken Authentication is categorized as A2.
 
 
</details>

### 29. Which of the following are indicators of weak session management? (Select all that apply.)

- [ ] **A)** Session IDs are sequential numbers
- [ ] **B)** Cookies lack the HttpOnly flag
- [ ] **C)** All API responses include CORS headers
- [ ] **D)** Session tokens are regenerated after login

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Sequential session IDs and missing HttpOnly flag indicate weak management. CORS headers and token regeneration are security measures.
 
 
</details>

### 30. Examine the following HTTP response header and identify a security misconfiguration.

```http
Set-Cookie: sessionid=abc123; Path=/; Secure; SameSite=Lax
```

- [ ] **A)** Missing HttpOnly flag on session cookie
- [ ] **B)** Secure flag is set unnecessarily
- [ ] **C)** SameSite attribute is misconfigured
- [ ] **D)** Cookie domain is too restrictive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Set-Cookie header lacks the HttpOnly flag, allowing JavaScript access to the session cookie.
 
 
</details>

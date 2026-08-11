<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/ISC2/SSCP.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>ISC2 SSCP</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Access Controls](#access-controls) (4 questions)
- [Cryptography](#cryptography) (3 questions)
- [Incident Response and Recovery](#incident-response-and-recovery) (4 questions)
- [Network and Communications Security](#network-and-communications-security) (5 questions)
- [Risk Identification, Monitoring and Analysis](#risk-identification-monitoring-and-analysis) (4 questions)
- [Security Concepts and Practices](#security-concepts-and-practices) (5 questions)
- [Systems and Application Security](#systems-and-application-security) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-11T02:42:14.482Z |
| Domains | 7 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Access Controls | 4 |
| Cryptography | 3 |
| Incident Response and Recovery | 4 |
| Network and Communications Security | 5 |
| Risk Identification, Monitoring and Analysis | 4 |
| Security Concepts and Practices | 5 |
| Systems and Application Security | 5 |

---

### **Access Controls**

### 1. At a login prompt, a user enters their username. Which security process is being performed at this exact moment?

- [ ] **A)** Identification
- [ ] **B)** Authentication
- [ ] **C)** Authorization
- [ ] **D)** Accounting

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Identification is the claim of identity. Authentication proves the claim, authorization grants permissions, and accounting records activity.
 
 
</details>

### 2. Which of the following are recognized primary authentication factors? (Select all that apply)

- [ ] **A)** Knowledge
- [ ] **B)** Possession
- [ ] **C)** Inherence
- [ ] **D)** Location

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The three primary authentication factors are knowledge (something you know), possession (something you have), and inherence (something you are). Location is sometimes used as a contextual attribute, but it is not one of the three primary factors.
 
 
</details>

### 3. In the access control log excerpt, one event corresponds to the verification of a submitted secret against a stored value. Which phase is that event?

```json
[ {"event": "user_login_attempt", "stage": "identification", "detail": "username submitted"}, {"event": "credential_validation", "stage": "authentication", "detail": "password hash compared"}, {"event": "file_access_request", "stage": "authorization", "detail": "ACL evaluated"}, {"event": "audit_log_write", "stage": "accounting", "detail": "access recorded"} ]
```

- [ ] **A)** Identification
- [ ] **B)** Authentication
- [ ] **C)** Authorization
- [ ] **D)** Accounting

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The event labeled credential_validation compares the submitted password hash to a stored value. That action is authentication, because it verifies the identity claim.
 
 
</details>

### 4. An authenticated user is denied access to a file and receives an 'Access Denied' message. What is the best interpretation of this event?

- [ ] **A)** Authentication failed; the user must re-enter credentials
- [ ] **B)** Authorization failed; the user's granted permissions do not include this file
- [ ] **C)** Identification was not completed
- [ ] **D)** The account is locked due to failed logins

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Authentication succeeded, but the access control decision made after authentication is authorization. A validly authenticated subject can still lack permission to a specific object.
 
 
</details>


---

### **Cryptography**

### 5. Which process transforms plaintext into ciphertext using a key and an algorithm in a cryptographic system?

- [ ] **A)** Encryption
- [ ] **B)** Decryption
- [ ] **C)** Hashing
- [ ] **D)** Cryptanalysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Encryption is the process of converting plaintext into ciphertext using a key and algorithm. It provides confidentiality, while decryption reverses the process and hashing is irreversible.
 
 
</details>

### 6. Which two statements about a cryptographic salt are true? Select two.

- [ ] **A)** It is a random value added before hashing.
- [ ] **B)** It must be kept secret from attackers.
- [ ] **C)** It prevents precomputed rainbow table attacks.
- [ ] **D)** It is derived from the encryption key.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> A salt is a random value added before hashing; it prevents precomputed rainbow table attacks and does not need to be secret.
 
 
</details>

### 7. In the authentication exchange code block, what is the primary purpose of the nonce value?

```python
client_nonce = generate_nonce()
response = hmac.new(session_key, client_nonce + request, digestmod='sha256')
server.verify(response, client_nonce)
```

- [ ] **A)** Ensure freshness and prevent replay
- [ ] **B)** Encrypt the request payload
- [ ] **C)** Replace the session key
- [ ] **D)** Keep the HMAC key secret

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A nonce is a number used once to provide freshness and prevent replay attacks. Its uniqueness matters more than secrecy.
 
 
</details>


---

### **Incident Response and Recovery**

### 8. According to the six-phase incident response lifecycle used in the SSCP domain, which phase begins the process?

- [ ] **A)** Preparation
- [ ] **B)** Detection
- [ ] **C)** Eradication
- [ ] **D)** Recovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Preparation establishes the IR policy, team, tools, and training so the organization is ready before an incident occurs.
 
 
</details>

### 9. Which two activities are considered part of the preparation phase of the incident response lifecycle?

- [ ] **A)** Developing the IR policy and training the CSIRT
- [ ] **B)** Conducting tabletop exercises
- [ ] **C)** Isolating infected hosts from the network
- [ ] **D)** Restoring systems from verified backups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Preparation builds readiness through policy, trained teams, tools, and exercises. Isolating and restoring occur during later lifecycle phases.
 
 
</details>

### 10. The array in the code block is missing one of the six incident response lifecycle phases. Which phase should be added?

```python
phases = [
    "Preparation",
    "Detection and Analysis",
    "Containment",
    "Eradication",
    "Recovery"
]
```

- [ ] **A)** Lessons Learned
- [ ] **B)** Preparation
- [ ] **C)** Containment
- [ ] **D)** Recovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The six-phase lifecycle includes preparation, detection and analysis, containment, eradication, recovery, and lessons learned.
 
 
</details>

### 11. In the incident response lifecycle, which phase directly follows detection and analysis according to the six-phase model?

- [ ] **A)** Containment
- [ ] **B)** Eradication
- [ ] **C)** Preparation
- [ ] **D)** Lessons Learned

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Containment limits the blast radius after an incident is detected and analyzed, before eradication and recovery.
 
 
</details>


---

### **Network and Communications Security**

### 12. Which OSI layer handles logical addressing and routing decisions?

- [ ] **A)** Network
- [ ] **B)** Data Link
- [ ] **C)** Transport
- [ ] **D)** Session

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The network layer handles IP addressing and routing. Data link handles MAC addresses, transport manages end-to-end communication, and session manages dialog control.
 
 
</details>

### 13. Which two protocols operate at the transport layer of the TCP/IP model?

- [ ] **A)** TCP
- [ ] **B)** UDP
- [ ] **C)** IP
- [ ] **D)** HTTP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> TCP and UDP are transport-layer protocols. IP operates at the network layer, and HTTP operates at the application layer.
 
 
</details>

### 14. Refer to the code block. Which PDU name corresponds to the network layer?

```javascript
const pduNames = ['Data', 'Segment', 'Packet', 'Frame', 'Bits'];
console.log(pduNames[2]);
```

- [ ] **A)** Packet
- [ ] **B)** Frame
- [ ] **C)** Segment
- [ ] **D)** Bits

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The network layer PDU is called a packet, while frames belong to the data link layer, segments to transport, and bits to physical.
 
 
</details>

### 15. Which protocol suite provides encryption for IP packets at the network layer?

- [ ] **A)** IPsec
- [ ] **B)** TLS
- [ ] **C)** SSH
- [ ] **D)** SSL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IPsec is the network-layer protocol suite used for VPNs and IP traffic protection. TLS and SSH operate at higher layers.
 
 
</details>

### 16. Which two statements correctly describe a stateful firewall?

- [ ] **A)** It tracks active connections in a state table.
- [ ] **B)** It performs deep application-layer inspection by default.
- [ ] **C)** It can block unsolicited inbound packets without a matching state.
- [ ] **D)** It is always deployed as a passive tap.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> A stateful firewall maintains session state and blocks unsolicited inbound traffic. It is inline and does not perform deep application inspection by default.
 
 
</details>


---

### **Risk Identification, Monitoring and Analysis**

### 17. What is the first step in the risk management lifecycle?

- [ ] **A)** Asset identification
- [ ] **B)** Threat modeling
- [ ] **C)** Vulnerability analysis
- [ ] **D)** Risk response

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Asset identification establishes what needs protection. Without an accurate inventory, threat modeling, vulnerability analysis, and risk response cannot be prioritized effectively.
 
 
</details>

### 18. Which of the following are standard risk response strategies recognized in the risk management lifecycle? (Choose all that apply.)

- [ ] **A)** Mitigation
- [ ] **B)** Avoidance
- [ ] **C)** Risk elimination
- [ ] **D)** Acceptance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> The four standard responses are mitigation, avoidance, transfer, and acceptance. 'Elimination' is not used; avoidance is the response that removes exposure.
 
 
</details>

### 19. The code block defines a value that the monitoring system uses to distinguish normal activity from unusual activity. What is this value called?

```python
baseline = average_daily_traffic + (2 * standard_deviation_daily_traffic)
```

- [ ] **A)** Baseline
- [ ] **B)** Benchmark
- [ ] **C)** Risk threshold
- [ ] **D)** Control objective

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A baseline is an organization-specific reference point of normal behavior. This expression captures typical traffic and a statistical variance, forming a baseline.
 
 
</details>

### 20. Which system provides centralized aggregation, normalization, correlation, and alerting of security data?

- [ ] **A)** SIEM
- [ ] **B)** DLP
- [ ] **C)** IDS
- [ ] **D)** Firewall

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A SIEM is the central platform for log aggregation, normalization, correlation, and alerting. DLP, IDS, and firewalls perform narrower functions.
 
 
</details>


---

### **Security Concepts and Practices**

### 21. Which fundamental security concept ensures that data is accessible only to authorized individuals, systems, or processes?

- [ ] **A)** Confidentiality
- [ ] **B)** Integrity
- [ ] **C)** Availability
- [ ] **D)** Non-repudiation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Confidentiality prevents unauthorized disclosure. Integrity protects accuracy, availability ensures access, and non-repudiation proves actions.
 
 
</details>

### 22. Which two controls are commonly used to protect the integrity of data and detect unauthorized modifications?

- [ ] **A)** Cryptographic hash functions
- [ ] **B)** Digital signatures
- [ ] **C)** Symmetric encryption
- [ ] **D)** RAID

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Hashes and digital signatures detect unauthorized changes. Encryption protects confidentiality, and RAID supports availability.
 
 
</details>

### 23. In the risk register entry shown in the code block, what is the $25,000 figure called?

```json
{
  "asset": "Customer Database",
  "threat": "SQL injection",
  "vulnerability": "Unpatched web application",
  "control": "Web Application Firewall",
  "remaining_risk": "$25,000"
}
```

- [ ] **A)** Residual risk
- [ ] **B)** Inherent risk
- [ ] **C)** Risk appetite
- [ ] **D)** Risk avoidance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Residual risk is what remains after controls are implemented. Inherent risk exists before controls, while appetite is the acceptable threshold.
 
 
</details>

### 24. Which security principle limits each user's access to only the information and resources required for their job role?

- [ ] **A)** Least privilege
- [ ] **B)** Defense in depth
- [ ] **C)** Separation of duties
- [ ] **D)** Due diligence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Least privilege restricts permissions to job needs. Defense in depth layers controls, separation of duties divides tasks, and due diligence is verification.
 
 
</details>

### 25. Which two activities are examples of security governance rather than security management?

- [ ] **A)** Board approves the organization's risk appetite
- [ ] **B)** Executive management reviews security policies annually
- [ ] **C)** An administrator configures firewall rule sets
- [ ] **D)** Analysts update antivirus signatures

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Governance sets direction and authority, including risk appetite and policy approval. Configuring tools is operational management.
 
 
</details>


---

### **Systems and Application Security**

### 26. What is the primary purpose of operating system hardening?

- [ ] **A)** Reduce the attack surface by eliminating unnecessary services and enforcing least privilege
- [ ] **B)** Increase system performance by overclocking hardware
- [ ] **C)** Automatically install all available vendor updates
- [ ] **D)** Replace the existing operating system with a cloud-based solution

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Hardening reduces attack surface by removing unneeded services, locking configurations, enforcing least privilege, and maintaining a known secure state.
 
 
</details>

### 27. Which of the following are insecure protocols that should be replaced with encrypted alternatives during hardening? (Choose all that apply.)

- [ ] **A)** Telnet
- [ ] **B)** FTP
- [ ] **C)** SNMPv1
- [ ] **D)** SSH

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Telnet, FTP, and SNMPv1 send data in clear text or use weak security. SSH is the secure alternative for remote administration.
 
 
</details>

### 28. Review the command in the code block. Which security principle is violated by this command?

```bash
chmod 777 /var/www/html/config.php
```

- [ ] **A)** Least privilege
- [ ] **B)** Defense in depth
- [ ] **C)** Separation of duties
- [ ] **D)** Non-repudiation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> World-writable permissions grant every user full read, write, and execute rights, violating least privilege and data integrity.
 
 
</details>

### 29. What is patch management?

- [ ] **A)** The process of obtaining, testing, and applying vendor updates to fix known vulnerabilities
- [ ] **B)** The process of replacing hardware components that are no longer under warranty
- [ ] **C)** The process of configuring firewall rules to block malicious traffic
- [ ] **D)** The process of creating user accounts for new employees

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Patch management is the lifecycle of acquiring, testing, deploying, and verifying software updates to remediate known security vulnerabilities.
 
 
</details>

### 30. Which capabilities are typically included in modern Endpoint Protection Platforms (EPPs)? (Choose all that apply.)

- [ ] **A)** Behavioral analysis
- [ ] **B)** Machine learning
- [ ] **C)** Signature-based detection
- [ ] **D)** Full-disk encryption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Modern EPPs combine signature detection with behavioral analysis, machine learning, and cloud threat intelligence. Full-disk encryption is a separate control.
 
 
</details>

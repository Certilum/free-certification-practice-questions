<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/OffSec/Offensive%20Security%20Certified%20Professional.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Offensive Security Certified Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Active Directory](#active-directory) (1 questions)
- [Exploitation](#exploitation) (2 questions)
- [Post-Exploitation](#post-exploitation) (1 questions)
- [Privilege Escalation](#privilege-escalation) (1 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 5 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:44.958Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Active Directory | 1 |
| Exploitation | 2 |
| Post-Exploitation | 1 |
| Privilege Escalation | 1 |

---

### **Active Directory**

### 1. In the context of payload delivery, what best describes a reverse shell?

- [ ] **A)** It initiates a connection from the target back to the attacker
- [ ] **B)** It opens a port on the target and waits for the attacker to connect
- [ ] **C)** It uses legitimate pre-installed system tools to download payloads
- [ ] **D)** It encodes the payload in Base64 to bypass signature detection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A reverse shell makes the target connect back to the attacker, bypassing inbound firewall restrictions. The other options describe bind shells, living off the land, and obfuscation techniques.
 
 
</details>


---

### **Exploitation**

### 2. What is the primary characteristic of a reverse shell?

- [ ] **A)** It initiates a connection from the target back to the attacker.
- [ ] **B)** It opens a port on the target and waits for the attacker to connect.
- [ ] **C)** It relies on DNS tunneling to establish the connection.
- [ ] **D)** It requires a public IP address on the target machine.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A reverse shell connects from the target to the attacker, making it useful for bypassing inbound firewall rules. Bind shells do the opposite by listening on the target.
 
 
</details>

### 3. Which statements accurately describe the difference between staged and stageless payloads?

- [ ] **A)** A staged payload starts with a small stub that later downloads the main payload from the attacker.
- [ ] **B)** A stageless payload is a single self-contained file that includes all the required code.
- [ ] **C)** A staged payload always performs better in every network environment than a stageless payload.
- [ ] **D)** A stageless payload must be downloaded in multiple parts before execution.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Staged payloads first send a small stub that retrieves the rest of the payload, while stageless payloads are complete single files. Staging helps when memory is limited.
 
 
</details>


---

### **Post-Exploitation**

### 4. Which type of shell initiates a connection from the target system back to the attacker, allowing it to bypass inbound firewall restrictions?

- [ ] **A)** Reverse shell
- [ ] **B)** Bind shell
- [ ] **C)** Staged shell
- [ ] **D)** Stageless shell

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A reverse shell works by making the target initiate an outbound connection to the attacker. This is effective because many firewalls block unsolicited inbound connections but permit outbound traffic. A bind shell, by contrast, opens a listening port on the target, which is more likely to be blocked by network security controls.
 
 
</details>


---

### **Privilege Escalation**

### 5. In the context of payload delivery during penetration testing, what is a reverse shell?

- [ ] **A)** Target connects back to attacker
- [ ] **B)** Attacker connects to target on open port
- [ ] **C)** Target opens a port and listens passively
- [ ] **D)** Attacker uploads a web shell to a server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A reverse shell initiates a connection from the target back to the attacker, bypassing inbound firewall rules and enabling remote command execution.
 
 
</details>

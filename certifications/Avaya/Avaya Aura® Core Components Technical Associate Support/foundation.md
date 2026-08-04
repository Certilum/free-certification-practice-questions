<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Avaya/Avaya%20Aura®%20Core%20Components%20Technical%20Associate%20Support" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Avaya Aura® Core Components Technical Associate Support</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Avaya Aura® Core Components Overview and Architecture](#avaya-aura-core-components-overview-and-architecture) (4 questions)
- [Maintenance and Troubleshooting](#maintenance-and-troubleshooting) (9 questions)
- [Security and Compliance Fundamentals](#security-and-compliance-fundamentals) (5 questions)
- [System Administration and Management](#system-administration-and-management) (7 questions)
- [User and Feature Support](#user-and-feature-support) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:16.837Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Avaya Aura® Core Components Overview and Architecture | 4 |
| Maintenance and Troubleshooting | 9 |
| Security and Compliance Fundamentals | 5 |
| System Administration and Management | 7 |
| User and Feature Support | 5 |

---

### **Avaya Aura® Core Components Overview and Architecture**

### 1. Which Avaya Aura component functions as the central SIP routing engine?

- [ ] **A)** Session Manager
- [ ] **B)** Communication Manager
- [ ] **C)** System Manager
- [ ] **D)** Media Server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Session Manager is the SIP routing engine that manages session control and routing policies.
 
 
</details>

### 2. Which two protocols allow endpoint registration within Avaya Aura?

- [ ] **A)** SIP
- [ ] **B)** H.323
- [ ] **C)** MGCP
- [ ] **D)** HTTP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Endpoints register via SIP with Session Manager or via H.323 with Communication Manager. MGCP only controls gateways.
 
 
</details>

### 3. Based on the provided SIP INVITE, which component is the initial sender of this message in a basic Avaya Aura call flow?

```text
INVITE sip:1002@domain.com SIP/2.0
Via: SIP/2.0/UDP 10.10.10.1:5060
From: <sip:1001@domain.com>;tag=12345
To: <sip:1002@domain.com>
Call-ID: abc123@10.10.10.1
CSeq: 1 INVITE
Contact: <sip:1001@10.10.10.1:5060>
```

- [ ] **A)** Phone A
- [ ] **B)** Session Manager
- [ ] **C)** Communication Manager
- [ ] **D)** Media Server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The INVITE originates from the calling endpoint (Phone A) to its configured proxy, Session Manager.
 
 
</details>

### 4. What is a mandatory requirement for virtualizing Avaya Aura components?

- [ ] **A)** The hypervisor must be on the Avaya Hardware Compatibility List
- [ ] **B)** CPU oversubscription of 4:1 is acceptable
- [ ] **C)** Snapshots should be taken weekly and maintained
- [ ] **D)** Live migration can be performed at any time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Avaya requires the hypervisor to be listed on the HCL; other practices violate guidelines.
 
 
</details>


---

### **Maintenance and Troubleshooting**

### 5. What is the recommended method for backing up Avaya Aura System Manager?

- [ ] **A)** Secure copy to an external server
- [ ] **B)** FTP to local disk
- [ ] **C)** USB flash drive
- [ ] **D)** HTTP to internal web server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Avaya recommends SCP (Secure Copy) for System Manager backups to ensure encryption and security.
 
 
</details>

### 6. Which two statements describe a full system backup in Avaya Aura?

- [ ] **A)** Includes operating system and applications
- [ ] **B)** Hardware-dependent restore
- [ ] **C)** Quick rollback for misconfigurations
- [ ] **D)** Can be restored to any hardware

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A full system backup captures OS and apps and must be restored to identical hardware; configuration-only backups are for quick rollbacks.
 
 
</details>

### 7. Review the backup command output. What does it indicate about the backup status?

```bash
# Example backup command output
Backup started: 2025-04-07 22:00:00
Checking disk space: OK
Copying files...
Backup completed successfully.

```

- [ ] **A)** The backup completed successfully
- [ ] **B)** The backup failed due to insufficient disk space
- [ ] **C)** The backup is still in progress
- [ ] **D)** The backup was not started

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The output shows no errors and a success message, indicating the backup completed without issues.
 
 
</details>

### 8. Which alarm severity in Avaya Aura requires immediate action and indicates a service outage?

- [ ] **A)** Critical
- [ ] **B)** Major
- [ ] **C)** Minor
- [ ] **D)** Warning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Critical severity alarms indicate a service outage requiring immediate action, as defined in the playbook.
 
 
</details>

### 9. Which alarm IDs are associated with common conditions in Avaya Aura? (Select two)

- [ ] **A)** 113 – Link Down
- [ ] **B)** 245 – License Violation
- [ ] **C)** 101 – CPU Overload
- [ ] **D)** 999 – System Restart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Common Avaya alarm IDs include 113 (link down) and 245 (license violation), as per the playbook.
 
 
</details>

### 10. Review the CLI output for clearing alarms. What does the command do?

```bash
avaya alarm clear

```

- [ ] **A)** Acknowledges the most recent alarm
- [ ] **B)** Clears all alarms on System Manager
- [ ] **C)** Lists all active alarms
- [ ] **D)** Restarts the alarm manager service

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The command 'avaya alarm clear' is used to clear alarms on System Manager, as shown in the playbook.
 
 
</details>

### 11. Which command in Communication Manager is used to trace a specific station's call flow?

- [ ] **A)** list trace station
- [ ] **B)** trace station
- [ ] **C)** trace trunk
- [ ] **D)** display trace

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The correct command is 'trace station' followed by the extension number to trace a specific station's calls.
 
 
</details>

### 12. Which two factors commonly cause one-way audio in Avaya Aura?

- [ ] **A)** NAT not properly handled
- [ ] **B)** Incorrect codec negotiation
- [ ] **C)** Firewall blocking media ports
- [ ] **D)** DNS resolution failure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> One-way audio is often due to NAT traversal issues or firewall blocking RTP port ranges, as per the playbook.
 
 
</details>

### 13. Review this trace output snippet. What does the 'RELEASING' event indicate?

```text
Event: RELEASING
Timestamp: 14:23:45

```

- [ ] **A)** The call is being connected
- [ ] **B)** The call is being terminated
- [ ] **C)** The call is on hold
- [ ] **D)** The call is ringing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In Avaya traces, 'RELEASING' indicates the call is being disconnected, as defined in the playbook.
 
 
</details>


---

### **Security and Compliance Fundamentals**

### 14. What is the main function of Transport Layer Security (TLS) in an Avaya Aura environment?

- [ ] **A)** Encrypt SIP signaling messages
- [ ] **B)** Encrypt media (RTP) streams
- [ ] **C)** Compress call data to save bandwidth
- [ ] **D)** Authenticate users via LDAP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TLS encrypts and authenticates SIP signaling (headers and SDP). Media encryption requires SRTP, not TLS.
 
 
</details>

### 15. Which two components are part of a defense-in-depth security strategy for Avaya Aura?

- [ ] **A)** Network segmentation with VLANs
- [ ] **B)** A single firewall rule permitting all traffic
- [ ] **C)** OS hardening (e.g. disabling root SSH)
- [ ] **D)** Using a shared administrative account

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Defense-in-depth combines multiple controls. VLAN segmentation and OS hardening are two distinct layers; a single rule or shared account weakens security.
 
 
</details>

### 16. Review the log entry below. What is the most likely cause of this error?

```log
2025-03-20 10:15:32 ERROR [SessionManager] TLS handshake with 10.1.20.5:5061 failed: Certificate verification failed – unable to verify the first certificate.
```

- [ ] **A)** Network connectivity loss
- [ ] **B)** Expired certificate in the trust chain
- [ ] **C)** Incorrect administrator password
- [ ] **D)** Firewall blocking port 5061

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The message 'Certificate verification failed' is a typical TLS handshake error caused by an expired or untrusted certificate.
 
 
</details>

### 17. Which TCP port is the default for encrypted SIP signaling in Avaya Aura?

- [ ] **A)** 5060
- [ ] **B)** 5061
- [ ] **C)** 8443
- [ ] **D)** 1720

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SIP over TLS uses port 5061. Port 5060 is for unencrypted SIP (UDP/TCP), 8443 is for System Manager web, 1720 is for H.323.
 
 
</details>

### 18. Which two security controls are classified as preventative in nature?

- [ ] **A)** Role-Based Access Control (RBAC)
- [ ] **B)** Audit logs and log monitoring
- [ ] **C)** Firewall rules restricting traffic
- [ ] **D)** Disaster recovery backups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> RBAC and firewall rules are preventative – they block actions. Audit logs are detective; backups are corrective.
 
 
</details>


---

### **System Administration and Management**

### 19. What must be configured before a System Manager license can be generated?

- [ ] **A)** Set the SMGR IP address via console menu
- [ ] **B)** Set the license password via console menu
- [ ] **C)** Enroll Communication Manager
- [ ] **D)** Configure NTP servers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The license password must be set at first boot via the console menu; otherwise, the license file will not match.
 
 
</details>

### 20. Which two passwords are set during the initial console configuration of System Manager? (Choose two.)

- [ ] **A)** craft
- [ ] **B)** admin
- [ ] **C)** root
- [ ] **D)** guest

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The console configuration sets the craft and root passwords. The admin password is set later via web UI.
 
 
</details>

### 21. Refer to the console menu below. Which option is used to configure network settings?

```text
Console Configuration Menu
1. Settings
   1.1 Network
   1.2 Time
2. Licensing
3. User Management
4. Security
```

- [ ] **A)** Settings > Network
- [ ] **B)** Settings > Time
- [ ] **C)** Licensing > License and Host ID
- [ ] **D)** User Management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The console menu's Settings > Network option is used to assign static IP, subnet, and gateway.
 
 
</details>

### 22. What is the purpose of the Communication Profile in System Manager?

- [ ] **A)** To store the user's personal phone call history
- [ ] **B)** To hold Avaya-specific telephony settings such as extension and station association
- [ ] **C)** To manage the user's email and calendar settings
- [ ] **D)** To define the user's LDAP authentication credentials

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Communication Profile contains telephony settings including Communication Profile Numbers and associated stations.
 
 
</details>

### 23. Which two elements are required to successfully register a station via System Manager? (Choose two.)

- [ ] **A)** A user record with a Communication Profile Number assigned
- [ ] **B)** A station object with a matching MAC address and type
- [ ] **C)** An active SIP trunk to the PSTN
- [ ] **D)** A completed backup of the System Manager database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Registration requires a user with CPN and a station object. The station must have correct MAC and set type.
 
 
</details>

### 24. Review the station template configuration below. What does this template define?

```text
Station Template: 9608G_Standard
Station Type: 9608G
Button 1: Line Appearance
Button 2: Call Forwarding
Button 3: Do Not Disturb
Feature Entitlement: Bridge Appearance
```

- [ ] **A)** The physical phone's key layout and feature entitlements
- [ ] **B)** The user's email address and SIP credentials
- [ ] **C)** The System Manager LDAP integration parameters
- [ ] **D)** The trunk group access code for external calls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Station templates define button assignments, feature keys, and station type for Avaya endpoints.
 
 
</details>

### 25. Which component defines the IP address of the remote SIP peer for a trunk?

- [ ] **A)** SIP Trunk Group
- [ ] **B)** SIP Signaling Group
- [ ] **C)** AAR Digit Manipulation Table
- [ ] **D)** Session Admission Control Policy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The signaling group defines the near-end and far-end IP addresses and transport protocol for SIP trunks.
 
 
</details>


---

### **User and Feature Support**

### 26. What is the primary function of an auto attendant in Avaya Aura?

- [ ] **A)** Route calls based on time of day.
- [ ] **B)** Act as an automated receptionist with menu options.
- [ ] **C)** Distribute calls to agents in a hunt group.
- [ ] **D)** Forward calls to voicemail when busy.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> An auto attendant presents callers with a menu and routes calls using DTMF detection, acting as a virtual receptionist.
 
 
</details>

### 27. Which of the following are valid types of call forwarding in Avaya Aura? (Choose three)

- [ ] **A)** Immediate (CFU)
- [ ] **B)** On Busy (CFB)
- [ ] **C)** On No Answer (CFNA)
- [ ] **D)** On Do Not Disturb (CFDND)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Avaya Aura supports CFU, CFB, and CFNA. 'On DND' is not a standard call forwarding type.
 
 
</details>

### 28. Refer to the code block. What does vector step 2 do?

```avaya-vector
Step 1: announcement greeting
Step 2: collect 1 digit timeout 5
Step 3: route-to based-on digit
```

- [ ] **A)** Plays an announcement.
- [ ] **B)** Collects a single digit from the caller.
- [ ] **C)** Routes the call to a specific extension.
- [ ] **D)** Disconnects the call.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 'collect' step waits for a DTMF digit with a timeout, used for menu selection.
 
 
</details>

### 29. What does MWI stand for in Avaya Aura Messaging integration?

- [ ] **A)** Message Waiting Indicator
- [ ] **B)** Main Window Interface
- [ ] **C)** Media Wire Integrity
- [ ] **D)** Management Web Interface

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MWI (Message Waiting Indicator) signals to users that a new voicemail is available, often via a lamp or stutter tone.
 
 
</details>

### 30. Which two Avaya Aura components are directly involved in voicemail call coverage routing?

- [ ] **A)** Communication Manager (CM)
- [ ] **B)** Session Manager (SM)
- [ ] **C)** System Manager (SMGR)
- [ ] **D)** Avaya Aura Contact Center (AACC)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CM sends calls to coverage paths via trunks/SIP, and SM routes those calls to the voicemail server.
 
 
</details>

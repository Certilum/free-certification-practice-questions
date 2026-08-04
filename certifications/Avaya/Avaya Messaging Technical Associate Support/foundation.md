<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Avaya/Avaya%20Messaging%20Technical%20Associate%20Support" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Avaya Messaging Technical Associate Support</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Administration and Maintenance](#administration-and-maintenance) (7 questions)
- [Installation and Configuration](#installation-and-configuration) (8 questions)
- [Messaging Platforms and Architecture](#messaging-platforms-and-architecture) (6 questions)
- [Security and Best Practices](#security-and-best-practices) (3 questions)
- [Troubleshooting and Support](#troubleshooting-and-support) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:27.136Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Administration and Maintenance | 7 |
| Installation and Configuration | 8 |
| Messaging Platforms and Architecture | 6 |
| Security and Best Practices | 3 |
| Troubleshooting and Support | 6 |

---

### **Administration and Maintenance**

### 1. Which interface is primarily used for user creation and provisioning in Avaya Messaging?

- [ ] **A)** System Manager
- [ ] **B)** Messaging Administration
- [ ] **C)** Command line on Messaging Server
- [ ] **D)** Avaya Support website

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> System Manager (SMGR) is the authoritative source for user creation and provisioning; Messaging Admin works with existing users.
 
 
</details>

### 2. Which two tasks are performed in Messaging Administration but not in System Manager?

- [ ] **A)** Modify mailbox Class of Service
- [ ] **B)** Reset Message Waiting Indicator
- [ ] **C)** Create new user accounts
- [ ] **D)** Manage RBAC roles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Messaging Administration handles mailbox COS and MWI reset; user creation and RBAC are System Manager functions.
 
 
</details>

### 3. Examine the command output. What does the 'Warning' threshold indicate about the mailbox?

```text
Quota Status for mailbox user01:
  Hard Quota: 500 MB
  Soft Quota: 100% of Hard
  Warning: 90% of Hard
  Current Size: 460 MB
```

- [ ] **A)** User receives notification but can still receive messages
- [ ] **B)** New message delivery is rejected
- [ ] **C)** Mailbox is automatically archived
- [ ] **D)** System sends critical alert to administrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Warning threshold triggers a user notification but does not block new message delivery; only Hard Quota blocks delivery.
 
 
</details>

### 4. What is the default polling interval for performance metrics collection in Avaya Messaging?

- [ ] **A)** Every 60 seconds
- [ ] **B)** Every 30 seconds
- [ ] **C)** Every 5 minutes
- [ ] **D)** Every 15 minutes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The system collects metrics every 60 seconds by default, as stated in the playbook for performance monitoring.
 
 
</details>

### 5. Which two conditions must be met for an alarm state to change to Yellow in Avaya Messaging?

- [ ] **A)** A sustained Warning condition over a time window
- [ ] **B)** A single transient warning event
- [ ] **C)** The threshold breach must last at least 5 minutes
- [ ] **D)** A Critical alarm is logged

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Yellow state requires a sustained Warning over a time window (typically 5 minutes), not a single transient event.
 
 
</details>

### 6. Review the log snippet. Which backup scope does this command represent?

```bash
root@server:~# avaya_backup --full --output /backup/avaya/ --messages
```

- [ ] **A)** Full backup with messages option
- [ ] **B)** Database-only backup
- [ ] **C)** Incremental backup
- [ ] **D)** Configuration-only backup

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command 'avaya_backup --full --output /backup/avaya/ --messages' includes both database and voice messages.
 
 
</details>

### 7. What must be performed before a patch rollback that modified the database schema?

- [ ] **A)** Restore from a full system backup
- [ ] **B)** Use PMU rollback function only
- [ ] **C)** Reapply the prerequisite patches
- [ ] **D)** Perform a mailbox export

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Schema-changing patches require a full backup restore for rollback because PMU rollback cannot revert database changes.
 
 
</details>


---

### **Installation and Configuration**

### 8. What is the default SIP port used by Avaya Aura Messaging (AAM) during initial installation and configuration?

- [ ] **A)** 5060
- [ ] **B)** 5000
- [ ] **C)** 443
- [ ] **D)** 446

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> According to the Avaya documentation, Avaya Aura Messaging uses TCP port 5060 for SIP communication. Port 5000 is used by Voicemail Pro for web admin, port 443 is used for HTTPS, and port 446 is used for internal AAM admin.
 
 
</details>

### 9. Which of the following are required pre-installation steps for Avaya Aura Messaging on a Windows Server? (Choose two.)

- [ ] **A)** Enable .NET Framework 4.7 and IIS features
- [ ] **B)** Install SQL Server Standard Edition with mixed-mode authentication
- [ ] **C)** Join the server to a workgroup only (no domain)
- [ ] **D)** Install the Avaya license file before running the installer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Avaya Aura Messaging requires .NET Framework 4.7 and IIS roles/features to be enabled, and it needs a supported SQL Server edition with mixed-mode authentication. Joining a domain is recommended, not a workgroup. The license file is imported after installation, not before.
 
 
</details>

### 10. Review the following SQL Server configuration. Which step must be completed before the Avaya Aura Messaging installer can create the database?

```sql
-- SQL Server is installed with default settings. The AAM installer on a different server fails with 'cannot connect to database server'.
```

- [ ] **A)** Enable TCP/IP protocol in SQL Server Configuration Manager
- [ ] **B)** Install the SQL Server Management Studio (SSMS) only
- [ ] **C)** Create a database named 'AAM_DB' manually
- [ ] **D)** Set SQL Server to listen on port 1434 only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> By default, SQL Server Express does not allow remote TCP/IP connections. The TCP/IP protocol must be enabled in SQL Server Configuration Manager (and the service restarted) so that the AAM installer can connect to the database server. SSMS is not required for the connection. The database is created by the installer automatically.
 
 
</details>

### 11. In Avaya Aura Messaging, which service must be started first after installation to ensure the Messaging Application Server (MAS) can function?

- [ ] **A)** Database Connection Service
- [ ] **B)** Messaging Application Server
- [ ] **C)** SIP Listener
- [ ] **D)** Web Admin

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Database Connection Service must be running before the Messaging Application Server (MAS) can access the backend database. MAS depends on the database to start. The SIP Listener and Web Admin are started after MAS is operational.
 
 
</details>

### 12. Which two configurations are essential for an Avaya Aura Messaging mailbox's initial setup?

- [ ] **A)** Class of Service (COS) assignment
- [ ] **B)** Primary greeting recording
- [ ] **C)** Schedule table attachment
- [ ] **D)** Email notification SMTP server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Every mailbox requires a Class of Service (COS) to define permissions and limits, and a schedule table to control which greeting is played at different times. The primary greeting can be recorded later. Email notification is optional and depends on the COS.
 
 
</details>

### 13. Study the following subscription scenario. What is the most likely reason the user cannot receive email notifications?

```plaintext
User profile: COS = 'Standard-CO', email = user@company.com, mailbox type = Full. Global SMTP settings: server = mail.company.com, port=25. User reports: 'I never receive voicemail notifications via email.'
```

- [ ] **A)** The COS assigned to the user does not allow email notification
- [ ] **B)** The user's extension is not registered in the telephone system
- [ ] **C)** The SMTP server is not configured in the messaging platform
- [ ] **D)** The mailbox is full and cannot send notifications

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Email notification is a feature that must be enabled at the Class of Service (COS) level. Even if the SMTP server is configured globally, if the user's COS disables notification, no emails will be sent. The extension registration and mailbox capacity are unrelated to notification delivery.
 
 
</details>

### 14. When configuring an auto attendant in Avaya Messaging, what must the auto attendant mailbox have to allow menu navigation?

- [ ] **A)** Allow Touch-Tone Commands / Menu Navigation
- [ ] **B)** Allow Message Forwarding
- [ ] **C)** Allow External Transfer
- [ ] **D)** Allow Broadcast Messages

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> For an auto attendant mailbox to respond to caller DTMF digits and navigate menus, the COS must have a setting that permits touch-tone commands or menu navigation. Without it, the system treats the mailbox as a simple voicemail box and plays only the greeting.
 
 
</details>

### 15. Which two of the following are steps in the user provisioning process for Avaya Messaging?

- [ ] **A)** Assign a Class of Service (COS) to the subscriber
- [ ] **B)** Create a mailbox with a unique extension
- [ ] **C)** Configure the SMTP relay for the whole system
- [ ] **D)** Enable call forwarding on the telephone system

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Each new subscriber must be assigned a Class of Service and have a mailbox created with a unique extension. SMTP relay is a global setting, not per-subscriber. Call forwarding is a telephone system feature, not part of Messaging user provisioning.
 
 
</details>


---

### **Messaging Platforms and Architecture**

### 16. Which Avaya product is a web-based client that provides unified messaging access to voicemail, email, and fax?

- [ ] **A)** Avaya Aura Messaging
- [ ] **B)** IP Office Voicemail Pro
- [ ] **C)** Avaya one-X Portal
- [ ] **D)** Avaya System Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Avaya one-X Portal is a web-based unified messaging client that provides access to voicemail, email, and fax. It is not a messaging backend; it requires a platform like Aura Messaging or IP Office to function.
 
 
</details>

### 17. Which of the following statements correctly describe Avaya Aura Messaging? (Choose two.)

- [ ] **A)** It supports up to 300,000 mailboxes.
- [ ] **B)** It runs on a Windows operating system.
- [ ] **C)** It uses SIP registration for integration with Session Manager.
- [ ] **D)** It provides a drag-and-drop call flow editor.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Avaya Aura Messaging is a Linux-based enterprise solution supporting up to 300,000 users and integrates via SIP with Session Manager. The drag-and-drop call flow editor is a feature of IP Office Voicemail Pro, not Aura Messaging.
 
 
</details>

### 18. A user reports they can dial into voicemail but cannot access it through a web browser. Logging into the portal server, you see the following status. Which component is most likely at fault?

```text
Service 'Apache Tomcat' is stopped.
Startup type: Automatic
Current status: Stopped
```

- [ ] **A)** Avaya Aura Messaging server
- [ ] **B)** IP Office Voicemail Pro
- [ ] **C)** Avaya one-X Portal server
- [ ] **D)** Avaya Communication Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Because the user can still access voicemail via phone (TUI), the messaging backend is working. The portal (one-X Portal) is the interface for web access; its service being stopped explains the issue. Always check the portal server when web access fails but phone access works.
 
 
</details>

### 19. In an Avaya Aura Messaging environment, which tool is specifically used for backup and restore of messaging data?

- [ ] **A)** System Manager
- [ ] **B)** Enterprise Management System (EMS)
- [ ] **C)** Session Manager
- [ ] **D)** Avaya one-X Portal Admin

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> EMS (Enterprise Management System) is the dedicated backup/restore tool for Avaya Aura Messaging. System Manager is for administration and provisioning, not for backup. Session Manager handles SIP routing, and one-X Portal Admin manages the portal configuration.
 
 
</details>

### 20. Which two signaling protocols are commonly used for integrating Avaya Aura Messaging with Avaya Aura Communication Manager?

- [ ] **A)** SIP
- [ ] **B)** H.323
- [ ] **C)** PRI (Q.931)
- [ ] **D)** FXS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Avaya Aura Messaging integrates primarily via SIP trunking and also supports H.323 for legacy implementations. PRI is a digital trunk technology that uses Q.931 signaling, but the question asks for signaling protocols; PRI itself is not a protocol but an interface. FXS is an analog interface type, not a signaling protocol.
 
 
</details>

### 21. A technician is troubleshooting Message Waiting Indicator (MWI) and captures the following SIP exchange between Aura Messaging and Session Manager. What does this response indicate?

```text
SUBSCRIBE sip:user@domain.com SIP/2.0
To: <sip:user@domain.com>
From: <sip:notifier@domain.com>;tag=abc123
Event: message-summary

SIP/2.0 200 OK
To: <sip:user@domain.com>;tag=def456
From: <sip:notifier@domain.com>;tag=abc123
```

- [ ] **A)** The MWI lamp on the phone is now lit.
- [ ] **B)** The MWI subscription was successfully accepted.
- [ ] **C)** The message was deleted from the mailbox.
- [ ] **D)** The messaging server is not reachable.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A 200 OK response to a SUBSCRIBE message indicates that the subscription request was approved by the notifier (Aura Messaging). It does not guarantee the lamp is lit; that requires a subsequent NOTIFY with message-waiting status. The 200 OK confirms the subscription establishment.
 
 
</details>


---

### **Security and Best Practices**

### 22. What is the primary objective of security hardening for Avaya messaging servers?

- [ ] **A)** Increase processing speed
- [ ] **B)** Reduce attack surface and apply least-privilege
- [ ] **C)** Enable all optional services
- [ ] **D)** Disable all network encryption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Security hardening reduces the attack surface by removing non-essential services and applying least-privilege principles.
 
 
</details>

### 23. Which two elements must be included in an audit trail entry according to Avaya best practices?

- [ ] **A)** Timestamp of the event
- [ ] **B)** User ID of the actor
- [ ] **C)** Full message content
- [ ] **D)** Password hash of the user

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Avaya best practices require audit logs to include timestamps and user identification to ensure non-repudiation.
 
 
</details>

### 24. Refer to the SDP code snippet. What encryption protocol is indicated for the media stream?

```sdp
a=crypto:1 AES_CM_128_HMAC_SHA1_80 inline:9uEN2B8QI0gWq+2C5YnTpA==
```

- [ ] **A)** TLS
- [ ] **B)** SRTP
- [ ] **C)** LDAPS
- [ ] **D)** S/MIME

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The presence of 'a=crypto:1 AES_CM_128_HMAC_SHA1_80' in the SDP body indicates that SRTP is being used to encrypt the media.
 
 
</details>


---

### **Troubleshooting and Support**

### 25. Which error code indicates an LDAP connection timeout in Avaya Messaging?

- [ ] **A)** 16001
- [ ] **B)** 18002
- [ ] **C)** 19004
- [ ] **D)** 20001

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Error code 18002 specifically denotes an LDAP connection timeout, as stated in the key concepts for logon failure root causes.
 
 
</details>

### 26. Which of the following are common causes of media problems (e.g., garbled audio) during voicemail capture? (Select all that apply.)

- [ ] **A)** Codec mismatch between endpoint and messaging server
- [ ] **B)** Firewall blocking RTP ports (e.g., 5000-5999 UDP)
- [ ] **C)** Insufficient disk I/O on the messaging application server
- [ ] **D)** Improper SMTP relay configuration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Media problems often stem from codec mismatches, firewall interference with RTP, or disk I/O bottlenecks during recording. SMTP relay issues affect message delivery, not media quality.
 
 
</details>

### 27. Review the following command used for SIP message tracing. What does this command do?

```bash
traceSM -u 5000
```

- [ ] **A)** Captures SIP signaling for extension 5000
- [ ] **B)** Displays system event logs for the messaging server
- [ ] **C)** Shows the status of all messaging ports
- [ ] **D)** Traces message delivery flow for a specific mailbox

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command `traceSM -u 5000` captures SIP signaling for extension 5000, allowing analysis of call setup and teardown.
 
 
</details>

### 28. What is the first layer to check when a user cannot log into voicemail?

- [ ] **A)** Authentication and directory synchronization
- [ ] **B)** Network connectivity and firewall rules
- [ ] **C)** Media codec configuration
- [ ] **D)** SMTP relay settings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Logon failures primarily involve authentication or directory issues; other layers like network or media are secondary.
 
 
</details>

### 29. Which of the following are symptoms of a message delivery delay? (Select all that apply.)

- [ ] **A)** Growing queue depth on the Message Delivery Status Dashboard
- [ ] **B)** DNS resolution failures for external domains
- [ ] **C)** Users hear silence or robotic speech when leaving a message
- [ ] **D)** SMTP relay throttling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Queue depth increase, DNS failures, and SMTP throttling cause delays. Audio issues indicate media problems, not delivery delays.
 
 
</details>

### 30. The following log snippet shows an error. Based on the error code, what is the most likely cause?

```text
ERR-19004: Media timeout occurred for call ID 12345
```

- [ ] **A)** Media timeout due to idle session or network interruption
- [ ] **B)** Authentication failure with LDAP
- [ ] **C)** SMTP queue full
- [ ] **D)** Mailbox quota exceeded

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Error code 19004 corresponds to a media timeout, often caused by an idle session (e.g., call on hold) or network interruption.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Avaya/Avaya%20Experience%20Portal%20with%20Proactive%20Outreach%20Manager%20Technical%20Associate%20Support" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Avaya Experience Portal with POM Technical Associate Support</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [AEP and POM Installation and Configuration](#aep-and-pom-installation-and-configuration) (8 questions)
- [Application and Script Management](#application-and-script-management) (6 questions)
- [Avaya Experience Portal (AEP) and POM Fundamentals](#avaya-experience-portal-aep-and-pom-fundamentals) (6 questions)
- [System Administration and Maintenance](#system-administration-and-maintenance) (6 questions)
- [Troubleshooting and Technical Support](#troubleshooting-and-technical-support) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:21.994Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| AEP and POM Installation and Configuration | 8 |
| Application and Script Management | 6 |
| Avaya Experience Portal (AEP) and POM Fundamentals | 6 |
| System Administration and Maintenance | 6 |
| Troubleshooting and Technical Support | 4 |

---

### **AEP and POM Installation and Configuration**

### 1. Which of the following must be verified BEFORE starting the installation of Avaya Experience Portal (AEP)?

- [ ] **A)** Activate the license file for AEP
- [ ] **B)** Verify the Product Compatibility Matrix
- [ ] **C)** Install Presence of Mind (POM) first
- [ ] **D)** Create agent logins in the system

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> According to the playbook, the Product Compatibility Matrix (PCM) must be verified before installation to ensure all components are compatible. Licensing activation occurs after installation, POM is installed after AEP, and agent logins are created post-deployment.
 
 
</details>

### 2. Which of the following are core components of Avaya Experience Portal (AEP)? (Select two.)

- [ ] **A)** Media Server
- [ ] **B)** Application Server
- [ ] **C)** Database Server
- [ ] **D)** Session Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The AEP core components are Media Server, Application Server, and Management Console. Database Server is external, and Session Manager is part of Avaya Aura ecosystem but not a core AEP component.
 
 
</details>

### 3. Examine the following extracted line from a POM configuration file. What does this setting control?

```properties
lockout.maxAttempts=5
```

- [ ] **A)** The heartbeat interval between POM and managed nodes
- [ ] **B)** The maximum number of failed login attempts before account lockout
- [ ] **C)** The encryption cipher suite for TLS connections
- [ ] **D)** The logging level for POM audit trails

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The parameter 'lockout.maxAttempts' in a configuration file like LoginSecurity.properties controls the number of failed login attempts before the account is locked. The snippet demonstrates a security policy parameter.
 
 
</details>

### 4. What happens when an Avaya Experience Portal license limit is exceeded?

- [ ] **A)** New calls are immediately rejected with a 503 error
- [ ] **B)** The system continues to operate for a grace period of 30 days
- [ ] **C)** The license becomes permanently invalid and must be replaced
- [ ] **D)** All existing calls are terminated instantly

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AEP licenses are enforced as soft limits. When exceeded, a critical event is logged and the system enters a 30-day grace period before enforcing restrictions. Immediate rejection or termination is not standard behavior.
 
 
</details>

### 5. Which protocols must be explicitly allowed through the firewall for proper Avaya AEP operation? (Select two.)

- [ ] **A)** SIP (UDP/TCP 5060)
- [ ] **B)** RTP (UDP 16384-32767)
- [ ] **C)** HTTP (TCP 80)
- [ ] **D)** FTP (TCP 21)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SIP is used for signaling and RTP for media. HTTP may be used for management but is not essential for core call processing. FTP is not standard for AEP operation.
 
 
</details>

### 6. The following snippet is from an AEP installation log. What does the highlighted entry indicate?

```text
ERROR [LicenseManager] License validation failed: HOSTID mismatch. Expected: a1b2c3d4e5f6, got: f6e5d4c3b2a1.
```

- [ ] **A)** Network interface configuration is complete
- [ ] **B)** License file upload failed due to HOSTID mismatch
- [ ] **C)** Media Server role assignment was successful
- [ ] **D)** Application Server registration with Media Server succeeded

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The log message 'License validation failed: HOSTID mismatch' indicates that the license file's HOSTID does not match the server's MAC address. This is a common error during license activation after installation.
 
 
</details>

### 7. Which AEP component is responsible for handling voice prompts, speech recognition, and DTMF detection?

- [ ] **A)** Media Server
- [ ] **B)** Application Server
- [ ] **C)** Management Console
- [ ] **D)** Resource Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Media Server handles all media-related functions including voice prompts, speech recognition, and DTMF detection. The Application Server runs call flows, Management Console provides GUI, and Resource Manager allocates channels.
 
 
</details>

### 8. Which of the following are capabilities provided by Platform Operations Manager (POM)? (Select two.)

- [ ] **A)** Centralized monitoring of all AEP nodes
- [ ] **B)** License management and tracking
- [ ] **C)** IVR application development
- [ ] **D)** Agent desktop softphone integration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> POM provides centralized monitoring (dashboards, alerts) and license management for both AEP and POM. IVR development is done in Orchestration Designer, and agent desktop integration is provided by POM's presence features, but not a core POM function.
 
 
</details>


---

### **Application and Script Management**

### 9. What is the primary purpose of VoiceXML in Avaya Experience Portal?

- [ ] **A)** Manage call control events
- [ ] **B)** Handle user interaction with prompts and input
- [ ] **C)** Control network-level call bridging
- [ ] **D)** Deploy applications via POM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> VoiceXML handles the user interaction layer (prompts, DTMF, speech), while CCXML manages telephony control.
 
 
</details>

### 10. Which two functions are performed by CCXML scripts? (Choose two)

- [ ] **A)** Play audio prompts
- [ ] **B)** Place and bridge calls
- [ ] **C)** Collect DTMF input
- [ ] **D)** Monitor call state events

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> CCXML controls call setup, bridging, and event monitoring; VoiceXML handles prompts and input.
 
 
</details>

### 11. Refer to the VoiceXML snippet. What is missing for robust error handling?

```xml
<field name="digits">
  <prompt>Please enter your PIN.</prompt>
  <grammar src="grammars/pin.gram" type="application/srgs+xml"/>
  <filled>...</filled>
</field>
```

- [ ] **A)** A <nomatch> handler
- [ ] **B)** A <catch> for error.badfetch
- [ ] **C)** A <noinput> handler
- [ ] **D)** Both noinput and nomatch handlers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> Without noinput and nomatch handlers, the caller may be stuck if no input or invalid input is received.
 
 
</details>

### 12. In POM, where are application script files uploaded?

- [ ] **A)** Resources tab
- [ ] **B)** Manifest tab
- [ ] **C)** Activation tab
- [ ] **D)** Service Number configuration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Resources tab in POM is used to upload all application files including scripts, prompts, and grammars.
 
 
</details>

### 13. Which two actions are required to roll back a script version in POM? (Choose two)

- [ ] **A)** Re-upload the old script file
- [ ] **B)** Update application's script association to a prior version
- [ ] **C)** Restart the AEP service
- [ ] **D)** Activate the previous version via version history

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Rollback involves selecting a prior version in the application's script association and activating that version.
 
 
</details>

### 14. Given the CCXML snippet, which event handler is missing to prevent resource leaks?

```xml
<ccxml version="1.0">
  <eventprocessor>
    <transition event="connection.alerting">
      <accept/>
    </transition>
    <!-- missing handler -->
  </eventprocessor>
</ccxml>
```

- [ ] **A)** connection.connected
- [ ] **B)** connection.disconnected
- [ ] **C)** connection.failed
- [ ] **D)** connection.redirect

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> connection.disconnected handler ensures resources are released when a call ends.
 
 
</details>


---

### **Avaya Experience Portal (AEP) and POM Fundamentals**

### 15. Which AEP component terminates SIP trunks and processes media streams?

- [ ] **A)** Application Server (AS)
- [ ] **B)** Media Processing Platform (MPP)
- [ ] **C)** Management Console (MC)
- [ ] **D)** Portal Object Manager (POM)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The MPP is the media-handling component that terminates SIP trunks and processes RTP streams.
 
 
</details>

### 16. Select the two AEP components that do not handle call media or application logic.

- [ ] **A)** Media Processing Platform (MPP)
- [ ] **B)** Application Server (AS)
- [ ] **C)** Portal Object Manager (POM)
- [ ] **D)** Management Console (MC)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C, D**
 
> 💡  **Explanation** 
> 
> POM provides monitoring and reporting; MC provides configuration. Neither handles media or application logic.
 
 
</details>

### 17. Which component generated the following log entry?

```log
2019-03-21 10:00:00 [MPP] RTP stream established with codec G.711
```

- [ ] **A)** Application Server
- [ ] **B)** Media Processing Platform
- [ ] **C)** Management Console
- [ ] **D)** Portal Object Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> MPP logs record RTP stream establishment. Other components do not generate such media logs.
 
 
</details>

### 18. Which component provides centralized policy definition for AEP?

- [ ] **A)** System Manager
- [ ] **B)** Application Server
- [ ] **C)** Portal Object Manager (POM)
- [ ] **D)** Session Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> POM is the policy orchestrator for AEP, managing policies and deployments.
 
 
</details>

### 19. Select two true statements about AEP call flow and media processing.

- [ ] **A)** Media Server executes VoiceXML scripts.
- [ ] **B)** Media Server uses MRCP to receive commands from Application Server.
- [ ] **C)** Session Manager handles SIP signaling.
- [ ] **D)** POM processes media streams during calls.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> The Media Server receives MRCP commands from the Application Server. The Session Manager handles SIP signaling.
 
 
</details>

### 20. Based on the alert, which AEP component is being monitored?

```text
POM Alert: AVP1 port utilization at 92%
```

- [ ] **A)** Application Server
- [ ] **B)** Media Processing Platform
- [ ] **C)** Management Console
- [ ] **D)** Database Server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AVP refers to the Avaya Voice Platform, which is the media processing component.
 
 
</details>


---

### **System Administration and Maintenance**

### 21. Which of the following tasks should be performed daily in Avaya Experience Portal maintenance?

- [ ] **A)** Run database REINDEX
- [ ] **B)** Verify service states and disk usage
- [ ] **C)** Review and purge logs older than 30 days
- [ ] **D)** Apply security patches from Avaya

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Daily health checks include verifying service states, disk usage, and log anomalies. REINDEX is monthly, log purge is weekly/monthly, patches are monthly.
 
 
</details>

### 22. Which of the following components must be included in a monthly backup of the Avaya Experience Portal? (Select all that apply.)

- [ ] **A)** AEP database (PostgreSQL/Oracle)
- [ ] **B)** Configuration XML files (call flows, settings)
- [ ] **C)** License files from Avaya
- [ ] **D)** Only the POM configuration file

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Monthly backups should cover database, config files, and licenses. POM config is also needed but not the only component; all layers must be backed up.
 
 
</details>

### 23. Refer to the following code block. What does executing this command accomplish in an Avaya Experience Portal environment?

```sql
psql -h localhost -U postgres -d aep_db -c "ANALYZE;"
```

- [ ] **A)** Start the POM service
- [ ] **B)** Perform a database backup
- [ ] **C)** Update database statistics
- [ ] **D)** Reindex all tables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The command 'ANALYZE;' updates query statistics in PostgreSQL. It is part of monthly database maintenance.
 
 
</details>

### 24. What severity level in POM logs indicates a critical failure that requires immediate attention?

- [ ] **A)** INFO
- [ ] **B)** WARN
- [ ] **C)** ERROR
- [ ] **D)** FATAL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> FATAL indicates critical component failure. ERROR may need investigation, but FATAL requires immediate action.
 
 
</details>

### 25. Which of the following user roles in Avaya Experience Portal have read-only access? (Select all that apply.)

- [ ] **A)** System Administrator
- [ ] **B)** Monitor
- [ ] **C)** Read-Only User
- [ ] **D)** Application Administrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Monitor and Read-Only User roles have no configuration rights. System Administrator and Application Administrator can modify settings.
 
 
</details>

### 26. Examine the code block. This command is used during which maintenance activity?

```sql
REINDEX TABLE session_history;
```

- [ ] **A)** Daily health check
- [ ] **B)** Weekly log rotation
- [ ] **C)** Monthly database maintenance
- [ ] **D)** Yearly capacity planning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The 'REINDEX TABLE' command is part of monthly database maintenance to rebuild indexes on high-churn tables.
 
 
</details>


---

### **Troubleshooting and Technical Support**

### 27. Which log file is primarily used to check for AEP service start failures?

- [ ] **A)** /var/log/avaya/aep/startup.log
- [ ] **B)** /var/log/avaya/pom/pom-core.log
- [ ] **C)** /var/log/avaya/aep/catalina.out
- [ ] **D)** /var/log/avaya/aep/module_sip_stack.log

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The startup.log under /var/log/avaya/aep records AEP service initialization steps and is the primary source for diagnosing start failures.
 
 
</details>

### 28. Which two commands are used to verify license status for AEP and POM respectively?

- [ ] **A)** aep-license list
- [ ] **B)** pom-license list
- [ ] **C)** aep-admin service-status
- [ ] **D)** pom-admin service-status

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> aep-license list and pom-license list are the dedicated commands to view license information on AEP and POM servers.
 
 
</details>

### 29. Examine the following log output and determine the most likely cause of the call failure.

```text
2025-01-15 14:23:10.456 ERROR [MediaServer] - No available media resources for call ID 1234
2025-01-15 14:23:10.458 ERROR [MediaServer] - Resource not available: transcoder pool exhausted
2025-01-15 14:23:10.460 WARN [SIP] - Returning 503 Service Unavailable for INVITE
```

- [ ] **A)** SIP trunk registration timeout
- [ ] **B)** Media server resource exhaustion
- [ ] **C)** Certificate expiration on the gateway
- [ ] **D)** Database connection pool exhaustion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The log shows 'No available media resources' and 'Resource not available' which points to media server capacity issues.
 
 
</details>

### 30. What default port does POM use for internal JMX communication?

- [ ] **A)** 8089
- [ ] **B)** 8443
- [ ] **C)** 4720
- [ ] **D)** 8080

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> POM uses port 8089 for internal JMX. Port 8443 is for HTTPS, 4720 for SIP, and 8080 is AEP HTTP.
 
 
</details>

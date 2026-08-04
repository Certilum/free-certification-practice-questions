<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Avaya/Avaya%20Workforce%20Engagement%20Technical%20Associate%20Support" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Avaya Workforce Engagement Technical Associate Support</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Avaya Oceana and Avaya Aura Contact Center Concepts](#avaya-oceana-and-avaya-aura-contact-center-concepts) (6 questions)
- [Avaya Workforce Optimization Solutions](#avaya-workforce-optimization-solutions) (7 questions)
- [Installation and Configuration](#installation-and-configuration) (8 questions)
- [Security and Compliance](#security-and-compliance) (3 questions)
- [Support and Troubleshooting](#support-and-troubleshooting) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:29.852Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Avaya Oceana and Avaya Aura Contact Center Concepts | 6 |
| Avaya Workforce Optimization Solutions | 7 |
| Installation and Configuration | 8 |
| Security and Compliance | 3 |
| Support and Troubleshooting | 6 |

---

### **Avaya Oceana and Avaya Aura Contact Center Concepts**

### 1. Which platform extends Avaya Aura Contact Center with omni-channel and workflow-driven capabilities?

- [ ] **A)** Avaya Oceana
- [ ] **B)** Avaya Aura Contact Center
- [ ] **C)** Avaya Workforce Management
- [ ] **D)** Avaya Session Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Avaya Oceana is the digital-first engagement platform that extends AACC with omni-channel, workflow, and workforce engagement capabilities.
 
 
</details>

### 2. Which two components are part of the Avaya Workforce Engagement ecosystem? (Choose two.)

- [ ] **A)** Avaya Interaction Recording Engine
- [ ] **B)** Avaya Quality Monitoring
- [ ] **C)** Avaya Aura Communication Manager
- [ ] **D)** Avaya Session Border Controller

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> AIRE and AQM are part of WFO/WFE. Communication Manager and SBC are core infrastructure, not WFE components.
 
 
</details>

### 3. Study the following configuration snippet. Which Avaya component must be properly configured for WFO to receive real-time agent state changes?

```text
// Example: WFO subscriber configuration
DMCC Subscriber:
  Server: 192.168.1.10
  Port: 4721
  Application: AvayaWFOV11
  License: DMCC Agent Events
```

- [ ] **A)** Avaya Aura Application Enablement Services
- [ ] **B)** Avaya Session Manager
- [ ] **C)** Avaya Oceana Experience Portal
- [ ] **D)** Avaya Communication Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AES exposes DMCC API for real-time agent state; other components do not provide this specific service.
 
 
</details>

### 4. Which technology does Avaya Oceana use to capture voice interactions for recording?

- [ ] **A)** SIPREC
- [ ] **B)** SRTP
- [ ] **C)** RTP
- [ ] **D)** WebRTC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SIPREC (Session Recording Protocol) is used by Oceana to receive forked RTP streams from the SBC for voice capture.
 
 
</details>

### 5. Which two functions are considered core contact center routing responsibilities? (Choose two.)

- [ ] **A)** Skill-based agent selection
- [ ] **B)** Call queuing and priority handling
- [ ] **C)** Generating agent schedules
- [ ] **D)** Forecasting call volumes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Skill-based routing and queuing are real-time routing actions; scheduling and forecasting are WFO functions.
 
 
</details>

### 6. Examine the rule below. This is an example of which Oceana feature that executes conditional actions based on customer data?

```text
RULE: VIP Customer Offer Callback
  IF customer.segment == "VIP" AND interaction.type == "chat" AND abandoned_count > 2 THEN
    set priority = high
    offer callback = true
```

- [ ] **A)** Smart Decisions
- [ ] **B)** Journey Profiler
- [ ] **C)** Engagement Manager
- [ ] **D)** Admin Pro

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Smart Decisions is the rule engine in Oceana that applies conditional actions based on interaction metadata.
 
 
</details>


---

### **Avaya Workforce Optimization Solutions**

### 7. What is the primary purpose of Avaya Workforce Management (WFM)?

- [ ] **A)** Record customer interactions for compliance
- [ ] **B)** Align agent staffing with predicted demand
- [ ] **C)** Analyze customer sentiment in real time
- [ ] **D)** Provide a unified agent desktop interface

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Avaya WFM aligns contact center staffing with predicted demand by forecasting volumes and scheduling agents accordingly.
 
 
</details>

### 8. Select the two forecasting horizons available in Avaya WFM.

- [ ] **A)** Long-term forecasting
- [ ] **B)** Short-term forecasting
- [ ] **C)** Real-time forecasting
- [ ] **D)** Predictive forecasting

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Avaya WFM supports long-term (strategic) and short-term (tactical) forecasting. Real-time and predictive are not standard WFM forecasting types.
 
 
</details>

### 9. Based on the configuration snippet, which WFM scheduling rule is defined?

```plaintext
SCHEDULE_RULE: 'MaxConsecutiveDays = 5'
```

- [ ] **A)** Maximum consecutive working days
- [ ] **B)** Minimum rest between shifts
- [ ] **C)** Skill assignment priority
- [ ] **D)** Agent availability threshold

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet 'MaxConsecutiveDays = 5' defines the maximum number of consecutive working days an agent can be scheduled.
 
 
</details>

### 10. What is the function of selective recording in Avaya Quality Management (AQM)?

- [ ] **A)** Records all calls for designated agents
- [ ] **B)** Records calls based on predefined triggers
- [ ] **C)** Records only calls scheduled at specific times
- [ ] **D)** Allows agents to manually start recording mid-call

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Selective recording uses predefined triggers such as agent skill or time of day to record only targeted interactions.
 
 
</details>

### 11. Which two features are part of Avaya Quality Management (AQM)?

- [ ] **A)** Evaluation forms
- [ ] **B)** Real-time adherence monitoring
- [ ] **C)** Call recording
- [ ] **D)** Forecast generation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> AQM provides call recording (selective/permanent) and evaluation forms for scoring interactions. Adherence is WFM; forecasting is WFM.
 
 
</details>

### 12. From the snippet, which AQM evaluation step is described?

```yaml
CALIBRATION_SESSION:
  threshold: 2
```

- [ ] **A)** Calibration of evaluators
- [ ] **B)** Scoring of an interaction
- [ ] **C)** Assignment of a form to a recording
- [ ] **D)** Feedback to the agent

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet 'CALIBRATION_SESSION: threshold: 2' indicates a calibration session comparing scores from multiple evaluators.
 
 
</details>

### 13. What is the primary data source for Avaya Performance Management (APM) historical reports?

- [ ] **A)** Avaya Workforce Management
- [ ] **B)** Avaya Aura Contact Center or CMS
- [ ] **C)** Avaya Interaction Analytics
- [ ] **D)** Direct from agent desktops

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> APM ingests historical data from Avaya Aura Contact Center and Avaya CMS via connectors, not from WFM or desktops.
 
 
</details>


---

### **Installation and Configuration**

### 14. What is the mandatory SQL Server collation for an Avaya Workforce Engagement deployment?

- [ ] **A)** SQL_Latin1_General_CP1_CI_AS
- [ ] **B)** Latin1_General_CI_AI
- [ ] **C)** SQL_Latin1_General_CP1_CS_AS
- [ ] **D)** Latin1_General_BIN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Avaya WE installer requires SQL_Latin1_General_CP1_CI_AS (case-insensitive, accent-sensitive) for consistent data sorting. Other collations will cause unrecoverable database inconsistencies.
 
 
</details>

### 15. Which prerequisites must be validated before installing Avaya Workforce Engagement on a Windows Server? (Select two)

- [ ] **A)** The .NET Framework 4.7.2 or later is installed
- [ ] **B)** The server has Internet access for licensing
- [ ] **C)** IIS with ASP.NET and WebSockets roles is configured
- [ ] **D)** The SQL Server Agent service is set to Manual startup

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Pre-installation validation includes verifying .NET Framework 4.7.2+ and IIS roles (ASP.NET, WebSockets). Internet access is not required for licensing (license files can be imported), and SQL Agent must be automatic, not manual.
 
 
</details>

### 16. During the installation of Avaya WE, the installer fails to connect to the SQL Server. Based on the following script snippet, what is the most likely cause?

```sql
-- Pre-check script excerpt
USE [master]
IF NOT EXISTS (SELECT * FROM sys.server_principals WHERE name = 'AWE_Setup')
BEGIN
    CREATE LOGIN [AWE_Setup] WITH PASSWORD = 'P@ssw0rd';
END
GO
-- The setup encounters: 'Login failed for user 'AWE_Setup'.'
```

- [ ] **A)** SQL Server is in Windows Authentication only mode
- [ ] **B)** SQL Server TCP/IP protocol is disabled
- [ ] **C)** The SQL Server service account lacks network access
- [ ] **D)** The .NET Framework version is too old

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The installer uses a SQL login (e.g., 'sa') to create the database. If SQL Server is configured for Windows Authentication only, the connection fails. TCP/IP disable causes 'protocol not available' error, not 'login failed' (the script shows a login error).
 
 
</details>

### 17. In a single-server Avaya WE deployment, which component is installed last?

- [ ] **A)** Client-side components such as desktop recording agents
- [ ] **B)** Database server (SQL Server)
- [ ] **C)** Core WE services (Recording, Quality Management)
- [ ] **D)** Web-based administration console

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The installation order is: database first, then core services, then web console, and finally client components. Client-side agents are installed last to ensure the server infrastructure is fully operational.
 
 
</details>

### 18. Which steps are required after a first-time installation of Avaya Workforce Management (WFM) before configuring Quality Management? (Select two)

- [ ] **A)** Define contact center parameters in WFM Admin Console
- [ ] **B)** Configure PM dashboard KPI definitions
- [ ] **C)** Run WFM-to-QM synchronization utility
- [ ] **D)** Install the Avaya License Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> After WFM install, you must define contact center parameters (forecast profiles, schedules) and then run the WFM-to-QM sync to import employee records into QM. PM dashboard configuration is a later step, and License Manager should already be installed before any module.
 
 
</details>

### 19. Analyze the following code block from a PowerShell script used during Avaya WE deployment. What does the script accomplish?

```powershell
Stop-Service w32time
w32tm /config /manualpeerlist:"time.google.com" /syncfromflags:manual /reliable:yes
Start-Service w32time
w32tm /resync
```

- [ ] **A)** It configures the Windows Time Service to use an external NTP server
- [ ] **B)** It sets the SQL Server Agent service to Automatic
- [ ] **C)** It creates a new Active Directory user for the service account
- [ ] **D)** It imports the Avaya WE license file into the licensing server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The script configures w32tm to use a reliable external NTP source (time.google.com) and sets the NT5DS synchronization type. This is a prerequisite for accurate time-stamping. The exam often tests that time synchronization must be external NTP, not domain controller only.
 
 
</details>

### 20. Which integration point is used for passive recording of SIP calls in an Avaya Aura environment with Workforce Engagement?

- [ ] **A)** SIPREC (RFC 7865)
- [ ] **B)** DMCC (Device, Media, and Call Control)
- [ ] **C)** TSAPI (Telephony Services API)
- [ ] **D)** XMPP (Extensible Messaging and Presence Protocol)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SIPREC is designed for passive recording by replicating the media stream at the Session Manager level. DMCC is for active recording, TSAPI only provides call events, and XMPP is used for presence/IM integration, not recording.
 
 
</details>

### 21. Which of the following are required when integrating Avaya Workforce Engagement with Avaya Aura for recording? (Select two)

- [ ] **A)** AES (Application Enablement Services) configured with DMCC
- [ ] **B)** A dedicated network interface for media capture
- [ ] **C)** Avaya Aura Utility Services installed on the same server
- [ ] **D)** A public internet connection for certificate validation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> AES must be configured for DMCC to provide call control and media control. A dedicated NIC (or SPAN port) is needed for passive recording to capture media without affecting the production network. Utility Services and public internet are not required.
 
 
</details>


---

### **Security and Compliance**

### 22. What encryption standard does Avaya recommend for protecting recorded media files stored on disk?

- [ ] **A)** AES-128
- [ ] **B)** AES-256
- [ ] **C)** 3DES
- [ ] **D)** RC4

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Avaya recommends AES-256 encryption for data at rest, such as recorded media files. AES-128 is considered insufficient for high-security deployments, while 3DES and RC4 are deprecated and insecure.
 
 
</details>

### 23. Which of the following are required to meet GDPR compliance when deploying Avaya Workforce Engagement? (Select all that apply.)

- [ ] **A)** Obtaining explicit consent before recording calls
- [ ] **B)** Storing all recordings indefinitely for legal purposes
- [ ] **C)** Providing data subject access to recorded interactions
- [ ] **D)** Using self-signed certificates to save costs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> GDPR requires explicit consent for recording (Article 7) and the right to access recorded data (Article 15). Indefinite storage violates data minimization, and self-signed certificates are not acceptable for production environments.
 
 
</details>

### 24. Examine the code snippet below. Which security best practice is missing from the configuration of Avaya Recording Server?

```powershell
# Example configuration snippet showing HTTPS setup with self-signed cert
$cert = New-SelfSignedCertificate -DnsName "awerecording.avaya.com" -CertStoreLocation "Cert:\LocalMachine\My"
New-WebBinding -Name "AWE Recording Site" -Protocol https -Port 443 -IPAddress "*"

```

- [ ] **A)** Enabling TLS 1.2 for management web interface
- [ ] **B)** Installing a CA-signed certificate
- [ ] **C)** Disabling unwanted Windows services
- [ ] **D)** Configuring audit logging for failed logins

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code shows a self-signed certificate being used for HTTPS. Production deployments must use a certificate signed by a trusted CA to prevent man-in-the-middle attacks.
 
 
</details>


---

### **Support and Troubleshooting**

### 25. What is the first step in the Avaya troubleshooting methodology for a recording issue?

- [ ] **A)** Isolate the symptom by checking if the issue affects all agents or specific users.
- [ ] **B)** Restart the recording service immediately.
- [ ] **C)** Escalate to Level 3 support with all available logs.
- [ ] **D)** Reinstall the WFO core service.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The methodology emphasizes symptom isolation as the first step to narrow down the scope before any action.
 
 
</details>

### 26. Which two items are essential when collecting logs during troubleshooting?

- [ ] **A)** Ensure all server clocks are synchronized using NTP.
- [ ] **B)** Only collect logs from the web server.
- [ ] **C)** Capture logs from all relevant tiers (media, database, web).
- [ ] **D)** Delete old logs to free space before collection.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Time synchronization and multi-tier log capture are vital for correlating events across components.
 
 
</details>

### 27. Examine the log snippet below. What does the severity level 'ERROR' indicate?

```plaintext
INFO: Service started successfully
WARNING: Media server response delayed
ERROR: Failed to connect to database - retrying
```

- [ ] **A)** A recoverable problem that requires investigation.
- [ ] **B)** The application is about to stop working.
- [ ] **C)** The system is operating normally.
- [ ] **D)** A configuration change has been applied.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ERROR indicates a condition needing investigation; it is not necessarily fatal.
 
 
</details>

### 28. What is a common cause of recording failures in Avaya WFE?

- [ ] **A)** Expired recording channel license.
- [ ] **B)** Agent not logged into the phone.
- [ ] **C)** Browser cache corruption.
- [ ] **D)** Incorrect time zone on the user's workstation.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> License expiry can silently cause recording failures; always verify license status first.
 
 
</details>

### 29. Which two conditions indicate that an issue should be escalated to Level 3?

- [ ] **A)** The issue affects multiple tenants or contact centers.
- [ ] **B)** The basic isolation steps have been completed and documented.
- [ ] **C)** The suspected root cause is a software defect that requires a patch.
- [ ] **D)** The customer reports a single agent cannot log in.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Multi-tenant impact and suspected software defects are clear escalation triggers.
 
 
</details>

### 30. Review the following log entry. What does the error code '0x80070570' typically indicate?

```plaintext
RecorderCtrl[1234]: Error 0x80070570 - File corruption for agent 5678
```

- [ ] **A)** File corruption during recording session.
- [ ] **B)** License key mismatch.
- [ ] **C)** Network timeout reached.
- [ ] **D)** Database connection pool exhausted.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Error 0x80070570 is a Windows error indicating file corruption as seen in the scenario.
 
 
</details>

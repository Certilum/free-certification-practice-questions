<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Avaya/Avaya%20IP%20Office%E2%84%A2%20Platform%20Technical%20Associate%20Implement" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Avaya IP Office™ Platform Technical Associate Implement</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Avaya IP Office Platform Architecture](#avaya-ip-office-platform-architecture) (7 questions)
- [Implementation and Configuration](#implementation-and-configuration) (11 questions)
- [Integration and Advanced Features](#integration-and-advanced-features) (3 questions)
- [Maintenance and Troubleshooting](#maintenance-and-troubleshooting) (6 questions)
- [Security and Best Practices](#security-and-best-practices) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:24.588Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Avaya IP Office Platform Architecture | 7 |
| Implementation and Configuration | 11 |
| Integration and Advanced Features | 3 |
| Maintenance and Troubleshooting | 6 |
| Security and Best Practices | 3 |

---

### **Avaya IP Office Platform Architecture**

### 1. Which Avaya IP Office hardware platform is designed to support up to 3,000 users with hot-standby redundancy?

- [ ] **A)** IP500v2 base unit
- [ ] **B)** Server Edition (SE)
- [ ] **C)** 1600 Series IP Telephones
- [ ] **D)** Avaya S8300 appliance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Server Edition supports up to 3,000 users with active-standby redundancy, unlike IP500v2 which is limited to 384 users.
 
 
</details>

### 2. Which two deployment models does the Avaya IP Office platform support for small to medium enterprises? (Choose two.)

- [ ] **A)** Local (on-premise)
- [ ] **B)** Cloud (hosted by Avaya or partner)
- [ ] **C)** Hybrid (combined on-prem and cloud)
- [ ] **D)** Remote (branch) with centralized call control

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The supported deployment models are Local (on-premise) and Cloud (hosted). Hybrid and remote branch are not primary models.
 
 
</details>

### 3. The following license file snippet was generated for an IP Office system. What type of license is being assigned for each physical telephone with programmable keys?

```plaintext
# License File for IP500v2
# Serial: 123456789
Button: 50
User: 20
PowerUser: 5
MobileUser: 10
```

- [ ] **A)** Mobile User license
- [ ] **B)** Button license
- [ ] **C)** Power User license
- [ ] **D)** User license

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A Button license is required for each physical telephone with programmable buttons, as stated in the license file.
 
 
</details>

### 4. In a standard Avaya IP Office internal call between two H.323 IP phones on the same LAN, what is the default media path?

- [ ] **A)** Media goes through the IP Office server
- [ ] **B)** Media flows directly between the two phones
- [ ] **C)** Media is sent to the SIP trunk provider first
- [ ] **D)** Media is hairpinned through the voicemail system

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> By default, H.323 internal calls use direct RTP media between endpoints; signaling goes through the IP Office.
 
 
</details>

### 5. Which of the following are capabilities of the 1600 Series IP Telephones? (Choose two.)

- [ ] **A)** Support for G.711, G.729a, and G.722 codecs
- [ ] **B)** Color touchscreen display
- [ ] **C)** Built-in Bluetooth support
- [ ] **D)** Optional wall-mount kit and headset adapter (for 1608/1616)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> 1600 Series supports G.711, G.729a, G.722 codecs and optional wall-mount/headset adapter; no color screen or Bluetooth.
 
 
</details>

### 6. Review the following configuration output from an Avaya IP Office system. Which software variant is being used?

```plaintext
System Status
Variant: Preferred
Max Users: 300
Resilience: Active-Standby
Features: Hot-desking, one-X Portal, Advanced Call Routing
```

- [ ] **A)** Essential Edition
- [ ] **B)** Preferred Edition
- [ ] **C)** Server Edition
- [ ] **D)** Advanced Edition

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Preferred Edition supports up to 300 users with resilience, hot-desking, and one-X Portal, as indicated by the output.
 
 
</details>

### 7. What is the maximum number of users supported by Avaya IP Office Essential Edition?

- [ ] **A)** 100
- [ ] **B)** 250
- [ ] **C)** 300
- [ ] **D)** 1000

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Essential Edition supports a maximum of 100 users, as per Avaya official specifications.
 
 
</details>


---

### **Implementation and Configuration**

### 8. Which Avaya component is required to create multi-level auto attendant menus?

- [ ] **A)** Voicemail Pro
- [ ] **B)** Basic Voicemail
- [ ] **C)** System Status Application
- [ ] **D)** IP Office Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Voicemail Pro is needed for multi-level auto attendant; basic voicemail supports only single-level menus.
 
 
</details>

### 9. Which of the following are valid hunt group distributions in Avaya IP Office? (Select two.)

- [ ] **A)** Ring All
- [ ] **B)** Sequential
- [ ] **C)** Spiral
- [ ] **D)** Random

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Valid distributions: Ring All and Sequential. Spiral and Random are not IP Office hunt group types.
 
 
</details>

### 10. Examine the short code table. Which code is used to retrieve a group mailbox?

```plain
Short Codes:
*17 - Group Mailbox Access
*18 - Group Mailbox Admin
*19 - Voicemail On
*20 - Voicemail Off
```

- [ ] **A)** *17
- [ ] **B)** *18
- [ ] **C)** *19
- [ ] **D)** *20

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Short code *17 is the default for group mailbox retrieval; *18 is for group mailbox administration.
 
 
</details>

### 11. In Avaya IP Office, where is the phone’s MAC address typically configured?

- [ ] **A)** Extension Object
- [ ] **B)** User Object
- [ ] **C)** Hunt Group Object
- [ ] **D)** System Object

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The MAC address is configured in the Extension object, not the User object.
 
 
</details>

### 12. Which parameters must be identical across all nodes to form an SCN? (Select two.)

- [ ] **A)** SCN Name
- [ ] **B)** SCN Password
- [ ] **C)** Node ID
- [ ] **D)** System Password

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SCN Name and Password must match; Node ID must be unique per node.
 
 
</details>

### 13. Using the configuration excerpt, what is the default connection mode when Manager first opens a configuration?

```text
Manager Toolbar Status:
[icon: padlock] - Read Only mode active.
Click padlock to switch to Read/Write mode.
Current mode: Read Only
```

- [ ] **A)** Read Only
- [ ] **B)** Read/Write
- [ ] **C)** Supervisor
- [ ] **D)** Administrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Manager connects in Read Only mode; you must toggle to Read/Write to make changes.
 
 
</details>

### 14. Which transport protocol is commonly used for SIP trunk communication over the internet?

- [ ] **A)** UDP
- [ ] **B)** TCP
- [ ] **C)** TLS
- [ ] **D)** SCTP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> UDP is the most common transport for SIP due to low latency; TCP and TLS are used for reliability and security.
 
 
</details>

### 15. Which of the following are required when configuring a site-to-site VPN for IP Office? (Select two.)

- [ ] **A)** Pre-Shared Key
- [ ] **B)** Peer IP Address
- [ ] **C)** SCN Name
- [ ] **D)** SIP Domain

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VPN requires a pre-shared key and the peer's IP address; SCN and SIP are telephony features.
 
 
</details>

### 16. Examine the hunt group configuration. What destination takes effect after the timeout expires?

```text
Hunt Group: Support (500)
Timeout: 20 seconds
Overflow Destination: 500
Voicemail: Enabled
```

- [ ] **A)** Voicemail
- [ ] **B)** Operator
- [ ] **C)** Auto Attendant
- [ ] **D)** Another Hunt Group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The overflow destination is set to group voicemail; other options are not specified.
 
 
</details>

### 17. If a user object is deleted in IP Office, what happens to the associated extension?

- [ ] **A)** It remains but loses user-specific settings
- [ ] **B)** It is automatically deleted
- [ ] **C)** It is moved to a default user
- [ ] **D)** It becomes a hunt group member

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The extension stays but voicemail and COS are removed; it is not automatically deleted.
 
 
</details>

### 18. Which capabilities are provided by the System Status Application? (Select two.)

- [ ] **A)** Real-time system monitoring
- [ ] **B)** Configuration changes
- [ ] **C)** Call tracking and reporting
- [ ] **D)** User creation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> SSA monitors and reports; configuration changes are made in Manager.
 
 
</details>


---

### **Integration and Advanced Features**

### 19. Which component manages skills-based routing when integrating Avaya IP Office with Contact Center Select?

- [ ] **A)** ACCS
- [ ] **B)** IP Office Manager
- [ ] **C)** System Manager
- [ ] **D)** Contact Recorder

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Skills-based routing is managed by ACCS; IP Office only passes calls to the ACCS hunt group.
 
 
</details>

### 20. Which two elements are required for Microsoft Teams Direct Routing integration with IP Office?

- [ ] **A)** Public CA certificate
- [ ] **B)** SIP domain in Teams
- [ ] **C)** Static IP address only
- [ ] **D)** UDP port 5060 open

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A public CA certificate is needed for TLS; the SIP domain must match the SBC FQDN in Teams.
 
 
</details>

### 21. What event triggers an automatic failover in a Survivable Core Network pair?

```config
heartbeat-interval=2
missed-heartbeats=6
```

- [ ] **A)** Loss of heartbeat
- [ ] **B)** Manual force-failover
- [ ] **C)** Scheduled maintenance
- [ ] **D)** Power surge

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The standby detects 6 missed heartbeats (12 seconds) and assumes control automatically.
 
 
</details>


---

### **Maintenance and Troubleshooting**

### 22. What is the primary method to access the System Status Application (SSA) for Avaya IP Office?

- [ ] **A)** Via a web browser using the IP address of the control unit followed by /ssa
- [ ] **B)** By opening the Avaya IP Office Manager application and selecting the SSA tab
- [ ] **C)** Through the command line interface (CLI) using the 'ssa' command
- [ ] **D)** By connecting a monitor and keyboard directly to the IP Office chassis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SSA is accessed via a web browser at http://<IP_Office_IP>/ssa. The other options describe incorrect methods; Manager is for configuration, CLI is not the primary access, and direct console access is not the standard way for SSA.
 
 
</details>

### 23. Which of the following views are available in the System Status Application (SSA)? (Select all that apply.)

- [ ] **A)** Alarms
- [ ] **B)** Traces
- [ ] **C)** System Status
- [ ] **D)** Event Log

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> All four are standard views within SSA: Alarms, Traces, System Status, and Event Log. The playbook explicitly mentions each as key diagnostic components.
 
 
</details>

### 24. Review the following alarm log entry from an IP Office system. What severity level is indicated?

```plaintext
Alarm ID: 4712
Severity: Minor
Source: T1 Trunk Module (Slot 3)
Description: Disconnect Frame sequence error
Timestamp: 2023-08-14 14:22:05
```

- [ ] **A)** Critical
- [ ] **B)** Major
- [ ] **C)** Minor
- [ ] **D)** Informational

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The log shows a repeating Minor alarm about a T1 trunk disconnect sequence error. Minor alarms require investigation but are not immediately service-affecting, though they can escalate.
 
 
</details>

### 25. Which Avaya tool is specifically designed for deep-dive protocol analysis and performance counter capture over extended periods?

- [ ] **A)** System Monitor (SMON)
- [ ] **B)** System Status Application (SSA)
- [ ] **C)** IP Office Manager
- [ ] **D)** Avaya Diagnostic Assistant

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SMON is the tool for deep-dive analysis, capturing protocol traces and performance counters over time. SSA is for real-time health snapshots, Manager is for configuration, and Diagnostic Assistant is a different product.
 
 
</details>

### 26. Which of the following performance counters can be monitored using the System Status Application? (Select all that apply.)

- [ ] **A)** Current call count
- [ ] **B)** CPU load (1-minute average)
- [ ] **C)** Memory usage percentage
- [ ] **D)** Trunk utilization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> SSA displays all these counters: active calls, CPU load, memory usage, and trunk utilization. The playbook lists them as key metrics for monitoring system health.
 
 
</details>

### 27. In the SSA Traces tab, a technician sets the filter to 'Extension 200'. What will this trace capture?

```plaintext
Trace Filter Settings
- Filter Type: Extension
- Value: 200
- Protocol: All
- Capture Mode: Live
```

- [ ] **A)** All signaling and media messages involving extension 200
- [ ] **B)** Only call setup messages for extension 200
- [ ] **C)** All system events regardless of source
- [ ] **D)** Only error messages related to extension 200

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Trace filters capture all relevant events (signaling, media, system) for the specified extension. It does not limit to setup only, nor to errors alone, and it does not capture unrelated events.
 
 
</details>


---

### **Security and Best Practices**

### 28. What is the default system password for an Avaya IP Office Manager access?

- [ ] **A)** Blank (no password)
- [ ] **B)** admin
- [ ] **C)** password
- [ ] **D)** 1234

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The default system password in IP Office is blank. Avaya recommends setting a complex password immediately to secure the configuration database.
 
 
</details>

### 29. Which of the following are recommended security practices for an Avaya IP Office system? (Select all that apply.)

- [ ] **A)** Set a strong system password
- [ ] **B)** Expose the Web Manager directly to the internet
- [ ] **C)** Disable HTTP and force HTTPS for management
- [ ] **D)** Use default SNMP community strings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Setting a strong password and disabling HTTP (forcing HTTPS) are best practices. Exposing Web Manager or using default SNMP strings are security risks.
 
 
</details>

### 30. Review the following configuration excerpt from the IP Office Manager Security tab. What is the lockout reset timer value?

```text
Maximum Invalid Login Attempts: 5
Lockout Reset Timer: 30 minutes (default, not configurable)
Lockout applies to: Manager, SSA, one-X Portal
```

- [ ] **A)** 15 minutes
- [ ] **B)** 30 minutes
- [ ] **C)** 60 minutes
- [ ] **D)** Not configurable

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In IP Office, the lockout reset timer is hard-coded to 30 minutes and cannot be changed by the administrator.
 
 
</details>

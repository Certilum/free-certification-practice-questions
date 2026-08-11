<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/microsoft-certified-associate-badge.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Microsoft Certified: Security Operations Analyst Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Manage a security operations environment](#manage-a-security-operations-environment) (12 questions)
- [Perform threat hunting](#perform-threat-hunting) (7 questions)
- [Respond to security incidents](#respond-to-security-incidents) (11 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-11T02:42:30.281Z |
| Domains | 3 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Manage a security operations environment | 12 |
| Perform threat hunting | 7 |
| Respond to security incidents | 11 |

---

### **Manage a security operations environment**

### 1. Which Azure resource serves as the storage and querying foundation for Microsoft Sentinel?

- [ ] **A)** Log Analytics workspace
- [ ] **B)** Power BI workspace
- [ ] **C)** Microsoft 365 Defender portal
- [ ] **D)** Azure Automation account

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Microsoft Sentinel is a cloud-native SIEM that is enabled on a Log Analytics workspace, which stores and queries all security telemetry.
 
 
</details>

### 2. Which two roles are built-in Microsoft Sentinel roles for security operations?

- [ ] **A)** Microsoft Sentinel Reader
- [ ] **B)** Microsoft Sentinel Contributor
- [ ] **C)** Log Analytics Contributor
- [ ] **D)** Global Administrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Microsoft Sentinel Reader and Contributor are built-in Sentinel roles; Log Analytics Contributor and Global Administrator are not Sentinel-specific built-in roles.
 
 
</details>

### 3. The code block shows Azure CLI code. Which resource must exist before Microsoft Sentinel can be enabled?

```azure-cli
az monitor log-analytics workspace create --resource-group rg-sentinel --workspace-name law-security
```

- [ ] **A)** Log Analytics workspace
- [ ] **B)** Virtual network
- [ ] **C)** Storage account
- [ ] **D)** Azure SQL database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command creates a Log Analytics workspace, which is required before Microsoft Sentinel can be enabled.
 
 
</details>

### 4. A company wants to enable Microsoft Sentinel but has no Log Analytics workspace. What must be done first?

- [ ] **A)** Create or select a Log Analytics workspace
- [ ] **B)** Enable Microsoft Defender for Cloud
- [ ] **C)** Install a data connector
- [ ] **D)** Create a playbook

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Sentinel is layered on a Log Analytics workspace; without one, you must create a new workspace or select an existing one first.
 
 
</details>

### 5. Which two factors justify deploying multiple Microsoft Sentinel workspaces?

- [ ] **A)** Data residency and compliance constraints
- [ ] **B)** Operational boundaries between business units
- [ ] **C)** Desire for a single incident queue
- [ ] **D)** Lower overall cost

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Multiple workspaces are used for data sovereignty and operational or compliance boundaries; a single incident queue and lower cost favor one workspace.
 
 
</details>

### 6. The code block contains a KQL query. Which table is being queried?

```kql
SigninLogs
| where ResultType == "50057"
| project UserPrincipalName, IPAddress
```

- [ ] **A)** SigninLogs
- [ ] **B)** SecurityEvent
- [ ] **C)** CommonSecurityLog
- [ ] **D)** DeviceEvents

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query references the SigninLogs table, which contains Microsoft Entra ID authentication activity and sign-in events.
 
 
</details>

### 7. Which connector unifies alerts and incidents from multiple Microsoft Defender workloads into Microsoft Sentinel?

- [ ] **A)** Microsoft Defender XDR connector
- [ ] **B)** Microsoft Entra ID connector
- [ ] **C)** Azure Activity connector
- [ ] **D)** Common Event Format connector

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Microsoft Defender XDR connector ingests incidents and alerts from the Defender suite through service-to-service integration.
 
 
</details>

### 8. Which three components are typically required for custom log ingestion into Log Analytics?

- [ ] **A)** Data Collection Rule
- [ ] **B)** Data Collection Endpoint
- [ ] **C)** Custom log table
- [ ] **D)** Diagnostic setting

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Custom log ingestion requires a DCR, a DCE, and a custom table; diagnostic settings are for Azure resource logs, not custom ingestion.
 
 
</details>

### 9. The Azure CLI code block creates which security-related resource?

```azure-cli
az monitor data-collection rule create --resource-group rg --name DCR-SecurityEvents --location eastus
```

- [ ] **A)** Data Collection Rule
- [ ] **B)** Data Collection Endpoint
- [ ] **C)** Log Analytics workspace
- [ ] **D)** Logic App

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command creates a data collection rule, which directs the Azure Monitor Agent on what to collect and where to send it.
 
 
</details>

### 10. Where do you configure table-level retention for a Log Analytics workspace?

- [ ] **A)** The Tables blade of the Log Analytics workspace
- [ ] **B)** The Analytics blade of Microsoft Sentinel
- [ ] **C)** The Microsoft Defender XDR settings page
- [ ] **D)** The Azure Policy compliance blade

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Table-level retention and archive settings are managed in the Tables blade within the Azure Log Analytics workspace.
 
 
</details>

### 11. Which two retention periods are part of a Log Analytics table lifecycle?

- [ ] **A)** Interactive retention
- [ ] **B)** Archive retention
- [ ] **C)** Diagnostic retention
- [ ] **D)** Audit retention

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Log Analytics tables have interactive retention for hot queries and archive retention for long-term, low-cost storage.
 
 
</details>

### 12. The KQL code block references which authentication-related table?

```kql
SigninLogs
| where TimeGenerated > ago(1d)
| where ResultType == "0"
| summarize Count = count() by UserPrincipalName
```

- [ ] **A)** SigninLogs
- [ ] **B)** AuditLogs
- [ ] **C)** SecurityEvent
- [ ] **D)** DeviceLogonEvents

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query references SigninLogs, which contains Microsoft Entra ID sign-in activity used for authentication detections.
 
 
</details>


---

### **Perform threat hunting**

### 13. Which KQL operator is used to filter rows in a table based on a condition?

- [ ] **A)** where
- [ ] **B)** project
- [ ] **C)** summarize
- [ ] **D)** extend

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The where operator filters tabular data to rows that match a boolean expression. project selects columns, summarize aggregates, and extend adds calculated columns.
 
 
</details>

### 14. Which of the following are valid advanced hunting schema tables in Microsoft 365 Defender?

- [ ] **A)** DeviceProcessEvents
- [ ] **B)** IdentityLogonEvents
- [ ] **C)** EmailEvents
- [ ] **D)** SecurityEvent

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Advanced hunting uses domain-specific tables starting with Device, Identity, Email, and CloudApp. SecurityEvent is a Microsoft Sentinel Log Analytics table, not an advanced hunting schema table.
 
 
</details>

### 15. What is the primary purpose of the following KQL query?

```kql
SecurityEvent
| where EventID == 4625
| summarize FailedCount = count() by Account
| order by FailedCount desc
```

- [ ] **A)** Identify accounts with the most failed logon attempts
- [ ] **B)** List all successful logons by account
- [ ] **C)** Count total security events by computer
- [ ] **D)** Filter failed logons for a single account

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query filters EventID 4625, counts failed logons per account with summarize, and sorts descending to highlight the most targeted accounts.
 
 
</details>

### 16. In the MITRE ATT&CK framework, what term describes the method an adversary uses to achieve a tactic?

- [ ] **A)** Tactic
- [ ] **B)** Technique
- [ ] **C)** Procedure
- [ ] **D)** Sub-technique

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Tactics are strategic objectives, techniques are methods used by adversaries, and procedures are specific implementations. Sub-techniques add granular detail to techniques.
 
 
</details>

### 17. Which connectors can be used to ingest threat intelligence indicators into Microsoft Sentinel?

- [ ] **A)** Threat Intelligence - TAXII
- [ ] **B)** Threat Intelligence - Microsoft Graph Security API
- [ ] **C)** Threat Intelligence Upload API
- [ ] **D)** Custom Logs connector

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Sentinel ingests TI via TAXII, the Microsoft Graph Security API, and the Upload API. A custom logs connector is not the standard TI ingestion method.
 
 
</details>

### 18. What does the following KQL query identify?

```kql
ThreatIntelligenceIndicator
| where ExpirationDateTime > now()
| where PatternType == "ipv4-addr"
| join kind=inner (SigninLogs) on $left.NetworkIP == $right.IPAddress
```

- [ ] **A)** Find sign-in events from active malicious IP indicators
- [ ] **B)** List all sign-ins regardless of threat intelligence
- [ ] **C)** Show expired threat intelligence indicators
- [ ] **D)** Find sign-ins from IPs in a custom watchlist

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query filters active IPv4 indicators and inner-joins them with SigninLogs to return sign-ins that match known malicious IPs.
 
 
</details>

### 19. Which Microsoft Sentinel feature preserves a set of query results with notes and tags for later investigation?

- [ ] **A)** Bookmark
- [ ] **B)** Livestream
- [ ] **C)** Analytics rule
- [ ] **D)** Watchlist

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Bookmarks preserve query results, notes, and entities in Sentinel for later investigation. Livestream monitors continuously, and analytics rules automate detections.
 
 
</details>


---

### **Respond to security incidents**

### 20. In Microsoft Defender XDR, where are correlated alerts and evidence from endpoint, email, identity, and cloud apps consolidated into a single incident narrative?

- [ ] **A)** Microsoft 365 Defender portal
- [ ] **B)** Microsoft Sentinel
- [ ] **C)** Azure portal
- [ ] **D)** Microsoft 365 compliance center

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Microsoft Defender XDR is the integrated platform that correlates alerts from Defender for Endpoint, Office 365, Identity, and Cloud Apps. Sentinel is a SIEM, not the XDR incident console.
 
 
</details>

### 21. Which two items must an analyst provide before a Microsoft 365 Defender incident can be set to Resolved in the incident queue?

- [ ] **A)** Classification (True positive, False positive, Informational)
- [ ] **B)** Determination (Malicious, No threat, Limited threat)
- [ ] **C)** Incident deletion confirmation
- [ ] **D)** CSV export confirmation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The portal requires classification and determination to resolve an incident. Incidents cannot be deleted, and exporting evidence is optional.
 
 
</details>

### 22. You are writing an Advanced Hunting query to investigate a phishing campaign. The KQL query in the code block has a placeholder for the table that contains sign-in events. Which table should replace the placeholder?

```kql
EmailEvents
| where Timestamp > ago(7d)
| where Url == 'https://example.com/login'
| join kind=inner TABLE_NAME on AccountUpn
```

- [ ] **A)** IdentityLogonEvents
- [ ] **B)** EmailEvents
- [ ] **C)** EmailUrlInfo
- [ ] **D)** DeviceNetworkInfo

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IdentityLogonEvents is the Advanced Hunting table for identity sign-in activity; joining it with EmailEvents connects phishing clicks to subsequent logons.
 
 
</details>

### 23. In Microsoft Entra ID Protection, which report lists individual sign-in events together with the risk factors associated with each sign-in?

- [ ] **A)** Risk Detections report
- [ ] **B)** Risky Users report
- [ ] **C)** Audit logs
- [ ] **D)** Conditional Access report

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Risk Detections report shows individual sign-in risk events; Risky Users report aggregates risk per user account.
 
 
</details>

### 24. Which two statements about the Microsoft Sentinel investigation graph are true?

- [ ] **A)** It visualizes entity connections such as users, hosts, IPs, and files.
- [ ] **B)** It groups alerts that share common entities to reveal attack chains.
- [ ] **C)** It automatically executes playbooks to remediate incidents.
- [ ] **D)** It replaces workbooks for all executive reporting.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The investigation graph maps entity relationships and groups alerts by common entities. It does not execute playbooks, and workbooks remain the tool for dashboards and reporting.
 
 
</details>

### 25. The KQL query in the code block is designed to count Sentinel incidents by classification. Which status value should replace the placeholder to include only fully closed incidents?

```kql
SecurityIncident
| where Status == 'STATUS_PLACEHOLDER'
| summarize count() by Classification
```

- [ ] **A)** Closed
- [ ] **B)** Resolved
- [ ] **C)** New
- [ ] **D)** In Progress

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In Sentinel, Closed is the final status after all review is complete. Resolved may still be open for additional review, while New and In Progress are earlier lifecycle states.
 
 
</details>

### 26. Which Microsoft Defender for Endpoint response action prevents a specified application from starting new instances on a Windows device?

- [ ] **A)** Restrict app execution
- [ ] **B)** Isolate device
- [ ] **C)** Run antivirus scan
- [ ] **D)** Live Response

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Restrict app execution prevents new instances of the app on Windows. It does not terminate a currently running instance.
 
 
</details>

### 27. Which platforms support Live Response in Microsoft Defender for Endpoint?

- [ ] **A)** Windows
- [ ] **B)** macOS
- [ ] **C)** Linux
- [ ] **D)** Android

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Live Response is supported on Windows, macOS, and Linux. Mobile devices do not support Live Response; mobile incident response is handled through Intune.
 
 
</details>

### 28. The KQL query in the code block joins email records with attachment records. Which table should replace the placeholder to return file attachment information for a phishing email?

```kql
EmailEvents
| where NetworkMessageId == 'network-message-id'
| join kind=inner TABLE_NAME on NetworkMessageId
```

- [ ] **A)** EmailAttachmentInfo
- [ ] **B)** EmailUrlInfo
- [ ] **C)** EmailPostDeliveryEvents
- [ ] **D)** IdentityLogonEvents

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> EmailAttachmentInfo is the Advanced Hunting schema containing attachment metadata. EmailUrlInfo is for URLs, EmailPostDeliveryEvents for post-delivery actions, and IdentityLogonEvents for sign-in events.
 
 
</details>

### 29. Which Microsoft Defender for Office 365 feature retroactively moves a harmful email from a user's Inbox to quarantine or the Deleted Items folder?

- [ ] **A)** Zero-Hour Auto Purge (ZAP)
- [ ] **B)** Threat Explorer
- [ ] **C)** Advanced Hunting
- [ ] **D)** User submission

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ZAP is the post-delivery protection feature that moves already delivered malicious messages after detection. Threat Explorer and Advanced Hunting are investigation tools.
 
 
</details>

### 30. Which risk levels are used by Microsoft Entra ID Protection to classify identity risk?

- [ ] **A)** Low
- [ ] **B)** Medium
- [ ] **C)** High
- [ ] **D)** Elevated

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Entra ID Protection uses Low, Medium, and High risk levels. Elevated is not a defined risk level.
 
 
</details>

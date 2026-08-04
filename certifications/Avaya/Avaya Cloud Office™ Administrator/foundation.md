<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Avaya/Avaya%20Cloud%20Office%E2%84%A2%20Administrator" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Avaya Cloud Office™ Administrator</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Administration and Maintenance](#administration-and-maintenance) (6 questions)
- [Call Routing and Feature Configuration](#call-routing-and-feature-configuration) (7 questions)
- [Cloud Office Overview and Architecture](#cloud-office-overview-and-architecture) (4 questions)
- [Reporting and Monitoring](#reporting-and-monitoring) (5 questions)
- [User and Device Management](#user-and-device-management) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:19.413Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Administration and Maintenance | 6 |
| Call Routing and Feature Configuration | 7 |
| Cloud Office Overview and Architecture | 4 |
| Reporting and Monitoring | 5 |
| User and Device Management | 8 |

---

### **Administration and Maintenance**

### 1. Which task is the primary responsibility of an Avaya Cloud Office administrator regarding system backups?

- [ ] **A)** Exporting Auto Attendant scripts
- [ ] **B)** Backing up the entire SQL database
- [ ] **C)** Taking server snapshots
- [ ] **D)** Restoring voicemail recordings older than 90 days

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The administrator exports logical configurations like Auto Attendant scripts; infrastructure backups are handled by Avaya.
 
 
</details>

### 2. Which steps are part of managing a feature release in Avaya Cloud Office? (Select all that apply.)

- [ ] **A)** Reviewing release notes
- [ ] **B)** Creating a pilot group
- [ ] **C)** Rolling back the entire platform version
- [ ] **D)** Notifying pilot users about changes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Release notes, pilot groups, and user communication are key; version rollback is not possible in a cloud model.
 
 
</details>

### 3. Based on the change request snippet below, what required component is missing?

```json
{
  "change_id": "CR-2025-001",
  "description": "Modify main Auto Attendant greeting for holiday schedule",
  "justification": "HR request for seasonal update",
  "affected_objects": ["AA_main_number"],
  "risk_level": "low",
  "rollback_plan": ""
}
```

- [ ] **A)** Rollback plan
- [ ] **B)** Approver name
- [ ] **C)** Change window
- [ ] **D)** Risk level

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Every change request must include a rollback plan; other fields are also required but are present in the snippet.
 
 
</details>

### 4. Which security setting requires users to provide additional verification beyond a password?

- [ ] **A)** Password policy
- [ ] **B)** Multi-factor authentication (MFA)
- [ ] **C)** IP access restrictions
- [ ] **D)** Session timeout

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> MFA adds a second verification step; password policy, IP restrictions, and session timeout are different controls.
 
 
</details>

### 5. Which practices are considered best for maintaining an internal knowledge base for Avaya Cloud Office? (Select all that apply.)

- [ ] **A)** Using version control for procedures
- [ ] **B)** Updating documents only after major releases
- [ ] **C)** Cross-referencing related articles
- [ ] **D)** Limiting editing rights to a single administrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Version control and cross-references improve accuracy; updates should be continuous, and editing should be shared.
 
 
</details>

### 6. Given this CSV export of users, what is true about restoring a user from this file?

```csv
username,extension,email,department,role
jsmith,101,jsmith@company.com,Sales,User
awong,102,awong@company.com,IT,User
bclark,103,bclark@company.com,HR,User
```

- [ ] **A)** Advanced call forwarding settings are preserved
- [ ] **B)** Only basic user fields are restored
- [ ] **C)** Duplicate extension numbers are allowed
- [ ] **D)** The file must be in JSON format for import

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> CSV export contains only basic fields; advanced settings like call forwarding must be manually reconfigured.
 
 
</details>


---

### **Call Routing and Feature Configuration**

### 7. Which Avaya Cloud Office feature is designed to manage high-volume inbound calls by placing callers on hold and distributing them to agents?

- [ ] **A)** Auto Attendant
- [ ] **B)** Call Queue
- [ ] **C)** Hunt Group
- [ ] **D)** Paging Group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A Call Queue explicitly holds callers on hold and distributes them to agents, unlike a Hunt Group which rings members directly without holding.
 
 
</details>

### 8. Which two statements are true regarding emergency (E911) call routing in Avaya Cloud Office?

- [ ] **A)** Auto Attendant can be used to route 911 calls to the security desk.
- [ ] **B)** Emergency calls bypass all user call forwarding rules.
- [ ] **C)** The ELIN provides a callback number and location to the PSAP.
- [ ] **D)** Time-based routing rules are applied to emergency calls after hours.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Emergency calls always bypass forwarding and other routing rules. The ELIN (Emergency Location Identification Number) is transmitted to the PSAP for location and callback.
 
 
</details>

### 9. Examine the dial plan configuration snippet. What happens when a user dials 5555?

```yaml
dial_plan:
  extension_length: 4
  extension_range: "1000-1999"
  external_access_code: 9
```

- [ ] **A)** The call is routed externally because no external access code was dialed.
- [ ] **B)** The call is routed internally as an extension within the defined range.
- [ ] **C)** The call fails because the dialed digits do not match any configured pattern.
- [ ] **D)** The call is forwarded to the system operator.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> With extension length set to 4 and a range of 1000-1999, dialing 5555 matches the internal extension pattern, so it is routed internally.
 
 
</details>

### 10. What is the first step in the number porting process for Avaya Cloud Office?

- [ ] **A)** Submit a Letter of Authorization (LOA) to Avaya.
- [ ] **B)** Receive the Firm Order Commitment (FOC) date from the losing carrier.
- [ ] **C)** Configure the extension length in the dial plan.
- [ ] **D)** Test the cutover by placing a test call.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The porting process begins with a signed LOA, which Avaya then validates and submits to the losing carrier.
 
 
</details>

### 11. Which two Avaya Cloud Office features require an additional license to be enabled?

- [ ] **A)** Voicemail-to-email
- [ ] **B)** Call recording
- [ ] **C)** Silent Monitor
- [ ] **D)** Presence synchronization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Call recording and Silent Monitor (a monitoring feature) require specific licenses. Voicemail-to-email and presence sync are standard features.
 
 
</details>

### 12. Review the supervisor capability code. What must be configured before 'Whisper' coaching can be used during a live call?

```yaml
user:
  role: supervisor
  license: "ACO Supervisor Bundle"
  features:
    whisper: enabled
    barge: disabled
    silent_monitor: disabled
```

- [ ] **A)** The supervisor must have the ACO Supervisor license assigned.
- [ ] **B)** The agent must have Do Not Disturb enabled.
- [ ] **C)** A call queue must be configured for the agent.
- [ ] **D)** The supervisor's presence must be set to Available.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Monitoring features like Whisper require the supervisor to have the appropriate license (e.g., ACO Supervisor bundle) and be in a manager relationship with the agent.
 
 
</details>

### 13. What is the purpose of an Emergency Location Identification Number (ELIN) in Avaya Cloud Office?

- [ ] **A)** Identifies the user's extension number.
- [ ] **B)** Routes the call to the user's voicemail.
- [ ] **C)** Provides a callback number and physical location to the PSAP.
- [ ] **D)** Enables call recording for compliance.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The ELIN is a DID number associated with a location; it is transmitted to the PSAP so dispatchers can identify the caller's location and call back if needed.
 
 
</details>


---

### **Cloud Office Overview and Architecture**

### 14. Which component acts as the gateway between a customer's local network and the Avaya Cloud Office core, handling SIP signaling and media transcoding?

- [ ] **A)** Session Border Controller (SBC)
- [ ] **B)** Admin Portal
- [ ] **C)** Auto Attendant
- [ ] **D)** Call Queue

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The SBC serves as the gateway for SIP signaling and media, handling security and transcoding between the customer network and the cloud core.
 
 
</details>

### 15. Which of the following are key benefits of Avaya Cloud Office compared to an on-premises PBX? (Choose two.)

- [ ] **A)** No capital expenditure on hardware
- [ ] **B)** Automatic updates and maintenance by Avaya
- [ ] **C)** Requires dedicated on-premises servers for failover
- [ ] **D)** Physical control of all data centers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Avaya Cloud Office eliminates hardware CapEx and includes automatic updates; on-premises servers and physical data center control are not required.
 
 
</details>

### 16. An administrator configures a webhook for call completion events. Review the sample payload. Which field should the receiving system use to ensure idempotency?

```json
{
  "event_id": "abc-123-def",
  "event_type": "call.completed",
  "user_id": "user@example.com",
  "call_duration": 120,
  "timestamp": "2025-03-15T10:30:00Z"
}
```

- [ ] **A)** event_id
- [ ] **B)** user_id
- [ ] **C)** call_duration
- [ ] **D)** timestamp

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The event_id field is unique per delivery and should be used to detect and ignore duplicate events for idempotent processing.
 
 
</details>

### 17. Which deployment model provides physical isolation of customer infrastructure at the hypervisor level?

- [ ] **A)** Dedicated Private Cloud
- [ ] **B)** Multi-Tenant Public Cloud
- [ ] **C)** Hybrid Cloud
- [ ] **D)** On-Premises IP Office

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Dedicated Private Cloud provides isolated VMs or bare-metal servers, offering stronger tenant isolation than multi-tenant public cloud.
 
 
</details>


---

### **Reporting and Monitoring**

### 18. An administrator needs to generate a report showing the average time customers wait before hanging up. Which report type should they use?

- [ ] **A)** Standard Queue Activity Report
- [ ] **B)** Standard Agent Performance Report
- [ ] **C)** Custom Report with Abandoned Calls metrics
- [ ] **D)** Custom Report with Average Speed of Answer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Average Abandoned Call Wait Time is a metric found in the Queue Activity Report (standard). The scenario asks for 'average time customers wait before hanging up', which corresponds to abandoned calls, not answered calls. The standard Queue Activity Report includes this metric, making it the correct choice.
 
 
</details>

### 19. Which two metrics are directly associated with call quality monitoring in Avaya Cloud Office?

- [ ] **A)** Jitter
- [ ] **B)** Average Speed of Answer (ASA)
- [ ] **C)** Packet Loss
- [ ] **D)** Service Level Percentage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Jitter and packet loss are objective call quality metrics. ASA and Service Level are queue performance metrics, not direct call quality measurements.
 
 
</details>

### 20. Based on the following call quality data excerpt, which metric is exceeding the recommended threshold?

```plaintext
Call ID: 12345
MOS: 3.8
Jitter: 45 ms
Latency: 120 ms
Packet Loss: 0.2%
```

- [ ] **A)** Mean Opinion Score (MOS) of 3.8
- [ ] **B)** Jitter of 45 ms
- [ ] **C)** Latency of 120 ms
- [ ] **D)** Packet loss of 0.2%

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Avaya recommended threshold for jitter is less than 30 ms. A jitter of 45 ms exceeds that, indicating potential audio quality issues. MOS 3.8 is above 3.5 (good), latency 120 ms is below 150 ms, and packet loss 0.2% is below 0.5%.
 
 
</details>

### 21. An organization must retain audit logs for HIPAA compliance (minimum 6 years). What should the administrator configure?

- [ ] **A)** Set the retention policy to 6 years in the Avaya Cloud Office subscription settings
- [ ] **B)** Upgrade to a license tier that supports extended retention (e.g., 7 years) and set the retention period accordingly
- [ ] **C)** Export logs manually every 90 days and store them on a local server
- [ ] **D)** Enable legal hold for all logs to prevent automatic deletion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Avaya Cloud Office retention is tied to the license tier. Basic plans may only offer 90 days. To achieve 6 years, the tenant needs a higher tier (e.g., advanced compliance plan) that supports up to 7 years, and the retention period must be configured. Manual export is not a platform-supported method for continuous retention. Legal hold is for specific logs, not a blanket solution.
 
 
</details>

### 22. Which two diagnostic tools are appropriate for verifying network connectivity to Avaya Cloud Office?

- [ ] **A)** Ping
- [ ] **B)** System Status Application (SSA)
- [ ] **C)** Traceroute
- [ ] **D)** Call Detail Record (CDR) export

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Ping and traceroute are standard network diagnostic commands used to verify connectivity and path to Avaya's session border controllers. SSA is an endpoint-level tool for device diagnostics, not for network reachability. CDRs are for call history, not real-time connectivity.
 
 
</details>


---

### **User and Device Management**

### 23. What is the maximum number of users that can be created in a single CSV import in the Avaya Cloud Office portal?

- [ ] **A)** 100
- [ ] **B)** 500
- [ ] **C)** 1000
- [ ] **D)** 250

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The portal supports importing up to 500 users per CSV file as stated in the documentation.
 
 
</details>

### 24. Which Avaya Cloud Office roles can create new user accounts? (Select two.)

- [ ] **A)** Super Admin
- [ ] **B)** Admin
- [ ] **C)** User
- [ ] **D)** Read-only Admin

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Super Admin and Admin roles have permission to create users; User and Read-only Admin cannot.
 
 
</details>

### 25. A desk phone is registered but not ringing for inbound calls. Examine the configuration snippet and identify the most likely cause.

```json
{
  "device": {
    "mac": "00:11:22:33:44:55",
    "model": "J179",
    "status": "registered",
    "assigned_user": null,
    "extension": null
  }
}
```

- [ ] **A)** The device is not assigned to a user extension
- [ ] **B)** The DHCP option 242 is misconfigured
- [ ] **C)** The phone requires a factory reset
- [ ] **D)** The softphone license is missing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Without an assigned user extension, the phone cannot receive calls. Registration alone is insufficient.
 
 
</details>

### 26. Which error code typically indicates a firmware update failure due to a download timeout?

- [ ] **A)** E100
- [ ] **B)** E304
- [ ] **C)** E200
- [ ] **D)** E400

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> E304 corresponds to a download timeout, often caused by network issues.
 
 
</details>

### 27. Which two hunt group distribution methods are available in Avaya Cloud Office? (Select two.)

- [ ] **A)** Simultaneous
- [ ] **B)** Sequential
- [ ] **C)** Random
- [ ] **D)** Fixed order

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Avaya Cloud Office supports simultaneous, sequential, and round-robin distribution. Random and fixed order are not standard.
 
 
</details>

### 28. After a user is deleted, how long does their license remain consumed before becoming available for reuse? Use the dashboard snippet to answer.

```json
{
  "license_pool": {
    "total": 100,
    "assigned": 85,
    "unassigned": 15,
    "deleted_users": [
      { "name": "John Doe", "deleted_on": "2025-03-01", "license_held_until": "2025-03-31" }
    ]
  }
}
```

- [ ] **A)** Immediately
- [ ] **B)** 30 days
- [ ] **C)** 7 days
- [ ] **D)** 90 days

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Deleted users remain in the system for a 30-day grace period, during which the license is still considered used.
 
 
</details>

### 29. When a user belongs to multiple groups with conflicting feature access policies, which policy is applied by default?

- [ ] **A)** The most permissive policy
- [ ] **B)** The most restrictive policy
- [ ] **C)** The policy assigned to the first group
- [ ] **D)** An error is generated

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The system applies the most restrictive policy when conflicts exist, unless a user-level override is set.
 
 
</details>

### 30. Which statements about softphone licensing are correct? (Select two.)

- [ ] **A)** A softphone license is consumed when the admin assigns the entitlement to the user
- [ ] **B)** A softphone license is consumed when the user first logs into the client
- [ ] **C)** Multiple installations by the same user require only one license
- [ ] **D)** Each installation requires its own license

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The license is consumed upon assignment, not login. One license covers multiple installations with concurrent session limits.
 
 
</details>

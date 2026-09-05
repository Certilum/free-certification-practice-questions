<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CrowdStrike/CCFP.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>CrowdStrike Certified Falcon Practitioner</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Endpoint Security](#endpoint-security) (9 questions)
- [Platform Fundamentals](#platform-fundamentals) (9 questions)
- [Response and Investigation](#response-and-investigation) (6 questions)
- [Threat Intelligence](#threat-intelligence) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:27.392Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Endpoint Security | 9 |
| Platform Fundamentals | 9 |
| Response and Investigation | 6 |
| Threat Intelligence | 6 |

---

### **Endpoint Security**

### 1. What mathematical approach does CrowdAV use to evaluate file characteristics and behavior?

- [ ] **A)** Advanced mathematical models
- [ ] **B)** Static hash comparisons
- [ ] **C)** User login history
- [ ] **D)** Network packet signatures

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CrowdAV uses advanced mathematical models to analyze file characteristics and behavior, enabling ML-based detection.
 
 
</details>

### 2. Which two machine learning layers does Falcon use to protect against new malware variants?

- [ ] **A)** Sensor-based ML
- [ ] **B)** Cloud-based ML
- [ ] **C)** Heuristic ML
- [ ] **D)** Signature-based ML

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Falcon combines Sensor-based ML on the endpoint and Cloud-based ML in the cloud to provide layered defense.
 
 
</details>

### 3. Based on the configuration in the code block, what ML mode is applied to the Finance host group?

```json
{
  "host_group": "Finance",
  "ml_policy": {
    "mode": "Detection",
    "cloud_ml": true,
    "sensor_ml": true
  }
}
```

- [ ] **A)** Detection
- [ ] **B)** Prevention
- [ ] **C)** Aggressive
- [ ] **D)** Disabled

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet shows that the Finance host group has its ML policy mode set to Detection, not Prevention.
 
 
</details>

### 4. What does Behavioral Blocking monitor instead of relying on a specific file?

- [ ] **A)** Process actions and sequences
- [ ] **B)** File hashes
- [ ] **C)** IP addresses
- [ ] **D)** Usernames

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Behavioral Blocking examines suspicious sequences of process actions, enabling prevention of fileless attacks.
 
 
</details>

### 5. Which two of the following are Indicators of Attack (IOAs)?

- [ ] **A)** Credential dumping behavior
- [ ] **B)** Unauthorized encryption attempts
- [ ] **C)** Static file hashes
- [ ] **D)** Virus signatures

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> IOAs focus on behavior, such as credential dumping or unauthorized encryption, rather than static artifacts.
 
 
</details>

### 6. Based on the code block, which two exclusion types are configured?

```yaml
exclusions:
  - type: path
    value: "C:\\Program Files\\App"
  - type: process
    value: "autoupdate.exe"
```

- [ ] **A)** Path
- [ ] **B)** Process
- [ ] **C)** File hash
- [ ] **D)** Network IP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The configuration defines a path exclusion and a process exclusion to prevent false positives.
 
 
</details>

### 7. What happens when a Falcon sensor is set to Detection mode?

- [ ] **A)** The action is logged but allowed to complete
- [ ] **B)** The action is blocked before execution
- [ ] **C)** The sensor stops collecting telemetry
- [ ] **D)** The endpoint is immediately isolated

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Detection mode records the threat and allows the action to complete, while Prevention mode actively blocks it.
 
 
</details>

### 8. Which three types of activity does EDR visibility monitor besides file changes?

- [ ] **A)** Process activity
- [ ] **B)** Network connections
- [ ] **C)** Registry modifications
- [ ] **D)** CPU temperature

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> EDR visibility includes process, network, and registry activity, not just file modifications.
 
 
</details>

### 9. What deployment strategy does the sensor update policy in the code block represent?

```yaml
sensor_update_policy:
  ring_one: "IT test group"
  ring_two: "Finance workstations"
  ring_three: "All remaining hosts"
```

- [ ] **A)** Ring deployment
- [ ] **B)** Manual patch
- [ ] **C)** Disabled updates
- [ ] **D)** Global rollback

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy uses rings to test new sensor versions on subsets before broader rollouts.
 
 
</details>


---

### **Platform Fundamentals**

### 10. What does CrowdAV primarily use to evaluate file characteristics and behavior?

- [ ] **A)** Advanced mathematical models
- [ ] **B)** Static hash lookup
- [ ] **C)** Manual signature definitions
- [ ] **D)** Simply blocking all new files

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CrowdAV uses advanced mathematical models to analyze file characteristics and behavior, avoiding reliance on static hashes or signatures.
 
 
</details>

### 11. Which two ML layers does Falcon combine to provide defense-in-depth against new malware variants?

- [ ] **A)** Sensor-based ML (on-endpoint)
- [ ] **B)** Cloud-based ML (in-flight)
- [ ] **C)** Behavioral Blocking
- [ ] **D)** IOC matching

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Falcon uses both sensor-based on-endpoint ML and cloud-based in-flight ML, creating defense-in-depth for novel malware.
 
 
</details>

### 12. Review the policy snippet. What will the Falcon sensor do when the machine learning mode is set as shown?

```json
{
  "machine_learning": {
    "mode": "Detection"
  }
}
```

- [ ] **A)** Log the event but allow the action to complete
- [ ] **B)** Immediately kill the process
- [ ] **C)** Quarantine the file without logging
- [ ] **D)** Stop collecting telemetry

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In Detection mode the sensor logs the event but allows the action to complete; Prevention mode is needed to stop it.
 
 
</details>

### 13. When using Behavioral Blocking, what does the protection focus on?

- [ ] **A)** The 'what': suspicious sequences of actions
- [ ] **B)** The 'who': user identity
- [ ] **C)** Static file hashes
- [ ] **D)** Network IP reputation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Behavioral Blocking focuses on the 'what'—suspicious sequences of actions—rather than file identity or user identity.
 
 
</details>

### 14. Which two behaviors would Behavioral Blocking most likely flag as suspicious?

- [ ] **A)** Process attempting to inject code into memory
- [ ] **B)** Unusual PowerShell execution pattern
- [ ] **C)** A normal scheduled backup
- [ ] **D)** A user changing their password

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Behavioral Blocking targets suspicious actions like memory injection and unusual PowerShell patterns, while ignoring benign administrative activity.
 
 
</details>

### 15. Review the exclusion configuration. What is the primary risk associated with this broad global exclusion?

```json
{
  "exclusion": {
    "path": "*",
    "process": "*",
    "scope": "All Hosts"
  }
}
```

- [ ] **A)** It creates massive security blind spots
- [ ] **B)** It improves endpoint performance dramatically
- [ ] **C)** It strengthens ML detection
- [ ] **D)** It removes the sensor from hosts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A broad global exclusion creates security blind spots, as attackers can operate in excluded paths or processes without protection.
 
 
</details>

### 16. In the Falcon console, what does selecting 'Detection' for ML prevention mean for the sensor's response?

- [ ] **A)** The threat is noted but the action is allowed to complete
- [ ] **B)** The process is terminated before completion
- [ ] **C)** The file is quarantined automatically
- [ ] **D)** The endpoint is isolated immediately

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Detection mode means the threat is noted but its action is allowed to complete; actual protection requires Prevention mode.
 
 
</details>

### 17. Which two statements describe how Falcon sensor telemetry is collected?

- [ ] **A)** It captures granular data from the kernel level
- [ ] **B)** It does not interrupt user workflows
- [ ] **C)** It only records data after an alert fires
- [ ] **D)** It relies on the central console to poll the host

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The Falcon sensor captures kernel-level telemetry continuously without interrupting workflows, providing data for retrospective analysis.
 
 
</details>

### 18. Review the process tree. What does the parent-child relationship shown indicate to an analyst?

```text
outlook.exe (parent)
|-- powershell.exe (child)
```

- [ ] **A)** A classic indicator of exploitation
- [ ] **B)** Normal system administration activity
- [ ] **C)** A false positive from the sensor
- [ ] **D)** Evidence of machine learning training

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A host process like Outlook spawning a command shell is a classic indicator of exploitation and requires investigation.
 
 
</details>


---

### **Response and Investigation**

### 19. Which Falcon technology uses advanced mathematical models to analyze file characteristics and behavior?

- [ ] **A)** Machine Learning (ML) models
- [ ] **B)** Behavioral Blocking
- [ ] **C)** Sensor Update Policies
- [ ] **D)** Host Group assignments

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CrowdAV uses ML models to analyze file characteristics and behavior. Behavioral blocking focuses on process actions, not file attributes.
 
 
</details>

### 20. Which two statements correctly describe Sensor-based ML and Cloud-based ML in Falcon?

- [ ] **A)** Sensor-based ML runs locally on the endpoint.
- [ ] **B)** Cloud-based ML only inspects files after they have already been executed.
- [ ] **C)** Cloud-based ML runs in-flight and can detect novel variants.
- [ ] **D)** Cloud-based ML replaces the need for sensor-based ML.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Sensor-based ML is on the endpoint, while cloud-based ML operates in-flight. Both layers are needed for defense-in-depth against novel malware.
 
 
</details>

### 21. Review the policy excerpt in the code block. What will the Falcon sensor do when it encounters a suspicious file with ML configured to 'Detection'?

```json
{"prevention_policy":{"ml_detection":"Detection","behavioral_blocking":false}}
```

- [ ] **A)** It will log the detection and allow the action to complete.
- [ ] **B)** It will immediately block the file from executing.
- [ ] **C)** It will terminate the process because behavioral blocking is enabled.
- [ ] **D)** It will quarantine the file and roll back registry changes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Detection mode means the threat is noted but the action is allowed to complete. The code block also has behavioral blocking disabled.
 
 
</details>

### 22. What fundamental difference separates Behavioral Blocking from ML detection in CrowdStrike Falcon?

- [ ] **A)** Behavioral Blocking examines process actions; ML examines file attributes.
- [ ] **B)** Behavioral Blocking uses static hashes; ML uses process trees.
- [ ] **C)** ML monitors network connections; Behavioral Blocking monitors file content.
- [ ] **D)** ML is only cloud-based; Behavioral Blocking is only on the endpoint.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This is a common trap. ML focuses on file attributes and characteristics, while Behavioral Blocking focuses on suspicious sequences of process actions.
 
 
</details>

### 23. Which two examples best represent Behavioral Blocking rather than static file detection?

- [ ] **A)** A process attempts to inject code into memory.
- [ ] **B)** An unusual PowerShell execution pattern is observed.
- [ ] **C)** A file matches a known malware hash.
- [ ] **D)** A downloaded file has a clearly malicious static signature.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Behavioral blocking focuses on the 'what' or the action, such as code injection and unusual PowerShell patterns, rather than static file attributes or hashes.
 
 
</details>

### 24. The exclusion shown in the code block was created for a single false positive. Why is this configuration risky?

```json
{"exclusion":{"path":"C:\\Windows\\*","process":"*"}}
```

- [ ] **A)** It applies a broad exclusion that could create a blind spot for attackers.
- [ ] **B)** It excludes only a specific path and process.
- [ ] **C)** It increases ML aggressiveness for all files.
- [ ] **D)** It overrides the Sensor Update Policy ring.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Exclusions should be surgical and scoped to a specific path or process. A broad wildcard exclusion can create major security blind spots.
 
 
</details>


---

### **Threat Intelligence**

### 25. In the CrowdAV machine learning framework, which two layers of ML models provide defense-in-depth against novel malware variants?

- [ ] **A)** Sensor-based ML and Cloud-based ML
- [ ] **B)** Static ML and Dynamic ML
- [ ] **C)** Prevention ML and Detection ML
- [ ] **D)** Behavioral ML and Reputation ML

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CrowdAV combines sensor-based ML on the endpoint with cloud-based ML in flight, giving layered protection against new and unknown malware.
 
 
</details>

### 26. Which of the following are examples of suspicious sequences that Behavioral Blocking monitors?

- [ ] **A)** Process injecting code into memory
- [ ] **B)** Unusual PowerShell execution pattern
- [ ] **C)** Known malware file hash match
- [ ] **D)** Signed executable running normally

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Behavioral Blocking monitors process actions such as memory injection and unusual PowerShell usage, so it can prevent fileless attacks without relying on static file hashes.
 
 
</details>

### 27. Review the endpoint telemetry excerpt. Which Falcon concept best explains why the event is suspicious?

```json
{
  "event_type": "ProcessRollup2",
  "parent_process": "WINWORD.EXE",
  "child_process": "powershell.exe",
  "command_line": "powershell.exe -EncodedCommand AAA..."
}
```

- [ ] **A)** Parent-child process lineage indicates exploit chain
- [ ] **B)** Static file hash matches known malware
- [ ] **C)** Remote connection to a C2 IP address
- [ ] **D)** Registry modification for persistence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A document processor spawning PowerShell is classic malicious lineage; EDR reconstructs parent-child relationships to reveal exploitation.
 
 
</details>

### 28. In Falcon prevention policy tuning, what is the operational difference between 'Detection Only' and 'Prevention' modes?

- [ ] **A)** Detection logs; Prevention actively terminates
- [ ] **B)** Detection uses cloud ML; Prevention uses sensor ML
- [ ] **C)** Detection applies to servers; Prevention to workstations
- [ ] **D)** Detection blocks fileless attacks; Prevention blocks only files

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In Detection mode the sensor records the activity but allows it to complete; in Prevention mode the sensor actively kills the process.
 
 
</details>

### 29. Which exclusion practices align with disciplined NGAV management?

- [ ] **A)** Configure file, path, or process exclusions
- [ ] **B)** Use broad global exclusions for a single false positive
- [ ] **C)** Apply surgical path/process-specific exclusions
- [ ] **D)** Exclude entire drives to reduce support tickets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Disciplined exclusion management uses targeted file, path, or process exclusions to avoid false positives; broad exclusions create attacker bypasses.
 
 
</details>

### 30. Review the telemetry event. Which type of endpoint visibility does this event best illustrate?

```json
{
  "event_type": "NetworkConnection",
  "process": "svchost.exe",
  "remote_ip": "203.0.113.5",
  "remote_port": 443,
  "known_bad": true
}
```

- [ ] **A)** Network Connection Mapping
- [ ] **B)** Process Tree Visualization
- [ ] **C)** Registry and File Integrity
- [ ] **D)** Kernel memory scanning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This excerpt captures connection metadata and correlates it with a process, enabling command-and-control and data exfiltration visibility.
 
 
</details>

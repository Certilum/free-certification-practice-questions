<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Arista/Arista%20Network%20Detection%20&%20Response%20Specialist" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Arista Network Detection & Response Specialist</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Arista NDR Platform Architecture](#arista-ndr-platform-architecture) (6 questions)
- [Investigation and Forensics](#investigation-and-forensics) (6 questions)
- [Network Detection and Response Fundamentals](#network-detection-and-response-fundamentals) (5 questions)
- [Operational Management](#operational-management) (1 questions)
- [Response and Automation](#response-and-automation) (5 questions)
- [Threat Detection and Analytics](#threat-detection-and-analytics) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:03.811Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Arista NDR Platform Architecture | 6 |
| Investigation and Forensics | 6 |
| Network Detection and Response Fundamentals | 5 |
| Operational Management | 1 |
| Response and Automation | 5 |
| Threat Detection and Analytics | 7 |

---

### **Arista NDR Platform Architecture**

### 1. Which types of sensor are available for the Arista NDR platform?

- [ ] **A)** Physical appliances only
- [ ] **B)** Virtual appliances only
- [ ] **C)** Both physical and virtual appliances
- [ ] **D)** Cloud-native containers only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The document states that sensors are available as physical hardware and virtual machines (VMware, KVM, AMI).
 
 
</details>

### 2. Which two methods can supply network traffic to an Awake Security appliance?

- [ ] **A)** SPAN ports on switches
- [ ] **B)** Network TAPs
- [ ] **C)** NetFlow exports
- [ ] **D)** syslog messages

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The document specifies that the appliance receives traffic via SPAN or TAP. NetFlow and syslog are not traffic feeds.
 
 
</details>

### 3. Based on the cluster status output, what is the minimum number of nodes needed for quorum?

```text
Cluster Status:
Nodes: 3
Leader: node-1
Followers: node-2, node-3
Quorum: Required = 2, current = 3
```

- [ ] **A)** 1
- [ ] **B)** 2
- [ ] **C)** 3
- [ ] **D)** 4

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> With a three-node cluster using Raft consensus, quorum requires a majority (2 out of 3).
 
 
</details>

### 4. How does an Arista NDR virtual sensor in AWS receive network traffic?

- [ ] **A)** VPC Flow Logs
- [ ] **B)** VPC Traffic Mirroring
- [ ] **C)** AWS CloudTrail
- [ ] **D)** Direct Connect

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The document explains that VPC Traffic Mirroring (packet mirroring) is used to send full packets to the sensor.
 
 
</details>

### 5. Which two statements about Awake Security appliance license activation are correct?

- [ ] **A)** The license is uploaded via the web interface after initial console setup.
- [ ] **B)** The license can be applied using the CLI during initial configuration.
- [ ] **C)** The license is tied to the appliance serial number.
- [ ] **D)** The license is shared across all appliances without individual activation.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The document states licenses are uploaded via web UI and tied to the appliance serial number.
 
 
</details>

### 6. Examine the firewall rule. What TCP port is used for sensor-to-collector communication?

```text
Firewall Rule:
source: sensor-subnet
destination: collector-subnet
dport: 5555
protocol: TCP
```

- [ ] **A)** 443
- [ ] **B)** 5555
- [ ] **C)** 514
- [ ] **D)** 25

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The document specifies that sensors stream metadata to collectors over TCP port 5555.
 
 
</details>


---

### **Investigation and Forensics**

### 7. What does full session recording in Arista NDR capture?

- [ ] **A)** Entire packet headers and payloads
- [ ] **B)** Only flow summaries
- [ ] **C)** Only metadata
- [ ] **D)** Only alerts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Full session recording stores the entire packet, including headers and payload, enabling deep inspection.
 
 
</details>

### 8. Which of the following are considered entities in Arista NDR?

- [ ] **A)** Devices
- [ ] **B)** Users
- [ ] **C)** Flows
- [ ] **D)** Alerts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Entities include devices, users, and flows; alerts are events triggered by detection.
 
 
</details>

### 9. Based on the session record, which protocol was used?

```json
{
  "src_ip": "10.0.0.1",
  "dst_ip": "10.0.0.2",
  "src_port": 12345,
  "dst_port": 80,
  "protocol": "TCP"
}
```

- [ ] **A)** TCP
- [ ] **B)** UDP
- [ ] **C)** ICMP
- [ ] **D)** HTTP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The protocol field in the session record indicates TCP.
 
 
</details>

### 10. What is the first step in timeline analysis for root cause identification?

- [ ] **A)** Isolate the incident window
- [ ] **B)** Block the external IP
- [ ] **C)** Export all PCAP
- [ ] **D)** Escalate to management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The first step is to set a time window around the alert to capture pre-exploitation activities.
 
 
</details>

### 11. Which components are essential for a valid chain of custody in Arista NDR?

- [ ] **A)** SHA-256 hash
- [ ] **B)** Timestamp of export
- [ ] **C)** Exporter's username
- [ ] **D)** Encryption key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Hash, timestamp, and user identity are required; encryption key is separate.
 
 
</details>

### 12. Which flags in this ndr export command ensure integrity and security?

```bash
ndr export --start 2025-01-01 --end 2025-01-02 --encrypt --hash --output file.pcap
```

- [ ] **A)** --hash
- [ ] **B)** --encrypt
- [ ] **C)** --start
- [ ] **D)** --output

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> --hash adds integrity verification, --encrypt provides confidentiality.
 
 
</details>


---

### **Network Detection and Response Fundamentals**

### 13. What is a key advantage of Arista NDR over a traditional NIDS?

- [ ] **A)** Real-time signature updates
- [ ] **B)** Detects encrypted threats without decryption
- [ ] **C)** Aggregates logs from endpoints
- [ ] **D)** Requires deep packet inspection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Arista NDR uses metadata analysis to identify threats in encrypted traffic, unlike NIDS which requires decryption.
 
 
</details>

### 14. Which two capabilities are unique to Arista NDR compared to a SIEM?

- [ ] **A)** Behavioral analytics on network metadata
- [ ] **B)** Correlates logs from multiple sources
- [ ] **C)** Lateral movement detection via east-west traffic
- [ ] **D)** Long-term log storage for compliance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Arista NDR uses behavioral analytics and focuses on east-west traffic; SIEM correlates logs but lacks network metadata context.
 
 
</details>

### 15. Which protocol is used for NetFlow export in this configuration?

```cli
ip flow-export destination 10.0.0.1 2055 ???
```

- [ ] **A)** udp
- [ ] **B)** tcp
- [ ] **C)** sctp
- [ ] **D)** http

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NetFlow export traditionally uses UDP as the transport protocol for flow records.
 
 
</details>

### 16. What standardized format does Arista NDR use for threat intelligence exchange?

- [ ] **A)** STIX
- [ ] **B)** PDF
- [ ] **C)** CSV
- [ ] **D)** XML

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> STIX (Structured Threat Information Expression) is the standard format for describing threat data.
 
 
</details>

### 17. Which two compliance regulations require retention of security logs for at least one year?

- [ ] **A)** GDPR
- [ ] **B)** PCI DSS
- [ ] **C)** SOX
- [ ] **D)** HIPAA

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> PCI DSS requires one year retention for audit trails; HIPAA mandates six years for access logs.
 
 
</details>


---

### **Operational Management**

### 18. Which of the following best describes the primary purpose of a dashboard in the Arista NDR platform?

- [ ] **A)** To store raw packet captures for forensic analysis
- [ ] **B)** To serve as the primary decision-support tool for triage, investigation, and executive reporting
- [ ] **C)** To completely automate the incident response process
- [ ] **D)** To display the total number of alerts without any contextual information

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> According to the document, 'A dashboard is not merely a collection of charts; it serves as the primary decision-support tool for triage, investigation, and executive reporting.' The other options either describe storage, automation, or lack of context, which do not match the stated purpose.
 
 
</details>


---

### **Response and Automation**

### 19. What is the primary purpose of a playbook in the Arista NDR platform?

- [ ] **A)** To detect network anomalies in real time
- [ ] **B)** To automate a sequence of response actions triggered by security events
- [ ] **C)** To store historical network traffic data for compliance
- [ ] **D)** To configure firewall rules manually

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A playbook is a condition-driven automation workflow that orchestrates response actions after a detection trigger, bridging detection and remediation.
 
 
</details>

### 20. Which of the following are valid trigger types for an Arista NDR playbook?

- [ ] **A)** Event-driven (alert-based)
- [ ] **B)** Time-driven (scheduled)
- [ ] **C)** Manual-only (user invoked)
- [ ] **D)** Traffic volume threshold

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Playbooks can be triggered either from a detection alert (event-driven) or on a schedule (time-driven). Manual invocation is not a native trigger type.
 
 
</details>

### 21. Examine the syslog configuration snippet. Which default port is used for sending Arista NDR alerts to a SIEM?

```plaintext
syslog destination {
  host 192.168.1.100
  port 514
  protocol udp
  format cef
}
```

- [ ] **A)** 514
- [ ] **B)** 443
- [ ] **C)** 161
- [ ] **D)** 22

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Syslog messages are sent on UDP/TCP port 514 by default. Port 443 is HTTPS, 161 is SNMP, 22 is SSH.
 
 
</details>

### 22. What distinguishes a quarantine action from a block action in Arista NDR?

- [ ] **A)** Quarantine blocks all traffic; block only blocks specific ports
- [ ] **B)** Quarantine restricts communication to essential services; block stops all traffic to a destination
- [ ] **C)** Quarantine is permanent; block is temporary
- [ ] **D)** Quarantine applies at Layer 7; block at Layer 3

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Quarantine intelligently limits traffic to only allowed services (e.g., AD, patching) while blocking stops all traffic to a specific destination or direction.
 
 
</details>

### 23. Which identifiers can Arista NDR use to contain a host in a quarantine workflow?

- [ ] **A)** IP address
- [ ] **B)** MAC address
- [ ] **C)** Hostname
- [ ] **D)** User identity (Active Directory username)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Arista NDR supports containment by IP, MAC, and user identity. Hostname is not a native containment identifier.
 
 
</details>


---

### **Threat Detection and Analytics**

### 24. What is the primary purpose of behavioral analytics in Arista NDR?

- [ ] **A)** Detect known threats by exact signature matching
- [ ] **B)** Establish normal behavior and flag anomalies
- [ ] **C)** Replace all signature-based detection methods
- [ ] **D)** Automatically block all traffic from unknown sources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Behavioral analytics establishes a baseline of normal activity and flags deviations, unlike signature-based detection.
 
 
</details>

### 25. Which two statements are true about unsupervised learning in Arista NDR?

- [ ] **A)** Requires labeled training data
- [ ] **B)** Effective for zero-day attack discovery
- [ ] **C)** Groups similar behaviors into clusters
- [ ] **D)** Used exclusively for known malware classification

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Unsupervised learning does not use labels; it clusters similar behaviors and is effective for novel attacks.
 
 
</details>

### 26. In the provided rule snippet, what type of detection is being implemented?

```python
# Example: Behavioral baseline scoring
if flow.bytes > baseline.bytes * 3:
    score += 80
if flow.connections_out > 50:
    score += 60
```

- [ ] **A)** Signature-based detection
- [ ] **B)** Behavioral anomaly detection
- [ ] **C)** IoC exact match
- [ ] **D)** Threshold-based correlation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The rule uses a baseline deviation score, which is characteristic of behavioral anomaly detection.
 
 
</details>

### 27. What is the first step in the alert triage and false positive tuning workflow in Arista NDR?

- [ ] **A)** Immediately whitelist the source IP
- [ ] **B)** Review alert metadata to confirm the alert validity
- [ ] **C)** Adjust the detection model sensitivity
- [ ] **D)** Create a new detection rule for the behavior

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Initial triage requires reviewing alert metadata to confirm if it is a true or false positive.
 
 
</details>

### 28. Which two methods are part of false positive tuning in Arista NDR?

- [ ] **A)** Creating whitelist exceptions for known benign traffic
- [ ] **B)** Disabling all machine learning models permanently
- [ ] **C)** Adjusting detection rule thresholds and exclusions
- [ ] **D)** Ignoring all alerts from a specific subnet

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Whitelisting and rule adjustment are proper tuning methods; disabling models or ignoring subnets are too broad.
 
 
</details>

### 29. The code shows a configuration snippet from Arista NDR. What does this configuration achieve?

```yaml
# Time-based exception example
exception:
  source_ip: 10.2.3.4
  detection_type: dns_tunneling
  schedule:
    start: 03:00
    end: 04:00
    days: [mon, tue, wed, thu, fri]
```

- [ ] **A)** Enables exact match IoC detection
- [ ] **B)** Creates a time-based exception for a specific IP
- [ ] **C)** Increases the baseline learning window
- [ ] **D)** Configures a new threat intelligence feed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The configuration sets a schedule-based whitelist, which is a time-based exception for false positive tuning.
 
 
</details>

### 30. Which type of matching does Arista NDR use for file hashes in IoC detection?

- [ ] **A)** Fuzzy matching with Levenshtein distance
- [ ] **B)** Exact match only
- [ ] **C)** CIDR proximity matching
- [ ] **D)** Regex pattern matching

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> File hashes require an exact byte-for-byte match; fuzzy matching is not applicable to hashes.
 
 
</details>

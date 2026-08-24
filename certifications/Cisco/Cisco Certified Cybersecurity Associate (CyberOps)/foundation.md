<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cisco/CCNA" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Cisco Certified Cybersecurity Associate (CyberOps)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Network Security](#network-security) (8 questions)
- [Security Concepts](#security-concepts) (6 questions)
- [Security Operations and Monitoring](#security-operations-and-monitoring) (16 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:51:12.548Z |
| Domains | 3 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Network Security | 8 |
| Security Concepts | 6 |
| Security Operations and Monitoring | 16 |

---

### **Network Security**

### 1. Which network security technology operates inline and can actively block malicious traffic in real-time?

- [ ] **A)** Intrusion Detection System (IDS)
- [ ] **B)** Intrusion Prevention System (IPS)
- [ ] **C)** Stateful Inspection Firewall
- [ ] **D)** Network Access Control (NAC)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> An IPS operates inline and can drop, reject, or reset malicious packets in real-time. IDS is out-of-band and only alerts, while firewalls and NAC serve different primary functions.
 
 
</details>

### 2. Which two characteristics apply to a stateful inspection firewall?

- [ ] **A)** It tracks the state of active connections.
- [ ] **B)** It uses a state table to record connection information.
- [ ] **C)** It treats each packet independently without context.
- [ ] **D)** It only examines Layer 3 header information.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Stateful firewalls maintain a state table and track connection state (NEW, ESTABLISHED, etc.). They do not treat packets independently (that is stateless) and inspect beyond Layer 3.
 
 
</details>

### 3. Examine the following ACL configuration on a Cisco router:\naccess-list 100 permit tcp any host 192.168.1.100 eq www\naccess-list 100 deny ip any any\nWhat type of ACL is this?

```plaintext
access-list 100 permit tcp any host 192.168.1.100 eq www
access-list 100 deny ip any any
```

- [ ] **A)** Standard ACL
- [ ] **B)** Extended ACL
- [ ] **C)** Named ACL
- [ ] **D)** Dynamic ACL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Extended ACLs use numbers 100-199 and can filter based on source/destination IP, protocol (TCP/UDP), and port numbers. Standard ACLs only filter on source IP.
 
 
</details>

### 4. In a Zone-Based Firewall, what is the default action for traffic between two interfaces that belong to different zones when no policy map is applied?

- [ ] **A)** Permitted
- [ ] **B)** Denied
- [ ] **C)** Inspected
- [ ] **D)** Passed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In ZBFW, traffic between different zones is implicitly denied unless a zone-pair policy is configured. The 'inspect' or 'pass' actions must be explicitly defined to allow traffic.
 
 
</details>

### 5. Which two statements are true about DMZ design?

- [ ] **A)** A DMZ hosts servers that are accessible from the internet.
- [ ] **B)** Traffic from the DMZ to the internal network is unrestricted.
- [ ] **C)** A three-legged firewall model uses one firewall with three interfaces.
- [ ] **D)** The DMZ should be placed on the same subnet as the internal network to reduce complexity.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> DMZ hosts public-facing servers and uses a three-legged or dual-firewall model. Traffic from DMZ to internal is restricted, and DMZ is a separate network segment.
 
 
</details>

### 6. Read the following output from a switch configured for 802.1X:\nInterface: GigabitEthernet0/1\nPort-status: unauthorized\nWhat does the port-status value indicate?

```plaintext
Interface: GigabitEthernet0/1
Port-status: unauthorized
```

- [ ] **A)** The device has been authenticated and allowed on the network.
- [ ] **B)** The device has not yet been authenticated and network access is blocked.
- [ ] **C)** The port is administratively down due to a configuration error.
- [ ] **D)** The port is in spanning tree blocking state.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In 802.1X, the unauthorized state means the supplicant has not completed authentication, so the switch blocks all traffic except EAPoL frames until authentication succeeds.
 
 
</details>

### 7. Which SSH version should be used for secure remote management to avoid known vulnerabilities?

- [ ] **A)** SSHv1
- [ ] **B)** SSHv2
- [ ] **C)** SSHv3
- [ ] **D)** Telnet

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SSHv2 is the industry standard, providing encryption, host key verification, and resistance to man-in-the-middle attacks. SSHv1 is deprecated due to vulnerabilities.
 
 
</details>

### 8. Which two components are part of a secure syslog implementation?

- [ ] **A)** Using UDP port 514 for transport
- [ ] **B)** Using TLS encryption for transport
- [ ] **C)** Sending logs to a centralized server
- [ ] **D)** Disabling the logging feature on network devices

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Secure syslog requires encrypted transport (TLS) and a centralized server for analysis. UDP port 514 is unencrypted, and disabling logging reduces visibility.
 
 
</details>


---

### **Security Concepts**

### 9. Which security concept ensures that data is accessible only to authorized entities?

- [ ] **A)** Confidentiality
- [ ] **B)** Integrity
- [ ] **C)** Availability
- [ ] **D)** AAA

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Confidentiality is the property that information is not disclosed to unauthorized individuals. Integrity ensures data is not modified, availability ensures it is accessible, and AAA is about access control and accounting.
 
 
</details>

### 10. Which of the following are characteristics of the principle of Least Privilege? (Select two)

- [ ] **A)** Users are granted the maximum set of permissions by default
- [ ] **B)** Processes and services should operate with the minimal rights necessary
- [ ] **C)** Access rights are periodically reviewed and adjusted
- [ ] **D)** All users in an organization share identical privilege levels

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Least Privilege dictates that users and processes get only the minimum permissions needed. Default maximum access violates this, and periodic reviews ensure privileges remain minimal.
 
 
</details>

### 11. Based on the code snippet, what type of malware is described?

```python
import socket
import sys

# Exploit SMB vulnerability to copy itself to remote hosts
def propagate():
    for host in scan_network():
        if exploit_smb(host):
            copy_self(host)

while True:
    propagate()
    time.sleep(60)
```

- [ ] **A)** Trojan
- [ ] **B)** Worm
- [ ] **C)** Ransomware
- [ ] **D)** Spyware

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code shows self-replication and network propagation without user action, which is characteristic of a worm.
 
 
</details>

### 12. What is the primary goal of a phishing attack?

- [ ] **A)** Credential harvesting
- [ ] **B)** Network service disruption
- [ ] **C)** Encryption of user files
- [ ] **D)** Physical intrusion into facilities

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Phishing primarily aims to trick users into revealing login credentials or personal information. Credential harvesting is the most common goal.
 
 
</details>

### 13. Which of the following are properties of cryptographic hashing? (Select two)

- [ ] **A)** The process is reversible given enough time
- [ ] **B)** The output is a fixed-length string regardless of input size
- [ ] **C)** Hashing provides confidentiality of the original data
- [ ] **D)** It is a one-way function

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Hash functions produce a fixed-length output and are one-way (cannot be reversed). They do not provide confidentiality; that is the role of encryption.
 
 
</details>

### 14. In the provided code snippet, what security objective is achieved by the digital signature?

```pseudocode
message = "Transfer $1000 to account 12345"
hash = SHA256(message)
signature = RSA_encrypt(hash, private_key)
# send message + signature + public_key
```

- [ ] **A)** Confidentiality
- [ ] **B)** Integrity only
- [ ] **C)** Authentication and integrity
- [ ] **D)** Non-repudiation only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> A digital signature encrypted with the sender's private key provides authentication of origin and integrity of the message. It does not provide confidentiality on its own.
 
 
</details>


---

### **Security Operations and Monitoring**

### 15. What is the primary function of a Security Information and Event Management (SIEM) system?

- [ ] **A)** Capture and analyze full network packet payloads
- [ ] **B)** Collect logs from multiple sources and correlate them for threat detection
- [ ] **C)** Provide real-time prevention of all known malware
- [ ] **D)** Replace the need for firewalls and intrusion prevention systems

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A SIEM aggregates logs from diverse sources, normalizes them, and applies correlation rules to detect security incidents.
 
 
</details>

### 16. Which two of the following are typical data sources for a SIEM system? (Choose two.)

- [ ] **A)** Syslog messages from network devices
- [ ] **B)** Full packet captures from every link
- [ ] **C)** NetFlow records from routers
- [ ] **D)** Physical access control system logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> SIEM commonly ingests Syslog events and NetFlow metadata. Full packet captures are typically handled by separate tools, and physical access logs are less common.
 
 
</details>

### 17. Examine the following Cisco IOS command. What is the purpose of the highlighted parameter?

```cisco-ios
logging trap 4
```

- [ ] **A)** It sets the IP address of the Syslog server
- [ ] **B)** It defines the maximum severity level (0-4) to be sent
- [ ] **C)** It specifies the source interface for logging
- [ ] **D)** It enables logging globally on the device

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 'logging trap 4' command configures the device to send only messages with severity 0 (Emergency) through 4 (Warning) to the Syslog server.
 
 
</details>

### 18. What does NetFlow collect from network traffic?

- [ ] **A)** Full packet payloads including application data
- [ ] **B)** Metadata such as IP addresses, ports, and protocol
- [ ] **C)** Encrypted passwords and authentication tokens
- [ ] **D)** Detailed file contents and email bodies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> NetFlow exports metadata (5-tuple, bytes, packets) without inspecting payloads, making it suitable for traffic analysis but not deep packet inspection.
 
 
</details>

### 19. Which two of the following are Syslog severity levels defined in RFC 5424? (Choose two.)

- [ ] **A)** Alert (level 1)
- [ ] **B)** Critical (level 2)
- [ ] **C)** Warning (level 4)
- [ ] **D)** Debug (level 7)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Alert (1) and Critical (2) are valid levels. Warning is level 4 and Debug is level 7, but the question asks for two options that are correct from the given set; only Alert and Critical are listed.
 
 
</details>

### 20. Review the following hypothetical Syslog message. What severity level does it represent?

```syslog
*Mar 1 02:34:56.789: %LINEPROTO-3-UPDOWN: Line protocol on Interface GigabitEthernet0/1, changed state to down
```

- [ ] **A)** Emergency (0)
- [ ] **B)** Error (3)
- [ ] **C)** Notice (5)
- [ ] **D)** Informational (6)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The '%LINEPROTO-3-UPDOWN' message contains a '3', which corresponds to Syslog severity 3 (Error).
 
 
</details>

### 21. Which phase of incident response involves stopping the spread of a threat?

- [ ] **A)** Detection
- [ ] **B)** Analysis
- [ ] **C)** Containment
- [ ] **D)** Eradication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Containment aims to prevent the incident from escalating by isolating affected systems or blocking malicious activity.
 
 
</details>

### 22. Which two actions are part of the eradication phase of incident response? (Choose two.)

- [ ] **A)** Deleting malware from infected systems
- [ ] **B)** Restoring data from clean backups
- [ ] **C)** Revoking compromised user credentials
- [ ] **D)** Conducting a lessons-learned meeting

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Eradication removes the root cause, such as malware and compromised accounts. Restoring data is part of recovery; lessons-learned is post-incident.
 
 
</details>

### 23. The following is a routine firewall log entry. Classify the event. Which type of detection does it represent?

```syslog
Mar 1 10:00:00 192.168.1.1 %FW-4-DENY: access-list 101 denied tcp 10.0.0.2(54321) -> 203.0.113.5(80)
```

- [ ] **A)** Signature-based detection
- [ ] **B)** Anomaly-based detection
- [ ] **C)** Heuristic analysis
- [ ] **D)** Behavioral baseline

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The log shows a 'Deny' action based on a known rule (blocking a specific IP), which is signature-based (or rule-based) detection.
 
 
</details>

### 24. An organization uses anti-malware that checks files against a database of known threat hashes. What type of detection is this?

- [ ] **A)** Behavioral detection
- [ ] **B)** Signature-based detection
- [ ] **C)** Heuristic analysis
- [ ] **D)** Anomaly detection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Signature-based detection uses precomputed hashes or byte patterns to identify known malware. It is fast but cannot detect unknown variants.
 
 
</details>

### 25. Which two of the following are advantages of application whitelisting? (Choose two.)

- [ ] **A)** It can block zero-day malware that has no signature
- [ ] **B)** It eliminates the need for any other security software
- [ ] **C)** It reduces the attack surface by only allowing approved executables
- [ ] **D)** It automatically updates its rules based on user behavior

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Application whitelisting prevents execution of any untrusted code, including zero-day threats, and limits allowed software to a predefined list.
 
 
</details>

### 26. Examine the following Host-Based IDS alert. What is the most likely cause of this event?

```plaintext
HIDS Alert: File integrity violation - /Windows/System32/svchost.exe - expected hash: a1b2c3d4, observed hash: e5f6g7h8
```

- [ ] **A)** A rootkit has modified the system file
- [ ] **B)** A legitimate software update occurred
- [ ] **C)** The file was deleted by the user
- [ ] **D)** The log is a false positive from a scheduled scan

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The alert shows an unexpected hash change on a critical system file (svchost.exe), which typically indicates a rootkit or unauthorized modification.
 
 
</details>

### 27. In Syslog configuration on a Cisco IOS device, which command sets the IP address of the remote log collector?

- [ ] **A)** logging host 192.168.1.100
- [ ] **B)** log server 192.168.1.100
- [ ] **C)** syslog collector 192.168.1.100
- [ ] **D)** logging destination 192.168.1.100

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command 'logging host <ip>' configures the remote Syslog server destination on Cisco IOS devices.
 
 
</details>

### 28. Which two of the following are common Indicators of Compromise (IOCs) that can be found in security logs? (Choose two.)

- [ ] **A)** Known malicious IP address
- [ ] **B)** A user's forgotten password attempt
- [ ] **C)** Suspicious file hash
- [ ] **D)** Normal business email traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> IOCs are specific evidence of compromise, such as known bad IPs and file hashes. Forgotten passwords and normal traffic are not IOCs.
 
 
</details>

### 29. The following NetFlow configuration snippet is applied on a Cisco router. What key piece of information is missing?

```cisco-ios
ip flow-export version 9
ip flow-export source Loopback0
```

- [ ] **A)** The destination IP address of the NetFlow collector
- [ ] **B)** The NetFlow version (e.g., version 9)
- [ ] **C)** The source interface for flow export
- [ ] **D)** The 'ip flow-export destination' command

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> The configuration shows the version and source interface but lacks the required 'ip flow-export destination' command to specify the collector IP and port.
 
 
</details>

### 30. During which incident response phase is a host-based intrusion detection system most actively used?

- [ ] **A)** Detection
- [ ] **B)** Analysis
- [ ] **C)** Containment
- [ ] **D)** Recovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> HIDS generates alerts during detection, but those alerts are analyzed in the Analysis phase to validate and scope the incident.
 
 
</details>

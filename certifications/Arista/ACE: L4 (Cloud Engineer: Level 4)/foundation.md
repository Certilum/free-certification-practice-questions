<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Arista/ACE:%20L4%20(Arista%20Cloud%20Engineer:%20Level%204)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>ACE: L4 (Cloud Engineer: Level 4)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Advanced Troubleshooting and Optimization](#advanced-troubleshooting-and-optimization) (2 questions)
- [Automation and Orchestration](#automation-and-orchestration) (7 questions)
- [Cloud Infrastructure Design](#cloud-infrastructure-design) (9 questions)
- [Cloud Operations and Monitoring](#cloud-operations-and-monitoring) (6 questions)
- [Security and Compliance](#security-and-compliance) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:53.028Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Advanced Troubleshooting and Optimization | 2 |
| Automation and Orchestration | 7 |
| Cloud Infrastructure Design | 9 |
| Cloud Operations and Monitoring | 6 |
| Security and Compliance | 6 |

---

### **Advanced Troubleshooting and Optimization**

### 1. Which method of packet capture on Arista EOS copies frames directly from the ASIC to a destination port with minimal performance impact?

- [ ] **A)** Off-chip mirroring using tcpdump
- [ ] **B)** On-chip mirroring using monitor session
- [ ] **C)** Mirror-to-CPU via hardware capture profile
- [ ] **D)** Using show platform port-asic drop

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> On-chip mirroring (monitor session) uses ASIC to copy frames, minimizing CPU impact.
 
 
</details>

### 2. Which of the following are true about CoPP (Control Plane Protection) impact on debug traps when mirroring to CPU? (Select all that apply)

- [ ] **A)** CoPP can drop debug packets before they reach the kernel
- [ ] **B)** CoPP policer applies to all traffic mirrored to CPU
- [ ] **C)** CoPP is not applied to hardware monitor sessions
- [ ] **D)** CoPP raises burst rates for debug sessions automatically

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> CoPP policer applies to CPU-bound traffic; high-rate debug packets may be dropped. Hardware monitor sessions bypass CoPP.
 
 
</details>


---

### **Automation and Orchestration**

### 3. Which of the following best describes the primary function of CloudVision Portal (CVP) in an Arista network?

- [ ] **A)** It acts as a centralized management and automation platform for the entire network fabric.
- [ ] **B)** It replaces the need for device-level CLI commands entirely.
- [ ] **C)** It is a tool for monitoring but does not handle configuration changes.
- [ ] **D)** It manages individual device configurations but does not support intent-based networking.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CloudVision is a management and automation platform that provides a single point of control, enabling intent-based operations across the fabric. It does not replace CLI but abstracts it, and it does handle configuration changes and monitoring.
 
 
</details>

### 4. Which two components are part of the Arista Automation Framework? (Choose two.)

- [ ] **A)** eAPI (JSON-RPC over HTTP/HTTPS)
- [ ] **B)** SNMP (Simple Network Management Protocol)
- [ ] **C)** CloudVision eXchange (CVX)
- [ ] **D)** NETCONF over SSH

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The Arista Automation Framework includes eAPI and CloudVision eXchange (CVX) for multi-cluster management. SNMP and NETCONF are not part of the Arista's specific automation framework as described in the playbook.
 
 
</details>

### 5. Examine the following Python snippet used to authenticate with CloudVision REST API. What critical step is missing for handling token expiry in a production script?

```python
import requests

url = "https://cvp.example.com/cvpservice/login/authenticate"
payload = {"userId": "admin", "password": "secret"}
response = requests.post(url, json=payload)
token = response.json()["sessionId"]
# Later use token in headers
headers = {"Authorization": f"Bearer {token}"}
# Subsequent API calls use this token indefinitely
```

- [ ] **A)** The script does not check if the token has expired and does not implement a refresh mechanism.
- [ ] **B)** The script uses HTTP instead of HTTPS.
- [ ] **C)** The script does not parse the JSON response.
- [ ] **D)** The script does not set the 'Content-Type' header.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In production, tokens expire; a robust script must check expiration and refresh automatically. The snippet shows a one-time authentication without any refresh logic. The other options are not present as issues in the snippet.
 
 
</details>

### 6. What is the purpose of TerminAttr agent on Arista switches?

- [ ] **A)** It establishes a secure outbound gRPC connection to CloudVision for telemetry and configuration.
- [ ] **B)** It is a CLI tool for manual switch configuration.
- [ ] **C)** It acts as an SNMP trap receiver.
- [ ] **D)** It performs routing protocol updates between switches.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TerminAttr is a daemon that establishes an outbound gRPC tunnel to CloudVision, enabling configuration pushes and telemetry streaming. It is not a CLI tool, not SNMP, and does not perform routing.
 
 
</details>

### 7. Which two statements about eAPI (Extended API) on Arista switches are correct? (Choose two.)

- [ ] **A)** eAPI uses JSON-RPC over HTTP/HTTPS.
- [ ] **B)** eAPI supports both 'enable' and 'config' modes.
- [ ] **C)** eAPI uses SSH as the transport protocol.
- [ ] **D)** eAPI is stateful and maintains session context.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> eAPI is a JSON-RPC API over HTTP/HTTPS, supporting enable and config modes. It is stateless, not SSH-based, and does not maintain session context.
 
 
</details>

### 8. Consider the following Terraform configuration block. What does this configuration do in the context of Arista CloudVision integration?

```hcl
resource "arista_cloudvision_configlet" "example" {
  name    = "DC1-VLANs"
  config  = "vlan 100\nname prod"
}
```

- [ ] **A)** It creates a new configlet in CloudVision with the specified name and configuration.
- [ ] **B)** It applies the configlet to a device device.
- [ ] **C)** It deletes an existing configlet from CloudVision.
- [ ] **D)** It retrieves the current state of a configlet.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code defines a Terraform resource for an Arista CloudVision configlet. The 'config' parameter contains the CLI commands. This is a creation operation. Applying to a device would require a separate resource.
 
 
</details>

### 9. What is the difference between Ansible and Terraform in terms of their automation paradigms?

- [ ] **A)** Ansible is imperative (procedural), while Terraform is declarative (desired state).
- [ ] **B)** Ansible is declarative, while Terraform is imperative.
- [ ] **C)** Both are declarative, but Terraform uses YAML.
- [ ] **D)** Both are imperative, but Ansible uses HCL.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Ansible defines steps to achieve a state (imperative), while Terraform defines the end state and computes the steps (declarative). Ansible uses YAML, Terraform uses HCL.
 
 
</details>


---

### **Cloud Infrastructure Design**

### 10. What encapsulation method does VXLAN use to carry Layer 2 frames over Layer 3 networks?

- [ ] **A)** MAC-in-UDP
- [ ] **B)** IP-in-IP
- [ ] **C)** GRE
- [ ] **D)** MPLS-in-UDP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> VXLAN encapsulates the original Layer 2 frame inside a UDP packet using MAC-in-UDP encapsulation (MAC header + payload inside UDP).
 
 
</details>

### 11. Which two components are part of an EVPN control plane for VXLAN?

- [ ] **A)** BGP
- [ ] **B)** VXLAN Network Identifier (VNI)
- [ ] **C)** MP-BGP with EVPN address family
- [ ] **D)** VLAN ID

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> EVPN uses BGP as the transport protocol and the MP-BGP EVPN address family to exchange MAC and IP reachability information.
 
 
</details>

### 12. In the provided code snippet for Arista EOS, which command sets the source interface for VXLAN traffic?

```arista_eos
interface Vxlan1
 source-interface Loopback0
!
```

- [ ] **A)** source-interface Loopback0
- [ ] **B)** vxlan source-interface Loopback0
- [ ] **C)** ip local-interface Loopback0
- [ ] **D)** interface vxlan1 source-interface Loopback0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In Arista EOS, the VTEP source interface is configured with 'source-interface Loopback0' under interface Vxlan1.
 
 
</details>

### 13. How many logical networks does VXLAN support?

- [ ] **A)** 16 million
- [ ] **B)** 4094
- [ ] **C)** 4 billion
- [ ] **D)** 65535

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> VXLAN uses a 24-bit VNI (VXLAN Network Identifier) allowing up to 16 million logical networks.
 
 
</details>

### 14. Which two EVPN route types are directly related to MAC and IP advertisement?

- [ ] **A)** Type 2 (MAC/IP Advertisement)
- [ ] **B)** Type 5 (IP prefix advertisement)
- [ ] **C)** Type 3 (Inclusive Multicast)
- [ ] **D)** Type 1 (Ethernet AD)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Type 2 advertises MAC and IP, Type 5 advertises IP prefixes. Type 3 builds multicast tunnels, Type 1 is for multihoming.
 
 
</details>

### 15. Given the EVPN route type in the code comment, which BGP NLRI type is responsible for distributing multicast membership?

```plaintext
! BGP EVPN route types:
! Type 3 - Inclusive Multicast Ethernet Tag
! Used for BUM replication
```

- [ ] **A)** Type 3
- [ ] **B)** Type 2
- [ ] **C)** Type 1
- [ ] **D)** Type 5

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> EVPN Type 3 (Inclusive Multicast Ethernet Tag) is used to build multicast tunnels or head-end replication lists for BUM traffic.
 
 
</details>

### 16. Which IP address does a VTEP use as source for VXLAN encapsulation?

- [ ] **A)** Loopback address
- [ ] **B)** Physical interface IP
- [ ] **C)** VLAN SVI IP
- [ ] **D)** Management interface IP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The VTEP uses a loopback IP address (unique per switch) as the source and destination of VXLAN tunnels.
 
 
</details>

### 17. Which two statements are true about the relationship between underlay and overlay in VXLAN/EVPN?

- [ ] **A)** The underlay is unaware of VXLAN or EVPN.
- [ ] **B)** The overlay provides tenant isolation.
- [ ] **C)** The underlay must support VXLAN encapsulation.
- [ ] **D)** The overlay uses the same routing instance as the underlay.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The underlay is a simple IP network for VTEP reachability; the overlay (VXLAN/EVPN) is isolated and handles tenant segmentation.
 
 
</details>

### 18. In the provided code, which command configures an anycast gateway MAC address on an Arista leaf?

```arista_eos
ip virtual-router address 10.1.1.1
! Configures anycast gateway on leaf
```

- [ ] **A)** ip virtual-router address
- [ ] **B)** ip anycast-address
- [ ] **C)** gateway address
- [ ] **D)** vrf gateway

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'ip virtual-router address' command (or 'ip virtual-router mac-address') configures the anycast gateway IP/MAC on Arista switches.
 
 
</details>


---

### **Cloud Operations and Monitoring**

### 19. What is the primary data encoding format used by CloudVision Telemetry?

- [ ] **A)** Google Protocol Buffers
- [ ] **B)** JSON
- [ ] **C)** XML
- [ ] **D)** BSON

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CloudVision Telemetry uses Google Protocol Buffers (protobuf) for efficient, compact binary encoding.
 
 
</details>

### 20. Which two models are used by CloudVision for data collection?

- [ ] **A)** Push-based streaming
- [ ] **B)** Pull-based polling
- [ ] **C)** Only push-based
- [ ] **D)** Only pull-based

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CloudVision supports both push-based streaming telemetry and traditional pull-based polling (SNMP).
 
 
</details>

### 21. Examine the following EOS CLI configuration. What does this command enable?

```eos
management telemetry
  mode streaming
```

- [ ] **A)** CloudVision Telemetry agent
- [ ] **B)** SNMP polling agent
- [ ] **C)** Syslog server
- [ ] **D)** gNMI collector

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command 'management telemetry' enables the CloudVision Telemetry agent on the device.
 
 
</details>

### 22. What is the name of Arista's in-memory real-time database that holds operational state?

- [ ] **A)** NetDB
- [ ] **B)** SysDB
- [ ] **C)** ConfigDB
- [ ] **D)** TimeSeriesDB

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NetDB (Network Database) is Arista's in-memory real-time database for operational and protocol state.
 
 
</details>

### 23. Which two of the following are types of telemetry streams in CloudVision?

- [ ] **A)** Periodic streaming
- [ ] **B)** Event-driven streaming
- [ ] **C)** Poll-based streaming
- [ ] **D)** Batch streaming

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CloudVision supports periodic (time-based) and event-driven (change-based) telemetry streams.
 
 
</details>

### 24. Refer to the code snippet. What protocol does CloudVision Telemetry use to transport data?

```eos
management telemetry
  destination collector 192.168.1.100 port 5700 protocol tcp
```

- [ ] **A)** TCP
- [ ] **B)** UDP
- [ ] **C)** ICMP
- [ ] **D)** SCTP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CloudVision Telemetry sends data over TCP or secured TLS sessions.
 
 
</details>


---

### **Security and Compliance**

### 25. What is the core tenet of Zero Trust networking according to Arista's security model?

- [ ] **A)** Trust but verify
- [ ] **B)** Never trust, always verify
- [ ] **C)** Always trust, verify occasionally
- [ ] **D)** Trust based on location

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Zero Trust's core tenet is 'never trust, always verify,' requiring continuous authentication, authorization, and encryption for every request, regardless of network location.
 
 
</details>

### 26. Which of the following are key components of a Zero Trust Architecture as defined by NIST SP 800-207? (Select all that apply.)

- [ ] **A)** Policy Engine (PE)
- [ ] **B)** Policy Administrator (PA)
- [ ] **C)** Policy Enforcement Point (PEP)
- [ ] **D)** Policy Decision Point (PDP)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> NIST SP 800-207 defines three core components: Policy Engine, Policy Administrator, and Policy Enforcement Point. PDP is part of the Policy Engine but not a separate core component.
 
 
</details>

### 27. Examine the Arista EOS configuration snippet. Which feature is being configured to secure hop-by-hop Layer 2 traffic?

```eos
interface Ethernet1
   macsec
   macsec cipher gcm-aes-256
   macsec key chain KEYCHAIN
   macsec key 0 key hex 0123456789ABCDEF0123456789ABCDEF
```

- [ ] **A)** IPsec
- [ ] **B)** MACsec
- [ ] **C)** SSL/TLS
- [ ] **D)** WireGuard

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The command 'macsec' under interface configuration enables MACsec (802.1AE) for Layer 2 encryption. The presence of 'cipher gcm-aes-256' confirms the protocol.
 
 
</details>

### 28. What is the main purpose of microsegmentation in a Zero Trust environment?

- [ ] **A)** To reduce the number of VLANs needed
- [ ] **B)** To prevent lateral movement by dividing the network into logical security zones
- [ ] **C)** To increase broadcast traffic efficiency
- [ ] **D)** To replace firewalls entirely

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Microsegmentation divides the network into logical zones based on workload or sensitivity, allowing fine-grained policies that prevent attackers from moving laterally after a breach.
 
 
</details>

### 29. Which Arista components map to the Zero Trust roles of Policy Administrator (PA) and Policy Enforcement Point (PEP)? (Select two answers.)

- [ ] **A)** CloudVision
- [ ] **B)** Arista EOS switch
- [ ] **C)** Firewall
- [ ] **D)** RADIUS server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CloudVision acts as both Policy Engine and Policy Administrator. Arista EOS switches serve as Policy Enforcement Points (PEPs).
 
 
</details>

### 30. Look at the ACL configuration. Which type of traffic is explicitly permitted by this Access Control List?

```eos
ip access-list standard HTTPS_ONLY
   permit tcp any any eq 443
   deny ip any any log
```

- [ ] **A)** HTTP (TCP/80)
- [ ] **B)** HTTPS (TCP/443)
- [ ] **C)** SSH (TCP/22)
- [ ] **D)** DNS (UDP/53)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The ACL entry 'permit tcp any any eq 443' allows HTTPS traffic on TCP port 443. The '500-600' range is not defined; only port 443 is explicitly permitted.
 
 
</details>

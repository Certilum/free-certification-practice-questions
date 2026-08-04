<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Arista/ACE:%20L2%20(Arista%20Cloud%20Engineer:%20Level%202)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>ACE: L2 (Cloud Engineer: Level 2)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Automation and Orchestration](#automation-and-orchestration) (7 questions)
- [Cloud Architecture and Design](#cloud-architecture-and-design) (5 questions)
- [Cloud Networking Fundamentals](#cloud-networking-fundamentals) (6 questions)
- [Monitoring and Troubleshooting](#monitoring-and-troubleshooting) (6 questions)
- [Security and Segmentation](#security-and-segmentation) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:47.735Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Automation and Orchestration | 7 |
| Cloud Architecture and Design | 5 |
| Cloud Networking Fundamentals | 6 |
| Monitoring and Troubleshooting | 6 |
| Security and Segmentation | 6 |

---

### **Automation and Orchestration**

### 1. What is CloudVision (CVP) in the context of Arista networks?

- [ ] **A)** A centralized network management and automation platform
- [ ] **B)** A CLI tool for configuring individual switches
- [ ] **C)** A routing protocol for data center fabrics
- [ ] **D)** A packet capture and analysis software

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CloudVision is a centralized management platform that abstracts device configurations into an intent-based model.
 
 
</details>

### 2. Which two northbound interfaces does CloudVision (CVP) expose for automation?

- [ ] **A)** REST API
- [ ] **B)** gNMI
- [ ] **C)** SNMP
- [ ] **D)** NetFlow

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CVP exposes REST API and gNMI among others; SNMP and NetFlow are legacy protocols not used for CVP integration.
 
 
</details>

### 3. Examine the following Python script that uses pyeapi to configure a VLAN. Identify the missing step before the configuration commands.

```python
import pyeapi

# Missing step
node = pyeapi.connect(host='10.0.0.1', username='admin', password='admin')

node.api('vlans').create(100)
```

- [ ] **A)** Authentication and session creation
- [ ] **B)** Importing the netmiko library
- [ ] **C)** Opening an SSH tunnel
- [ ] **D)** Starting a web server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> pyeapi requires authentication (e.g., using Node or connect methods) before sending config commands.
 
 
</details>

### 4. What is the primary function of TerminAttr on an Arista switch?

- [ ] **A)** Streaming state and receiving configuration push from CVP
- [ ] **B)** Performing packet forwarding lookups
- [ ] **C)** Managing routing protocols
- [ ] **D)** Collecting SNMP statistics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TerminAttr is the daemon that streams device state to CVP and accepts config pushes.
 
 
</details>

### 5. Which of the following are valid methods for Arista eAPI authentication?

- [ ] **A)** HTTP Basic Authentication
- [ ] **B)** Token-based authentication
- [ ] **C)** OAuth 2.0
- [ ] **D)** LDAP bind

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> eAPI supports HTTP Basic and token-based authentication; OAuth and LDAP bind are not used.
 
 
</details>

### 6. Analyze this Ansible task snippet. What is the purpose of the 'wait_for' parameter?

```yaml
- name: Check BGP state
  arista.eos.eos_command:
    commands:
      - show bgp summary
    wait_for:
      - result[0] contains 'Established'
```

- [ ] **A)** Polls the device until a condition is met or timeout expires
- [ ] **B)** Delays execution for a fixed number of seconds
- [ ] **C)** Waits for a user approval before continuing
- [ ] **D)** Schedules the task to run later

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'wait_for' parameter in eos_command polls the device output until the condition is satisfied or the timeout elapses.
 
 
</details>

### 7. Which CloudVision endpoint should be used to apply a configuration change in a transactional manner?

- [ ] **A)** /changeControl
- [ ] **B)** /configlet
- [ ] **C)** /inventory
- [ ] **D)** /user

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The /changeControl endpoint ensures transactional rollback and audit trail, unlike /configlet which only updates a snippet.
 
 
</details>


---

### **Cloud Architecture and Design**

### 8. Which layer in a leaf-spine architecture is responsible for connecting to servers and storage?

- [ ] **A)** Spine layer
- [ ] **B)** Leaf layer
- [ ] **C)** Core layer
- [ ] **D)** Access layer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Leaf switches connect directly to servers, storage, and other endpoints, while spines provide inter-leaf connectivity.
 
 
</details>

### 9. Which two statements are true about leaf-spine architecture?

- [ ] **A)** Each leaf connects to every spine
- [ ] **B)** Spines interconnect to provide redundancy
- [ ] **C)** ECMP is used for load balancing across spines
- [ ] **D)** Spanning Tree Protocol is required

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Leaf-spine uses a full mesh between leaves and spines, and ECMP distributes traffic. Spines do not connect to each other and STP is eliminated.
 
 
</details>

### 10. What does the command 'ip routing' enable on a leaf switch?

```none
ip routing
```

- [ ] **A)** Layer 2 switching
- [ ] **B)** IP forwarding
- [ ] **C)** VXLAN encapsulation
- [ ] **D)** Spanning tree

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 'ip routing' command enables Layer 3 forwarding (routing) of IP packets on the switch.
 
 
</details>

### 11. What is the minimum recommended number of spine switches for a highly available leaf-spine fabric?

- [ ] **A)** 1
- [ ] **B)** 2
- [ ] **C)** 4
- [ ] **D)** 8

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Arista recommends at least two spine switches to eliminate a single point of failure and provide redundancy.
 
 
</details>

### 12. Which two protocols can be used in the underlay of an Arista leaf-spine network?

- [ ] **A)** eBGP
- [ ] **B)** OSPF
- [ ] **C)** VXLAN
- [ ] **D)** EVPN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The underlay (physical network) uses IP routing protocols like eBGP (recommended) or OSPF. VXLAN and EVPN are overlay technologies.
 
 
</details>


---

### **Cloud Networking Fundamentals**

### 13. Which UDP port is standard for VXLAN encapsulation?

- [ ] **A)** 4789
- [ ] **B)** 4788
- [ ] **C)** 179
- [ ] **D)** 5000

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> VXLAN uses UDP destination port 4789 for MAC-in-UDP encapsulation.
 
 
</details>

### 14. Which two EVPN route types are part of the EVPN specification?

- [ ] **A)** Type-2
- [ ] **B)** Type-3
- [ ] **C)** Type-6
- [ ] **D)** Type-0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> EVPN includes Type-2 (MAC/IP) and Type-3 (IMET) routes, among others.
 
 
</details>

### 15. Based on the output, which route type is not shown and is used for ES auto-discovery?

```text
BGP EVPN routes:
Type-2: MAC 00:11:22:33:44:55
Type-3: VNI 100
Type-5: 10.0.0.0/24
```

- [ ] **A)** Type-1
- [ ] **B)** Type-2
- [ ] **C)** Type-3
- [ ] **D)** Type-4

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> EVPN Type-1 route is used for Ethernet Segment auto-discovery.
 
 
</details>

### 16. What does the acronym VNI represent in VXLAN?

- [ ] **A)** VXLAN Network Identifier
- [ ] **B)** VLAN Network Identifier
- [ ] **C)** VXLAN Node Identifier
- [ ] **D)** Virtual Node Interface

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> VNI stands for VXLAN Network Identifier, a 24-bit field.
 
 
</details>

### 17. Select two correct statements regarding anycast VTEP in Arista EVPN.

- [ ] **A)** It uses a shared IP address across multiple leafs.
- [ ] **B)** It uses a shared MAC address across leafs.
- [ ] **C)** It enables active-active redundancy.
- [ ] **D)** It requires a multicast underlay.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Anycast VTEP uses a common IP but unique MAC per leaf, providing active-active redundancy.
 
 
</details>

### 18. Which address family is missing from this BGP configuration for EVPN support?

```text
router bgp 65000
  neighbor 10.0.0.1 remote-as 65001
  ! missing address family
```

- [ ] **A)** address-family l2vpn evpn
- [ ] **B)** address-family vpnv4
- [ ] **C)** address-family ipv4
- [ ] **D)** address-family rtfilter

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> EVPN requires the address-family l2vpn evpn under BGP configuration.
 
 
</details>


---

### **Monitoring and Troubleshooting**

### 19. Which protocol is used by Arista EOS to manage telemetry subscriptions?

- [ ] **A)** SNMP
- [ ] **B)** gNMI
- [ ] **C)** NETCONF
- [ ] **D)** RESTCONF

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> gNMI (gRPC Network Management Interface) is the standard protocol used by Arista for telemetry subscriptions.
 
 
</details>

### 20. Which of the following are valid telemetry subscription modes in Arista EOS? (Select two.)

- [ ] **A)** ON_CHANGE
- [ ] **B)** SAMPLE
- [ ] **C)** POLL
- [ ] **D)** PUSH_ONLY

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Arista EOS supports ON_CHANGE and SAMPLE subscription modes. POLL is not a valid telemetry mode; it is associated with SNMP.
 
 
</details>

### 21. Examine the command output below. What does it indicate about the telemetry agent status?

```console
show telemetry agent status
Agent: telemetry_agent
State: Connected
Destination: 10.10.10.1:9001
Encoding: protobuf
Compression: gzip
Streams Active: 5
Last Error: None
```

- [ ] **A)** The telemetry agent is connected and sending data.
- [ ] **B)** The telemetry agent is not configured.
- [ ] **C)** The telemetry agent is disconnected but retrying.
- [ ] **D)** The telemetry agent has encountered a configuration error.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'show telemetry agent status' output displays 'State: Connected' and 'Streams Active: 5', indicating the agent is successfully connected and sending data.
 
 
</details>

### 22. Which data type is best suited for monitoring interface byte counts over time?

- [ ] **A)** Gauge
- [ ] **B)** Counter
- [ ] **C)** Histogram
- [ ] **D)** State

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Counters are cumulative integers that increase monotonically, making them ideal for monitoring traffic volume over time.
 
 
</details>

### 23. Which of the following are advantages of streaming telemetry over SNMP? (Select two.)

- [ ] **A)** Push-based data delivery reduces polling overhead.
- [ ] **B)** Higher polling frequency due to pull model.
- [ ] **C)** Supports sub-second update intervals.
- [ ] **D)** Uses UDP for guaranteed delivery.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Streaming telemetry pushes data, reducing device CPU load, and supports sub-second updates. SNMP uses UDP and is pull-based.
 
 
</details>

### 24. Evaluate the following telemetry configuration. Which mode and path are being subscribed to?

```eos
telemetry agent test
  subscription int-counters path /interfaces/interface/state/counters mode sample sample-interval 30
```

- [ ] **A)** Sample mode subscribing to /interfaces/interface/state/counters
- [ ] **B)** On-change mode subscribing to /interfaces/interface/state/counters
- [ ] **C)** Sample mode subscribing to /system/memory/state
- [ ] **D)** On-change mode subscribing to /system/memory/state

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The configuration shows 'mode sample sample-interval 30' and the path '/interfaces/interface/state/counters', matching a sample-based subscription for interface counters.
 
 
</details>


---

### **Security and Segmentation**

### 25. What is the maximum number of VLANs allowed in 802.1Q?

- [ ] **A)** 4096
- [ ] **B)** 4094
- [ ] **C)** 16 million
- [ ] **D)** 65535

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> IEEE 802.1Q defines a 12-bit VLAN ID field, allowing a maximum of 4094 usable VLANs (0 and 4095 are reserved).
 
 
</details>

### 26. Which of the following are characteristics of VXLAN? (Select two)

- [ ] **A)** Encapsulates Ethernet frames in UDP packets
- [ ] **B)** Uses a 24-bit VNI for network identification
- [ ] **C)** Uses a 12-bit VLAN ID
- [ ] **D)** Always requires multicast in the underlay

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VXLAN encapsulates Ethernet in UDP and uses a 24-bit VNI. It can use multicast or BGP EVPN for control plane; multicast is not always required.
 
 
</details>

### 27. Refer to the configuration. What is the VNI assigned to VLAN 10?

```eos
interface Vxlan1
   vxlan source-interface Loopback0
   vxlan udp-port 4789
   vlan-to-vni vlan 10 vni 10010
```

- [ ] **A)** 10
- [ ] **B)** 10010
- [ ] **C)** 4789
- [ ] **D)** 0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The command 'vlan-to-vni vlan 10 vni 10010' maps VLAN 10 to VNI 10010.
 
 
</details>

### 28. What is the role of BGP EVPN in VXLAN?

- [ ] **A)** Data plane encryption
- [ ] **B)** Control plane for distributing MAC/IP routes
- [ ] **C)** Underlay routing protocol
- [ ] **D)** Firewall integration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> BGP EVPN acts as the control plane for VXLAN, exchanging MAC and IP routes between VTEPs to enable host-based learning.
 
 
</details>

### 29. Which two statements about MACsec are true? (Select two)

- [ ] **A)** Encrypts the Ethernet payload using AES-GCM
- [ ] **B)** Operates at Layer 3
- [ ] **C)** Requires 802.1X to function
- [ ] **D)** Provides hop-by-hop encryption at Layer 2

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> MACsec (802.1AE) provides hop-by-hop encryption at Layer 2 using AES-GCM. It can use PSK or dynamic keys via 802.1X, but is not dependent on 802.1X.
 
 
</details>

### 30. Based on the configuration, which 802.1X role is this interface configured as?

```eos
interface Ethernet1
   description Server Port
   dot1x pae authenticator
   dot1x port-control auto
```

- [ ] **A)** Supplicant
- [ ] **B)** Authenticator
- [ ] **C)** Authentication server
- [ ] **D)** None

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The command 'dot1x pae authenticator' configures the interface as a 802.1X authenticator.
 
 
</details>

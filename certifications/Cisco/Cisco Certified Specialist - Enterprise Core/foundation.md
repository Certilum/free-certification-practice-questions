<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cisco/Cisco%20Certified%20Specialist%20-%20Enterprise%20Core.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Cisco Certified Specialist - Enterprise Core</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Architecture](#architecture) (4 questions)
- [Automation](#automation) (4 questions)
- [Infrastructure](#infrastructure) (10 questions)
- [Network Assurance](#network-assurance) (3 questions)
- [Security](#security) (6 questions)
- [Virtualization](#virtualization) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:08.694Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Architecture | 4 |
| Automation | 4 |
| Infrastructure | 10 |
| Network Assurance | 3 |
| Security | 6 |
| Virtualization | 3 |

---

### **Architecture**

### 1. What QoS mechanism buffers excess traffic to avoid drops?

- [ ] **A)** Policing
- [ ] **B)** Shaping
- [ ] **C)** WRED
- [ ] **D)** Tail drop

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Shaping buffers excess packets to stay within a rate, preventing drops.
 
 
</details>

### 2. Which two features are characteristic of a spine-leaf architecture?

- [ ] **A)** Uses Spanning Tree Protocol
- [ ] **B)** Provides equal-cost multi-path routing
- [ ] **C)** Optimized for east-west traffic
- [ ] **D)** Requires a core layer of switches

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Spine-leaf uses ECMP and is designed for east-west traffic, avoiding STP.
 
 
</details>

### 3. Based on the policy-map, what queuing type does class VOICE get?

```cisco-ios
policy-map QOS
 class VOICE
  priority level 1
  police cir 1000000
 class DATA
  bandwidth percent 50
  random-detect
!
```

- [ ] **A)** LLQ
- [ ] **B)** CBWFQ
- [ ] **C)** FIFO
- [ ] **D)** WRED

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The `priority` command under class VOICE indicates Low Latency Queuing.
 
 
</details>

### 4. Which technology uses a 24-bit identifier for network segments?

- [ ] **A)** VLAN
- [ ] **B)** VXLAN
- [ ] **C)** OTV
- [ ] **D)** STP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> VXLAN uses a 24-bit VXLAN Network Identifier (VNI) to isolate up to 16 million segments.
 
 
</details>


---

### **Automation**

### 5. What is network automation in the context of the Cisco ENCOR exam?

- [ ] **A)** The use of software, APIs, and programmable infrastructure to manage, configure, test, deploy, and operate network devices and services.
- [ ] **B)** The manual configuration of each network device using CLI commands to ensure security.
- [ ] **C)** The replacement of all network engineers with automated scripts.
- [ ] **D)** The use of SNMP to monitor network performance without making changes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Network automation involves systematic use of software and APIs for managing network devices, not just monitoring or manual CLI. It does not replace engineers but shifts their focus.
 
 
</details>

### 6. Which of the following are benefits of network automation? (Choose all that apply.)

- [ ] **A)** Reduced human error and faster troubleshooting
- [ ] **B)** Agility and faster time-to-service
- [ ] **C)** Eliminates the need for any manual CLI commands
- [ ] **D)** Consistent policy enforcement across devices

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Automation reduces errors, speeds up service delivery, and enforces consistent policies. However, it does not completely eliminate CLI usage; engineers still use CLI for troubleshooting and exceptions.
 
 
</details>

### 7. Given the following JSON snippet from a Cisco DNA Center API response, what is the healthScore of the site named 'HQ-Building'?

```json
{
  "response": [
    {
      "siteId": "12345678-1234-1234-1234-123456789abc",
      "siteName": "HQ-Building",
      "healthScore": 85,
      "issues": [
        {"issueType": "AP_DOWN", "severity": "HIGH"}
      ]
    },
    {
      "siteId": "abcdef12-...",
      "siteName": "BRANCH-OFFICE",
      "healthScore": 92,
      "issues": []
    }
  ],
  "totalRecords": 2
}
```

- [ ] **A)** 85
- [ ] **B)** 92
- [ ] **C)** 90
- [ ] **D)** 100

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In the JSON, the first object in the response array has siteName 'HQ-Building' and healthScore 85. The other values belong to different sites or are incorrect.
 
 
</details>

### 8. Which HTTP method should be used to retrieve information from a REST API?

- [ ] **A)** GET
- [ ] **B)** POST
- [ ] **C)** PUT
- [ ] **D)** DELETE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> GET is used to retrieve data without side effects. POST creates, PUT updates/replaces, and DELETE removes resources.
 
 
</details>


---

### **Infrastructure**

### 9. What is the default native VLAN on a Cisco switch trunk port?

- [ ] **A)** VLAN 1
- [ ] **B)** VLAN 99
- [ ] **C)** VLAN 1002
- [ ] **D)** VLAN 4095

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> By default, VLAN 1 is the native VLAN on Cisco switch trunk ports. It carries untagged frames. Best practices recommend changing it to an unused VLAN for security.
 
 
</details>

### 10. Which two commands are used to verify Spanning Tree Protocol operation on a Cisco switch? (Choose two.)

- [ ] **A)** show spanning-tree
- [ ] **B)** show vlan brief
- [ ] **C)** show spanning-tree vlan 10
- [ ] **D)** show interfaces trunk

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> 'show spanning-tree' (or 'show spanning-tree vlan <vlan>') displays STP root, port roles, and states. 'show vlan brief' shows VLANs and port assignments, not STP. 'show interfaces trunk' shows trunk status, not STP.
 
 
</details>

### 11. Examine the configuration snippet. What is the purpose of the 'channel-group' command?

```cisco-ios
interface GigabitEthernet0/1
 channel-group 1 mode active
```

- [ ] **A)** It bundles multiple physical interfaces into a single logical EtherChannel interface.
- [ ] **B)** It enables rapid spanning tree on the interface.
- [ ] **C)** It sets the interface as a trunk port.
- [ ] **D)** It assigns the interface to a specific VLAN.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'channel-group <number> mode <mode>' command assigns a physical interface to an EtherChannel bundle (port-channel). It does not affect STP, trunking, or VLAN assignment directly.
 
 
</details>

### 12. What is the default administrative distance of OSPF internal routes on a Cisco router?

- [ ] **A)** 110
- [ ] **B)** 90
- [ ] **C)** 20
- [ ] **D)** 120

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cisco default administrative distance for OSPF is 110. EIGRP internal is 90, eBGP is 20, RIP is 120.
 
 
</details>

### 13. Which two statements about DHCP snooping are correct? (Choose two.)

- [ ] **A)** It filters rogue DHCP servers on untrusted ports.
- [ ] **B)** It must be enabled globally and per VLAN.
- [ ] **C)** It automatically configures IP addresses on client devices.
- [ ] **D)** It is used to block STP BPDUs.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DHCP snooping is a security feature that blocks unauthorized DHCP servers. It requires both global enable ('ip dhcp snooping') and VLAN enable ('ip dhcp snooping vlan <vlan>'). It does not assign IP addresses (that's the DHCP server) and does not affect BPDUs.
 
 
</details>

### 14. Analyze the NTP configuration. What is the role of the 'prefer' keyword in this command?

```cisco-ios
ntp server 192.168.1.1 prefer
```

- [ ] **A)** It indicates the preferred NTP server if multiple servers have the same stratum.
- [ ] **B)** It forces the router to synchronize to that server regardless of stratum.
- [ ] **C)** It enables NTP authentication for that server.
- [ ] **D)** It sets the server as the only NTP source.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'prefer' keyword tells the NTP algorithm to favor that server among those with the same stratum. It does not override stratum differences, enable authentication, or restrict to a single server.
 
 
</details>

### 15. Which SNMP version supports authentication and encryption?

- [ ] **A)** SNMPv3
- [ ] **B)** SNMPv2c
- [ ] **C)** SNMPv1
- [ ] **D)** SNMPv4

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SNMPv3 provides authentication (MD5/SHA) and encryption (DES/AES). SNMPv2c uses only community strings (plaintext), and SNMPv1 also lacks security.
 
 
</details>

### 16. Which two features are used to protect the control plane on a Cisco switch? (Choose two.)

- [ ] **A)** Control Plane Policing (CoPP)
- [ ] **B)** Access Control Lists (ACLs)
- [ ] **C)** Port Security
- [ ] **D)** Control Plane Protection (CPPr)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> CoPP and CPPr are both control plane protection mechanisms. ACLs protect the data plane, and Port Security is for edge ports. CPPr is an advanced version of CoPP, but both serve the same purpose.
 
 
</details>

### 17. Refer to the SPAN configuration. What will be the effect of this configuration?

```cisco-ios
monitor session 1 source interface GigabitEthernet0/1 both
monitor session 1 destination interface GigabitEthernet0/2
```

- [ ] **A)** All traffic sent and received on GigabitEthernet0/1 is mirrored to GigabitEthernet0/2.
- [ ] **B)** Only incoming traffic on GigabitEthernet0/1 is sent to GigabitEthernet0/2.
- [ ] **C)** Traffic on GigabitEthernet0/2 is copied to GigabitEthernet0/1.
- [ ] **D)** The switch will block traffic on GigabitEthernet0/1.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'monitor session 1 source interface GigabitEthernet0/1 both' captures both directions (rx and tx) and sends it to destination interface GigabitEthernet0/2. Default direction is 'both' if not specified.
 
 
</details>

### 18. What is the purpose of the 'ip helper-address' command on a Cisco router interface?

- [ ] **A)** It forwards DHCP broadcast requests to a remote DHCP server.
- [ ] **B)** It assigns an IP address to the interface.
- [ ] **C)** It enables routing of multicast traffic.
- [ ] **D)** It translates private IP addresses to public.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> 'ip helper-address' is used for DHCP relay. It converts client broadcast DHCPDISCOVER into a unicast directed to the specified server, allowing DHCP across subnets.
 
 
</details>


---

### **Network Assurance**

### 19. Which protocol does Cisco DNA Center primarily use to discover network devices?

- [ ] **A)** CDP
- [ ] **B)** LLDP
- [ ] **C)** SNMP
- [ ] **D)** SNMP, CDP, and LLDP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> Cisco DNA Center uses a combination of SNMP, CDP, and LLDP to discover devices, not just one protocol.
 
 
</details>

### 20. Which of the following are valid authentication methods used by Cisco ISE for network access control? (Choose two.)

- [ ] **A)** 802.1X
- [ ] **B)** TACACS+
- [ ] **C)** MAC Authentication Bypass (MAB)
- [ ] **D)** SSH Key Exchange

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> ISE uses 802.1X and MAB for network access; TACACS+ is for device administration, and SSH is not an authentication method for NAC.
 
 
</details>

### 21. In the following Python code intended for RESTCONF, what is the correct media type for the Content-Type header to modify a network interface configuration?

```python
import requests
url = 'https://192.168.1.1/restconf/data/Cisco-IOS-XE-native:native/interface/GigabitEthernet=1/0/1'
headers = {'Accept': 'application/yang-data+json', 'Content-Type': 'application/yang-data+json'}
response = requests.put(url, auth=('admin', 'pass'), headers=headers, verify=False)
```

- [ ] **A)** application/json
- [ ] **B)** application/yang-data+json
- [ ] **C)** application/xml
- [ ] **D)** text/plain

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> RESTCONF requires the media type application/yang-data+json to indicate that the payload is JSON-encoded YANG data.
 
 
</details>


---

### **Security**

### 22. Which AAA protocol encrypts the entire packet payload?

- [ ] **A)** TACACS+
- [ ] **B)** RADIUS
- [ ] **C)** LDAP
- [ ] **D)** Kerberos

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TACACS+ encrypts the entire packet payload, whereas RADIUS encrypts only the password.
 
 
</details>

### 23. Which two statements accurately describe AAA protocols?

- [ ] **A)** TACACS+ uses TCP port 49.
- [ ] **B)** RADIUS encrypts the entire packet.
- [ ] **C)** RADIUS uses UDP ports 1812 and 1813.
- [ ] **D)** TACACS+ combines authentication and authorization.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> TACACS+ uses TCP port 49, and RADIUS uses UDP ports 1812/1813. RADIUS only encrypts the password.
 
 
</details>

### 24. The following configuration is missing a global command. What command must be added?

```cisco-ios
!
aaa authentication login default group tacacs+ local
!
```

- [ ] **A)** aaa new-model
- [ ] **B)** aaa authentication login default local
- [ ] **C)** username admin password cisco
- [ ] **D)** aaa authorization exec default local

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'aaa new-model' command must be issued globally before any AAA method lists can be configured.
 
 
</details>

### 25. What does Control Plane Policing (CoPP) protect?

- [ ] **A)** Control Plane (CPU)
- [ ] **B)** Data Plane
- [ ] **C)** Management Plane
- [ ] **D)** Forwarding Plane

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CoPP filters and rate-limits traffic destined to the route processor (control plane/CPU).
 
 
</details>

### 26. Which two statements about MACsec are true?

- [ ] **A)** It provides Layer 2 encryption.
- [ ] **B)** It encrypts end-to-end across the network.
- [ ] **C)** It uses MKA (MACsec Key Agreement).
- [ ] **D)** It encrypts Ethernet headers.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> MACsec is a Layer 2 hop-by-hop encryption technology that uses MKA for key agreement.
 
 
</details>

### 27. Based on the output, which uRPF mode is enabled on the interface?

```cisco-ios
GigabitEthernet0/1 is up, line protocol is up
  Internet address is 192.168.1.1/24
  IP verify source reachability via rx
```

- [ ] **A)** Strict mode
- [ ] **B)** Loose mode
- [ ] **C)** Invalid mode
- [ ] **D)** Not configured

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The output shows 'IP verify source reachability via rx', indicating strict uRPF mode.
 
 
</details>


---

### **Virtualization**

### 28. Which device virtualization technology creates multiple independent virtual switches with separate control, data, and management planes on a single physical chassis?

- [ ] **A)** VDC
- [ ] **B)** VRF
- [ ] **C)** VXLAN
- [ ] **D)** EVPN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> VDC (Virtual Device Context) virtualizes the entire switch including control, data, and management planes. VRFs only virtualize the routing table.
 
 
</details>

### 29. Which two of the following statements about VXLAN are true?

- [ ] **A)** VXLAN uses a 24-bit segment identifier called the VNI.
- [ ] **B)** VXLAN encapsulates Layer 2 frames inside UDP/IP packets.
- [ ] **C)** VXLAN requires a 12-bit VLAN tag for operation.
- [ ] **D)** VXLAN can support up to 4096 segments.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VXLAN uses a 24-bit VNI to support up to 16 million segments and encapsulates Ethernet frames in UDP. It does not use 12-bit VLAN IDs nor is it limited to 4096 segments.
 
 
</details>

### 30. Refer to the configuration snippet. What does it represent?

```cisco-ios
interface nve1
 source-interface loopback0
 member vni 10010 mcast-group 239.1.1.1
```

- [ ] **A)** VXLAN
- [ ] **B)** VDC
- [ ] **C)** VRF
- [ ] **D)** OTV

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The configuration creates an NVE interface with a source IP and a member VNI with multicast group, which is used for VXLAN overlay.
 
 
</details>

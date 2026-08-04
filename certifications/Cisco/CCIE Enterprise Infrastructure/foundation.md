<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cisco/CCIE%20Enterprise%20Infrastructure.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>CCIE Enterprise Infrastructure</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Automation and Programmability](#automation-and-programmability) (4 questions)
- [Network Assurance and Optimization](#network-assurance-and-optimization) (4 questions)
- [Network Infrastructure](#network-infrastructure) (6 questions)
- [Security Services](#security-services) (5 questions)
- [Software-Defined Infrastructure](#software-defined-infrastructure) (5 questions)
- [Transport Technologies and Solutions](#transport-technologies-and-solutions) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:50.586Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Automation and Programmability | 4 |
| Network Assurance and Optimization | 4 |
| Network Infrastructure | 6 |
| Security Services | 5 |
| Software-Defined Infrastructure | 5 |
| Transport Technologies and Solutions | 6 |

---

### **Automation and Programmability**

### 1. What is Paramiko in the context of network automation?

- [ ] **A)** A high-level multi-vendor SSH library
- [ ] **B)** A low-level SSH protocol implementation for Python
- [ ] **C)** A configuration management tool that supports idempotency
- [ ] **D)** A REST API client for Cisco devices

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Paramiko is a low-level implementation of SSHv2 in Python, providing raw SSH connectivity without vendor abstraction.
 
 
</details>

### 2. Which of the following are true about Netmiko? (Select two.)

- [ ] **A)** It is built on top of Paramiko
- [ ] **B)** It automatically provides structured data output
- [ ] **C)** It supports multiple device platforms
- [ ] **D)** It enforces idempotency by default

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Netmiko is built on Paramiko and provides a simplified interface for over 30 platforms, but does not return structured data or guarantee idempotency.
 
 
</details>

### 3. What is the return type of the `send_command()` method in Netmiko?

```python
from netmiko import ConnectHandler
device = {"device_type": "cisco_ios", "ip": "192.168.1.1", "username": "admin", "password": "cisco"}
connection = ConnectHandler(**device)
output = connection.send_command("show ip int brief")
print(type(output))
```

- [ ] **A)** A string containing the device output
- [ ] **B)** A list of lines parsed from the output
- [ ] **C)** A dictionary with structured data
- [ ] **D)** A JSON object

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> `send_command()` returns a single string containing the raw CLI output from the device.
 
 
</details>

### 4. Which Git command fetches changes from a remote repository but does NOT merge them?

- [ ] **A)** git pull
- [ ] **B)** git fetch
- [ ] **C)** git clone
- [ ] **D)** git merge

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> `git fetch` downloads objects and refs from a remote repository, leaving the local branch unchanged.
 
 
</details>


---

### **Network Assurance and Optimization**

### 5. Which version of NetFlow introduced template-based flexible export format?

- [ ] **A)** Version 5
- [ ] **B)** Version 7
- [ ] **C)** Version 9
- [ ] **D)** Version 10 (IPFIX)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> NetFlow version 9 introduced a flexible template-based export format, which was later standardized as IPFIX (version 10).
 
 
</details>

### 6. Which of the following are features of SNMPv3 compared to SNMPv2c? (Choose two.)

- [ ] **A)** Authentication using MD5/SHA
- [ ] **B)** Community strings in plaintext
- [ ] **C)** Encryption with DES/AES
- [ ] **D)** Uses UDP port 162 for traps

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> SNMPv3 adds authentication (MD5, SHA) and encryption (DES, AES), while SNMPv2c uses plaintext community strings and has no encryption.
 
 
</details>

### 7. Examine the IP SLA configuration snippet. What is the missing command to enable the UDP jitter probe on the destination router?

```cisco-ios
ip sla 10
 udp-jitter 10.1.1.2 16384 codec g711alaw
 threshold 100
 timeout 500
 frequency 30
ip sla schedule 10 life forever start-time now
```

- [ ] **A)** ip sla responder
- [ ] **B)** ip sla responder udp-echo
- [ ] **C)** no ip sla responder
- [ ] **D)** ip sla schedule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> For UDP jitter IP SLA probes, the destination router must have the 'ip sla responder' command configured to listen and respond to the probe.
 
 
</details>

### 8. Which syslog severity level indicates an emergency condition?

- [ ] **A)** 0
- [ ] **B)** 1
- [ ] **C)** 3
- [ ] **D)** 7

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Syslog severity level 0 is Emergency, the highest severity. Level 1 is Alert, level 3 is Error, level 7 is Debug.
 
 
</details>


---

### **Network Infrastructure**

### 9. Which Spanning Tree Protocol variant significantly reduces convergence time by introducing edge ports and point-to-point link types?

- [ ] **A)** STP (802.1D)
- [ ] **B)** RSTP (802.1w)
- [ ] **C)** MST (802.1s)
- [ ] **D)** PVST+

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> RSTP (802.1w) reduces convergence time from up to 50 seconds to sub-second by introducing edge ports and using proposal/agreement handshakes on point-to-point links.
 
 
</details>

### 10. Select two characteristics of Multiple Spanning Tree Protocol (MST).

- [ ] **A)** Maps multiple VLANs to a single spanning tree instance
- [ ] **B)** Requires separate BPDUs for each VLAN
- [ ] **C)** Defines MST regions with matching name and revision number
- [ ] **D)** Runs one spanning tree per VLAN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> MST maps multiple VLANs to a single instance, reducing BPDU overhead. Regions must have identical name and revision number to be part of the same region.
 
 
</details>

### 11. Refer to the OSPF configuration snippet. What is the OSPF network type configured on the interface?

```cisco-ios
interface GigabitEthernet0/1
 ip ospf network point-to-point
```

- [ ] **A)** Broadcast
- [ ] **B)** Point-to-point
- [ ] **C)** Non-broadcast
- [ ] **D)** Point-to-multipoint

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 'ip ospf network point-to-point' command sets the interface to point-to-point network type, which avoids DR/BDR election and uses only one neighbor.
 
 
</details>

### 12. What is the default administrative distance of eBGP routes in Cisco IOS?

- [ ] **A)** 20
- [ ] **B)** 110
- [ ] **C)** 120
- [ ] **D)** 170

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> eBGP routes have a default administrative distance of 20, while iBGP routes have AD 200.
 
 
</details>

### 13. Select two features that are exclusive to IGMPv3 compared to IGMPv2.

- [ ] **A)** Membership Report messages
- [ ] **B)** Source-specific join requests (INCLUDE mode)
- [ ] **C)** Leave Group messages
- [ ] **D)** Exclude mode for source filtering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> IGMPv3 introduces INCLUDE and EXCLUDE modes for source-specific filtering, enabling SSM. Both are absent in IGMPv2.
 
 
</details>

### 14. Examine the PIM configuration output. What is the role of this router in the PIM-SM domain?

```cisco-ios
ip pim rp-address 192.168.1.1
ip pim sparse-mode
```

- [ ] **A)** Rendezvous Point (RP)
- [ ] **B)** First-hop router
- [ ] **C)** Last-hop router
- [ ] **D)** Bootstrap Router

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command 'ip pim rp-address 192.168.1.1' statically defines the RP address, so this router is configured as the RP for the domain.
 
 
</details>


---

### **Security Services**

### 15. What does Control Plane Policing (CoPP) primarily protect?

- [ ] **A)** Data plane
- [ ] **B)** Control plane
- [ ] **C)** Management plane
- [ ] **D)** Forwarding plane

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> CoPP protects the control plane by rate-limiting traffic destined to it, preventing CPU overload.
 
 
</details>

### 16. Which two technologies are used in Cisco TrustSec for authentication?

- [ ] **A)** 802.1X
- [ ] **B)** MAB
- [ ] **C)** CoPP
- [ ] **D)** MACsec

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> TrustSec uses 802.1X for user/device authentication and MAB as a fallback for devices without 802.1X supplicants.
 
 
</details>

### 17. Based on the configuration snippet, what is the purpose of the zone-pair command?

```cisco-ios
zone-pair security ZP source INSIDE destination OUTSIDE
 service-policy type inspect POLICY
```

- [ ] **A)** It defines a security zone for interfaces.
- [ ] **B)** It creates a unidirectional policy link between two zones.
- [ ] **C)** It assigns an interface to a zone.
- [ ] **D)** It enables stateful inspection for all traffic.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A zone-pair connects a source zone to a destination zone and allows application of a policy map for traffic flowing in that direction.
 
 
</details>

### 18. What is the primary difference between IPS and IDS on a Cisco router?

- [ ] **A)** IPS can drop packets; IDS can only alert.
- [ ] **B)** IDS can drop packets; IPS can only alert.
- [ ] **C)** Both can drop packets.
- [ ] **D)** Both can only alert.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IPS operates inline and can drop malicious packets, while IDS works in promiscuous mode and only generates alerts.
 
 
</details>

### 19. Which two protocols are commonly used for AAA in Cisco device administration?

- [ ] **A)** TACACS+
- [ ] **B)** RADIUS
- [ ] **C)** SNMP
- [ ] **D)** SSH

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> TACACS+ and RADIUS are the primary AAA protocols used for authentication, authorization, and accounting on Cisco devices.
 
 
</details>


---

### **Software-Defined Infrastructure**

### 20. What is the primary function of the Control Plane node in a Cisco SD-Access fabric?

- [ ] **A)** It forwards data traffic between endpoints.
- [ ] **B)** It maintains the LISP database mapping endpoints to their location.
- [ ] **C)** It provides external connectivity through Border Gateway Protocol.
- [ ] **D)** It manages device onboarding and template provisioning.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Control Plane node runs LISP and maintains the EID-to-RLOC mapping, enabling endpoint location discovery without data forwarding.
 
 
</details>

### 21. Which of the following are components of a Cisco SD-WAN architecture? (Choose all that apply.)

- [ ] **A)** vManage
- [ ] **B)** vSmart
- [ ] **C)** DNA Center
- [ ] **D)** vEdge

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Cisco SD-WAN includes vManage (management), vSmart (control), and vEdge (data). DNA Center is part of SD-Access, not SD-WAN.
 
 
</details>

### 22. Examine the YANG snippet. What is the data type of the leaf 'mtu'?

```yang
leaf mtu {
  type uint16;
  default 1500;
}
```

- [ ] **A)** string
- [ ] **B)** uint16
- [ ] **C)** boolean
- [ ] **D)** enumeration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The leaf 'mtu' is typed as uint16 in the YANG module, representing a 16-bit unsigned integer.
 
 
</details>

### 23. What is the primary role of Cisco DNA Center in an SD-Access fabric?

- [ ] **A)** It acts as the AAA server assigning SGTs to endpoints.
- [ ] **B)** It provides centralized management for fabric provisioning and policy.
- [ ] **C)** It forwards data packets between fabric edges and borders.
- [ ] **D)** It maintains the LISP mapping database for endpoint mobility.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> DNA Center orchestrates the fabric lifecycle including design, provisioning, policy creation, and assurance; it does not forward data or authenticate users.
 
 
</details>

### 24. Which security features are available on a cEdge router in Cisco SD-WAN? (Choose all that apply.)

- [ ] **A)** Zone-based firewall
- [ ] **B)** Intrusion Prevention System (IPS)
- [ ] **C)** TLS/SSL decryption
- [ ] **D)** Scalable Group Tag (SGT) classification

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> cEdge routers support advanced security like ZBF, IPS, and TLS decryption. SGT classification is an SD-Access feature, not native to cEdge.
 
 
</details>


---

### **Transport Technologies and Solutions**

### 25. Which protocol is used to distribute outer transport labels in an MPLS core?

- [ ] **A)** LDP
- [ ] **B)** BGP
- [ ] **C)** OSPF
- [ ] **D)** IS-IS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> LDP is used to distribute labels for FECs, typically for transport labels in MPLS core.
 
 
</details>

### 26. Which of the following are true about VPWS? (Select two)

- [ ] **A)** It requires MAC learning
- [ ] **B)** It is a point-to-point L2VPN
- [ ] **C)** It uses FEC 129 typically
- [ ] **D)** It uses FEC 128 typically

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> VPWS is point-to-point and typically uses FEC 128 for label signaling.
 
 
</details>

### 27. Examine the following configuration snippet. What is the purpose of the 'segment-routing mpls' command under IS-IS?

```text
router isis 1
 net 49.0001.1921.6800.1001.00
 segment-routing mpls
```

- [ ] **A)** Enables LDP
- [ ] **B)** Enables prefix-SID advertisements
- [ ] **C)** Enables SRGB
- [ ] **D)** Enables TI-LFA

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> It enables IS-IS to advertise prefix-SIDs for segment routing.
 
 
</details>

### 28. What is the purpose of a Route Target (RT) in MPLS L3VPN?

- [ ] **A)** Make VPNv4 prefixes unique
- [ ] **B)** Control import/export of routes into VRF
- [ ] **C)** Label distribution
- [ ] **D)** Establish MP-BGP session

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> RTs control which routes are imported/exported between VRFs.
 
 
</details>

### 29. Which of the following are characteristics of VPLS? (Select two)

- [ ] **A)** Point-to-point connectivity
- [ ] **B)** MAC learning is data-plane driven
- [ ] **C)** Uses split horizon to prevent loops
- [ ] **D)** Requires FEC 128 for auto-discovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> VPLS is multipoint, uses data-plane MAC learning and split horizon.
 
 
</details>

### 30. Examine the following SRv6 configuration. What does the locator represent?

```text
segment-routing srv6
 locator LOC1
 prefix FC00:1::/48
```

- [ ] **A)** The function
- [ ] **B)** The routable prefix
- [ ] **C)** The SRH
- [ ] **D)** The Next Header

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The locator is the routable IPv6 prefix that identifies a node.
 
 
</details>

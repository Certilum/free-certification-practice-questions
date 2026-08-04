<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Arista/ACE:%20L3%20(Arista%20Cloud%20Engineer:%20Level%203)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>ACE: L3 (Cloud Engineer: Level 3)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Advanced Troubleshooting and Operations](#advanced-troubleshooting-and-operations) (2 questions)
- [Automation and Orchestration](#automation-and-orchestration) (6 questions)
- [Cloud Data Center Architecture](#cloud-data-center-architecture) (7 questions)
- [Cloud Network Services and Security](#cloud-network-services-and-security) (5 questions)
- [Overlay Networking with EVPN/VXLAN](#overlay-networking-with-evpn-vxlan) (10 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:50.391Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Advanced Troubleshooting and Operations | 2 |
| Automation and Orchestration | 6 |
| Cloud Data Center Architecture | 7 |
| Cloud Network Services and Security | 5 |
| Overlay Networking with EVPN/VXLAN | 10 |

---

### **Advanced Troubleshooting and Operations**

### 1. Which transport protocol is utilized by CloudVision for streaming telemetry?

- [ ] **A)** gRPC
- [ ] **B)** SNMP
- [ ] **C)** NETCONF
- [ ] **D)** HTTP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CloudVision Telemetry uses gRPC over TCP for streaming data from devices to the TWS.
 
 
</details>

### 2. Identify two stages that are part of a packet walk in an Arista EOS device.

- [ ] **A)** Ingress parser
- [ ] **B)** CPU processing
- [ ] **C)** ACL lookup
- [ ] **D)** tcpdump capture

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> A packet walk examines ingress, forwarding, ACL, and egress stages in the ASIC pipeline, not CPU-bound activities.
 
 
</details>


---

### **Automation and Orchestration**

### 3. What is the primary protocol used by Arista eAPI for communication?

- [ ] **A)** JSON-RPC
- [ ] **B)** SOAP
- [ ] **C)** REST
- [ ] **D)** gRPC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Arista eAPI uses JSON-RPC over HTTP/HTTPS for programmatic access to CLI commands.
 
 
</details>

### 4. Which two data formats does Arista eAPI support for command output?

- [ ] **A)** JSON
- [ ] **B)** XML
- [ ] **C)** Text
- [ ] **D)** YAML

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> eAPI supports 'json' and 'text' formats; JSON returns structured data, text returns raw CLI output.
 
 
</details>

### 5. In the following eAPI request snippet, what does the 'format' parameter specify?

```json
{
  "jsonrpc": "2.0",
  "method": "runCmds",
  "params": {
    "version": 1,
    "cmds": ["show version"],
    "format": "json"
  },
  "id": 1
}
```

- [ ] **A)** The output format of the command results
- [ ] **B)** The encoding of the request body
- [ ] **C)** The version of the API
- [ ] **D)** The authentication method

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In eAPI, the 'format' parameter defines whether command output is returned as JSON or text.
 
 
</details>

### 6. Which HTTP methods does RESTCONF use for configuration operations?

- [ ] **A)** GET, POST, PUT, PATCH, DELETE
- [ ] **B)** GET, POST, UPDATE
- [ ] **C)** GET, PUT, DELETE only
- [ ] **D)** POST, PATCH, DELETE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RESTCONF uses GET, POST, PUT, PATCH, and DELETE to manipulate YANG-modeled data.
 
 
</details>

### 7. Which two YANG model families are supported by Arista RESTCONF?

- [ ] **A)** OpenConfig
- [ ] **B)** IETF
- [ ] **C)** Native EOS YANG
- [ ] **D)** Cisco YANG

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> RESTCONF on Arista supports both OpenConfig and native EOS YANG models.
 
 
</details>

### 8. Based on the following RESTCONF URI, what resource is being accessed?

```http
GET /restconf/data/openconfig-interfaces:interfaces/interface=Loopback0/config/description
```

- [ ] **A)** The description of Loopback0 interface
- [ ] **B)** The IPv4 address of Loopback0
- [ ] **C)** All interfaces on the device
- [ ] **D)** The operational status of Loopback0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The path /restconf/data/openconfig-interfaces:interfaces/interface=Loopback0/config/description retrieves the description of Loopback0.
 
 
</details>


---

### **Cloud Data Center Architecture**

### 9. What is the primary function of the CloudVision Portal (CVP) in Arista's architecture?

- [ ] **A)** Centralized orchestration and lifecycle management
- [ ] **B)** Data plane forwarding
- [ ] **C)** State replication for overlay services
- [ ] **D)** Telemetry agent on switches

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CVP is the centralized management plane responsible for orchestration, change control, and intent reconciliation.
 
 
</details>

### 10. Which of the following are valid layers of the Arista CloudVision platform architecture? (Select two.)

- [ ] **A)** CloudVision Portal (CVP)
- [ ] **B)** CloudVision eXchange (CVX)
- [ ] **C)** CloudVision Firewall (CVF)
- [ ] **D)** CloudVision Load Balancer (CVL)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The three layers are CVP, CVX, and CVA. CVF and CVL are not part of CloudVision.
 
 
</details>

### 11. Refer to the following configuration snippet. What protocol does TerminAttr use to stream state data to CloudVision?

```bash
daemon TerminAttr
exec /usr/bin/TerminAttr -ingestgrp=cloud-vision -grpc-server=10.0.0.1:9910 -vrf=MGMT -smashexcludes=...
no sh

```

- [ ] **A)** gRPC over TLS
- [ ] **B)** SNMP
- [ ] **C)** HTTP
- [ ] **D)** FTP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TerminAttr uses gRPC (port 9910) over TLS to stream state changes in near-real-time.
 
 
</details>

### 12. In a Spine-Leaf architecture, how are loops prevented?

- [ ] **A)** Layer 3 ECMP
- [ ] **B)** Spanning Tree Protocol
- [ ] **C)** TRILL
- [ ] **D)** STP with RSTP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Spine-Leaf uses Layer 3 ECMP to distribute traffic across multiple paths, eliminating the need for STP.
 
 
</details>

### 13. Which of the following are characteristics of a Spine-Leaf topology? (Select two.)

- [ ] **A)** Every leaf connects to every spine
- [ ] **B)** Spines can interconnect with each other
- [ ] **C)** Leaves never connect directly to other leaves
- [ ] **D)** Leaf switches are always L2 only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Spine-Leaf is a full-mesh between leaf and spine; spines do not interconnect, and leaves do not connect to other leaves.
 
 
</details>

### 14. Analyze the following underlay configuration. Which routing protocol is being used for the underlay?

```eos
interface Ethernet1
 description To Spine-1
 no switchport
 ipv6 enable
! router bgp 65000
 router-id 10.0.0.1
 neighbor 2001::1 remote-as 65001
 address-family ipv4
  neighbor 2001::1 activate

```

- [ ] **A)** EBGP unnumbered
- [ ] **B)** OSPF
- [ ] **C)** IS-IS
- [ ] **D)** RIP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet shows BGP with IPv4 unnumbered configuration, which is EBGP unnumbered (RFC 5549).
 
 
</details>

### 15. What is the purpose of the CloudVision eXchange (CVX) component?

- [ ] **A)** State replication and advanced overlay service insertion
- [ ] **B)** Primary UI and API gateway
- [ ] **C)** Data plane packet forwarding
- [ ] **D)** Telemetry collection from switches

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CVX acts as a service insertion and state replication bus, enabling features like VXLAN routing and LB integration.
 
 
</details>


---

### **Cloud Network Services and Security**

### 16. What is the purpose of a VXLAN Network Identifier (VNI) in multi-tenancy?

- [ ] **A)** To encrypt traffic between VTEPs
- [ ] **B)** To provide a unique tenant identifier for logical isolation
- [ ] **C)** To route traffic between spine switches
- [ ] **D)** To identify the physical port of a server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The VNI (VXLAN Network Identifier) is a 24-bit segment ID that uniquely identifies a tenant overlay network, enabling isolation and overlapping addresses.
 
 
</details>

### 17. Which of the following are components of Arista's service chaining? (Select all that apply.)

- [ ] **A)** Service Function Forwarder (SFF)
- [ ] **B)** Service Node (SN)
- [ ] **C)** Policy Controller (CloudVision)
- [ ] **D)** Route Reflector (RR)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The SFF (leaf switch) forwards traffic between service nodes, SN is the actual service appliance, and CloudVision orchestrates the policies. A route reflector is not a direct component.
 
 
</details>

### 18. What is the result of the following command on an Arista switch?

```eos
ip access-list standard TEST permit 10.0.0.0/8
interface Ethernet1
ip access-group TEST in
```

- [ ] **A)** All traffic is blocked on interface Ethernet1
- [ ] **B)** Traffic from 10.0.0.0/8 is permitted, all other traffic is denied
- [ ] **C)** Only TCP traffic on port 80 is permitted
- [ ] **D)** The interface is shut down

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The ACL permits traffic from source 10.0.0.0/8 and implicitly denies all other traffic due to the implicit deny all at the end of every ACL.
 
 
</details>

### 19. What is the primary function of Control Plane Policing (CoPP) on an Arista switch?

- [ ] **A)** It filters all data plane traffic
- [ ] **B)** It rate-limits traffic destined to the CPU
- [ ] **C)** It encrypts management traffic
- [ ] **D)** It blocks BGP updates

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> CoPP applies QoS policers to control-plane traffic, limiting the rate of packets like BGP, OSPF, SSH, and thus protecting the CPU from overload.
 
 
</details>

### 20. Which of the following are tag-based attributes in Arista MSS-G micro-segmentation? (Select all that apply.)

- [ ] **A)** Environment (e.g., Prod, Dev)
- [ ] **B)** Tier (e.g., Web, App, DB)
- [ ] **C)** MAC address
- [ ] **D)** Application name

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> MSS-G uses tags like Environment, Tier, and Application to group workloads. MAC address is a low-level identifier, not a high-level tag.
 
 
</details>


---

### **Overlay Networking with EVPN/VXLAN**

### 21. Which EVPN route type is used to advertise MAC and IP host information?

- [ ] **A)** Type-1 (Ethernet Auto-Discovery)
- [ ] **B)** Type-2 (MAC/IP Advertisement)
- [ ] **C)** Type-3 (Inclusive Multicast Ethernet Tag)
- [ ] **D)** Type-4 (Ethernet Segment)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Type-2 MAC/IP Advertisement Route is designed for host MAC and IP reachability, allowing optimized forwarding and ARP suppression.
 
 
</details>

### 22. Which two components are essential for symmetric Integrated Routing and Bridging (IRB) in EVPN/VXLAN?

- [ ] **A)** L3 VNI
- [ ] **B)** Type-5 (IP Prefix) routes
- [ ] **C)** Type-2 (MAC/IP) routes only
- [ ] **D)** Ingress replication underlay

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Symmetric IRB uses a dedicated L3 VNI and Type-5 routes to perform routing on both ingress and egress VTEPs, enabling optimal east-west traffic.
 
 
</details>

### 23. Based on the configuration, what is the purpose of the 'rd auto' command?

```arista_eos
router bgp 65001
 address-family l2vpn evpn
 vlan-aware-bundle TENANT-A
  rd auto
  route-target both auto
 exit-address-family
```

- [ ] **A)** Automatically generates a unique Route Distinguisher using switch IP and VNI
- [ ] **B)** Sets the RD to the BGP AS number
- [ ] **C)** Disables the RD and uses MAC address instead
- [ ] **D)** Assigns a random RD per VLAN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'rd auto' command in Arista EOS automatically derives the Route Distinguisher from the switch's router-id and the VNI, ensuring uniqueness per EVPN instance.
 
 
</details>

### 24. Which EVPN route type is responsible for Designated Forwarder (DF) election in active-active multihoming?

- [ ] **A)** Type-1 (Ethernet Auto-Discovery)
- [ ] **B)** Type-2 (MAC/IP Advertisement)
- [ ] **C)** Type-4 (Ethernet Segment)
- [ ] **D)** Type-5 (IP Prefix Advertisement)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Type-4 Ethernet Segment Route is exchanged between leaf nodes attached to the same ES and used for Designated Forwarder election per VLAN.
 
 
</details>

### 25. Which two statements about VXLAN bridging are true?

- [ ] **A)** It extends VLANs across multiple leaf switches by encapsulating Ethernet frames in UDP
- [ ] **B)** It requires spanning-tree protocol (STP) to prevent loops
- [ ] **C)** It uses EVPN Type-2 routes to learn remote MAC addresses
- [ ] **D)** It replaces the underlay routing for all traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> VXLAN bridging encapsulates Ethernet frames in UDP to extend VLANs, and uses EVPN control plane (Type-2 routes) for MAC learning. STP is not required; the control plane prevents loops.
 
 
</details>

### 26. In this configuration, what is the purpose of the 'vxlan vlan 100 vni 10100' command?

```arista_eos
interface Vxlan1
 vxlan vlan 100 vni 10100
 vxlan vlan 200 vni 10200
 source-interface Loopback0

```

- [ ] **A)** It maps VLAN 100 to VNI 10100 for VXLAN encapsulation
- [ ] **B)** It creates a Layer 3 routing interface for VLAN 100
- [ ] **C)** It enables multicast replication for VLAN 100
- [ ] **D)** It assigns an IP gateway to VLAN 100

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'vxlan vlan <vlan> vni <vni>' command under the VXLAN interface maps a local VLAN to a specific VXLAN Network Identifier (VNI) for overlay encapsulation.
 
 
</details>

### 27. What is the role of a VTEP in VXLAN?

- [ ] **A)** It encapsulates and decapsulates VXLAN frames
- [ ] **B)** It performs routing between VRFs
- [ ] **C)** It acts as a BGP route reflector
- [ ] **D)** It provides DHCP services

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A VTEP is responsible for VXLAN encapsulation and decapsulation, enabling overlay communication over the underlay network.
 
 
</details>

### 28. Which two EVPN route types are used for L2 extension across multi-pod deployments?

- [ ] **A)** Type-2 (MAC/IP Advertisement)
- [ ] **B)** Type-3 (Inclusive Multicast Ethernet Tag)
- [ ] **C)** Type-5 (IP Prefix Advertisement)
- [ ] **D)** Type-1 (Ethernet Auto-Discovery) only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Type-2 routes advertise MAC/IP for host reachability, and Type-3 routes build the BUM forwarding domain. Both are required for L2 extension across pods.
 
 
</details>

### 29. What does 'ip virtual-router mac-address 00:1c:73:00:00:01' accomplish in this configuration?

```arista_eos
interface Vlan100
 ip address virtual 192.168.1.1/24
 ip virtual-router address 192.168.1.254
 ip virtual-router mac-address 00:1c:73:00:00:01

```

- [ ] **A)** It assigns a common MAC to all leaf gateways for anycast behavior
- [ ] **B)** It sets the physical MAC of the SVI
- [ ] **C)** It enables VRRP for gateway redundancy
- [ ] **D)** It defines the VTEP source MAC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'ip virtual-router mac-address' sets a shared virtual MAC for the anycast gateway, ensuring seamless host mobility across leaf switches.
 
 
</details>

### 30. What is the main benefit of ARP suppression on a VTEP?

- [ ] **A)** It reduces broadcast flooding by allowing the VTEP to proxy-reply
- [ ] **B)** It eliminates the need for BGP EVPN
- [ ] **C)** It increases ARP request retransmission rate
- [ ] **D)** It enables VLAN pruning on trunk ports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ARP suppression uses EVPN-learned mappings to respond to ARP requests locally, significantly reducing broadcast traffic over the VXLAN fabric.
 
 
</details>

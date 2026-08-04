<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cisco/CCNP%20Enterprise.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>CCNP Enterprise</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Architecture](#architecture) (5 questions)
- [Automation](#automation) (5 questions)
- [Infrastructure](#infrastructure) (9 questions)
- [Network Assurance](#network-assurance) (4 questions)
- [Security](#security) (4 questions)
- [Virtualization](#virtualization) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:00.988Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Architecture | 5 |
| Automation | 5 |
| Infrastructure | 9 |
| Network Assurance | 4 |
| Security | 4 |
| Virtualization | 3 |

---

### **Architecture**

### 1. In the Cisco hierarchical network design model, which layer is responsible for high-speed switching and should not enforce policies?

- [ ] **A)** Access layer
- [ ] **B)** Distribution layer
- [ ] **C)** Core layer
- [ ] **D)** Collapsed core

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Core layer provides high-speed, non-blocking switching and should not be burdened with policy enforcement such as ACLs or QoS re-marking. Policy is applied at the Distribution layer.
 
 
</details>

### 2. Which of the following are characteristics of HSRP? (Choose two)

- [ ] **A)** It uses a virtual IP and virtual MAC address
- [ ] **B)** It supports active/active load balancing across multiple gateways
- [ ] **C)** It is a Cisco proprietary protocol
- [ ] **D)** It uses multicast address 224.0.0.18 for hello messages

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> HSRP is Cisco proprietary and uses a virtual IP/MAC. It is active/standby, not active/active. GLBP provides load balancing. HSRP uses 224.0.0.2 (v1) or 224.0.0.102 (v2); 224.0.0.18 is VRRP.
 
 
</details>

### 3. Examine the configuration snippet. Which protocol is being configured?

```cisco-ios
crypto isakmp policy 10
authentication pre-share
crypto isakmp key cisco address 192.168.1.1
crypto ipsec transform-set TSET esp-aes esp-sha-hmac
crypto map CMAP 10 ipsec-isakmp
 set peer 192.168.1.1
 set transform-set TSET
 match address 100
```

- [ ] **A)** IPsec
- [ ] **B)** SSL
- [ ] **C)** DTLS
- [ ] **D)** GRE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet shows a crypto ISAKMP policy and IPsec transform set, which are components of an IPsec VPN configuration. DTLS is used with Cisco SD-WAN control plane, not shown here.
 
 
</details>

### 4. Which SD-Access component maintains the EID-to-RLOC mapping database?

- [ ] **A)** Fabric Edge Node
- [ ] **B)** Fabric Border Node
- [ ] **C)** Control Plane Node
- [ ] **D)** DNA Center

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Control Plane Node runs the LISP map-server/map-resolver function and keeps the EID-to-RLOC database. Fabric Edge nodes register mappings, and Border nodes connect to external networks. DNA Center is the management controller.
 
 
</details>

### 5. Which two wireless architectures allow local data forwarding without tunneling client traffic to a controller? (Choose two)

- [ ] **A)** Autonomous AP
- [ ] **B)** Centralized WLC (CAPWAP central switching)
- [ ] **C)** FlexConnect with local switching
- [ ] **D)** Cloud-based (Meraki) with central switching

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Autonomous APs bridge traffic locally inherently. FlexConnect can be configured for local switching. Centralized WLC tunnels all data to the controller. Cloud-based central switching tunnels data to the cloud; local LAN mode would be local, but the option specifies 'central switching'.
 
 
</details>


---

### **Automation**

### 6. Which data modeling language defines the structure and constraints for network device configuration?

- [ ] **A)** XML
- [ ] **B)** JSON
- [ ] **C)** YAML
- [ ] **D)** YANG

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> YANG is a data modeling language that defines the structure, semantics, and constraints for network device configuration and state data.
 
 
</details>

### 7. Which two characteristics describe Ansible in the context of network automation? (Choose two.)

- [ ] **A)** Uses a declarative model and stores state in .tfstate
- [ ] **B)** Uses a push model where control nodes execute playbooks
- [ ] **C)** Checks the live device state each run for idempotency
- [ ] **D)** Requires agents installed on managed devices

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Ansible uses a push model and achieves idempotency by checking live device state each run. It is agentless.
 
 
</details>

### 8. In the provided JSON snippet, what makes it invalid according to JSON syntax rules?

```json
{interface: {name: "GigabitEthernet0/1", enabled: true}}
```

- [ ] **A)** Keys are not enclosed in double quotes
- [ ] **B)** Boolean value is not lowercase
- [ ] **C)** Trailing comma after the last property
- [ ] **D)** Missing colon between key and value

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> JSON requires keys to be strings enclosed in double quotes. The snippet uses unquoted keys.
 
 
</details>

### 9. Which HTTP header is used to pass the Meraki API key in REST API requests?

- [ ] **A)** X-Auth-Token
- [ ] **B)** Authorization
- [ ] **C)** X-Cisco-Meraki-API-Key
- [ ] **D)** API-Key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Meraki requires the API key in the X-Cisco-Meraki-API-Key header. DNA Center uses X-Auth-Token.
 
 
</details>

### 10. Which two components are essential in a CI/CD pipeline for network automation? (Choose two.)

- [ ] **A)** Git for version control
- [ ] **B)** Jenkins for pipeline orchestration
- [ ] **C)** RESTCONF for device communication
- [ ] **D)** CLI for direct configuration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A CI/CD pipeline relies on Git as a single source of truth and Jenkins to automate the build, test, and deploy stages.
 
 
</details>


---

### **Infrastructure**

### 11. In a network with switches having bridge priorities 4096, 8192, and 4096 but different MAC addresses, which switch becomes the root bridge?

- [ ] **A)** The switch with priority 4096 and lowest MAC
- [ ] **B)** The switch with priority 8192
- [ ] **C)** The switch with highest MAC among 4096
- [ ] **D)** All switches become root

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Root bridge election uses lowest priority; if tie, lowest MAC address wins.
 
 
</details>

### 12. Which EtherChannel negotiation modes allow LACP to form a bundle? (Choose two)

- [ ] **A)** active-active
- [ ] **B)** active-passive
- [ ] **C)** passive-passive
- [ ] **D)** on-on

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> LACP active initiates PDUs; passive listens. Active-active or active-passive work; passive-passive does not.
 
 
</details>

### 13. A third MAC address is detected on the port configured as shown. What is the immediate result?

```cisco-ios
interface GigabitEthernet1/0/1
 switchport port-security
 switchport port-security maximum 2
 switchport port-security violation shutdown
```

- [ ] **A)** Port remains up, packet dropped silently
- [ ] **B)** Port remains up, syslog generated
- [ ] **C)** Port is err-disabled
- [ ] **D)** Port shuts down and recovers after 300 seconds

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Violation mode shutdown places the port in err-disabled state immediately.
 
 
</details>

### 14. Which OSPF LSA type is used to advertise external routes in a regular area?

- [ ] **A)** Type 3
- [ ] **B)** Type 4
- [ ] **C)** Type 5
- [ ] **D)** Type 7

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Type 5 LSA is used for external routes. Type 7 is for NSSA areas.
 
 
</details>

### 15. Which BGP attributes are considered before AS_PATH length in the path selection algorithm? (Choose two)

- [ ] **A)** Weight
- [ ] **B)** Local Preference
- [ ] **C)** MED
- [ ] **D)** Origin

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Weight (highest) is first, then local preference, then locally originated.
 
 
</details>

### 16. What is the seed metric for OSPF routes redistributed into EIGRP using the configuration shown?

```cisco-ios
router eigrp 100
 redistribute ospf 1 metric 100000 10 255 1 1500
```

- [ ] **A)** Bandwidth 100000, delay 10, reliability 255, load 1, MTU 1500
- [ ] **B)** Default EIGRP metric
- [ ] **C)** Metric is infinite until set
- [ ] **D)** The metric is taken from OSPF cost

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The redistribute command explicitly sets the seed metric to the values provided.
 
 
</details>

### 17. Which PIM mode uses an explicit join model and requires a Rendezvous Point?

- [ ] **A)** PIM Dense Mode
- [ ] **B)** PIM Sparse Mode
- [ ] **C)** PIM Bidirectional
- [ ] **D)** PIM SSM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> PIM-SM uses explicit joins and an RP. PIM-DM floods initially.
 
 
</details>

### 18. Which of the following are features of IGMPv3 compared to IGMPv2? (Choose two)

- [ ] **A)** Support for Source-Specific Multicast
- [ ] **B)** Group-specific queries
- [ ] **C)** Fast leave
- [ ] **D)** Querier election based on priority

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> IGMPv3 supports SSM and group-specific queries. Fast leave is IGMPv2 feature.
 
 
</details>

### 19. What is the purpose of the 'connect-source' parameter in the MSDP configuration shown?

```cisco-ios
ip msdp peer 192.168.1.1 connect-source Loopback0
```

- [ ] **A)** Sets the source interface for TCP connection
- [ ] **B)** Defines the RP address
- [ ] **C)** Specifies the multicast group
- [ ] **D)** Enables authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> connect-source sets the local interface used as source for the MSDP TCP session.
 
 
</details>


---

### **Network Assurance**

### 20. Which SNMPv3 security level provides both authentication and encryption?

- [ ] **A)** noAuthNoPriv
- [ ] **B)** authNoPriv
- [ ] **C)** authPriv
- [ ] **D)** authPriv with AES

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> authPriv provides authentication (MD5/SHA) and encryption (DES/3DES/AES).
 
 
</details>

### 21. Which two syslog severity levels indicate the most critical conditions?

- [ ] **A)** Emergency (0)
- [ ] **B)** Alert (1)
- [ ] **C)** Critical (2)
- [ ] **D)** Error (3)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Emergencies (0) and Alerts (1) are the highest severity; Critical is level 2.
 
 
</details>

### 22. Based on the configuration line, what security level is being configured?

```cisco-ios
snmp-server group ADMIN v3 priv
```

- [ ] **A)** noAuthNoPriv
- [ ] **B)** authNoPriv
- [ ] **C)** authPriv
- [ ] **D)** authPriv with AES-256

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The command 'snmp-server group ADMIN v3 priv' specifies the priv security level, meaning authentication and encryption.
 
 
</details>

### 23. Which protocol is used to collect flow-level traffic analytics on a network?

- [ ] **A)** SNMP
- [ ] **B)** Syslog
- [ ] **C)** NetFlow
- [ ] **D)** IP SLA

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> NetFlow exports flow data (packet/byte counts, etc.) to collectors for traffic analysis.
 
 
</details>


---

### **Security**

### 24. Which protocol is preferred for device administration with per-command authorization?

- [ ] **A)** RADIUS
- [ ] **B)** TACACS+
- [ ] **C)** LDAP
- [ ] **D)** Kerberos

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> TACACS+ encrypts the entire packet and supports per-command authorization, unlike RADIUS.
 
 
</details>

### 25. Which two mechanisms restrict management access to a router?

- [ ] **A)** VTY ACLs
- [ ] **B)** Port Security
- [ ] **C)** CoPP
- [ ] **D)** SPAN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> VTY ACLs filter SSH/Telnet sources; CoPP can police management traffic destined to CPU.
 
 
</details>

### 26. What is the effect of the given CoPP configuration?

```cisco-ios
class-map match-all CM-BGP
 match protocol bgp
policy-map COPP
 class CM-BGP
  police 8000 conform transmit exceed drop
 class class-default
  police 1000000 conform transmit exceed drop
```

- [ ] **A)** Drops all ICMP traffic to the router
- [ ] **B)** Rate-limits BGP, drops BGP exceeding 8000 bps
- [ ] **C)** Allows all BGP traffic without limit
- [ ] **D)** Applies policy to transit traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The policy police BGP at 8000 bps; conforming traffic is transmitted, exceeding is dropped.
 
 
</details>

### 27. What is the default violation mode for Cisco port security?

- [ ] **A)** Protect
- [ ] **B)** Restrict
- [ ] **C)** Shutdown
- [ ] **D)** Err-disable

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The default is 'shutdown', which places the port in err-disabled state.
 
 
</details>


---

### **Virtualization**

### 28. Which technology enables a single router to maintain multiple isolated routing tables?

- [ ] **A)** VRF
- [ ] **B)** VSS
- [ ] **C)** VXLAN
- [ ] **D)** GRE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> VRF (Virtual Routing and Forwarding) creates separate routing tables per instance, isolating traffic at Layer 3.
 
 
</details>

### 29. Which two characteristics are true about Cisco VSS? (Choose two)

- [ ] **A)** Uses a Virtual Switch Link (VSL)
- [ ] **B)** Provides active/active data plane forwarding
- [ ] **C)** Requires independent control planes per chassis
- [ ] **D)** Uses StackWise cabling for inter-chassis connection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VSS uses VSL to interconnect chassis and allows both switches to forward data while sharing a single control plane.
 
 
</details>

### 30. After applying 'ip vrf forwarding TENANT-A' on an interface, what is the immediate next required step?

```cisco-ios
ip vrf TENANT-A
!
interface GigabitEthernet1/0/1
 ip vrf forwarding TENANT-A
```

- [ ] **A)** Reapply the IP address on the interface
- [ ] **B)** Enable OSPF under the VRF
- [ ] **C)** Configure a route distinguisher
- [ ] **D)** Create a VXLAN tunnel endpoint

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'ip vrf forwarding' command clears any existing IP address, so it must be reconfigured immediately.
 
 
</details>

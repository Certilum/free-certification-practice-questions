<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cisco/Cisco%20Enterprise%20Advanced%20Routing%20and%20Services%20(ENARSI).png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Cisco Enterprise Advanced Routing and Services (ENARSI)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Infrastructure Security](#infrastructure-security) (6 questions)
- [Infrastructure Services](#infrastructure-services) (8 questions)
- [Layer 3 Technologies](#layer-3-technologies) (10 questions)
- [VPN Technologies](#vpn-technologies) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:51:24.713Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Infrastructure Security | 6 |
| Infrastructure Services | 8 |
| Layer 3 Technologies | 10 |
| VPN Technologies | 6 |

---

### **Infrastructure Security**

### 1. In Cisco enterprise ACLs, what source information does an IPv4 standard access control list use to filter traffic?

- [ ] **A)** Source IP address
- [ ] **B)** Destination IP address
- [ ] **C)** Protocol and port number
- [ ] **D)** MAC address

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Standard IPv4 ACLs filter traffic based solely on source IP address and are best placed near the destination.
 
 
</details>

### 2. Which statements correctly describe the implicit default behavior in IPv4 and IPv6 access control lists?

- [ ] **A)** Both use an implicit deny any at the end
- [ ] **B)** IPv6 ACLs implicitly permit Neighbor Discovery traffic
- [ ] **C)** IPv4 ACLs implicitly permit all ICMP traffic
- [ ] **D)** IPv6 ACLs require explicit permits for Neighbor Discovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> IPv4 and IPv6 ACLs end with an implicit deny any; IPv6 ACLs also permit Neighbor Discovery traffic automatically for address resolution.
 
 
</details>

### 3. In the displayed IPv4 ACL, what happens to traffic that matches no explicit permit statement in the list?

```cisco
access-list 100 permit tcp any host 192.168.1.10 eq www
```

- [ ] **A)** It is silently denied
- [ ] **B)** It is permitted by default
- [ ] **C)** It is forwarded as established traffic
- [ ] **D)** It is logged and dropped

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IPv4 ACLs conclude with an implicit deny any, so packets that match no explicit permit statement are silently dropped.
 
 
</details>

### 4. Which condition must be true for strict mode Unicast Reverse Path Forwarding to forward a received packet?

- [ ] **A)** Source route points back to the ingress interface
- [ ] **B)** Source route exists anywhere in the FIB
- [ ] **C)** Destination route uses the default route
- [ ] **D)** Packet has an ACL permit entry

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Strict uRPF requires the source address to have a FIB route pointing back out the exact ingress interface where the packet arrived.
 
 
</details>

### 5. Which statements about Unicast Reverse Path Forwarding operation are correct in enterprise edge deployments?

- [ ] **A)** Strict mode can drop traffic during asymmetric routing
- [ ] **B)** Loose mode verifies only that a route to the source exists
- [ ] **C)** uRPF depends on Cisco Express Forwarding
- [ ] **D)** uRPF does not require a FIB lookup

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Strict uRPF drops packets in asymmetric routing scenarios, loose mode only checks source reachability, and uRPF requires CEF because it uses the FIB.
 
 
</details>

### 6. In the shown Modular QoS CLI configuration, what does the keyword control-plane identify for CoPP?

```cisco
policy-map COPP
 class CRITICAL
  police 8000 conform-action transmit exceed-action drop
control-plane
 service-policy input COPP
```

- [ ] **A)** Enters the control-plane configuration submode
- [ ] **B)** Enters interface configuration mode
- [ ] **C)** Creates a new policy-map
- [ ] **D)** Moves to global configuration mode

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The control-plane command enters the dedicated control-plane configuration submode, where a service policy is attached to protect the route processor.
 
 
</details>


---

### **Infrastructure Services**

### 7. Which command is used to create a DHCP address pool on a Cisco IOS router?

- [ ] **A)** ip dhcp pool LAN
- [ ] **B)** ip helper-address 10.10.10.5
- [ ] **C)** ip address dhcp
- [ ] **D)** ip dhcp excluded-address 10.10.10.1 10.10.10.10

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The ip dhcp pool command creates a DHCP pool and enters DHCP pool configuration mode. The other commands configure DHCP relay, DHCP client, and address exclusions.
 
 
</details>

### 8. Which two DHCP options are commonly used with Cisco lightweight access points and vendor-specific provisioning?

- [ ] **A)** Option 43
- [ ] **B)** Option 60
- [ ] **C)** Option 82
- [ ] **D)** Option 67

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Option 43 carries vendor-specific data such as WLC IP addresses, while Option 60 identifies the vendor class. Option 82 is relay agent information and Option 67 is a boot file option.
 
 
</details>

### 9. Refer to the configuration in the exhibit. What happens to DHCP client broadcasts arriving on this interface?

```cisco-ios
interface GigabitEthernet0/1
 ip address 192.168.10.1 255.255.255.0
 ip helper-address 10.10.10.5
```

- [ ] **A)** It unicasts the DHCP broadcast to 10.10.10.5.
- [ ] **B)** It drops the DHCP broadcast.
- [ ] **C)** It answers from the local DHCP pool.
- [ ] **D)** It floods the request on all interfaces.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The ip helper-address command on the inbound interface converts DHCP broadcast traffic into unicast and forwards it to the centralized server at 10.10.10.5.
 
 
</details>

### 10. How does traffic shaping treat packets that exceed the configured rate?

- [ ] **A)** Buffers them for later transmission
- [ ] **B)** Drops them immediately
- [ ] **C)** Re-marks them and sends them immediately
- [ ] **D)** Ignores them and allows the burst

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Traffic shaping buffers excess traffic in queues and paces transmission over time, smoothing bursts to meet WAN rate limits.
 
 
</details>

### 11. Which two features are provided by SNMPv3 security?

- [ ] **A)** Authentication using MD5 or SHA
- [ ] **B)** Encryption using DES, 3DES, or AES
- [ ] **C)** Community string validation
- [ ] **D)** NetFlow export support

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SNMPv3 provides message integrity through authentication and data confidentiality through encryption. Community strings are associated with SNMPv1 and SNMPv2c.
 
 
</details>

### 12. Refer to the exhibit. What is the purpose of the source command in this Flexible NetFlow exporter configuration?

```cisco-ios
flow exporter EXPORTER
 destination 192.168.100.50
 source Loopback0
 transport udp 9995
```

- [ ] **A)** It sets the source IP for exported flow records.
- [ ] **B)** It defines the collector destination IP.
- [ ] **C)** It enables NetFlow on Loopback0.
- [ ] **D)** It selects the UDP export port.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The source command defines the source interface for exported flow records, giving collectors and firewalls a consistent IP address to identify the exporter.
 
 
</details>

### 13. In Cisco IOS EEM, which component watches for triggers such as Syslog messages or interface events?

- [ ] **A)** Event detector
- [ ] **B)** Applet
- [ ] **C)** Action
- [ ] **D)** Environment variable

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> EEM event detectors continuously monitor for conditions such as Syslog messages, SNMP traps, timers, and interface state changes. Applets then run actions when those events occur.
 
 
</details>

### 14. Which two statements correctly describe IP SLA?

- [ ] **A)** It actively generates synthetic traffic.
- [ ] **B)** It can trigger routing failover via object tracking.
- [ ] **C)** It only reports physical interface state.
- [ ] **D)** It cannot measure latency or jitter.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> IP SLA actively generates synthetic traffic to measure network performance, and it can be linked to object tracking to influence routing decisions and failover behavior.
 
 
</details>


---

### **Layer 3 Technologies**

### 15. Which two parameters are used by EIGRP to calculate the default composite metric?

- [ ] **A)** Bandwidth and Delay
- [ ] **B)** Load and Reliability
- [ ] **C)** Delay and MTU
- [ ] **D)** Hop Count and Load

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> EIGRP defaults to K1 and K3, so bandwidth and delay are the only active metric components.
 
 
</details>

### 16. Which of the following are required for EIGRP routers to establish neighbor adjacency? (Select all that apply.)

- [ ] **A)** Autonomous System (AS) number matches
- [ ] **B)** K-values are identical
- [ ] **C)** Primary subnets match on the connecting interface
- [ ] **D)** OSPF process ID matches

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> EIGRP adjacency requires identical AS numbers, K-values, and primary subnet match; OSPF process ID is not relevant.
 
 
</details>

### 17. Refer to the exhibit. What is the effect of the EIGRP interface configuration shown?

```cisco-ios
interface GigabitEthernet0/1
 ip address 10.2.1.1 255.255.255.0
 ip summary-address eigrp 100 10.10.0.0 255.255.248.0
```

- [ ] **A)** It manually advertises a summarized route on the interface
- [ ] **B)** It enables automatic classful summarization
- [ ] **C)** It filters EIGRP updates from the interface
- [ ] **D)** It configures the seed metric for redistributed routes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The ip summary-address eigrp command manually creates an interface-level summary route for the specified prefix.
 
 
</details>

### 18. Which address type is used by OSPFv3 for neighbor discovery and next-hop routing?

- [ ] **A)** IPv6 link-local addresses
- [ ] **B)** IPv4 primary interface addresses
- [ ] **C)** IPv6 global unicast addresses
- [ ] **D)** IPv4 secondary interface addresses

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OSPFv3 uses IPv6 link-local addresses in the fe80::/10 range for neighbor discovery and next-hop routing.
 
 
</details>

### 19. Which mechanisms does OSPF use to prevent loops in a multi-area enterprise design? (Select all that apply.)

- [ ] **A)** All inter-area traffic must traverse Area 0
- [ ] **B)** Non-backbone areas can forward traffic directly between one another
- [ ] **C)** Rigorous LSA dissemination rules restrict route propagation
- [ ] **D)** DUAL computes loop-free feasible successors

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> OSPF prevents loops by forcing inter-area traffic through Area 0 and using strict LSA dissemination rules.
 
 
</details>

### 20. Refer to the exhibit. Which statement correctly describes how OSPFv3 is enabled on the interface?

```cisco-ios
interface GigabitEthernet0/0
 ipv6 address 2001:db8:1::1/64
 ipv6 ospf 100 area 0
```

- [ ] **A)** OSPFv3 is enabled per interface using a process ID and area
- [ ] **B)** OSPFv3 is enabled by entering a network statement in the global OSPF process
- [ ] **C)** OSPFv3 requires IPv4 primary addresses on the interface
- [ ] **D)** OSPFv3 is enabled globally and does not require an interface association

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OSPFv3 is enabled on the interface with a process ID and area; network statements are not used in OSPFv3.
 
 
</details>

### 21. Which statement correctly describes the BGP Weight attribute?

- [ ] **A)** It is Cisco-proprietary and locally significant
- [ ] **B)** It is advertised to external BGP peers
- [ ] **C)** It is identical to Local Preference
- [ ] **D)** It is a well-known transitive BGP attribute

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Weight is a Cisco-proprietary, locally significant BGP attribute that is never advertised to neighbors.
 
 
</details>

### 22. Which two BGP attributes are evaluated by Cisco routers during the path selection process? (Choose two.)

- [ ] **A)** Weight
- [ ] **B)** Local Preference
- [ ] **C)** MAC address
- [ ] **D)** LDP label

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Weight and Local Preference are both evaluated during BGP best-path selection.
 
 
</details>

### 23. Refer to the exhibit. What is the effect of the summary-only keyword in the BGP aggregate command?

```cisco-ios
router bgp 65000
 neighbor 192.0.2.1 remote-as 65001
 address-family ipv4
  neighbor 192.0.2.1 activate
  aggregate-address 203.0.113.0 255.255.255.0 summary-only
```

- [ ] **A)** It prevents more-specific routes from being advertised
- [ ] **B)** It advertises only the more-specific routes
- [ ] **C)** It changes the MED of the aggregate route
- [ ] **D)** It filters inbound updates from the peer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The summary-only keyword suppresses more-specific component routes so only the aggregate is advertised.
 
 
</details>

### 24. What happens immediately when an interface is assigned to a VRF?

- [ ] **A)** The existing IP address is removed
- [ ] **B)** The interface automatically becomes an access port
- [ ] **C)** The interface is placed into shutdown state
- [ ] **D)** The Route Distinguisher is removed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Assigning an interface to a VRF removes its existing IP address, so the address must be reconfigured.
 
 
</details>


---

### **VPN Technologies**

### 25. In a DMVPN network, which protocol dynamically maps private tunnel addresses to public NBMA addresses?

- [ ] **A)** Next Hop Resolution Protocol (NHRP)
- [ ] **B)** Multipoint GRE (mGRE)
- [ ] **C)** Generic Routing Encapsulation (GRE)
- [ ] **D)** Internet Key Exchange version 2 (IKEv2)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NHRP acts as the ARP equivalent for NBMA networks, dynamically mapping inner tunnel addresses to outer public addresses in DMVPN.
 
 
</details>

### 26. Which three technologies are combined in Cisco DMVPN? Select all that apply.

- [ ] **A)** GRE
- [ ] **B)** IPsec
- [ ] **C)** NHRP
- [ ] **D)** VTI

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> DMVPN combines GRE, IPsec, and NHRP to provide scalable, secure hub-and-spoke and spoke-to-spoke VPNs.
 
 
</details>

### 27. Based on the displayed output, which Cisco IOS command was used?

```cisco-ios
Interface: Tunnel0
Tunnel Source: 192.168.1.1
Peers: 3 active
NHRP Registration: 1 registered
NHRP Shortcuts: enabled
NHRP Redirects: enabled
```

- [ ] **A)** show dmvpn
- [ ] **B)** show ip nhrp
- [ ] **C)** show crypto session
- [ ] **D)** show ip route

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The output contains DMVPN-specific tunnel, NHRP registration, and peer details, which are displayed by 'show dmvpn'.
 
 
</details>

### 28. In DMVPN Phase 3, which command must be configured on the hub tunnel interface to advertise redirects?

- [ ] **A)** ip nhrp redirect
- [ ] **B)** ip nhrp shortcut
- [ ] **C)** ip nhrp map multicast dynamic
- [ ] **D)** ip nhrp network-id 1

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> DMVPN Phase 3 uses 'ip nhrp redirect' on the hub and 'ip nhrp shortcut' on spokes to enable direct spoke-to-spoke paths.
 
 
</details>

### 29. Which two commands allow DMVPN Phase 3 spokes to establish direct tunnels without hairpinning through the hub? Select all that apply.

- [ ] **A)** ip nhrp redirect
- [ ] **B)** ip nhrp shortcut
- [ ] **C)** ip nhrp map multicast dynamic
- [ ] **D)** ip nhrp authentication test

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Phase 3 requires 'ip nhrp redirect' on the hub and 'ip nhrp shortcut' on the spokes to allow direct tunnels.
 
 
</details>

### 30. A DMVPN hub is configured as shown. Spokes register successfully, but multicast routing updates are not forwarded. Which command is missing from the tunnel interface?

```cisco-ios
interface Tunnel0
 ip address 10.0.0.1 255.255.255.0
 ip nhrp network-id 1
 ip nhrp authentication SecretKey
 tunnel source GigabitEthernet0/1
 tunnel mode gre multipoint
```

- [ ] **A)** ip nhrp map multicast dynamic
- [ ] **B)** ip nhrp shortcut
- [ ] **C)** ip nhrp redirect
- [ ] **D)** ip nhrp interest

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The missing 'ip nhrp map multicast dynamic' command prevents multicast routing updates from reaching dynamically registered spokes.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cisco/CCNA" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Cisco Certified Network Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Automation and Programmability](#automation-and-programmability) (4 questions)
- [IP Connectivity](#ip-connectivity) (6 questions)
- [IP Services](#ip-services) (4 questions)
- [Network Access](#network-access) (7 questions)
- [Network Fundamentals](#network-fundamentals) (4 questions)
- [Security Fundamentals](#security-fundamentals) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:06.126Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Automation and Programmability | 4 |
| IP Connectivity | 6 |
| IP Services | 4 |
| Network Access | 7 |
| Network Fundamentals | 4 |
| Security Fundamentals | 5 |

---

### **Automation and Programmability**

### 1. What is the primary characteristic of Software-Defined Networking (SDN)?

- [ ] **A)** Centralized control plane
- [ ] **B)** Distributed control plane
- [ ] **C)** Use of proprietary protocols only
- [ ] **D)** Elimination of all routing protocols

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SDN decouples the control plane from the data plane, centralizing network intelligence into a controller.
 
 
</details>

### 2. Select the correct mappings of HTTP methods to CRUD operations.

- [ ] **A)** GET - Retrieve
- [ ] **B)** POST - Create
- [ ] **C)** PUT - Delete
- [ ] **D)** DELETE - Update

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> GET retrieves data, POST creates a new resource. PUT replaces, DELETE removes.
 
 
</details>

### 3. Given the JSON response below, what is the IP address of interface GigabitEthernet1?

```json
{
  "interface": {
    "name": "GigabitEthernet1",
    "ip-address": "10.0.0.1",
    "netmask": "255.255.255.0"
  }
}
```

- [ ] **A)** 10.0.0.1
- [ ] **B)** 10.0.0.2
- [ ] **C)** 192.168.1.1
- [ ] **D)** 172.16.0.1

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The JSON shows the ip address under the interface object as 10.0.0.1.
 
 
</details>

### 4. Which configuration management tool uses an agentless push model?

- [ ] **A)** Ansible
- [ ] **B)** Puppet
- [ ] **C)** Chef
- [ ] **D)** SaltStack

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Ansible is agentless and uses a push model via SSH. Puppet and Chef use agent-based pull.
 
 
</details>


---

### **IP Connectivity**

### 5. Examine the following output. Which router ID is used by the router in the OSPF process?

```cisco-ios
router ospf 1
 router-id 1.1.1.1
 network 192.168.1.0 0.0.0.255 area 0
```

- [ ] **A)** 1.1.1.1
- [ ] **B)** 2.2.2.2
- [ ] **C)** 192.168.1.1
- [ ] **D)** 0.0.0.0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The router ID is explicitly set to 1.1.1.1 via the 'router-id' command under the OSPF process.
 
 
</details>

### 6. Refer to the configuration. What is the purpose of the 'encapsulation dot1Q 10' command under the subinterface?

```cisco-ios
interface GigabitEthernet0/0.10
 encapsulation dot1Q 10
 ip address 192.168.10.1 255.255.255.0
```

- [ ] **A)** It assigns an IP address to the subinterface.
- [ ] **B)** It enables 802.1Q trunking and associates the subinterface with VLAN 10.
- [ ] **C)** It sets the MTU for the subinterface.
- [ ] **D)** It configures the subinterface for ISL encapsulation.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 'encapsulation dot1Q 10' command enables 802.1Q trunking and ties the subinterface to VLAN 10 for tagging.
 
 
</details>

### 7. Analyze the routing table entry below. What does the 'S' stand for in the 'S*' code?

```cisco-ios
S*  0.0.0.0/0 [1/0] via 192.168.1.1
```

- [ ] **A)** Static route
- [ ] **B)** OSPF route
- [ ] **C)** RIP route
- [ ] **D)** Directly connected route

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In Cisco IOS, 'S' indicates a static route. The asterisk (*) means the route is a candidate for default route (gateway of last resort).
 
 
</details>

### 8. Review the IPv6 neighbor cache output. What is the state of the neighbor at 2001:db8::1?

```cisco-ios
2001:db8::1   00:1a:2b:3c:4d:5e   STALE   GigabitEthernet0/0
```

- [ ] **A)** REACHABLE
- [ ] **B)** STALE
- [ ] **C)** INCOMPLETE
- [ ] **D)** DELAY

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The state is STALE, indicating no positive confirmation within the last 30 seconds.
 
 
</details>

### 9. What is the default administrative distance for OSPF routes?

- [ ] **A)** 90
- [ ] **B)** 110
- [ ] **C)** 120
- [ ] **D)** 1

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> OSPF internal routes have a default AD of 110. EIGRP internal is 90, RIP is 120.
 
 
</details>

### 10. Which two statements about route summarization are correct?

- [ ] **A)** Summarization reduces the size of the routing table.
- [ ] **B)** OSPF automatically summarizes at classful boundaries.
- [ ] **C)** EIGRP manual summarization creates a Null0 route.
- [ ] **D)** Summarization is always performed by redistributing routes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Summarization reduces table size; EIGRP creates a discard route to Null0. OSPF does not auto-summarize; redistribution is separate.
 
 
</details>


---

### **IP Services**

### 11. During the DHCP DORA process, which message is the first broadcast sent by the client to locate a server?

- [ ] **A)** Discover
- [ ] **B)** Offer
- [ ] **C)** Request
- [ ] **D)** Acknowledgement

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The DHCP Discover is the first broadcast sent by the client to locate available servers.
 
 
</details>

### 12. Which of the following statements about DHCP relay agents are true? (Select all that apply.)

- [ ] **A)** Forwards DHCP broadcasts across subnets
- [ ] **B)** Requires the 'ip helper-address' command on the client-facing interface
- [ ] **C)** Is configured directly on the DHCP server
- [ ] **D)** Operates using UDP ports 67 and 68

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> A DHCP relay forwards broadcasts to a remote server using the 'ip helper-address' command and relays on UDP ports 67/68.
 
 
</details>

### 13. A network administrator wants to enable DNS resolution on a Cisco router. Which command is missing in the configuration snippet?

```cisco-ios
ip name-server 8.8.8.8
ip domain-name cisco.com
!
```

- [ ] **A)** ip domain-lookup
- [ ] **B)** ip host
- [ ] **C)** dns-server
- [ ] **D)** ip dns server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'ip domain-lookup' command globally enables DNS resolution on Cisco IOS devices.
 
 
</details>

### 14. What transport protocol and port number does NTP use to synchronize time?

- [ ] **A)** TCP port 123
- [ ] **B)** UDP port 123
- [ ] **C)** UDP port 161
- [ ] **D)** TCP port 514

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> NTP operates over UDP port 123 for time synchronization.
 
 
</details>


---

### **Network Access**

### 15. What is the primary purpose of a Virtual Local Area Network (VLAN)?

- [ ] **A)** To extend the LAN across multiple geographic locations
- [ ] **B)** To logically segment a switched network into isolated broadcast domains
- [ ] **C)** To provide routing between different network subnets
- [ ] **D)** To increase the physical bandwidth of a network link

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A VLAN creates separate broadcast domains within a switch, improving security and scalability by isolating traffic.
 
 
</details>

### 16. Which of the following are valid Dynamic Trunking Protocol (DTP) modes on a Cisco switch? (Choose two.)

- [ ] **A)** Dynamic Desirable
- [ ] **B)** Dynamic Active
- [ ] **C)** Dynamic Auto
- [ ] **D)** Dynamic Preferred

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> DTP modes are Dynamic Desirable and Dynamic Auto. Dynamic Active and Dynamic Preferred are not valid DTP modes.
 
 
</details>

### 17. Refer to the show command output. What is the native VLAN for the trunk port?

```cisco-ios
Switch# show interfaces trunk
Port      Mode         Encapsulation  Status        Native vlan
Gi0/1     on           802.1q         trunking      10

Port      Vlans allowed on trunk
Gi0/1     1-1005

Port      Vlans allowed and active in management domain
Gi0/1     1,10,20,100

Port      Vlans in spanning tree forwarding state and not pruned
Gi0/1     1,10,20,100
```

- [ ] **A)** VLAN 1
- [ ] **B)** VLAN 10
- [ ] **C)** VLAN 20
- [ ] **D)** VLAN 100

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The show interfaces trunk output indicates the native VLAN as VLAN 10.
 
 
</details>

### 18. What is the default native VLAN on a Cisco switch trunk port?

- [ ] **A)** VLAN 0
- [ ] **B)** VLAN 1
- [ ] **C)** VLAN 100
- [ ] **D)** VLAN 1002

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The default native VLAN on Cisco switches is VLAN 1. It is recommended to change it to an unused VLAN for security.
 
 
</details>

### 19. Which of the following statements about DTP are true? (Choose two.)

- [ ] **A)** DTP is an IEEE standard protocol.
- [ ] **B)** DTP is a Cisco proprietary protocol.
- [ ] **C)** DTP automatically negotiates trunk links between switches.
- [ ] **D)** DTP is required for trunking to work.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> DTP is Cisco proprietary and used for automatic trunk negotiation. Trunking can be configured manually without DTP.
 
 
</details>

### 20. Examine the configuration. What is the DTP mode on interface GigabitEthernet0/1?

```cisco-ios
interface GigabitEthernet0/1
 switchport mode dynamic desirable
```

- [ ] **A)** Access
- [ ] **B)** Trunk
- [ ] **C)** Dynamic Desirable
- [ ] **D)** Dynamic Auto

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The command 'switchport mode dynamic desirable' sets the DTP mode to Dynamic Desirable, which actively negotiates a trunk.
 
 
</details>

### 21. Which switch becomes the root bridge in a Spanning Tree Protocol (STP) network?

- [ ] **A)** Highest MAC address
- [ ] **B)** Lowest bridge ID
- [ ] **C)** Highest port number
- [ ] **D)** Most physical ports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The root bridge is elected based on the lowest bridge ID, which combines priority and MAC address.
 
 
</details>


---

### **Network Fundamentals**

### 22. Refer to the ACL entry. Which type of traffic does this ACL permit?

```cisco-acl
access-list 100 permit tcp any any eq 80
```

- [ ] **A)** HTTP traffic
- [ ] **B)** HTTPS traffic
- [ ] **C)** All TCP traffic
- [ ] **D)** All IP traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The ACL permits TCP traffic to destination port 80, which is used by HTTP.
 
 
</details>

### 23. Refer to the network diagram description. How many links are required for a full mesh of 4 nodes?

```python
n = 4
links = n*(n-1)/2
print(links)
```

- [ ] **A)** 4
- [ ] **B)** 6
- [ ] **C)** 8
- [ ] **D)** 12

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A full mesh of n nodes requires n(n-1)/2 links. For 4 nodes, it is 4*3/2 = 6 links.
 
 
</details>

### 24. Examine the encapsulation order. Which PDU is formed at the Network layer?

```text
Data -> Application (Data) -> Transport (Segment) -> Network (Packet) -> Data Link (Frame) -> Physical (Bits)
```

- [ ] **A)** Packet
- [ ] **B)** Frame
- [ ] **C)** Segment
- [ ] **D)** Bits

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> At the Network layer, the PDU is called a packet (or IP datagram).
 
 
</details>

### 25. Refer to the IPv6 address. What is the correct compressed form?

```text
2001:0db8:0000:0000:0000:0000:0000:0001
```

- [ ] **A)** 2001:db8::1
- [ ] **B)** 2001:db8:0:0:0:0:0:1
- [ ] **C)** 2001:db8:0::1
- [ ] **D)** 2001:db8::0:1

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The address 2001:0db8:0000:0000:0000:0000:0000:0001 is compressed to 2001:db8::1 by removing leading zeros and replacing consecutive zero groups with ::.
 
 
</details>


---

### **Security Fundamentals**

### 26. What is the default action of an Access Control List (ACL) when a packet does not match any entry?

- [ ] **A)** The packet is permitted
- [ ] **B)** The packet is denied (implicit deny)
- [ ] **C)** The packet is forwarded to the next ACL
- [ ] **D)** The router sends an ICMP message

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Every ACL ends with an implicit deny any any; unmatched packets are dropped.
 
 
</details>

### 27. Which of the following are true about standard ACLs? (Choose two.)

- [ ] **A)** They filter based on source IP only
- [ ] **B)** They can filter by destination port
- [ ] **C)** They are identified by numbers 100-199
- [ ] **D)** Best practice is to apply them near the destination

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Standard ACLs use source IP only and should be placed near the destination. Extended ACLs use port numbers and numbers 100-199.
 
 
</details>

### 28. Refer to the configuration. What is the issue with this ACL?

```cisco-ios
access-list 10 permit host 192.168.1.1
access-list 10 deny any
```

- [ ] **A)** The ACL is missing a permit any any at the end
- [ ] **B)** The order of entries is incorrect
- [ ] **C)** The ACL has an implicit deny that blocks all other traffic
- [ ] **D)** The ACL number is invalid

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The ACL only permits specific traffic; the implicit deny will block everything else, which may be intended.
 
 
</details>

### 29. Which type of firewall maintains a state table to track active connections?

- [ ] **A)** Stateless firewall
- [ ] **B)** Stateful firewall
- [ ] **C)** Proxy firewall
- [ ] **D)** Packet filter

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A stateful firewall uses a state table to remember connection states, unlike stateless firewalls.
 
 
</details>

### 30. Which of the following are security threats covered in the CCNA? (Choose two.)

- [ ] **A)** Phishing
- [ ] **B)** Distributed Denial of Service (DDoS)
- [ ] **C)** SQL Injection
- [ ] **D)** Man-in-the-Middle

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Phishing and DDoS are explicitly covered in the Security Fundamentals section. SQL injection and MiTM are not.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cisco/%20CCNA%20Automation.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Cisco Certified DevNet Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Automation and Programmability](#automation-and-programmability) (6 questions)
- [IP Connectivity and Services](#ip-connectivity-and-services) (5 questions)
- [IP Services](#ip-services) (4 questions)
- [Network Access](#network-access) (3 questions)
- [Network Fundamentals (Expanded)](#network-fundamentals-expanded) (6 questions)
- [Security Fundamentals](#security-fundamentals) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:51:16.807Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Automation and Programmability | 6 |
| IP Connectivity and Services | 5 |
| IP Services | 4 |
| Network Access | 3 |
| Network Fundamentals (Expanded) | 6 |
| Security Fundamentals | 6 |

---

### **Automation and Programmability**

### 1. What is a primary benefit of automation in network management?

- [ ] **A)** Reduces human error
- [ ] **B)** Increases manual complexity
- [ ] **C)** Eliminates the need for network engineers
- [ ] **D)** Slows down provisioning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Automation reduces configuration drift and human error by enforcing a single source of truth and accelerating provisioning.
 
 
</details>

### 2. Which two characteristics are true of controller-based networking compared to traditional?

- [ ] **A)** Centralized control plane
- [ ] **B)** Distributed data plane
- [ ] **C)** Box-by-box CLI configuration
- [ ] **D)** Uses only SNMP for monitoring

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Controller-based networking centralizes the control plane while the data plane remains distributed; it uses model-driven APIs rather than box-by-box CLI.
 
 
</details>

### 3. Based on the code block, which HTTP verb is used to create a new network resource?

```python
import requests
url = "https://192.168.1.1/api/v1/vlans"
payload = {"vlan": {"id": 10, "name": "Guest"}}
response = requests.post(url, json=payload)
print(response.status_code)
```

- [ ] **A)** POST
- [ ] **B)** GET
- [ ] **C)** PUT
- [ ] **D)** DELETE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> POST is used to create a new resource; GET retrieves, PUT updates/replaces, and DELETE removes.
 
 
</details>

### 4. Which Python library is commonly used for SSH-based network automation?

- [ ] **A)** netmiko
- [ ] **B)** requests
- [ ] **C)** json
- [ ] **D)** flask

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Netmiko is a Python library that simplifies SSH connections to network devices; requests is for HTTP, json for parsing data.
 
 
</details>

### 5. Which two automation tools use a declarative language?

- [ ] **A)** Ansible
- [ ] **B)** Puppet
- [ ] **C)** Chef
- [ ] **D)** Bash scripts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Ansible uses declarative YAML playbooks; Puppet uses a declarative DSL; Chef is procedural (Ruby).
 
 
</details>

### 6. In the Git workflow shown, what does the 'git commit' command accomplish?

```bash
git add router_config.txt
git commit -m "Updated OSPF area configuration"
git push origin main
```

- [ ] **A)** Stores changes locally with a message
- [ ] **B)** Pushes changes to the remote repository
- [ ] **C)** Creates a new branch
- [ ] **D)** Merges two branches

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> git commit saves staged changes to the local repository with a descriptive message; push sends to remote.
 
 
</details>


---

### **IP Connectivity and Services**

### 7. Which inter-VLAN routing method uses subinterfaces on a single physical router interface?

- [ ] **A)** SVI
- [ ] **B)** ROAS
- [ ] **C)** HSRP
- [ ] **D)** STP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Router-on-a-Stick uses subinterfaces with dot1Q encapsulation to route between VLANs.
 
 
</details>

### 8. Which two protocols are used for dynamic IP address assignment and name resolution?

- [ ] **A)** DHCP
- [ ] **B)** DNS
- [ ] **C)** ICMP
- [ ] **D)** SNMP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DHCP assigns IP parameters; DNS translates domain names to IP addresses.
 
 
</details>

### 9. Complete the command to enable PAT on a Cisco router: `ip nat inside source list 1 interface GigabitEthernet0/0 ______`

```cisco-ios
ip nat inside source list 1 interface GigabitEthernet0/0 _____
```

- [ ] **A)** overload
- [ ] **B)** static
- [ ] **C)** pool
- [ ] **D)** dynamic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> 'overload' enables PAT, allowing multiple inside addresses to share one global IP.
 
 
</details>

### 10. Which ICMP message type is sent by a router when a packet's TTL expires?

- [ ] **A)** Type 0
- [ ] **B)** Type 3
- [ ] **C)** Type 8
- [ ] **D)** Type 11

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> ICMP Type 11 (Time Exceeded) is sent when TTL decrements to 0.
 
 
</details>

### 11. Which two show commands can be used to verify inter-VLAN routing configuration?

- [ ] **A)** show vlan
- [ ] **B)** show ip route
- [ ] **C)** show mac address-table
- [ ] **D)** show running-config

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> show vlan lists VLANs; show ip route displays routes between VLAN subnets.
 
 
</details>


---

### **IP Services**

### 12. What does stratum 16 indicate in the context of NTP on a Cisco device?

- [ ] **A)** The device is synchronized
- [ ] **B)** The device is unsynchronized
- [ ] **C)** The device is the master clock
- [ ] **D)** The device has a stratum error

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Stratum 16 indicates that the device is not synchronized to any time source. A synchronized device will have a stratum value less than 16.
 
 
</details>

### 13. Which SNMP versions use community strings for authentication?

- [ ] **A)** SNMPv1
- [ ] **B)** SNMPv2c
- [ ] **C)** SNMPv3
- [ ] **D)** None of the above

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SNMPv1 and SNMPv2c use community strings as plaintext passwords. SNMPv3 uses user-based authentication with MD5 or SHA.
 
 
</details>

### 14. Consider the following NTP configuration snippet. What is the purpose of the 'prefer' keyword?

```cisco-ios
ntp server 192.168.1.1 prefer
```

- [ ] **A)** It sets the server as the only NTP source
- [ ] **B)** It makes this server the preferred choice among multiple servers
- [ ] **C)** It enables authentication for this server
- [ ] **D)** It forces the client to ignore other servers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 'prefer' keyword tells the NTP client to favor that server when multiple servers provide acceptable time, but it is not an exclusive directive.
 
 
</details>

### 15. Which syslog severity level corresponds to 'Warning'?

- [ ] **A)** 0
- [ ] **B)** 3
- [ ] **C)** 4
- [ ] **D)** 5

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Syslog severity levels: 0=Emergency, 1=Alert, 2=Critical, 3=Error, 4=Warning, 5=Notice, 6=Informational, 7=Debug.
 
 
</details>


---

### **Network Access**

### 16. What is the purpose of the 802.1Q tag in an Ethernet frame on a trunk link?

- [ ] **A)** To identify the VLAN membership of the frame
- [ ] **B)** To encrypt the frame for security
- [ ] **C)** To replace the source MAC address
- [ ] **D)** To indicate the frame length

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 802.1Q tag carries a VLAN ID that distinguishes frames from different VLANs on a trunk link.
 
 
</details>

### 17. Which of the following are port roles in Spanning Tree Protocol (STP)? (Choose two.)

- [ ] **A)** Root Port
- [ ] **B)** Designated Port
- [ ] **C)** Access Port
- [ ] **D)** Trunk Port

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> STP defines Root Port and Designated Port as standard roles; Access Port and Trunk Port are not STP roles.
 
 
</details>

### 18. Consider the following configuration snippet applied to an interface. What will be the result?

```cisco-ios
interface GigabitEthernet0/1
 channel-group 1 mode passive
```

- [ ] **A)** The interface will negotiate an EtherChannel only if the peer is active.
- [ ] **B)** The interface will form a static EtherChannel.
- [ ] **C)** The interface will immediately become part of channel-group 1 without negotiation.
- [ ] **D)** The interface will not send LACP PDUs and will wait for a peer.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> LACP passive mode only responds to received LACP PDUs; it does not initiate negotiation.
 
 
</details>


---

### **Network Fundamentals (Expanded)**

### 19. Which OSI layer is equivalent to the TCP/IP Internet layer?

- [ ] **A)** Network (Layer 3)
- [ ] **B)** Data Link (Layer 2)
- [ ] **C)** Transport (Layer 4)
- [ ] **D)** Physical (Layer 1)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The TCP/IP Internet layer handles routing and logical addressing, which corresponds to OSI Layer 3 (Network).
 
 
</details>

### 20. Given the IP address 192.168.1.145 with subnet mask 255.255.255.240, which two statements are correct?

- [ ] **A)** The network address is 192.168.1.144
- [ ] **B)** The broadcast address is 192.168.1.159
- [ ] **C)** The subnet mask is 255.255.255.224
- [ ] **D)** There are 16 usable hosts per subnet

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The /28 mask creates a block of 16 addresses. Network is 192.168.1.144, broadcast .159, usable .145-.158 (14 hosts).
 
 
</details>

### 21. Refer to the Python code. What will be the printed IPv6 address?

```python
import ipaddress
mac = "00:0d:bb:11:22:33"
prefix = "2001:db8:1:1::/64"
# EUI-64 calculation
eui64 = ipaddress.IPv6Address(prefix) | int(mac.replace(':', ''), 16) ^ 0x020000000000
print(eui64)
```

- [ ] **A)** 2001:db8:1:1:20d:bbff:fe11:2233
- [ ] **B)** 2001:db8:1:1:00d:bbff:fe11:2233
- [ ] **C)** 2001:db8:1:1:20d:bbff:fe11:2233/64
- [ ] **D)** 2001:db8:1:1:02d:bbff:fe11:2233

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> EUI-64 flips the 7th bit of the first MAC byte (00 -> 02) and inserts FFFE, yielding 020D:BBFF:FE11:2233, then combined with prefix.
 
 
</details>

### 22. When an Ethernet switch receives a frame with an unknown destination MAC, what action does it take?

- [ ] **A)** Floods the frame out of all ports except the ingress port
- [ ] **B)** Forwards the frame only to the ingress port
- [ ] **C)** Drops the frame
- [ ] **D)** Sends an ARP request

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An unknown unicast frame is flooded to all ports (except the one it came from) to find the destination.
 
 
</details>

### 23. Which two security protocols are considered secure for enterprise wireless networks?

- [ ] **A)** WPA2 with AES-CCMP
- [ ] **B)** WPA3 with SAE
- [ ] **C)** WPA with TKIP
- [ ] **D)** WEP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> WPA2-AES and WPA3-SAE are the recommended secure options. WPA-TKIP and WEP are deprecated due to vulnerabilities.
 
 
</details>

### 24. The Ansible playbook snippet targets which layer of a three-tier network topology?

```yaml
- name: Configure access port
  ios_config:
    lines:
      - switchport mode access
      - switchport access vlan 10
      - spanning-tree portfast
    parents: interface GigabitEthernet0/1
```

- [ ] **A)** Access layer
- [ ] **B)** Distribution layer
- [ ] **C)** Core layer
- [ ] **D)** Spine layer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The task configures switchport access VLAN and port security, typical for access layer switches connecting end devices.
 
 
</details>


---

### **Security Fundamentals**

### 25. Which of the following best defines a vulnerability in the context of network security?

- [ ] **A)** A potential harmful event
- [ ] **B)** A weakness in a system
- [ ] **C)** An attack mechanism
- [ ] **D)** A policy violation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A vulnerability is a flaw or gap that can be exploited by a threat.
 
 
</details>

### 26. Which two protocols are commonly used for AAA authentication in Cisco networks?

- [ ] **A)** TACACS+
- [ ] **B)** RADIUS
- [ ] **C)** LDAP
- [ ] **D)** Kerberos

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> TACACS+ and RADIUS are the standard AAA protocols; LDAP and Kerberos are for directory services and authentication respectively.
 
 
</details>

### 27. Refer to the code block. What is the purpose of this Cisco IOS command?

```cisco-ios
crypto key generate rsa general-keys label mykey modulus 2048
```

- [ ] **A)** A symmetric key
- [ ] **B)** A public/private key pair
- [ ] **C)** A digital certificate
- [ ] **D)** A certificate signing request

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The command 'crypto key generate rsa' creates asymmetric key pair used for encryption and signing.
 
 
</details>

### 28. Which security program element primarily focuses on human behavior and decision-making?

- [ ] **A)** Physical security
- [ ] **B)** User awareness
- [ ] **C)** Firewall configuration
- [ ] **D)** Encryption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> User awareness programs target employee behavior, such as recognizing phishing and following security policies.
 
 
</details>

### 29. Which of the following are valid types of Access Control Lists (ACLs) on Cisco devices?

- [ ] **A)** Standard
- [ ] **B)** Extended
- [ ] **C)** Named
- [ ] **D)** Dynamic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Standard, extended, and named ACLs are the three main types; 'dynamic' is not a separate ACL type.
 
 
</details>

### 30. The code block contains a Python script used for network automation. Which security concept does the hardcoded password represent?

```python
import requests
base64.b64encode(b"admin:cisco123")
headers = {"Authorization": "Basic " + encoded}
```

- [ ] **A)** Threat
- [ ] **B)** Vulnerability
- [ ] **C)** Exploit
- [ ] **D)** Risk

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Hardcoded credentials are a vulnerability – a weakness that can be exploited by an attacker.
 
 
</details>

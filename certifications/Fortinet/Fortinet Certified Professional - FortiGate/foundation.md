<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Fortinet/Fortinet%20FortiGate%207.6%20Administrator" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Fortinet Certified Professional - FortiGate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Content Inspection](#content-inspection) (8 questions)
- [Deployment and System Configuration](#deployment-and-system-configuration) (6 questions)
- [Firewall Policies and Authentication](#firewall-policies-and-authentication) (7 questions)
- [Routing](#routing) (5 questions)
- [VPN](#vpn) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:40.309Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Content Inspection | 8 |
| Deployment and System Configuration | 6 |
| Firewall Policies and Authentication | 7 |
| Routing | 5 |
| VPN | 4 |

---

### **Content Inspection**

### 1. In a routed deployment, what must be configured before a FortiGate can forward internet-bound traffic to a next-hop device?

- [ ] **A)** A default route to the ISP gateway
- [ ] **B)** A DNS server address
- [ ] **C)** A DHCP scope on port1
- [ ] **D)** A hostname for the device

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A routed deployment requires a default route toward the ISP or next hop. Once this route exists, the FortiGate can forward inspected traffic to the internet.
 
 
</details>

### 2. Which two CLI configuration blocks are used to set a hostname and configure DNS servers on a FortiGate?

- [ ] **A)** config system global
- [ ] **B)** config system dns
- [ ] **C)** config firewall policy
- [ ] **D)** config router static

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The hostname is set under config system global, and DNS server addresses are configured under config system dns. Both are part of initial deployment and system configuration.
 
 
</details>

### 3. View the CLI code block and identify which FortiGate system global parameter is being configured.

```plaintext
config system global
    set hostname FGT-303
end
```

- [ ] **A)** Hostname
- [ ] **B)** Admin timeout
- [ ] **C)** Timezone
- [ ] **D)** DNS server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block contains a system global section that sets the hostname. The other listed settings are not modified by the configuration shown.
 
 
</details>

### 4. Out of the box, which FortiGate interface is normally used to open the web-based setup wizard?

- [ ] **A)** port1
- [ ] **B)** port2
- [ ] **C)** modem
- [ ] **D)** dmz

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The factory-default FortiGate places the setup IP address on port1, allowing the administrator to access the web-based configuration wizard.
 
 
</details>

### 5. Which two secure management protocols can be enabled on a FortiGate interface for administration purposes?

- [ ] **A)** HTTPS
- [ ] **B)** SSH
- [ ] **C)** Telnet
- [ ] **D)** RDP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> HTTPS and SSH are encrypted management protocols used for FortiGate GUI and CLI access. Telnet is unencrypted, and RDP is not a supported FortiGate administrative access option.
 
 
</details>

### 6. Refer to the code block. Which address is configured as the system DNS primary server?

```plaintext
config system dns
    set primary 208.91.112.53
    set secondary 208.91.112.52
end
```

- [ ] **A)** 208.91.112.53
- [ ] **B)** 208.91.112.52
- [ ] **C)** 192.168.1.99
- [ ] **D)** 203.0.113.1

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block sets the primary DNS server to 208.91.112.53 and the secondary DNS server to 208.91.112.52.
 
 
</details>

### 7. Where must a FortiGate content-inspection profile be referenced so that traffic is actually inspected during FortiGate deployment?

- [ ] **A)** Firewall policy
- [ ] **B)** DNS server
- [ ] **C)** DHCP server
- [ ] **D)** Static route

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Content-inspection profiles are attached to firewall policies. Without that attachment, matching traffic is forwarded without security-profile inspection.
 
 
</details>

### 8. Which two types of FortiGate security profiles are used to inspect network content in a firewall policy?

- [ ] **A)** Antivirus
- [ ] **B)** Web filter
- [ ] **C)** DHCP server
- [ ] **D)** Routing table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Antivirus profiles scan file content and malware patterns, while web filter profiles inspect HTTP and HTTPS content. DHCP and routing are not security profiles.
 
 
</details>


---

### **Deployment and System Configuration**

### 9. In which FortiGate operation mode does the device perform NAT and act as a gateway/router?

- [ ] **A)** Transparent mode
- [ ] **B)** NAT mode
- [ ] **C)** Replay mode
- [ ] **D)** Sniffer mode

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> NAT mode makes FortiGate a routed gateway: it performs NAT on traffic crossing its interfaces. Transparent mode works as an invisible Layer 2 bridge.
 
 
</details>

### 10. Which two CLI commands can you use to back up the FortiGate configuration?

- [ ] **A)** execute backup config tftp <server> <filename>
- [ ] **B)** execute backup config disk <filename>
- [ ] **C)** execute restore config tftp <server> <filename>
- [ ] **D)** execute factoryreset

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> execute backup config stores a configuration copy to TFTP or local disk. Restore and factory reset do not create a backup file.
 
 
</details>

### 11. View the output from the FortiGate command in the exhibit. What does Operation Mode: NAT indicate about the deployment?

```text
get system status
FortiGate-VM64 v7.4.3
Firmware Signature: certified
Operation Mode: NAT
Current Time: Thu Jan 1 10:00:00 2025
```

- [ ] **A)** Routed device with NAT.
- [ ] **B)** Layer 2 transparent bridge.
- [ ] **C)** Factory default state.
- [ ] **D)** Traffic inspection only.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Operation Mode: NAT confirms FortiGate is a routed deployment with NAT enabled. Transparent mode would report Transparent instead.
 
 
</details>

### 12. Which FortiGate configuration object makes it possible for one physical port to carry multiple 802.1Q VLANs?

- [ ] **A)** Hardware switch
- [ ] **B)** VLAN subinterface
- [ ] **C)** Software switch
- [ ] **D)** Loopback interface

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A VLAN subinterface is configured with the logical VLAN ID and allows one physical port to carry multiple tagged VLANs.
 
 
</details>

### 13. When securing administrative access with trusted hosts, which two statements are correct?

- [ ] **A)** Restricts access to defined source addresses.
- [ ] **B)** No remote administration is allowed by default.
- [ ] **C)** Misconfiguration can lock out the administrator.
- [ ] **D)** Used only for FortiManager registration.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Trusted host restrictions limit administrative source addresses and can lock out admins if misconfigured. Leaving the list empty permits remote access from any source.
 
 
</details>

### 14. Review the FortiGate interface configuration in the exhibit. Which two statements are true?

```text
config system interface
    edit "port1"
        set mode static
        set ip 192.168.1.99 255.255.255.0
        set allowaccess ping https ssh
        set type physical
    next
end
```

- [ ] **A)** IP address is manually configured.
- [ ] **B)** Subnet mask is 255.255.255.0.
- [ ] **C)** HTTPS access is disabled.
- [ ] **D)** IP address is obtained from DHCP.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Static mode with an IP address means manual configuration. The netmask is /24 and allowaccess permits HTTPS and SSH.
 
 
</details>


---

### **Firewall Policies and Authentication**

### 15. Which FortiGate CLI configuration mode is used to create and edit IPv4 firewall policies?

- [ ] **A)** config firewall policy
- [ ] **B)** config firewall address
- [ ] **C)** config system interface
- [ ] **D)** config system admin

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Firewall security policies are configured under config firewall policy. Address objects, interfaces, and administrators have separate CLI contexts.
 
 
</details>

### 16. Which two valid actions can be configured for a FortiGate firewall security policy?

- [ ] **A)** ACCEPT
- [ ] **B)** DENY
- [ ] **C)** TRUST
- [ ] **D)** REDIRECT

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A FortiGate firewall policy allows traffic with the ACCEPT action or blocks traffic with the DENY action. TRUST and REDIRECT are not standard policy action values.
 
 
</details>

### 17. Review the FortiGate CLI policy configuration in the code block. Which traffic classification is permitted by this rule?

```fortigate-cli
config firewall policy
    edit 1
        set name "Allow_Ping"
        set srcintf "inside"
        set dstintf "outside"
        set srcaddr "all"
        set dstaddr "all"
        set action accept
        set schedule "always"
        set service "PING"
        set logtraffic all
    next
end
```

- [ ] **A)** ICMP echo requests from the inside interface to the outside interface
- [ ] **B)** HTTP requests from the inside interface to the outside interface
- [ ] **C)** Telnet sessions from the outside interface to the inside interface
- [ ] **D)** DNS queries from the outside interface to the inside interface

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy uses the PING service and the action accept, so ICMP traffic from inside to outside is explicitly allowed. Other services are not matched by the policy.
 
 
</details>

### 18. How does FortiGate decide which security policy applies when multiple policies match the same packet?

- [ ] **A)** The first matching policy in the ordered policy list
- [ ] **B)** The policy with the highest internal ID
- [ ] **C)** The most specific policy regardless of its position
- [ ] **D)** Every matching policy is evaluated alternately

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> FortiGate searches the policy list from top to bottom and applies the action of the first matching policy. The policy ID does not determine the matching order.
 
 
</details>

### 19. Which two policy objects are required so a FortiGate deny rule applies only to Engineering-to-HR traffic?

- [ ] **A)** Source address object
- [ ] **B)** Destination address object
- [ ] **C)** Traffic-shaping policy
- [ ] **D)** Log severity level

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A firewall policy uses source and destination address objects to identify the networks it applies to. Traffic shaping and log settings do not define which traffic matches the rule.
 
 
</details>

### 20. Review the code block. What type of remote authentication server is represented by the objects being defined?

```fortigate-cli
config user ldap
    edit "corp-dc"
        set server "10.10.10.20"
        set cnid "cn"
        set dn "dc=corp,dc=local"
        set type regular
        set binddn "CN=forti,CN=Users,DC=corp,DC=local"
        set bindpassword "encrypted"
    next
end
```

- [ ] **A)** LDAP server
- [ ] **B)** RADIUS server
- [ ] **C)** TACACS+ server
- [ ] **D)** Local user database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The FortiGate CLI context config user ldap configures LDAP directory authentication. RADIUS, TACACS+, and local users use different configuration contexts.
 
 
</details>

### 21. Which FortiGate security policy stores user and group information to enforce identity-based access?

- [ ] **A)** Identity-based security policy
- [ ] **B)** Central NAT policy
- [ ] **C)** DoS policy
- [ ] **D)** Address-based security policy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An identity-based firewall policy uses users and groups, which requires authentication before traffic is allowed. NAT, DoS, and pure address policies do not require user identity.
 
 
</details>


---

### **Routing**

### 22. When FortiGate receives multiple routes with the same prefix length to one destination, which characteristic makes one route preferred?

- [ ] **A)** Lower administrative distance
- [ ] **B)** Higher administrative distance
- [ ] **C)** Shorter prefix length
- [ ] **D)** Older route age

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> FortiGate uses administrative distance to rank route sources. A lower administrative distance makes a route more preferred when the destination prefix is the same.
 
 
</details>

### 23. Which two methods can populate the FortiGate routing table after directly connected routes are created?

- [ ] **A)** Static route definitions
- [ ] **B)** Dynamic routing protocols
- [ ] **C)** Access policy configuration
- [ ] **D)** Firewall address objects

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> FortiGate learns non-connected routes by static route definitions or by dynamic routing protocols such as OSPF and BGP. Firewall objects and policies do not create routing entries.
 
 
</details>

### 24. According to the routing table output, which route type is used for the default gateway entry?

```text
get router info routing-table all
Codes: K - kernel, C - connected, S - static, R - RIP, B - BGP
O - OSPF, * - default route

S*      0.0.0.0/0 [10/0] via 172.16.1.254, port2
```

- [ ] **A)** Static route
- [ ] **B)** Connected route
- [ ] **C)** OSPF route
- [ ] **D)** Kernel route

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The route table code block shows a static default entry with the S flag and default-route marker. A static default route sends traffic to the configured gateway.
 
 
</details>

### 25. In the IPv4 routing table, which destination network is matched by a FortiGate default route when no more-specific route exists?

- [ ] **A)** 0.0.0.0/0
- [ ] **B)** 0.0.0.0/32
- [ ] **C)** 255.255.255.255/0
- [ ] **D)** 127.0.0.0/8

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A default route is the IPv4 prefix 0.0.0.0/0. It matches every destination and is used only when FortiGate has no more-specific prefix.
 
 
</details>

### 26. Which two items are required in a basic FortiGate static route configuration for IPv4 traffic?

- [ ] **A)** Destination prefix
- [ ] **B)** Gateway or outgoing interface
- [ ] **C)** Source IP address
- [ ] **D)** Service port

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A static route defines the prefix to reach and a forwarding instruction, such as a gateway or an outgoing interface. It does not depend on source IP or service.
 
 
</details>


---

### **VPN**

### 27. What is the default operation mode of a FortiGate when it is deployed as an IPsec VPN gateway?

- [ ] **A)** NAT mode
- [ ] **B)** Transparent mode
- [ ] **C)** Offline mode
- [ ] **D)** Proxy mode

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> FortiGate defaults to NAT mode, which allows routes and firewall policies to control VPN traffic. Transparent mode is selected for layer-2 deployments.
 
 
</details>

### 28. Which two system configuration items are essential before a FortiGate site-to-site IPsec VPN can forward data?

- [ ] **A)** Addressing on the WAN interface
- [ ] **B)** Firewall policy permitting VPN traffic
- [ ] **C)** DHCP service on the LAN interface
- [ ] **D)** Phone extension registration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A reachable public address and a firewall policy permitting VPN traffic are required. DHCP and phone registration are unrelated optional services.
 
 
</details>

### 29. According to the command output provided in the code block, what is the current state of the FortiGate IPsec gateway?

```cli
diagnose vpn ike gateway list
vd: root/0
name: HQ-to-Branch
interface: wan1
version: 1
state: up

```

- [ ] **A)** The gateway is up and active
- [ ] **B)** The gateway is down and unreachable
- [ ] **C)** The gateway is administratively disabled
- [ ] **D)** The gateway is in factory reset mode

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block shows state UP, so the VPN gateway is established and can process tunnel traffic.
 
 
</details>

### 30. What is the VPN deployment called when only corporate-network traffic enters the tunnel and other traffic uses the local Internet connection?

- [ ] **A)** Split tunneling
- [ ] **B)** Full tunneling
- [ ] **C)** NAT mode VPN
- [ ] **D)** Transparent VPN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Split tunneling sends only corporate-destined traffic through the VPN tunnel; general Internet traffic exits through the local gateway.
 
 
</details>

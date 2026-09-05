<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Fortinet/Fortinet%20Enterprise%20Firewall%207.6%20Administrator" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Fortinet NSE 7 - Enterprise Firewall 7.6 Administrator</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Central Management and Monitoring](#central-management-and-monitoring) (4 questions)
- [Routing](#routing) (6 questions)
- [Security Profiles](#security-profiles) (6 questions)
- [System Configuration](#system-configuration) (8 questions)
- [VPN](#vpn) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:42.881Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Central Management and Monitoring | 4 |
| Routing | 6 |
| Security Profiles | 6 |
| System Configuration | 8 |
| VPN | 6 |

---

### **Central Management and Monitoring**

### 1. In a FortiGate system configuration, which default TCP port is used by FGFM to communicate with FortiManager?

- [ ] **A)** TCP 541
- [ ] **B)** TCP 443
- [ ] **C)** TCP 22
- [ ] **D)** UDP 514

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> FGFM is the FortiGate-FortiManager management protocol. It uses TCP port 541 to form the central-management tunnel by default.
 
 
</details>

### 2. Which two event-forwarding mechanisms are commonly enabled on a centrally managed FortiGate to send operational events to external monitoring tools? (Choose two.)

- [ ] **A)** SNMP traps
- [ ] **B)** Syslog messages
- [ ] **C)** FGFM tunnel
- [ ] **D)** LLDP advertisements

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SNMP traps send asynchronous alerts, and syslog messages forward events to central collectors. FGFM is a management tunnel, while LLDP is a link-layer discovery protocol.
 
 
</details>

### 3. The code block shows system configuration settings applied to a FortiGate. Which central monitoring method is enabled?

```fortios
config system snmp
    set status enable
    set trap-status enable
end
```

- [ ] **A)** SNMP agent
- [ ] **B)** NetFlow/IPFIX flow export
- [ ] **C)** Syslog event forwarding
- [ ] **D)** Security Fabric logging

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code enables the SNMP agent and SNMP trap status so central monitoring systems can poll the device and receive SNMP alerts.
 
 
</details>

### 4. Which Fortinet product provides centralized system configuration and administrative control for a large number of FortiGate devices?

- [ ] **A)** FortiManager platform
- [ ] **B)** FortiAnalyzer platform
- [ ] **C)** FortiSandbox platform
- [ ] **D)** FortiProxy platform

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> FortiManager is the central management platform for system and policy configuration. FortiAnalyzer is responsible for central logging and analytics.
 
 
</details>


---

### **Routing**

### 5. What is the main purpose of the routing table on a FortiGate?

- [ ] **A)** To select the next hop for a destination prefix
- [ ] **B)** To translate private source IP addresses
- [ ] **C)** To map IP addresses to MAC addresses
- [ ] **D)** To scan files for malware

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The routing table stores known destination prefixes and associated next hops. When the firewall receives traffic, it consults the routing table to decide the next interface and gateway for forwarding.
 
 
</details>

### 6. Which two non-dynamic ways can add routes to a FortiGate routing table? (Choose two.)

- [ ] **A)** Directly connected interfaces
- [ ] **B)** IPsec phase1 settings
- [ ] **C)** Configured static routes
- [ ] **D)** Proxy authentication policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Connected routes are generated automatically when an interface has a valid IP address and is enabled. Static routes are manually configured by an administrator to define explicit paths.
 
 
</details>

### 7. What is the effect of the FortiOS configuration displayed in the code?

```fortios
config router static
    edit 1
        set dst 0.0.0.0/0
        set gateway 10.0.0.1
        set device "wan1"
    next
end
```

- [ ] **A)** It creates a default route through 10.0.0.1
- [ ] **B)** It enables OSPF on the wan1 interface
- [ ] **C)** It sets the device hostname
- [ ] **D)** It configures a DNS server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code enters the static route configuration, defines a destination of 0.0.0.0/0, and sends traffic to gateway 10.0.0.1 through wan1. This is a default static route.
 
 
</details>

### 8. Why is administrative distance used in FortiGate routing?

- [ ] **A)** It determines which route source is more trusted
- [ ] **B)** It measures the physical length of network cables
- [ ] **C)** It selects the oldest administrator account
- [ ] **D)** It defines the order of firewall policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Administrative distance is a trust rating assigned to a route source. Lower values are preferred, so the route learned from a more trusted source is selected when there are multiple routes to the same destination.
 
 
</details>

### 9. Which two values does a FortiGate evaluate when more than one route exists to the same destination prefix? (Choose two.)

- [ ] **A)** Administrative distance
- [ ] **B)** Route metric or cost
- [ ] **C)** Firewall policy sequence number
- [ ] **D)** Interface VLAN ID

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Administrative distance is evaluated first to compare route source trust. If the distances tie, route metric or cost is compared; lower metric values are preferred.
 
 
</details>

### 10. Based on the routing output shown in the code, which destination will be forwarded using the default route?

```fortios
get router info routing-table all
Codes: K - kernel, C - connected, S - static, R - RIP, B - BGP

S*      0.0.0.0/0 [10/0] via 10.0.0.1, wan1
C       10.0.0.0/24 is directly connected, wan1
```

- [ ] **A)** 192.168.2.10
- [ ] **B)** 10.0.0.25
- [ ] **C)** 10.0.0.1
- [ ] **D)** 127.0.0.1

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The routing table contains a connected route for 10.0.0.0/24 and a default static route via 10.0.0.1. A packet to 192.168.2.10 does not match the connected network, so it is sent through the default route.
 
 
</details>


---

### **Security Profiles**

### 11. How are security profiles applied to traffic in a FortiGate Enterprise Firewall configuration?

- [ ] **A)** Firewall policy
- [ ] **B)** Static route
- [ ] **C)** Interface alias
- [ ] **D)** SNMP community

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Security profiles are enforcement objects in FortiOS. They inspect traffic only when they are attached to a firewall policy, because the firewall policy defines which traffic is allowed to enter or leave the FortiGate.
 
 
</details>

### 12. Which two of the following are FortiGate security profile types?

- [ ] **A)** Antivirus
- [ ] **B)** Web Filter
- [ ] **C)** Virtual Domain
- [ ] **D)** External Storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Antivirus and Web Filter are FortiGate security profile types. Virtual domains and external storage are administrative or system resources, not security inspection profiles.
 
 
</details>

### 13. Review the antivirus profile output in the code block. Which virus database option is selected for the profile?

```text
config antivirus profile
    edit "corporate-av"
        set virus-db extended
    next
end
```

- [ ] **A)** Extended
- [ ] **B)** Regular
- [ ] **C)** Quarantine
- [ ] **D)** Allow

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The FortiGate antivirus profile in the code block includes the command set virus-db extended. This selects the extended antivirus database, while the other options do not describe a valid virus database mode in this command.
 
 
</details>

### 14. Which security profile is designed to block known malware during file transfers?

- [ ] **A)** Antivirus
- [ ] **B)** Application Control
- [ ] **C)** DNS Filter
- [ ] **D)** Traffic Shaper

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Antivirus profiles scan traffic for known malware and can block infected files. Application Control classifies applications, DNS Filter controls DNS requests, and Traffic Shaper manages bandwidth.
 
 
</details>

### 15. Which two statements about FortiGate security profiles are correct?

- [ ] **A)** A security profile contains inspection settings grouped by security function.
- [ ] **B)** A single security profile can be referenced by multiple firewall policies.
- [ ] **C)** Security profiles replace the firewall policy action.
- [ ] **D)** Security profiles must be configured inside a static route to function.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Security profiles are reusable objects that contain settings for a specific security function, such as antivirus or web filtering. They are enforced through firewall policies and do not replace the policy action.
 
 
</details>

### 16. Inspect the CLI output in the code block. Which category of security profile is assigned to this firewall policy?

```text
config firewall policy
    edit 101
        set srcintf "port1"
        set dstintf "port2"
        set srcaddr "all"
        set dstaddr "all"
        set action accept
        set schedule "always"
        set service "HTTP"
        set utm-status enable
        set profile-type "single"
        set av-profile "default"
    next
end
```

- [ ] **A)** Antivirus profile
- [ ] **B)** Web filter profile
- [ ] **C)** IPS profile
- [ ] **D)** Application control profile

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block contains the line set av-profile \"default\" inside a firewall policy. The av-profile setting identifies the antivirus security profile that will be applied to matching traffic.
 
 
</details>


---

### **System Configuration**

### 17. What is the purpose of an administrator profile in FortiGate?

- [ ] **A)** Defines GUI and CLI access permissions
- [ ] **B)** Assigns the FortiGate hostname
- [ ] **C)** Sets the time zone for NTP
- [ ] **D)** Configures the DNS server address

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Administrative profiles are used to define permission levels and access rights, while hostname, time, and DNS parameters are configured elsewhere in the system.
 
 
</details>

### 18. Which of the following are supported methods for accessing the FortiGate CLI? (Select all that apply.)

- [ ] **A)** SSH
- [ ] **B)** Console
- [ ] **C)** HTTPS
- [ ] **D)** SNMP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SSH and console are direct FortiGate CLI access methods. HTTPS is used for the web GUI, and SNMP is a monitoring protocol, not a CLI access method.
 
 
</details>

### 19. Review the code block. Which FortiGate configuration mode is shown in the CLI session?

```fortigate
config system admin
edit admin
set password P@ssw0rd
end
```

- [ ] **A)** Admin user edit mode
- [ ] **B)** Global system mode
- [ ] **C)** Interface configuration mode
- [ ] **D)** Router configuration mode

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Within config system admin, the edit admin command enters the administrator user edit context, allowing password or permission settings.
 
 
</details>

### 20. Which FortiGate system parameter is used to set the device hostname?

- [ ] **A)** hostname
- [ ] **B)** default gateway
- [ ] **C)** NTP server
- [ ] **D)** admin password

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The hostname is the displayed name that identifies the FortiGate. Other options relate to NTP, gateway, or credentials, not the device label.
 
 
</details>

### 21. Which actions require a FortiGate administrator to have read-write privileges? (Select all that apply.)

- [ ] **A)** Changing firewall policies
- [ ] **B)** Upgrading firmware
- [ ] **C)** Viewing the dashboard
- [ ] **D)** Running the get command

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Read-only administration supports monitoring commands only; modifying policies or upgrading firmware requires read-write rights.
 
 
</details>

### 22. Refer to the code block. What is the hostname reported by the FortiGate?

```text
FortiGate-760 # get system status
Version: FortiGate-760 v7.6.0,build0123
Hostname: FGT-760-HA
Model: FortiGate-760
Serial Number: FG76000000000000
```

- [ ] **A)** FGT-760-HA
- [ ] **B)** FortiGate-760
- [ ] **C)** FG76000000000000
- [ ] **D)** v7.6.0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The output line Hostname: FGT-760-HA indicates the device name used in prompts and logs.
 
 
</details>

### 23. What should an administrator do before upgrading FortiGate firmware?

- [ ] **A)** Back up the current configuration
- [ ] **B)** Delete unused administrator profiles
- [ ] **C)** Change the hostname
- [ ] **D)** Disable NTP synchronization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Backing up configuration before an upgrade preserves current settings and allows rollback. Disabling services and rebooting are not preparation requirements.
 
 
</details>

### 24. Which elements are saved when creating a FortiGate configuration backup? (Select all that apply.)

- [ ] **A)** System settings
- [ ] **B)** Administrator accounts
- [ ] **C)** Live VPN tunnel state
- [ ] **D)** Cached DNS replies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Backups store configuration objects such as system settings and admin accounts. Session state and packet data are runtime data, not configuration backup.
 
 
</details>


---

### **VPN**

### 25. Which FortiGate system service should be enabled so the device clock stays synchronized for VPN certificate validation?

- [ ] **A)** NTP synchronization
- [ ] **B)** DHCP address assignment
- [ ] **C)** SNMP trap reporting
- [ ] **D)** Web proxy caching

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NTP keeps the FortiGate clock synchronized, which is required for judging certificate validity periods during VPN authentication.
 
 
</details>

### 26. Which two FortiGate system settings must be available before an IPsec VPN peer can be reached by its fully qualified domain name?

- [ ] **A)** DNS server addresses
- [ ] **B)** A route that can reach the DNS server
- [ ] **C)** SNMP read-only community
- [ ] **D)** Console idle timeout

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A fully-qualified domain name must be resolved by DNS servers, and the FortiGate needs a route to reach those servers.
 
 
</details>

### 27. Review the FortiGate command block. What system function does this configuration define?

```fortios
config system dns
    set primary 208.91.112.53
    set secondary 208.91.112.56
end
```

- [ ] **A)** DNS server addresses
- [ ] **B)** NTP server addresses
- [ ] **C)** Firewall address objects
- [ ] **D)** Administrative LDAP servers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The block enters the DNS configuration context and assigns primary and secondary DNS servers.
 
 
</details>

### 28. Which command permanently saves modified FortiGate system configuration in the CLI?

- [ ] **A)** write
- [ ] **B)** execute reboot
- [ ] **C)** get system status
- [ ] **D)** diagnose debug

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The write command saves the running configuration to the flash-based startup configuration.
 
 
</details>

### 29. Which two system-level settings should be checked when preparing FortiGate for an IPsec or SSL VPN deployment?

- [ ] **A)** System clock synchronized by NTP
- [ ] **B)** DNS servers configured for FQDN resolution
- [ ] **C)** SNMP read-only community configured
- [ ] **D)** DHCP IP pool configured

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> NTP keeps certificates valid by synchronized time; DNS is needed when VPN peers are specified by FQDN.
 
 
</details>

### 30. Refer to the CLI configuration. Which system interface configuration is represented?

```fortios
config system interface
    edit "wan1"
        set mode dhcp
        set allowaccess ping
    next
end
```

- [ ] **A)** The interface obtains its IP address by DHCP
- [ ] **B)** The interface acts as an IPsec tunnel endpoint
- [ ] **C)** The interface is assigned a static IP address
- [ ] **D)** The interface is a hardware switch member

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The mode dhcp setting tells the interface to obtain an IP address dynamically from a DHCP server.
 
 
</details>

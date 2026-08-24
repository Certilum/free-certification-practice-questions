<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CompTIA/CompTIA%20Network%2B%20Certification" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>CompTIA Network+</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Network Implementation](#network-implementation) (6 questions)
- [Network Operations](#network-operations) (6 questions)
- [Network Security](#network-security) (4 questions)
- [Network Troubleshooting](#network-troubleshooting) (7 questions)
- [Networking Concepts](#networking-concepts) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:51:37.507Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Network Implementation | 6 |
| Network Operations | 6 |
| Network Security | 4 |
| Network Troubleshooting | 7 |
| Networking Concepts | 7 |

---

### **Network Implementation**

### 1. What is the primary characteristic of static routing compared to dynamic routing protocols?

- [ ] **A)** Automatic adaptation to network topology changes
- [ ] **B)** Manual configuration by the network administrator
- [ ] **C)** Continuous updates using routing protocols
- [ ] **D)** High scalability in large networks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Static routing requires manual entry of routes by the network administrator, offering high predictability and security but lacks scalability and automatic adaptation.
 
 
</details>

### 2. Which of the following are benefits of implementing Virtual Local Area Networks (VLANs) on a network switch? (Select TWO)

- [ ] **A)** Segmentation of broadcast domains
- [ ] **B)** Enhanced security through traffic isolation
- [ ] **C)** Automatic loop prevention without STP
- [ ] **D)** Increased physical cabling requirements

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VLANs allow logical segmentation of broadcast domains and isolate traffic, improving security and reducing unnecessary broadcast traffic.
 
 
</details>

### 3. Based on the provided IP configuration snippet, what is the network address for the host PC-A?

```json
{
  "device": "PC-A",
  "ip_configuration": {
    "ip_address": "192.168.1.10",
    "subnet_mask": "255.255.255.0",
    "default_gateway": "192.168.1.1",
    "dns_server": "8.8.8.8"
  }
}
```

- [ ] **A)** 192.168.1.0/24
- [ ] **B)** 192.168.0.0/16
- [ ] **C)** 192.0.0.0/8
- [ ] **D)** 192.168.1.10/32

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The IP address is 192.168.1.10 with a subnet mask of 255.255.255.0 (which is /24). The network address is therefore 192.168.1.0.
 
 
</details>

### 4. What is the primary function of Software-Defined Wide Area Network (SD-WAN) technology?

- [ ] **A)** Replacing physical transport lines entirely with virtual links
- [ ] **B)** Centralized orchestration and dynamic path selection across multiple links
- [ ] **C)** Restricting traffic to a single dedicated MPLS circuit
- [ ] **D)** Operating strictly at the physical layer of the OSI model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SD-WAN abstracts and orchestrates underlying physical transports (like MPLS, broadband, 5G), allowing dynamic, policy-based routing and application-aware traffic steering.
 
 
</details>

### 5. Which of the following are characteristic applications or properties of single-mode fiber (SMF) optic cabling? (Select TWO)

- [ ] **A)** Used for long-haul and metropolitan area network (MAN) deployments
- [ ] **B)** Typically utilizes LEDs as the light source
- [ ] **C)** Supports higher bandwidth over longer distances using lasers
- [ ] **D)** Core size of 50 or 62 micrometers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Single-mode fiber has a small core (typically 9 microns), uses lasers for light transmission, and is designed for high-bandwidth, long-distance applications.
 
 
</details>

### 6. According to the provided STP port state descriptions, which state allows the port to populate the MAC address table but not yet forward user data?

```text
STP Port States:
- Blocking: Receives BPDUs, does not forward traffic (default initial state)
- Listening: Sends and receives BPDUs, prepares to forward
- Learning: Populates MAC table, prepares to forward
- Forwarding: Normal operation, sends and receives BPDUs and traffic
```

- [ ] **A)** Blocking
- [ ] **B)** Listening
- [ ] **C)** Learning
- [ ] **D)** Forwarding

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> In the Learning state, the switch populates its MAC address table with the source addresses of received frames, but it does not yet forward traffic to avoid loops.
 
 
</details>


---

### **Network Operations**

### 7. A junior network technician notices a critical security vulnerability on a core distribution switch and wants to apply the vendor firmware patch immediately during peak business hours to prevent potential exploitation. What is the correct professional action according to standard organizational procedures?

- [ ] **A)** Submit a formal change request, assess the risks, and schedule the patch deployment during the next approved maintenance window or seek emergency CAB approval.
- [ ] **B)** Apply the patch immediately to the production switch to prevent exploitation, documenting the change only after service is restored.
- [ ] **C)** Bypass the standard change management process because security vulnerabilities require immediate remediation regardless of operational impact.
- [ ] **D)** Defer the patch deployment indefinitely until the vendor releases a less disruptive update that does not require a reboot.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The correct professional action is to submit a formal change request to assess risks and schedule the patch during an approved maintenance window, or seek emergency Change Advisory Board (CAB) approval. Bypassing change management protocols, even for urgent security patches, violates standard governance and can cause severe operational disruptions.
 
 
</details>

### 8. Which of the following documents are considered essential components of comprehensive network documentation according to CompTIA best practices? (Select 3)

- [ ] **A)** Physical network diagrams detailing cabling, rack layouts, and hardware ports.
- [ ] **B)** Logical network diagrams illustrating VLANs, subnets, and routing protocols.
- [ ] **C)** Standard Operating Procedures (SOPs) defining routine maintenance and change workflows.
- [ ] **D)** The company's quarterly financial auditing reports and balance sheets.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Comprehensive network documentation must include physical layouts (such as rack elevations and cabling paths), logical structures (including VLANs and IP subnet allocations), and operational workflows like Standard Operating Procedures (SOPs) to ensure consistency and quick recovery. Financial auditing reports and corporate marketing materials do not assist network technicians in troubleshooting, capacity planning, or maintaining infrastructure baselines.
 
 
</details>

### 9. Based on the provided CLI output for interface FastEthernet0/1, which metric indicates a physical layer issue, such as cabling interference or a faulty transceiver?

```text
Interface: FastEthernet0/1
  Description: Link to Core Switch
  Input packets: 14,520
  Input discards: 12
  Output packets: 13,980
  Output discards: 4
  CRC errors: 45
  Frame Check Sequence (FCS) failures: 42
```

- [ ] **A)** The high count of CRC errors and FCS failures.
- [ ] **B)** The total count of input and output packets.
- [ ] **C)** The description field linking to the core switch.
- [ ] **D)** The low number of output discards.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A high count of CRC (Cyclic Redundancy Check) errors and Frame Check Sequence (FCS) failures on a network interface typically points directly to physical layer issues. Common causes include cabling interference, faulty transceivers, dirty fiber optics, or electrical noise on the copper line. Standard input/output packet counts and low discard values do not indicate physical corruption.
 
 
</details>

### 10. In disaster recovery planning, which metric determines the maximum acceptable amount of data loss, measured in time units since the outage began?

- [ ] **A)** Recovery Point Objective (RPO)
- [ ] **B)** Recovery Time Objective (RTO)
- [ ] **C)** Business Impact Analysis (BIA) threshold
- [ ] **D)** Service Level Agreement (SLA) compliance target

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Recovery Point Objective (RPO) defines the maximum acceptable amount of data loss after a disruptive event, measured as the age of the data that must be restored. In contrast, the Recovery Time Objective (RTO) specifies the target duration for restoring services. Understanding RPO is critical for scheduling backup frequencies to ensure data loss is kept within business-tolerable limits.
 
 
</details>

### 11. Which of the following statements regarding disaster recovery site types are correct? (Select 3)

- [ ] **A)** Cold sites provide basic physical facilities and utilities but require the organization to install and configure all network hardware and software on-site.
- [ ] **B)** Warm sites contain pre-configured hardware and network connections but rely on periodic manual data backups, resulting in potential data loss.
- [ ] **C)** Hot sites offer fully operational infrastructure with real-time data replication, allowing near-instantaneous failover with minimal data loss.
- [ ] **D)** Warm sites provide real-time data replication and active-active network configurations, making them functionally identical to hot sites.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Disaster recovery sites are categorized by their readiness and data replication levels. Cold sites provide basic facilities but require hardware installation, warm sites have pre-configured hardware but rely on periodic backups, and hot sites offer real-time replication for instantaneous cutover. Warm sites do not provide real-time replication, distinguishing them from hot sites.
 
 
</details>

### 12. Based on the interactive syslog excerpt, what is the operational status of the GigabitEthernet0/0 interface's line protocol?

```text
Jan 15 10:12:01 router01 %LINK-3-UPDOWN: Interface GigabitEthernet0/0, changed state to up
Jan 15 10:14:22 router01 %LINEPROTO-5-UPDOWN: Line Protocol on GigabitEthernet0/0, changed state to down
Jan 15 10:15:10 router01 %SYSLOG-5-CONFIG: Configured from console by admin
```

- [ ] **A)** The line protocol changed state to down.
- [ ] **B)** The interface changed state to administratively down.
- [ ] **C)** The system configuration was saved by the console user.
- [ ] **D)** The interface link went up and protocol stayed up permanently.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The syslog message `%LINEPROTO-5-UPDOWN` indicates that the line protocol (Layer 3 logical connection) on interface GigabitEthernet0/0 changed state to 'down'. This is distinct from the physical interface state (`%LINK-3-UPDOWN`), which went 'up', meaning the physical cable is connected but the logical routing or keepalives failed.
 
 
</details>


---

### **Network Security**

### 13. What is the primary objective of the Principle of Least Privilege in network security management?

- [ ] **A)** The maximum access required for future expansion
- [ ] **B)** The absolute minimum access necessary to perform specific tasks
- [ ] **C)** Full administrative access to all local subsystems
- [ ] **D)** Access levels that match the highest privilege group in the directory

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Principle of Least Privilege restricts access to the minimal permissions needed for job functions, reducing the attack surface and limiting damage from compromised credentials.
 
 
</details>

### 14. Which of the following components are part of the Authentication, Authorization, and Accounting (AAA) framework? (Select two)

- [ ] **A)** Verifying the identity of a user or device (Authentication)
- [ ] **B)** Enforcing traffic shaping policies on the uplink port
- [ ] **C)** Determining what resources and actions an authenticated entity is permitted to access (Authorization)
- [ ] **D)** Automatically assigning dynamic IP addresses via DHCP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The AAA framework consists of Authentication (verifying identity), Authorization (defining permitted actions/resources), and Accounting (tracking resource usage and logins).
 
 
</details>

### 15. Based on the provided access control list (ACL) configuration, which traffic is explicitly denied?

```text
access-list 101 permit tcp any any eq 80
access-list 101 deny tcp any any eq 23
access-list 101 permit tcp any any eq 443
```

- [ ] **A)** HTTP (Port 80)
- [ ] **B)** HTTPS (Port 443)
- [ ] **C)** Telnet (Port 23)
- [ ] **D)** DNS (Port 53)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The ACL contains a rule to deny TCP traffic on port 23, which corresponds to the Telnet service, while permitting ports 80 and 443.
 
 
</details>

### 16. What is the primary purpose of an access control vestibule, commonly referred to as a mantrap, in physical security?

- [ ] **A)** To monitor environmental conditions like temperature and humidity
- [ ] **B)** To prevent unauthorized individuals from following authorized personnel into a secure area
- [ ] **C)** To provide continuous video surveillance of server racks
- [ ] **D)** To automatically update operating system patch levels on access control terminals

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A mantrap is a double-door entryway that isolates a user between two interlocking doors, preventing tailgating and ensuring identity verification before granting access to the secure area.
 
 
</details>


---

### **Network Troubleshooting**

### 17. According to the CompTIA Network+ troubleshooting methodology, what is the very first step in the systematic process when a network outage is reported?

- [ ] **A)** Establish a theory of probable cause.
- [ ] **B)** Identify the problem.
- [ ] **C)** Test the theory to determine cause.
- [ ] **D)** Document findings, actions, and outcomes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The first step in the CompTIA methodology is to identify the problem by gathering symptoms, questioning users, and isolating the scope of the failure before creating theories.
 
 
</details>

### 18. Which of the following activities are part of the 'Identify the problem' step in the CompTIA troubleshooting methodology? (Choose all that apply)

- [ ] **A)** Questioning users to gather symptom details.
- [ ] **B)** Determining if recent changes were made to the network.
- [ ] **C)** Replacing suspected faulty network hardware immediately.
- [ ] **D)** Testing the theory using a loopback plug.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Identifying the problem involves gathering information, questioning users, identifying symptoms, and determining if any recent changes were made to duplicate the issue and isolate its scope.
 
 
</details>

### 19. Based on the provided command-line output, what is the most likely reason the client device is experiencing a lack of network connectivity?

```text
IP Configuration
Ethernet adapter Ethernet0:
   IPv4 Address . . . . . . . . . . : 169.254.21.7
   Subnet Mask . . . . . . . . . . . : 255.255.0.0
   Default Gateway . . . . . . . . . : (blank)
   DHCP Server . . . . . . . . . . . : (blank)
```

- [ ] **A)** The DNS server is misconfigured.
- [ ] **B)** The DHCP server is unreachable or down, causing APIPA assignment.
- [ ] **C)** The default gateway is blocking traffic.
- [ ] **D)** The subnet mask is incorrect.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> An IP address in the 169.254.0.0/16 range with no default gateway or DHCP server listed indicates Automatic Private IP Addressing (APIPA) was used because the DHCP server was unreachable.
 
 
</details>

### 20. What type of physical layer issue occurs when unshielded twisted-pair cabling runs parallel to high-voltage electrical lines?

- [ ] **A)** Attenuation
- [ ] **B)** Electromagnetic Interference (EMI)
- [ ] **C)** Crosstalk
- [ ] **D)** Duplex mismatch

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Electromagnetic Interference (EMI) occurs when external magnetic fields, such as those from high-voltage power lines, induce unwanted voltage in nearby unshielded copper cables, corrupting data frames.
 
 
</details>

### 21. Which of the following tools are specifically designed to diagnose physical cabling issues such as breaks, split pairs, and continuity? (Choose two)

- [ ] **A)** Cable tester
- [ ] **B)** Time Domain Reflectometer (TDR)
- [ ] **C)** Protocol analyzer
- [ ] **D)** DHCP snooping configuration tool

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A basic cable tester verifies pinout and continuity, while a Time Domain Reflectometer (TDR) measures cable length and pinpoints physical breaks or impedance mismatches on copper lines.
 
 
</details>

### 22. Based on the switch port statistics shown in the interactive output, what configuration issue is most likely occurring on this link?

```text
Switch# show interfaces FastEthernet 0/12
  Input packets: 1000, Output packets: 950
  Input errors: 0, Output errors: 0
  CRC errors: 4125
  Late collisions: 3012
  Collisions: 5000
```

- [ ] **A)** A split pair wiring fault
- [ ] **B)** A duplex mismatch
- [ ] **C)** A broadcast storm
- [ ] **D)** An IP address conflict

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> High counts of CRC errors and late collisions on an Ethernet interface typically indicate a duplex mismatch, where one port operates in full-duplex while the connected device operates in half-duplex.
 
 
</details>

### 23. What is the consequence of a 'split pair' error in twisted-pair Ethernet cabling termination?

- [ ] **A)** Complete link down immediately
- [ ] **B)** Massive crosstalk and electromagnetic interference due to destroyed pair balance
- [ ] **C)** Automatic speed negotiation to 10 Mbps
- [ ] **D)** DHCP scope exhaustion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Split pairs break the physical balance of the twisted pairs, which ruins the cable's ability to cancel out crosstalk, resulting in massive electromagnetic interference and data corruption.
 
 
</details>


---

### **Networking Concepts**

### 24. Which transport-layer protocol is used by the Simple File Transfer Protocol (TFTP) for network booting and lightweight file transfers?

- [ ] **A)** TCP
- [ ] **B)** UDP
- [ ] **C)** ICMP
- [ ] **D)** ARP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> TFTP uses UDP port 69 for lightweight, connectionless file transfers, commonly used in network device booting environments.
 
 
</details>

### 25. Which of the following transport protocols and port numbers are associated with the Domain Name System (DNS)? (Choose two)

- [ ] **A)** UDP port 53
- [ ] **B)** TCP port 53
- [ ] **C)** TCP port 22
- [ ] **D)** UDP port 69

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DNS primarily uses UDP port 53 for standard queries but falls back to TCP port 53 for zone transfers and large responses.
 
 
</details>

### 26. Based on the provided command-line filter, which remote access protocol is being captured on the network interface?

```bash
tcpdump -i eth0 'port 22'
```

- [ ] **A)** SSH
- [ ] **B)** Telnet
- [ ] **C)** HTTP
- [ ] **D)** SMTP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The tcpdump command filters traffic on port 22, which is the default port used by SSH for secure remote access.
 
 
</details>

### 27. At which layer of the OSI model does a standard network switch operate when forwarding frames based on MAC addresses?

- [ ] **A)** Physical Layer (Layer 1)
- [ ] **B)** Data Link Layer (Layer 2)
- [ ] **C)** Network Layer (Layer 3)
- [ ] **D)** Transport Layer (Layer 4)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Standard switches operate at the Data Link Layer (Layer 2) of the OSI model, forwarding frames using MAC addresses.
 
 
</details>

### 28. Which of the following are primary responsibilities of the Transport Layer (Layer 4) of the OSI model? (Choose two)

- [ ] **A)** Logical addressing and routing
- [ ] **B)** Segmentation and reassembly of data
- [ ] **C)** Physical signal transmission
- [ ] **D)** Flow control and error recovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> The Transport Layer handles end-to-end communication, including segmentation, flow control, and error recovery to ensure reliable data delivery.
 
 
</details>

### 29. Based on the OSI encapsulation mapping provided in the code block, what is the Protocol Data Unit (PDU) at the Network Layer?

```text
OSI Layer Mapping:
Layer 7: Application (Data)
Layer 4: Transport (Segment)
Layer 3: Network (Packet)
Layer 2: Data Link (Frame)
Layer 1: Physical (Bits)
```

- [ ] **A)** Frame
- [ ] **B)** Segment
- [ ] **C)** Packet
- [ ] **D)** Bits

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Network Layer (Layer 3) of the OSI model encapsulates data into packets containing source and destination logical addresses.
 
 
</details>

### 30. Which network service is used to automatically assign IP addresses and other network configuration parameters to devices on a local network?

- [ ] **A)** DNS
- [ ] **B)** DHCP
- [ ] **C)** SNMP
- [ ] **D)** NTP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Dynamic Host Configuration Protocol (DHCP) automatically assigns IP addresses, subnet masks, and other parameters to network clients.
 
 
</details>

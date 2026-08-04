<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Arista/ACE:%20L1%20(Arista%20Cloud%20Engineer:%20Level%201)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>ACE: L1 (Cloud Engineer: Level 1)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Arista CloudVision Platform](#arista-cloudvision-platform) (9 questions)
- [Cloud Network Design and Troubleshooting](#cloud-network-design-and-troubleshooting) (3 questions)
- [Cloud Networking Fundamentals](#cloud-networking-fundamentals) (7 questions)
- [Network Automation and Programmability](#network-automation-and-programmability) (6 questions)
- [Security and Compliance in the Cloud](#security-and-compliance-in-the-cloud) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:45.071Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Arista CloudVision Platform | 9 |
| Cloud Network Design and Troubleshooting | 3 |
| Cloud Networking Fundamentals | 7 |
| Network Automation and Programmability | 6 |
| Security and Compliance in the Cloud | 5 |

---

### **Arista CloudVision Platform**

### 1. What is the default screen displayed after logging into the Arista CloudVision Portal?

- [ ] **A)** Dashboard
- [ ] **B)** Network Topology
- [ ] **C)** Device Inventory
- [ ] **D)** Events & Audit

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The dashboard is the first screen after login, providing a summary of network health and events.
 
 
</details>

### 2. Which two features are part of the CloudVision Portal navigation? (Choose two.)

- [ ] **A)** Dashboard widgets
- [ ] **B)** Topology view
- [ ] **C)** SNMP
- [ ] **D)** CLI

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Dashboard widgets and Topology view are key portal components; SNMP and CLI are not navigation features.
 
 
</details>

### 3. Based on the code snippet, which CloudVision view displays network connections derived from LLDP?

```python
from cvprac.cvp_client import CvpClient

# Connect to CloudVision
client = CvpClient()
client.connect(["cvp1.example.com"], "admin", "password")

# Retrieve network topology data (LLDP-derived links)
topology = client.api.get_topology()
```

- [ ] **A)** Topology view
- [ ] **B)** Devices view
- [ ] **C)** Events view
- [ ] **D)** Provisioning view

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Topology view visualizes LLDP/CDP neighbors; it is not the Devices or Events list.
 
 
</details>

### 4. What is the purpose of a configlet in CloudVision?

- [ ] **A)** Reusable, modular configuration snippets applied to managed devices for centralized configuration management.
- [ ] **B)** A pre-built virtual machine image used to deploy CloudVision nodes.
- [ ] **C)** A log file that records all configuration changes made through CloudVision.
- [ ] **D)** A network protocol used to push configurations from CloudVision to switches.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Configlets are modular configuration fragments applied to devices for central management.
 
 
</details>

### 5. Which two steps are part of the CloudVision device onboarding lifecycle? (Choose two.)

- [ ] **A)** DHCP-based IP address assignment
- [ ] **B)** Applying configlets to the device
- [ ] **C)** Manual CLI configuration
- [ ] **D)** SNMP-based polling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> ZTP starts with DHCP and ends with applying configlets; CLI and SNMP are not core onboarding steps.
 
 
</details>

### 6. Given the DHCP option, which server does the switch contact during ZTP bootstrap?

```python
def evaluate_ztp_server(selected):
    correct_server = "TFTP/HTTP file server"
    return selected == correct_server

# Example usage:
print(evaluate_ztp_server("TFTP/HTTP file server"))  # True
```

- [ ] **A)** A file server, such as TFTP or HTTP, hosting the bootfile
- [ ] **B)** A DNS server resolving the switch hostname
- [ ] **C)** An NTP server providing time synchronization
- [ ] **D)** A syslog server collecting switch logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Option 67 specifies the bootfile URL usually pointing to a script or configuration server.
 
 
</details>

### 7. Which role in CloudVision can approve pending tasks?

- [ ] **A)** Admin
- [ ] **B)** Network-Operator
- [ ] **C)** Operator
- [ ] **D)** Observer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Only the Admin role can approve tasks; Operator and Network-Operator cannot.
 
 
</details>

### 8. Which two statements about CloudVision dashboard widgets are true? (Choose two.)

- [ ] **A)** Widgets can be customized and rearranged to fit the operator's preferences.
- [ ] **B)** Widgets show only aggregated metrics for the entire network.
- [ ] **C)** Widgets can display both aggregated network-wide data and per-device data.
- [ ] **D)** Widgets update instantly with no latency.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Widgets are customizable and show both aggregate and individual device data, but have small delay.
 
 
</details>

### 9. Refer to the image bundle definition; what does an image bundle contain?

```yaml
imageBundle:
  name: "EOS-4.26.1F"
  images:
    - "EOS-4.26.1F.swi"
  extensions:
    - "TerminAttr-1.21.2.swix"
```

- [ ] **A)** An image bundle: EOS images and optional extensions for device upgrades
- [ ] **B)** A configlet: device configuration snippets managed in CloudVision
- [ ] **C)** A container: hierarchical grouping of devices and their roles
- [ ] **D)** A tag: metadata key/value pairs assigned to devices

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Image bundles group EOS images and optionally extensions for device upgrades.
 
 
</details>


---

### **Cloud Network Design and Troubleshooting**

### 10. What does VXLAN (Virtual Extensible LAN) encapsulate?

- [ ] **A)** Layer 2 Ethernet frames into UDP/IP packets
- [ ] **B)** IP packets into MPLS labels
- [ ] **C)** TCP segments into GRE tunnels
- [ ] **D)** Fibre Channel frames into FCIP packets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> VXLAN encapsulates tenant Ethernet frames into UDP packets for transport across a Layer 3 underlay.
 
 
</details>

### 11. Which two components provide Layer 3 isolation for tenants in a multitenant network?

- [ ] **A)** VRF (Virtual Routing and Forwarding)
- [ ] **B)** BGP EVPN (Ethernet Virtual Private Network)
- [ ] **C)** VLAN (Virtual Local Area Network)
- [ ] **D)** VXLAN (Virtual Extensible LAN)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VRF provides separate routing tables per tenant, while BGP EVPN distributes tenant routes, enabling Layer 3 isolation.
 
 
</details>

### 12. Examine the configuration snippet. What is the purpose of this command?

```text
vlan 100
   vxlan vni 10000
```

- [ ] **A)** It maps a VLAN to VXLAN Network Identifier (VNI) 10000 for VXLAN encapsulation.
- [ ] **B)** It assigns IP address 10000 to the VLAN interface.
- [ ] **C)** It enables VXLAN routing between VLAN 100 and an external BGP peer.
- [ ] **D)** It creates a new VXLAN tunnel interface named VNI 10000.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command 'vxlan vni 10000' under a VLAN configuration maps that VLAN to VNI 10000 for VXLAN encapsulation.
 
 
</details>


---

### **Cloud Networking Fundamentals**

### 13. Which cloud service model gives complete control over the operating system and networking?

- [ ] **A)** Infrastructure as a Service (IaaS)
- [ ] **B)** Platform as a Service (PaaS)
- [ ] **C)** Software as a Service (SaaS)
- [ ] **D)** Function as a Service (FaaS)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IaaS gives customers full control over the OS, applications, and virtual networking; the provider only manages physical hardware.
 
 
</details>

### 14. Which two responsibilities belong to the customer in an IaaS model?

- [ ] **A)** Patching the guest operating system
- [ ] **B)** Configuring virtual firewalls
- [ ] **C)** Managing physical server hardware
- [ ] **D)** Maintaining the hypervisor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> In IaaS, the customer patches the OS and configures virtual firewalls; the provider handles physical infrastructure.
 
 
</details>

### 15. Examine the VPC configuration snippet. What is missing for the web server to be reachable from the internet?

```hcl
resource "aws_vpc" "main" {
  cidr_block = "10.0.0.0/16"
}

resource "aws_subnet" "public" {
  vpc_id     = aws_vpc.main.id
  cidr_block = "10.0.1.0/24"
}

resource "aws_internet_gateway" "igw" {
  vpc_id = aws_vpc.main.id
}

resource "aws_route_table" "public" {
  vpc_id = aws_vpc.main.id
}

resource "aws_route" "internet_access" {
  route_table_id         = aws_route_table.public.id
  destination_cidr_block = "0.0.0.0/0"
  gateway_id             = aws_internet_gateway.igw.id
}

resource "aws_route_table_association" "public" {
  subnet_id      = aws_subnet.public.id
  route_table_id = aws_route_table.public.id
}

resource "aws_security_group" "web" {
  vpc_id = aws_vpc.main.id

  ingress {
    from_port   = 80
    to_port     = 80
    protocol    = "tcp"
    cidr_blocks = ["0.0.0.0/0"]
  }

  egress {
    from_port   = 0
    to_port     = 0
    protocol    = "-1"
    cidr_blocks = ["0.0.0.0/0"]
  }
}

resource "aws_instance" "web" {
  ami                    = "ami-0abcdef1234567890"
  instance_type          = "t2.micro"
  subnet_id              = aws_subnet.public.id
  vpc_security_group_ids = [aws_security_group.web.id]
}
```

- [ ] **A)** A public IPv4 address or Elastic IP address associated with the instance's network interface
- [ ] **B)** A route table entry for 0.0.0.0/0 pointing to the internet gateway
- [ ] **C)** An internet gateway attached to the VPC
- [ ] **D)** A security group rule allowing inbound HTTP traffic from 0.0.0.0/0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Even with a route to IGW, the instance needs a public or Elastic IP to be reachable from the internet.
 
 
</details>

### 16. What is the maximum number of VLANs supported by the 802.1Q standard?

- [ ] **A)** 4,094
- [ ] **B)** 4,096
- [ ] **C)** 1,024
- [ ] **D)** 65,536

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> 802.1Q uses a 12-bit VLAN ID, permitting a maximum of 4096 VLANs (0-4095).
 
 
</details>

### 17. Which two statements about VXLAN are correct?

- [ ] **A)** VXLAN encapsulates Ethernet frames in UDP packets, typically using destination port 4789.
- [ ] **B)** VXLAN uses a 24-bit VNI, supporting approximately 16 million logical networks.
- [ ] **C)** VXLAN operates only within a Layer 2 broadcast domain and cannot cross Layer 3 boundaries.
- [ ] **D)** VXLAN uses a 12-bit VLAN ID, limiting it to 4094 segments.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VXLAN encapsulates Ethernet in UDP (port 4789) and uses a 24-bit VNI, allowing 16 million segments over a Layer 3 underlay.
 
 
</details>

### 18. Study the EVPN route output. Which route type is this?

```text
BGP routing table entry for [2] [0] [48] [00:1c:73:00:00:01] [32] [10.0.0.1]
Paths: (1 available, best #1)
  NextHop: 192.0.2.1
```

- [ ] **A)** Type 2 (MAC/IP Advertisement Route)
- [ ] **B)** Type 1 (Ethernet Auto-Discovery Route)
- [ ] **C)** Type 3 (Inclusive Multicast Ethernet Tag Route)
- [ ] **D)** Type 5 (IP Prefix Route)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Type-2 routes carry MAC and IP information for host reachability in EVPN.
 
 
</details>

### 19. What is the primary role of a VTEP in a VXLAN fabric?

- [ ] **A)** It encapsulates and decapsulates VXLAN traffic at the tunnel endpoints
- [ ] **B)** It routes traffic between VXLAN VNIs using IP multicast
- [ ] **C)** It provides the physical underlay switching fabric for VXLAN traffic
- [ ] **D)** It authenticates end hosts before they join a VXLAN segment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A VTEP terminates VXLAN tunnels – it encapsulates outbound frames and decapsulates inbound frames.
 
 
</details>


---

### **Network Automation and Programmability**

### 20. Which command-line interface mode permits alteration of the currently running configuration on an Arista network switch?

- [ ] **A)** Global configuration mode
- [ ] **B)** Privileged EXEC mode
- [ ] **C)** Interface configuration mode
- [ ] **D)** Line configuration mode

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Global configuration mode is reached via the 'configure terminal' command and allows direct changes to the running configuration.
 
 
</details>

### 21. Which two authentication methods are supported by the CloudVision REST API for external access?

- [ ] **A)** Session cookies obtained from a successful login
- [ ] **B)** Service tokens issued to service accounts for non-interactive automation
- [ ] **C)** Basic authentication with a username and password in the HTTP Authorization header
- [ ] **D)** SSH key pairs used for cryptographic API authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The CloudVision REST API supports session cookies from login and service tokens; basic auth and SSH keys are not standard methods.
 
 
</details>

### 22. Based on the 'show vlan' output provided in the code block, how many VLANs are present in the database?

```cli
show vlan

VLAN ID Name                Status    Ports
------- ------------------- --------- -------------------------------
1       default             active    Et1-4
10      engineering          active    Et5-8
20      marketing            active    Et9-12
```

- [ ] **A)** 1
- [ ] **B)** 2
- [ ] **C)** 3
- [ ] **D)** 4

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The 'show vlan' output displays three VLANs: default VLAN 1 and custom VLANs 10 and 20.
 
 
</details>

### 23. What is the primary purpose of a CloudVision configlet in network automation?

- [ ] **A)** Version-controlled EOS configuration snippets that enforce desired state across devices via CloudVision
- [ ] **B)** Physical appliances used to aggregate and route network traffic between data centers
- [ ] **C)** Python-based scripts that dynamically generate device configurations on demand
- [ ] **D)** Routing protocols that enable CloudVision to discover neighboring Arista switches

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Configlets are version-controlled EOS configuration snippets that enforce desired state across devices via CloudVision.
 
 
</details>

### 24. Which two automation tools are most commonly associated with managing Arista EOS devices?

- [ ] **A)** Ansible
- [ ] **B)** Terraform
- [ ] **C)** Puppet
- [ ] **D)** Chef

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The playbook identifies Ansible and Terraform as the foundational automation tools for Arista devices.
 
 
</details>

### 25. Referring to the gNMI path in the code block, what type of data does this subscription retrieve?

```gnmi
subscribe {
  path: "/interfaces/interface[name=Ethernet1]/state/counters"
  mode: STREAM
  encoding: JSON_IETF
}
```

- [ ] **A)** Operational counters for interface Ethernet1
- [ ] **B)** Configuration settings for interface Ethernet1
- [ ] **C)** LLDP neighbor information for interface Ethernet1
- [ ] **D)** Routing table entries for the default VRF

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The path '/interfaces/interface[name=Ethernet1]/state/counters' targets operational counters for that interface.
 
 
</details>


---

### **Security and Compliance in the Cloud**

### 26. What is the primary purpose of MACsec as defined by IEEE 802.1AE?

- [ ] **A)** To provide hop-by-hop encryption and integrity verification at Layer 2 for Ethernet frames
- [ ] **B)** To provide end-to-end encryption between applications over the internet
- [ ] **C)** To authenticate users before they can access the network
- [ ] **D)** To encrypt data at the application layer to protect cloud storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MACsec (IEEE 802.1AE) provides hop-by-hop encryption and integrity verification at Layer 2, securing Ethernet frames.
 
 
</details>

### 27. Which of the following are core principles of cloud network security best practices? (Select all that apply)

- [ ] **A)** Implementing least privilege access controls
- [ ] **B)** Using micro-segmentation to isolate workloads
- [ ] **C)** Encrypting data in transit and at rest
- [ ] **D)** Relying solely on a perimeter firewall for defense

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Least privilege, micro-segmentation, and encryption are core principles. Over-reliance on a perimeter firewall is not a best practice.
 
 
</details>

### 28. An engineer wants to verify MACsec session status on an Arista switch. Which command should be used?

```bash
show macsec status
```

- [ ] **A)** show macsec status
- [ ] **B)** show macsec profile
- [ ] **C)** show macsec counters
- [ ] **D)** show macsec keychain

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command 'show macsec status' displays the operational state of MACsec on the device.
 
 
</details>

### 29. What does the shared responsibility model in cloud security primarily entail?

- [ ] **A)** The cloud provider is responsible for securing all customer application code and data.
- [ ] **B)** The customer is responsible for the security of the underlying physical data centers.
- [ ] **C)** The customer is responsible for securing their data, identities, and network configurations.
- [ ] **D)** The cloud provider assumes full responsibility for all security controls in the cloud.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> In the shared responsibility model, the provider secures the infrastructure, while the customer secures their data, identities, and network.
 
 
</details>

### 30. Which of the following are valid types of ACLs supported by Arista EOS? (Select all that apply)

- [ ] **A)** IPv4 ACL
- [ ] **B)** IPv6 ACL
- [ ] **C)** MAC ACL
- [ ] **D)** DNS ACL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Arista EOS supports IPv4, IPv6, and MAC ACLs. DNS ACLs are not a standard ACL type.
 
 
</details>

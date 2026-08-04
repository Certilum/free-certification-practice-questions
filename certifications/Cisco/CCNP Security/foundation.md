<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cisco/CCNP%20Security.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>CCNP Security</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Automation and Programmability](#automation-and-programmability) (4 questions)
- [Cloud and Content Security](#cloud-and-content-security) (3 questions)
- [Endpoint Security and Forensics](#endpoint-security-and-forensics) (4 questions)
- [Network Security](#network-security) (6 questions)
- [Security Concepts](#security-concepts) (9 questions)
- [Security Services](#security-services) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:03.575Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Automation and Programmability | 4 |
| Cloud and Content Security | 3 |
| Endpoint Security and Forensics | 4 |
| Network Security | 6 |
| Security Concepts | 9 |
| Security Services | 4 |

---

### **Automation and Programmability**

### 1. What is the mandatory encoding format used by NETCONF for data representation?

- [ ] **A)** XML
- [ ] **B)** JSON
- [ ] **C)** Both XML and JSON
- [ ] **D)** YAML

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NETCONF mandates XML encoding for all RPCs and data, as defined in RFC 6241. JSON is not supported in NETCONF, whereas RESTCONF supports both JSON and XML.
 
 
</details>

### 2. Which of the following are considered secure practices when managing credentials in Python automation scripts for Cisco security devices? (Choose all that apply.)

- [ ] **A)** Storing credentials in environment variables
- [ ] **B)** Using a configuration file with restricted file permissions (e.g., 600)
- [ ] **C)** Implementing token-based authentication with periodic token refresh
- [ ] **D)** Hardcoding the username and password directly in the script

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Hardcoding credentials is insecure and violates best practices. Environment variables, restricted config files, and token-based methods with expiry are all recommended. Always avoid exposing secrets in source code or logs.
 
 
</details>

### 3. What is the primary purpose of the following code snippet?

```python
import requests

fmc_user = 'admin'
fmc_pass = 'password'
fmc_server = 'https://fmc.example.com'

url = f'{fmc_server}/api/fmc/v1/domain/e276abec/fmc/token'
response = requests.post(url, auth=(fmc_user, fmc_pass), verify=False)
token = response.json().get('accessToken')
print('Token:', token)
```

- [ ] **A)** Authenticate and obtain a session token from FMC
- [ ] **B)** Retrieve a list of network objects from FMC
- [ ] **C)** Deploy a configuration change to an FTD device
- [ ] **D)** Delete an existing access policy from FMC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code uses the FMC REST API to POST credentials to the token endpoint and extracts the access token from the response. This token is then used for subsequent API calls.
 
 
</details>

### 4. Which network management protocol provides transactional commit and rollback capabilities for YANG-based configuration changes?

- [ ] **A)** NETCONF
- [ ] **B)** RESTCONF
- [ ] **C)** SNMP
- [ ] **D)** CLI (Command Line Interface)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NETCONF (RFC 6241) supports candidate and running datastores, enabling transactional commits and rollback via <commit> and <discard-changes> operations. RESTCONF does not provide such transactional guarantees.
 
 
</details>


---

### **Cloud and Content Security**

### 5. In the IaaS cloud model, which party is responsible for patching the operating system running on a virtual machine?

- [ ] **A)** The cloud provider
- [ ] **B)** The customer
- [ ] **C)** The hypervisor vendor
- [ ] **D)** The application owner

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In IaaS, the customer retains control over the operating system, applications, and data, and is responsible for patching the OS. The provider secures the hypervisor and physical infrastructure.
 
 
</details>

### 6. Which of the following are deployment modes of a Cloud Access Security Broker (CASB)? (Select all that apply.)

- [ ] **A)** Forward proxy
- [ ] **B)** Reverse proxy
- [ ] **C)** API-based
- [ ] **D)** VPN concentrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> CASB can be deployed as a forward proxy, reverse proxy, or API-based. VPN concentrator is not a CASB deployment mode.
 
 
</details>

### 7. Refer to the IAM policy snippet. What cloud resource does this policy allow Cisco Secure Cloud Analytics to read?

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": "ec2:DescribeFlowLogs",
      "Resource": "*"
    }
  ]
}
```

- [ ] **A)** VPC Flow Logs
- [ ] **B)** CloudTrail logs
- [ ] **C)** S3 bucket data
- [ ] **D)** DNS queries

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy allows the ec2:DescribeFlowLogs action, which is necessary for Secure Cloud Analytics to retrieve VPC Flow Logs metadata. CloudTrail logs require different permissions.
 
 
</details>


---

### **Endpoint Security and Forensics**

### 8. When the AMP connector encounters a file with an unknown hash and network connectivity is available, what is the default action?

- [ ] **A)** Blocks the file execution
- [ ] **B)** Allows execution and optionally sends the file to the cloud for analysis
- [ ] **C)** Quarantines the file until analysis is complete
- [ ] **D)** Ignores the file and does not log the event

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> When unknown, AMP allows execution and optionally submits the file to Threat Grid for sandboxing based on policy.
 
 
</details>

### 9. Which of the following are characteristics of an Endpoint Detection and Response (EDR) solution? (Choose two.)

- [ ] **A)** Behavioral analytics and anomaly detection
- [ ] **B)** Primarily signature-based file scanning
- [ ] **C)** Real-time prevention of all known threats
- [ ] **D)** Threat hunting through historical telemetry

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> EDR focuses on detection, investigation, and response using behavioral analytics and historical data, not just signatures or prevention.
 
 
</details>

### 10. Refer to the code block. In a live forensics investigation, which command should be executed first according to the order of volatility?

```bash
1. dd if=/dev/sda of=/mnt/evidence/disk.img
2. memdump > /mnt/evidence/memory.dmp
3. netstat -an > /mnt/evidence/connections.txt
4. lsmod > /mnt/evidence/modules.txt
```

- [ ] **A)** 1
- [ ] **B)** 2
- [ ] **C)** 3
- [ ] **D)** 4

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Memory (RAM) is the most volatile and must be captured first; disk and logs are less volatile.
 
 
</details>

### 11. In an AnyConnect VPN with posture assessment, when does ISE evaluate the device posture?

- [ ] **A)** Before user authentication
- [ ] **B)** After authentication but before final authorization
- [ ] **C)** After full network access is granted
- [ ] **D)** During the VPN tunnel establishment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Posture is evaluated after AAA authentication and before the final authorization is applied.
 
 
</details>


---

### **Network Security**

### 12. Which of the following is a characteristic of Firepower Threat Defense (FTD) Transparent mode?

- [ ] **A)** Supports dynamic routing protocols such as OSPF and BGP
- [ ] **B)** Allows NAT address translation on data interfaces
- [ ] **C)** Functions as a Layer 2 bridge without IP changes to traffic
- [ ] **D)** Requires a unique IP subnet on each data interface

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Transparent mode works as a Layer 2 bridge, inspecting traffic without modifying source/destination IPs. It does not support dynamic routing, NAT, or require per-interface IP subnets.
 
 
</details>

### 13. Which are prerequisites for registering an FTD device with the Firepower Management Center (FMC)? (Choose two.)

- [ ] **A)** NTP synchronization on the FTD
- [ ] **B)** A unique registration key generated on the FMC
- [ ] **C)** The FTD must be in Routed mode
- [ ] **D)** A static route to the FMC via the management interface

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Registration requires the FMC IP and a registration key. NTP sync is also critical for certificate validation. The mode (Routed/Transparent) does not affect registration, and a default gateway is sufficient if the management network is directly connected.
 
 
</details>

### 14. Review the following CLI output and determine which TCP port is used for FTD-FMC registration:

```cisco_cli
> show manager
FMC IP: 192.168.1.100 (port 8305)
Registration key: ****
State: Registered
```

- [ ] **A)** 22
- [ ] **B)** 443
- [ ] **C)** 8305
- [ ] **D)** 8443

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The command 'show manager' displays the FMC connection details. By default, FTD uses TCP port 8305 for registration. Port 22 is for SSH (policy deployment), 443 is for HTTPS (smart licensing), and 8443 is a common alternative but not default for registration.
 
 
</details>

### 15. In an ASA Active/Standby failover configuration, what is synchronized from the active to the standby unit by default?

- [ ] **A)** Dynamic NAT translations (xlates)
- [ ] **B)** Stateful connection information (conns)
- [ ] **C)** The entire configuration file per sync interval
- [ ] **D)** All static and dynamic ARP entries

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> By default, stateful failover replicates connection table entries (conns) and static NAT xlates. Dynamic NAT entries (xlates) are not synced; they are rebuilt on the new active unit. Configuration is synced via 'write standby' or automatic sync only when saved.
 
 
</details>

### 16. Which two types of NAT are supported on a Cisco ASA in Routed mode? (Choose two.)

- [ ] **A)** Policy NAT (Twice NAT)
- [ ] **B)** Dynamic PAT with overload
- [ ] **C)** NAT64 for IPv6 translation
- [ ] **D)** Transparent bridging NAT

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> ASA supports both Policy NAT (Twice NAT) and Dynamic PAT. NAT64 is not standard on ASA. Transparent bridging NAT is not a valid term; transparent mode does not support NAT.
 
 
</details>

### 17. The following output shows the ACL configuration on an ASA outside interface. An inbound packet destined to 203.0.113.10 reaches the firewall. After ACL processing, which IP address is the destination examined by the NAT engine?

```cisco_cli
access-list OUTSIDE_IN extended permit tcp any host 203.0.113.10 eq 443
```

- [ ] **A)** 203.0.113.10 (the original destination)
- [ ] **B)** 10.1.1.10 (the real internal IP)
- [ ] **C)** 0.0.0.0 (any address)
- [ ] **D)** The source IP of the packet

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> For inbound traffic, ACL on outside checks the original destination IP (mapped IP) before NAT un-translation. Only after the ACL permits the packet does the NAT engine un-translate the destination to the real IP. Therefore, the ACL must match the mapped IP, not the real IP.
 
 
</details>


---

### **Security Concepts**

### 18. What is a vulnerability in the context of network security?

- [ ] **A)** A potential danger that could exploit a weakness to cause harm
- [ ] **B)** A weakness in system design that could be exploited by a threat agent
- [ ] **C)** An action taken by a threat actor to breach security
- [ ] **D)** The likelihood that a threat will exploit a vulnerability

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A vulnerability is a weakness in design, implementation, or operation that a threat agent can exploit.
 
 
</details>

### 19. Which of the following are types of malware? (Select two.)

- [ ] **A)** Virus
- [ ] **B)** Firewall
- [ ] **C)** Trojan
- [ ] **D)** Proxy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Malware includes viruses and trojans. Firewalls and proxies are security tools, not malware.
 
 
</details>

### 20. Study the following ACL configuration and answer the question.

```cisco-ios
access-list 100 deny ip any any
```

- [ ] **A)** It denies all IP traffic
- [ ] **B)** It permits all IP traffic
- [ ] **C)** It denies only TCP traffic
- [ ] **D)** It permits only UDP traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The ACL 'deny ip any any' blocks all IP packets from any source to any destination.
 
 
</details>

### 21. Which of the following is a symmetric encryption algorithm?

- [ ] **A)** RSA
- [ ] **B)** AES
- [ ] **C)** ECC
- [ ] **D)** Diffie-Hellman

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AES (Advanced Encryption Standard) is a symmetric block cipher widely used for bulk encryption.
 
 
</details>

### 22. Which of the following are components of a Public Key Infrastructure (PKI)? (Select two.)

- [ ] **A)** Root Certificate Authority
- [ ] **B)** Symmetric Key
- [ ] **C)** Certificate Revocation List
- [ ] **D)** Hash Function

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> A PKI includes a Root CA and CRL. Symmetric keys and hash functions are not exclusive PKI components.
 
 
</details>

### 23. Refer to the TACACS+ server configuration and answer the question.

```cisco-ios
tacacs-server host 10.1.1.1 key secret123
```

- [ ] **A)** TACACS+ uses TCP as the transport protocol
- [ ] **B)** TACACS+ uses UDP as the transport protocol
- [ ] **C)** TACACS+ encrypts only the password
- [ ] **D)** TACACS+ is an IETF standard

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TACACS+ runs over TCP (port 49) and encrypts the entire packet body, unlike RADIUS which uses UDP and encrypts only the password.
 
 
</details>

### 24. The three components of the AAA framework are:

- [ ] **A)** Authentication, Authorization, Accounting
- [ ] **B)** Access, Audit, Accounting
- [ ] **C)** Assurance, Authorization, Authentication
- [ ] **D)** Authentication, Accounting, Application

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AAA stands for Authentication, Authorization, and Accounting, centralizing access control, policy enforcement, and logging.
 
 
</details>

### 25. Which of the following are methods of network segmentation? (Select two.)

- [ ] **A)** VLANs
- [ ] **B)** VRF
- [ ] **C)** Encryption
- [ ] **D)** VPN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VLANs (Layer 2) and VRF (Layer 3) are segmentation methods. Encryption and VPN provide confidentiality, not segmentation.
 
 
</details>

### 26. Study the following zone-based firewall configuration and answer.

```cisco-ios
zone security INSIDE
interface GigabitEthernet0/1
 zone-member security INSIDE
```

- [ ] **A)** It creates a security zone and assigns an interface to it
- [ ] **B)** It defines a zone-pair policy for traffic inspection
- [ ] **C)** It applies a service policy to the zone
- [ ] **D)** It removes an interface from a zone

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The commands 'zone security INSIDE' and 'zone-member security INSIDE' create the zone and assign an interface to it.
 
 
</details>


---

### **Security Services**

### 27. What is the primary function of Cisco Umbrella's DNS-layer security?

- [ ] **A)** Block malicious domains before a connection is established
- [ ] **B)** Act as a stateful cloud-delivered firewall at layer 3/4
- [ ] **C)** Provide a full VPN tunnel for off-network devices
- [ ] **D)** Scan email attachments for malware

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cisco Umbrella's DNS-layer security intercepts DNS requests and blocks malicious domains by returning a sinkhole IP, thereby preventing any connection to threats. It does not act as a firewall, VPN, or email scanner.
 
 
</details>

### 28. Which two services are provided by Cisco Umbrella? (Choose two.)

- [ ] **A)** DNS-layer security
- [ ] **B)** Cloud-delivered firewall (CDFW)
- [ ] **C)** On-premises next-generation firewall (NGFW)
- [ ] **D)** Email encryption via CRES

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Cisco Umbrella provides DNS-layer security (blocking malicious domains) and a cloud-delivered firewall (CDFW) for IP/port filtering. It does not replace an on-premises NGFW and does not handle email encryption.
 
 
</details>

### 29. Refer to the code block. In an 802.1X deployment, which RADIUS attribute is used by Cisco ISE to deliver a downloadable ACL (dACL) to the network access device?

```cisco-ios
radius-server host 10.1.1.1 key cisco123
radius-server vsa send authentication
!
interface GigabitEthernet1/0/1
 authentication port-control auto
 dot1x pae authenticator
!
radius-server attribute 8 include-in-access-req
```

- [ ] **A)** Filter-ID
- [ ] **B)** Cisco-AVPair
- [ ] **C)** Session-Timeout
- [ ] **D)** Called-Station-ID

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The RADIUS Filter-ID attribute (often contains the dACL name) is used by Cisco ISE to send a downloadable ACL to the network device. Cisco-AVPair can carry other information, but Filter-ID is the standard attribute for dACL.
 
 
</details>

### 30. Which feature of Cisco Web Security Appliance (WSA) is used to inspect outbound web traffic for sensitive data like credit card numbers?

- [ ] **A)** Data Loss Prevention (DLP)
- [ ] **B)** URL Filtering
- [ ] **C)** Anti-malware scanning
- [ ] **D)** Proxy caching

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cisco WSA's DLP feature uses dictionaries and custom regex to inspect outbound web traffic for sensitive data such as credit card numbers or SSNs. URL filtering focuses on categories, anti-malware on malware, and caching is for performance.
 
 
</details>

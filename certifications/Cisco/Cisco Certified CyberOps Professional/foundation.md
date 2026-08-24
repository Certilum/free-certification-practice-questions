<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cisco/Cisco%20Certified%20Specialist%20-%20Security%20Core.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Cisco Certified CyberOps Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Programmability and Automation](#programmability-and-automation) (3 questions)
- [Security Architecture](#security-architecture) (6 questions)
- [Security Concepts](#security-concepts) (3 questions)
- [Security Engineering](#security-engineering) (9 questions)
- [Security Operations](#security-operations) (6 questions)
- [Vulnerability Management](#vulnerability-management) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:51:07.000Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Programmability and Automation | 3 |
| Security Architecture | 6 |
| Security Concepts | 3 |
| Security Engineering | 9 |
| Security Operations | 6 |
| Vulnerability Management | 3 |

---

### **Programmability and Automation**

### 1. Which HTTP method is idempotent and replaces an entire resource?

- [ ] **A)** GET
- [ ] **B)** POST
- [ ] **C)** PUT
- [ ] **D)** DELETE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> PUT is idempotent and replaces the entire resource. POST is non-idempotent, GET retrieves, DELETE removes.
 
 
</details>

### 2. Which two characteristics apply to Ansible automation framework?

- [ ] **A)** Agent-based management
- [ ] **B)** Declarative playbooks
- [ ] **C)** Uses YAML for playbooks
- [ ] **D)** Requires Python on devices

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Ansible is agentless and declarative, using YAML playbooks. It does not require Python on managed devices.
 
 
</details>

### 3. What syntax error is present in the following YAML snippet?

```yaml
- name: rule1
action: allow

```

- [ ] **A)** Missing colon
- [ ] **B)** Incorrect indentation
- [ ] **C)** Missing dash
- [ ] **D)** Extra quotation marks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 'action' key must be indented under the list item to be part of the mapping.
 
 
</details>


---

### **Security Architecture**

### 4. Which type of firewall goes beyond simple packet filtering to include application inspection, intrusion prevention, and SSL decryption?

- [ ] **A)** Stateful firewall
- [ ] **B)** Next-Generation Firewall (NGFW)
- [ ] **C)** Proxy firewall
- [ ] **D)** Packet filter

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Next-Generation Firewalls integrate features like IPS, URL filtering, and SSL decryption, unlike basic packet filters or stateful firewalls.
 
 
</details>

### 5. Which two phases are involved in establishing an IPsec site-to-site VPN?

- [ ] **A)** Phase 1 (IKE SA)
- [ ] **B)** Phase 2 (IPsec SA)
- [ ] **C)** Phase 3 (AH SA)
- [ ] **D)** Phase 4 (ESP SA)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> IPsec VPN establishment consists of Phase 1 for IKE SA and Phase 2 for IPsec SA. Phases 3 and 4 are not standard.
 
 
</details>

### 6. Given the following IPsec configuration, what is the primary purpose of applying the crypto map to the outgoing interface?

```cisco-ios
interface GigabitEthernet0/0
 ip address 10.1.1.1 255.255.255.0
 crypto map CMAP
```

- [ ] **A)** Defines interesting traffic
- [ ] **B)** Binds the transform set and peer IP
- [ ] **C)** Enables NAT traversal
- [ ] **D)** Initiates IKE main mode

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The crypto map binds the IPsec transform set and the peer IP address to the interface, enabling the tunnel.
 
 
</details>

### 7. Which protocol does Cisco AnyConnect use over UDP for better performance?

- [ ] **A)** SSL
- [ ] **B)** DTLS
- [ ] **C)** TLS
- [ ] **D)** IPsec

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Cisco AnyConnect uses DTLS (Datagram Transport Layer Security) over UDP to reduce latency and improve performance.
 
 
</details>

### 8. Which two methods are commonly used to enforce network segmentation?

- [ ] **A)** VLANs
- [ ] **B)** VRFs
- [ ] **C)** DHCP Snooping
- [ ] **D)** Port Security

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VLANs and VRFs are common segmentation methods. DHCP Snooping and Port Security are security features not directly used for segmentation.
 
 
</details>

### 9. From the 'show crypto isakmp sa' output, what does the state 'MM_ACTIVE' indicate?

```cisco-ios
show crypto isakmp sa
IPv4 Crypto ISAKMP SA
 dst             src             state          conn-id status
10.1.1.2        10.1.1.1        MM_ACTIVE      1001    ACTIVE
```

- [ ] **A)** Phase 1 has completed
- [ ] **B)** Phase 2 has completed
- [ ] **C)** Phase 1 is in progress
- [ ] **D)** Phase 2 is in progress

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MM_ACTIVE stands for Main Mode Active, which indicates that IKE Phase 1 (SA establishment) has completed successfully.
 
 
</details>


---

### **Security Concepts**

### 10. Which of the following best defines a vulnerability?

- [ ] **A)** A weakness that can be exploited to cause harm
- [ ] **B)** A potential danger that exploits a weakness
- [ ] **C)** The probability of a threat occurrence
- [ ] **D)** The consequence of a security incident

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A vulnerability is a weakness, not the threat itself or the risk. For example, an open port is a vulnerability.
 
 
</details>

### 11. Which of the following are considered social engineering attacks? (Select all that apply.)

- [ ] **A)** Phishing
- [ ] **B)** Spear-phishing
- [ ] **C)** Denial-of-service
- [ ] **D)** Man-in-the-middle

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Social engineering manipulates people, not systems. Phishing and spear-phishing target human behavior.
 
 
</details>

### 12. Interpret the following Cisco ASA log entry:

```log
ASA-4-106023: Built TCP connection 12345 from inside:192.168.1.10/50000 to outside:10.0.0.1/80
```

- [ ] **A)** A new TCP connection was established
- [ ] **B)** A TCP connection was denied
- [ ] **C)** A TCP connection was closed
- [ ] **D)** A TCP connection was translated by NAT

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The keyword 'Built' indicates a new connection was successfully created.
 
 
</details>


---

### **Security Engineering**

### 13. What is the primary role of the Firepower Management Center (FMC) in a Cisco Secure Firewall deployment?

- [ ] **A)** Centralized policy management and event analysis
- [ ] **B)** Inline traffic inspection and packet filtering
- [ ] **C)** VPN termination and NAT processing
- [ ] **D)** Local command-line configuration of the firewall

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> FMC is the centralized management platform for policy staging, deployment, and monitoring of multiple FTD devices, while the data plane resides on FTD.
 
 
</details>

### 14. Which two actions in FMC require a 'Deploy' operation to take effect on FTD devices?

- [ ] **A)** Creating a new network object
- [ ] **B)** Editing an existing access control rule
- [ ] **C)** Viewing connection events on the FMC dashboard
- [ ] **D)** Adding a device to FMC without policy change

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Any change to policies or objects in FMC must be deployed to the FTD devices to take effect; monitoring activities do not require deployment.
 
 
</details>

### 15. Examine the Snort rule in the code block. What action does this rule take on matching traffic?

```snort
alert tcp $HOME_NET any -> $EXTERNAL_NET 80 (msg:"Possible HTTP exploit"; flow:to_server; content:"|00 00 00|ASLR"; drop; sid:1000001;)
```

- [ ] **A)** Drop the packet and generate an alert
- [ ] **B)** Allow the packet and log only
- [ ] **C)** Reset the TCP session
- [ ] **D)** Add the source IP to a block list

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The rule uses 'drop' action which means the packet is dropped and an alert is generated. It does not specify a block or reset action.
 
 
</details>

### 16. What is the key difference between an inline IPS and a passive IDS?

- [ ] **A)** Inline can block traffic; passive can only alert
- [ ] **B)** Inline adds less latency than passive
- [ ] **C)** Passive requires a tap; inline uses a SPAN port
- [ ] **D)** Inline operates at Layer 7; passive at Layer 3

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Inline IPS sits in the traffic path and can actively drop or reset sessions, while passive IDS only monitors and sends alerts.
 
 
</details>

### 17. Which two protocols are essential for the operation of DMVPN?

- [ ] **A)** mGRE (Multipoint Generic Routing Encapsulation)
- [ ] **B)** NHRP (Next Hop Resolution Protocol)
- [ ] **C)** GDOI (Group Domain of Interpretation)
- [ ] **D)** L2TP (Layer 2 Tunneling Protocol)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DMVPN uses mGRE for tunnel encapsulation and NHRP for dynamic next-hop resolution. GDOI is used by GETVPN, not DMVPN.
 
 
</details>

### 18. Review the crypto configuration block. Which phase of IPsec does this configuration belong to?

```cisco-ios
crypto ikev2 policy 10
 encryption aes-cbc-256
 integrity sha256
 group 14
 lifetime seconds 86400
```

- [ ] **A)** Phase 1 (IKE policy)
- [ ] **B)** Phase 2 (IPsec transform set)
- [ ] **C)** Both phases
- [ ] **D)** Neither; this is for crypto maps

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The commands set IKE parameters (encryption, hash, DH group, lifetime) which are used during Phase 1 to establish the IKE SA.
 
 
</details>

### 19. In Cisco ISE architecture, what is the function of the Policy Service Node (PSN)?

- [ ] **A)** Handles authentication and policy enforcement for endpoints
- [ ] **B)** Provides administrative GUI and configuration management
- [ ] **C)** Collects and stores all log and monitoring data
- [ ] **D)** Acts as a certificate authority for device certificates

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The PSN (Policy Service Node) is the primary node that processes RADIUS requests, performs authorization, posture, and other network access services.
 
 
</details>

### 20. Which two EAP methods require a server-side certificate for authentication?

- [ ] **A)** PEAP (Protected EAP)
- [ ] **B)** EAP-TLS
- [ ] **C)** EAP-MD5
- [ ] **D)** EAP-FAST (using PAC)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Both PEAP and EAP-TLS use a TLS tunnel that requires the server to present a certificate. EAP-FAST uses a PAC instead of a certificate.
 
 
</details>

### 21. Examine the command in the code block. What is the primary purpose of this AMP for Endpoints command?

```bash
ampcli status
```

- [ ] **A)** Check the connection status of the AMP connector to the cloud
- [ ] **B)** Scan the system for malware immediately
- [ ] **C)** Isolate the endpoint from the network
- [ ] **D)** Apply a new policy definition

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'ampcli status' command shows the current state of the AMP connector, including cloud connectivity, policy version, and last scan time.
 
 
</details>


---

### **Security Operations**

### 22. What data source does Cisco Stealthwatch primarily use for network visibility?

- [ ] **A)** NetFlow/IPFIX
- [ ] **B)** Firewall logs
- [ ] **C)** SNMP traps
- [ ] **D)** Syslog messages

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cisco Stealthwatch uses NetFlow and IPFIX flow data from network devices to build behavioral baselines and detect anomalies.
 
 
</details>

### 23. Which of the following are capabilities of Cisco Stealthwatch? (Select all that apply)

- [ ] **A)** Behavioral modeling
- [ ] **B)** Encrypted traffic analytics
- [ ] **C)** Direct firewall rule management
- [ ] **D)** Cognitive analytics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Stealthwatch provides behavioral modeling, cognitive analytics, and encrypted traffic analytics but does not directly manage firewall rules.
 
 
</details>

### 24. Refer to the code block. What is the purpose of this configuration on a Cisco switch?

```cisco-ios

interface GigabitEthernet0/1
 ip flow ingress
 ip flow egress

```

- [ ] **A)** Enable NetFlow data collection
- [ ] **B)** Encrypt traffic on the interface
- [ ] **C)** Enable firewall inspection
- [ ] **D)** Configure IP routing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The commands 'ip flow ingress' and 'ip flow egress' enable NetFlow sampling on the interface, which Stealthwatch uses for telemetry.
 
 
</details>

### 25. What is the primary responsibility of a Tier 1 SOC analyst?

- [ ] **A)** Triaging and validating incoming alerts
- [ ] **B)** Performing deep forensic analysis
- [ ] **C)** Conducting proactive threat hunting
- [ ] **D)** Managing firewall policy changes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Tier 1 analysts triage and validate alerts, escalate confirmed threats, and close false positives.
 
 
</details>

### 26. Which HTTP methods are idempotent? (Select all that apply)

- [ ] **A)** GET
- [ ] **B)** POST
- [ ] **C)** PUT
- [ ] **D)** DELETE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Idempotent methods produce the same outcome when executed multiple times; GET, PUT, and DELETE are idempotent, while POST is not.
 
 
</details>

### 27. Refer to the code block. What authentication method is used?

```python

import requests
auth_url = "https://api.cisco.com/oauth/token"
payload = {"grant_type": "client_credentials", "client_id": "...", "client_secret": "..."}
response = requests.post(auth_url, data=payload)
token = response.json()["access_token"]
headers = {"Authorization": f"Bearer {token}"}
response = requests.get("https://api.umbrella.com/enforce", headers=headers)

```

- [ ] **A)** OAuth 2.0 client credentials grant
- [ ] **B)** API key
- [ ] **C)** Basic authentication
- [ ] **D)** Certificate-based authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The script requests an access token using client credentials and then uses it as a bearer token, which is OAuth 2.0.
 
 
</details>


---

### **Vulnerability Management**

### 28. What is the primary difference between authenticated and unauthenticated vulnerability scanning?

- [ ] **A)** Authenticated scanning uses credentials to log into systems; unauthenticated scanning does not.
- [ ] **B)** Authenticated scanning is always passive; unauthenticated scanning is always active.
- [ ] **C)** Authenticated scanning only works for network devices; unauthenticated scanning works for all devices.
- [ ] **D)** Authenticated scanning requires a scanner to be on the same subnet; unauthenticated scanning does not.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Authenticated scanning uses valid credentials to log into target systems, enabling deep inspection. Unauthenticated scanning relies on external probes and lacks internal access.
 
 
</details>

### 29. Which of the following are common vulnerability assessment methodologies? (Select two)

- [ ] **A)** Passive assessment
- [ ] **B)** Active assessment
- [ ] **C)** Forensic analysis
- [ ] **D)** Social engineering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Common methodologies include passive and active assessment. Forensic analysis and social engineering are separate disciplines, not vulnerability assessment methodologies.
 
 
</details>

### 30. Analyze the following scanning command. What is the primary purpose of this scan? (Choose one)

```bash
nmap -sP 192.168.1.0/24
```

- [ ] **A)** Discovery scan to identify live hosts
- [ ] **B)** Full vulnerability scan
- [ ] **C)** Service version detection
- [ ] **D)** Operating system fingerprinting

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The '-sP' flag performs a ping sweep (discovery scan) to find live hosts without deep vulnerability checking.
 
 
</details>

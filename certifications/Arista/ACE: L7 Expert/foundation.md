<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Arista/ACE:%20L7%20(Arista%20Cloud%20Engineer:%20Level%207)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>ACE: L7 Expert</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Arista L7 Security](#arista-l7-security) (7 questions)
- [Automation and Programmability](#automation-and-programmability) (9 questions)
- [Network Design for L7 Services](#network-design-for-l7-services) (8 questions)
- [Troubleshooting and Optimization](#troubleshooting-and-optimization) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:58.461Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Arista L7 Security | 7 |
| Automation and Programmability | 9 |
| Network Design for L7 Services | 8 |
| Troubleshooting and Optimization | 6 |

---

### **Arista L7 Security**

### 1. What distinguishes policy-based segmentation from VLAN-based segmentation in Arista CloudVision?

- [ ] **A)** Policy-based segmentation ties policies to logical groups independent of physical topology, while VLAN-based segmentation is tied to VLANs and subnets.
- [ ] **B)** Policy-based segmentation requires per-device ACL configuration, while VLAN-based segmentation is automated.
- [ ] **C)** Policy-based segmentation uses MAC addresses for filtering, while VLAN-based segmentation uses IP addresses.
- [ ] **D)** Policy-based segmentation only works with overlay networks like VXLAN, while VLAN-based segmentation works on native Ethernet.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CloudVision segmentation uses logical policy groups, not VLANs, enabling micro-segmentation within the same broadcast domain.
 
 
</details>

### 2. What are two key characteristics of Arista CloudVision's default behavior when segmentation is first enabled? (Choose two.)

- [ ] **A)** All inter-VLAN traffic is allowed until a deny rule overrides it when using RBACLs.
- [ ] **B)** All traffic is blocked until explicit allow policies are defined.
- [ ] **C)** Zone-based segmentation applies a default-deny posture.
- [ ] **D)** CloudVision uses a permissive default model for policy groups, not a default-deny.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> CloudVision's RBACL defaults to allow; only zone-based segmentation uses default-deny. Policy groups are permissive.
 
 
</details>

### 3. Examine the command output. Which Arista MACsec feature is being verified?

```bash
show mac security mka
MKA Session for Port-Channel1
  CAK-ID: 1234567890abcdef
  SAK Version: 2
  Key Server: 00:1c:73:00:00:01
  Status: Established
```

- [ ] **A)** The MKA session details showing the CAK-ID and SAK version.
- [ ] **B)** The encryption status showing whether MACsec is active.
- [ ] **C)** The cipher suite negotiation result between two peers.
- [ ] **D)** The replay window configuration and packet drop count.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The `show mac security mka` command displays MKA session information including CAK-ID and SAK version.
 
 
</details>

### 4. What type of frames are allowed on an Arista switch port before 802.1X authentication succeeds?

- [ ] **A)** Only EAPoL and control plane frames like CDP/LLDP are allowed.
- [ ] **B)** All data frames are allowed but with limited bandwidth.
- [ ] **C)** Only DHCP and ARP frames are permitted.
- [ ] **D)** All Ethernet frames are allowed until the supplicant fails authentication.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The uncontrolled port only allows EAPoL for authentication and CDP/LLDP; all other traffic is dropped until authorization.
 
 
</details>

### 5. Which two capabilities are detection-oriented features in Arista's threat detection and mitigation framework? (Choose two.)

- [ ] **A)** Behavioral Analytics using machine learning on network metadata.
- [ ] **B)** Guardian automated response actions.
- [ ] **C)** Encrypted Traffic Analysis via TLS fingerprinting.
- [ ] **D)** Dynamic ACL enforcement on switches.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Behavioral Analytics and Encrypted Traffic Analysis are detection features; Guardian and dynamic ACLs are mitigation features.
 
 
</details>

### 6. Study the policy snippet. What does this configuration enforce?

```plaintext
policy: allow user:employee to app:financials if device_posture=compliant and time=working_hours
```

- [ ] **A)** Any user with the tag 'employee' can access the 'finance' application if their device is compliant and during working hours.
- [ ] **B)** All traffic from 'employee' to 'finance' is allowed without further checks.
- [ ] **C)** Only users with 'admin' role can access the finance application during working hours.
- [ ] **D)** The rule denies access to the finance application for all users.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy allows employee tag to access finance app only if device is compliant and time is working hours, enforcing least privilege.
 
 
</details>

### 7. What is the difference between static and dynamic MACsec key management in Arista EOS?

- [ ] **A)** Static uses a pre-shared CAK configured on both ends, while dynamic derives the CAK from EAP authentication via RADIUS.
- [ ] **B)** Static uses certificates, while dynamic uses a shared secret.
- [ ] **C)** Static requires a RADIUS server, while dynamic can work without one.
- [ ] **D)** Static keys are automatically rotated, while dynamic keys must be manually rotated.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Static MACsec uses manually configured CAK; dynamic uses RADIUS to derive CAK via EAP, enabling centralized management.
 
 
</details>


---

### **Automation and Programmability**

### 8. In the AVD architecture, which layer is responsible for generating candidate device configurations?

- [ ] **A)** Input Layer
- [ ] **B)** Processing Layer
- [ ] **C)** Output Layer
- [ ] **D)** Validation Layer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Output Layer in AVD generates candidate configurations from processed design variables.
 
 
</details>

### 9. Which of the following are components of the AVD framework? (Select all that apply.)

- [ ] **A)** eos_designs role
- [ ] **B)** eos_device_configuration role
- [ ] **C)** cvp_provision role
- [ ] **D)** eos_command module

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> AVD includes eos_designs, eos_device_configuration, and cvp_provision roles; eos_command is not part of AVD.
 
 
</details>

### 10. Examine the following YAML variable excerpt. Which variable is used to define an MLAG peer pair in AVD?

```yaml
mlag_peer: leaf1-mlag-peer
mlag_domain: dc1_mlag

```

- [ ] **A)** mlag_peer
- [ ] **B)** mlag_domain
- [ ] **C)** node_terminus
- [ ] **D)** interface_map

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The variable 'mlag_peer' is used in AVD to define MLAG peer node names.
 
 
</details>

### 11. Which Ansible module is idempotent and used for declarative configuration changes on Arista EOS?

- [ ] **A)** eos_command
- [ ] **B)** eos_config
- [ ] **C)** eos_facts
- [ ] **D)** eos_system

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> eos_config is the idempotent module for declarative config changes; eos_command is for operational commands.
 
 
</details>

### 12. Which statements are true when comparing eAPI and RESTCONF? (Select all that apply.)

- [ ] **A)** eAPI uses JSON-RPC for command execution.
- [ ] **B)** RESTCONF uses YANG data models for configuration.
- [ ] **C)** Both APIs support atomic transactions.
- [ ] **D)** eAPI is a vendor-proprietary interface.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> eAPI is proprietary, JSON-RPC based; RESTCONF uses YANG and is standards-based. Atomic transactions are only in eAPI via runCmds.
 
 
</details>

### 13. Analyze the following eAPI JSON-RPC request. Which method is used to execute multiple commands with rollback on failure?

```json
{
  "jsonrpc": "2.0",
  "method": "runCmds",
  "params": {
    "format": "json",
    "timestamps": false,
    "autoComplete": false,
    "expandAliases": false,
    "cmds": ["enable", "configure", "interface Ethernet1", "ip address 10.1.1.1/24"],
    "version": 1
  },
  "id": 1
}
```

- [ ] **A)** runCmds
- [ ] **B)** runCmdsWithIndex
- [ ] **C)** execCommand
- [ ] **D)** configureSession

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'runCmds' method in eAPI executes commands atomically when stopOnFailure is true (default).
 
 
</details>

### 14. What is the primary function of CloudVision's Change Control feature?

- [ ] **A)** Automatically push configuration to all devices immediately.
- [ ] **B)** Provide real-time streaming telemetry dashboards.
- [ ] **C)** Orchestrate sequences of tasks with approval gates and rollback.
- [ ] **D)** Manage backup of device configurations to a remote server.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Change Control orders tasks, requires approval, and supports rollback for safe network changes.
 
 
</details>

### 15. Which of the following are valid CloudVision user roles? (Select all that apply.)

- [ ] **A)** Network Operator
- [ ] **B)** Network Administrator
- [ ] **C)** Super User
- [ ] **D)** Security Auditor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> CVP has three default roles: Network Operator, Network Administrator, and Super User.
 
 
</details>

### 16. Examine the CloudVision API endpoint. What action does a POST to this endpoint perform?

```http
POST /cvp/v1/configlets
Content-Type: application/json
{
  "name": "new-config",
  "config": "interface Ethernet1\n  description test"
}
```

- [ ] **A)** Create a new configlet.
- [ ] **B)** Retrieve device information.
- [ ] **C)** Trigger a change control execution.
- [ ] **D)** Delete a container assignment.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> POST to /cvp/v1/configlets creates a new configlet in CloudVision.
 
 
</details>


---

### **Network Design for L7 Services**

### 17. Which BGP EVPN route type is used to advertise MAC and IP addresses for service nodes in a VXLAN fabric?

- [ ] **A)** RT-2
- [ ] **B)** RT-5
- [ ] **C)** RT-3
- [ ] **D)** RT-1

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RT-2 (MAC/IP advertisement) is used to advertise endpoint MAC and IP addresses, including those of service nodes.
 
 
</details>

### 18. Which two statements are true about Symmetric IRB for L7 service insertion?

- [ ] **A)** Uses both source and destination VNIs
- [ ] **B)** Can cause traffic loops across leaf switches
- [ ] **C)** Preferred over asymmetric IRB for stateful services
- [ ] **D)** Requires Ethernet Segment multi-homing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Symmetric IRB uses both VNIs for routing and is preferred for stateful services to ensure symmetric flow.
 
 
</details>

### 19. Based on the provided VXLAN header snippet, which field encodes the service path identifier?

```plaintext
VXLAN Header:
  Flags: 0x08
  VNI: 5000
  Reserved: 0x00
  NSH Extension: present
```

- [ ] **A)** VNI 5000
- [ ] **B)** Flags (0x08)
- [ ] **C)** Reserved field
- [ ] **D)** NSH Extension presence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The VNI acts as the service path identifier in EVPN service chaining, distinguishing between tenant and service VNIs.
 
 
</details>

### 20. What is the recommended default health check interval and retry count for Arista L7 load balancers?

- [ ] **A)** 1 second, 1 retry
- [ ] **B)** 5 seconds, 3 retries
- [ ] **C)** 10 seconds, 2 retries
- [ ] **D)** 30 seconds, 1 retry

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Arista recommends a 5-second interval with 3 retries to balance failover speed and stability.
 
 
</details>

### 21. Which two encapsulation headers are required when using VXLAN-GPE for NSH service chaining?

- [ ] **A)** VXLAN
- [ ] **B)** NSH
- [ ] **C)** GRE
- [ ] **D)** MPLS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VXLAN-GPE encapsulates NSH headers; GRE and MPLS are not part of this standard.
 
 
</details>

### 22. Based on the output, is the service insertion configuration symmetric or asymmetric?

```plaintext
show service-insertion status
  Service VNI: 5000
  Symmetry: asymmetric
  Active flows: 150
```

- [ ] **A)** Asymmetric
- [ ] **B)** Symmetric
- [ ] **C)** Unknown
- [ ] **D)** Partially symmetric

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The output shows 'symmetry: asymmetric', which indicates that return traffic may not traverse the same service leaf, breaking stateful inspection.
 
 
</details>

### 23. Where are stateful L4-L7 appliances best placed in a leaf-spine fabric?

- [ ] **A)** Service leaf switches
- [ ] **B)** Spine switches
- [ ] **C)** Workload leaf switches
- [ ] **D)** Core routers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Dedicated service leaves are recommended to handle symmetric hairpinning and avoid asymmetric routing through spines.
 
 
</details>

### 24. Which two service insertion models are commonly used for stateful firewalls in Arista EVPN fabrics?

- [ ] **A)** Inline transparent (Layer 2 bridge)
- [ ] **B)** Out-of-path PBR with static routes
- [ ] **C)** VXLAN service graphs (SITR)
- [ ] **D)** Bump-in-the-wire without VXLAN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Inline transparent and VXLAN service graphs are both suited for stateful services; out-of-path PBR is typically for stateless.
 
 
</details>


---

### **Troubleshooting and Optimization**

### 25. What type of data collection does CloudVision use to obtain network metrics?

- [ ] **A)** Pull-based SNMP polling
- [ ] **B)** Push-model streaming telemetry
- [ ] **C)** Periodic CLI scrapes
- [ ] **D)** Syslog aggregation only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> CloudVision uses a push-model architecture where devices stream telemetry via the Telemetry Agent, not pull-based methods.
 
 
</details>

### 26. Which flow export technologies are supported on Arista switches for L7 analysis?

- [ ] **A)** sFlow
- [ ] **B)** NetFlow v9
- [ ] **C)** IPFIX
- [ ] **D)** SNMP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Arista supports sFlow and IPFIX for flow export. NetFlow v9 is also supported but not mentioned? The document mentions sFlow and IPFIX explicitly.
 
 
</details>

### 27. Examine the following command and determine its purpose in VXLAN/EVPN tuning.

```cisco-ios
load-balance vxlan inner-ip
```

- [ ] **A)** Enables inner IP hashing for VXLAN traffic
- [ ] **B)** Disables jumbo frame support
- [ ] **C)** Reduces BGP keepalive timers
- [ ] **D)** Increases ARP cache size

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command 'load-balance vxlan inner-ip' optimizes ECMP hashing by using inner packet fields, preventing polarization.
 
 
</details>

### 28. What does an 'UNREACHABLE' status in Ansible output signify?

- [ ] **A)** The task execution failed
- [ ] **B)** The device is unreachable via transport
- [ ] **C)** The playbook syntax is invalid
- [ ] **D)** The device user credentials are wrong

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> 'UNREACHABLE' means Ansible cannot establish an SSH or eAPI connection to the device.
 
 
</details>

### 29. Which of the following are common causes of security policy conflicts in Arista networks?

- [ ] **A)** Incorrect rule ordering
- [ ] **B)** Excessive bandwidth usage
- [ ] **C)** Implicit deny at zone boundaries
- [ ] **D)** Frequent firmware upgrades

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Rule ordering and implicit deny are common conflict sources; bandwidth and firmware upgrades are not direct causes.
 
 
</details>

### 30. Review the following tcpdump command and identify its purpose in L7 packet analysis.

```bash
tcpdump -i eth0 tcp port 80
```

- [ ] **A)** Capture only HTTP traffic on port 80
- [ ] **B)** Monitor all ICMP packets
- [ ] **C)** Filter for DNS queries only
- [ ] **D)** Capture traffic from a specific host

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The filter 'tcp port 80' captures only TCP traffic destined to HTTP, aiding in web application troubleshooting.
 
 
</details>

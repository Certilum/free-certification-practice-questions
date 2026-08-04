<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Broadcom/Cloud%20Foundation%20Networking.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>VCAP - VMware Cloud Foundation Networking</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Architecture and Design](#architecture-and-design) (9 questions)
- [Automation and Programmability](#automation-and-programmability) (6 questions)
- [Implementation and Configuration](#implementation-and-configuration) (7 questions)
- [Operations and Troubleshooting](#operations-and-troubleshooting) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:55.346Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Architecture and Design | 9 |
| Automation and Programmability | 6 |
| Implementation and Configuration | 7 |
| Operations and Troubleshooting | 8 |

---

### **Architecture and Design**

### 1. What is the primary role of a Tier-0 gateway in VMware Cloud Foundation networking?

- [ ] **A)** Provide east-west routing for workload segments
- [ ] **B)** Act as the edge router for north-south traffic to the physical network
- [ ] **C)** Encapsulate Geneve overlay traffic between hosts
- [ ] **D)** Manage DHCP and IP address pools for tenant segments

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Tier-0 gateway connects the VCF environment to the physical network, handling north-south routing via BGP/OSPF.
 
 
</details>

### 2. Which two statements about overlay segments in NSX-T are correct? (Choose two.)

- [ ] **A)** They use Geneve encapsulation
- [ ] **B)** They require a unique VLAN ID on the wire
- [ ] **C)** They support overlapping IP addresses for different tenants
- [ ] **D)** They are limited to the VLAN capacity of physical switches

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Overlay segments use Geneve encapsulation and allow IP overlap; they do not have an associated VLAN ID on the wire.
 
 
</details>

### 3. Review the code snippet. What is the purpose of the BFD configuration in this BGP setup?

```nsx-config
neighbor 10.0.0.1 bfd
neighbor 10.0.0.1 fall-over bfd

```

- [ ] **A)** It allows faster convergence by detecting link failures in sub-seconds
- [ ] **B)** It encrypts BGP session traffic for security
- [ ] **C)** It reduces BGP keepalive interval to 1 second
- [ ] **D)** It enables load balancing between multiple BGP peers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> BFD provides sub-second detection of link failures, enabling rapid BGP convergence in an active-active Tier-0 design.
 
 
</details>

### 4. What is the default DFW rule in a newly deployed NSX environment?

- [ ] **A)** Allow all traffic except management
- [ ] **B)** Deny all traffic including system traffic
- [ ] **C)** Allow all traffic by default
- [ ] **D)** Deny all except DHCP, DNS, and some system traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> The default DFW rule is to deny all traffic except for essential services like DHCP and DNS.
 
 
</details>

### 5. Which two components are part of the NSX-T micro-segmentation framework? (Choose two.)

- [ ] **A)** Distributed Firewall (DFW)
- [ ] **B)** VLAN ACLs on physical switches
- [ ] **C)** NSX Groups with dynamic membership
- [ ] **D)** Tier-0 gateway load balancing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Micro-segmentation uses DFW rules applied to dynamic NSX Groups; VLAN ACLs are not part of NSX.
 
 
</details>

### 6. Refer to the code snippet. Which NSX group method is being used to define the web tier?

```xml
<group>
  <expression>
    <tag>WebTier</tag>
    <object>VirtualMachine</object>
  </expression>
</group>

```

- [ ] **A)** IP set membership based on static IP ranges
- [ ] **B)** vCenter object tag-based dynamic membership
- [ ] **C)** Manual VM membership by vCenter UUID
- [ ] **D)** Active Directory user group membership

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The snippet shows a tag-based membership using a vCenter tag, making the group dynamic.
 
 
</details>

### 7. What is the minimum MTU requirement for the physical underlay to support Geneve overlay traffic?

- [ ] **A)** 1500 bytes
- [ ] **B)** 1600 bytes
- [ ] **C)** 1700 bytes
- [ ] **D)** 9000 bytes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Geneve adds 50 bytes overhead, so the underlay must support at least 1600 bytes MTU to avoid fragmentation.
 
 
</details>

### 8. Which two statements are true about Tier-1 gateways in VCF? (Choose two.)

- [ ] **A)** They provide default gateway for workload segments
- [ ] **B)** They are used for north-south BGP peering with physical routers
- [ ] **C)** They host services like NAT, load balancer, and VPN
- [ ] **D)** They require a direct physical uplink to ToR switches

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Tier-1 gateways serve as tenant gateways for east-west routing and host services; BGP peering is done at Tier-0.
 
 
</details>

### 9. Examine the code snippet. What is the purpose of the 'active-active' setting in this Tier-0 configuration?

```nsx-config
tier-0-gateway HA-mode active-active
edge-cluster ec-01

```

- [ ] **A)** It enables ECMP across multiple Edge nodes for higher throughput
- [ ] **B)** It provides stateful failover for NAT sessions
- [ ] **C)** It synchronizes configuration across all Edge VMs
- [ ] **D)** It activates BFD on all uplink interfaces

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Active-active mode allows multiple Tier-0 instances to forward traffic simultaneously using ECMP.
 
 
</details>


---

### **Automation and Programmability**

### 10. Which cmdlet must be used to authenticate to NSX Manager in PowerCLI?

- [ ] **A)** Connect-VIServer
- [ ] **B)** Connect-NsxtServer
- [ ] **C)** Connect-VMHost
- [ ] **D)** Connect-NetworkController

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Connect-NsxtServer is the correct cmdlet for authenticating to NSX Manager in PowerCLI. Connect-VIServer is for vCenter, not NSX Manager.
 
 
</details>

### 11. Which two NSX Policy API HTTP methods are idempotent? (Choose two.)

- [ ] **A)** POST
- [ ] **B)** PATCH
- [ ] **C)** PUT
- [ ] **D)** DELETE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> PATCH and PUT are idempotent when used for upsert or replace operations in the Policy API. POST is not idempotent because it may create duplicate resources. DELETE can be idempotent but is less commonly used for policy updates.
 
 
</details>

### 12. Examine the following PowerCLI script snippet. What is the purpose of the -VlanId parameter?

```powershell
New-NsxtSegment -Name "VLAN-Segment" -VlanId 100 -TransportZoneId "tz-id" -ConnectivityPath "/infra/tier-1s/t1-gw"
```

- [ ] **A)** It defines the VLAN ID for a VLAN-backed segment.
- [ ] **B)** It specifies the overlay transport zone ID.
- [ ] **C)** It sets the Tier-1 gateway connectivity path.
- [ ] **D)** It assigns the segment to a management network.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The -VlanId parameter is used when creating a VLAN-backed segment in NSX. Overlay segments do not require a VLAN ID. The other options are incorrect because -VlanId is specific to VLAN backing.
 
 
</details>

### 13. Which automation tool uses a declarative model where the desired end state of network resources is defined in configuration files?

- [ ] **A)** PowerCLI
- [ ] **B)** Ansible
- [ ] **C)** Terraform
- [ ] **D)** vRealize Orchestrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Terraform is declarative: you define the desired state and it automates the steps. PowerCLI and vRO are imperative/procedural. Ansible is procedural by default, though some modules may be declarative.
 
 
</details>

### 14. Which two Terraform providers are used to manage VCF networking resources? (Choose two.)

- [ ] **A)** vmware/vcf
- [ ] **B)** vmware/nsxt
- [ ] **C)** hashicorp/aws
- [ ] **D)** vmware/vsphere

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The vmware/vcf provider manages VCF-level constructs like network pools, while the vmware/nsxt provider manages NSX-T objects such as segments and gateways. vsphere provider is for vCenter, not VCF networking.
 
 
</details>

### 15. Analyze the following Ansible task snippet. What does the 'state: present' parameter achieve in this module?

```yaml
- name: Create overlay segment
  nsxt_policy_segment:
    display_name: "App-Segment"
    transport_zone_path: "/infra/sites/default/enforcement-points/default/transport-zones/xxx"
    subnet:
      - gateway_address: "192.168.10.1/24"
        dhcp_ranges: ["192.168.10.10-192.168.10.100"]
    state: present
```

- [ ] **A)** It ensures the NSX-T segment exists as declared.
- [ ] **B)** It removes the segment if it already exists.
- [ ] **C)** It forces a recreation of the segment.
- [ ] **D)** It pauses the playbook until the segment is present.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'state: present' parameter ensures that the resource (here an nsxt_policy_segment) exists with the specified configuration. It does not force recreation; it is idempotent. 'state: absent' would remove it.
 
 
</details>


---

### **Implementation and Configuration**

### 16. How many NSX-T Manager nodes does VMware Cloud Foundation deploy by default in the management domain?

- [ ] **A)** One
- [ ] **B)** Two
- [ ] **C)** Three
- [ ] **D)** Four

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> VCF always deploys a three-node NSX-T Manager cluster for high availability in the management domain.
 
 
</details>

### 17. Which of the following statements about Transport Zones in a VCF environment are correct? (Choose two.)

- [ ] **A)** Overlay Transport Zones are automatically created for each workload domain by SDDC Manager.
- [ ] **B)** VLAN Transport Zones are automatically created by SDDC Manager for every workload domain.
- [ ] **C)** A Transport Zone defines the scope of network connectivity and can be of type Overlay or VLAN.
- [ ] **D)** Transport Zones are only required for management domain networking, not for workload domains.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Overlay TZs are auto-created; VLAN TZs require manual creation. TZs define connectivity scope and can be Overlay or VLAN.
 
 
</details>

### 18. Given the NSX-T uplink profile snippet below, what teaming policy is being used?

```json
"teaming": {
  "policy": "LOADBALANCE_SRCID",
  "active_uplinks": ["uplink1", "uplink2"],
  "standby_uplinks": []
}
```

- [ ] **A)** FAILOVER_ORDER (Active/Standby)
- [ ] **B)** LOADBALANCE_SRCID (Active/Active)
- [ ] **C)** LOADBALANCE_SRCMAC
- [ ] **D)** LOADBALANCE_IP_HASH

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The snippet shows 'teaming_policy' set to 'LOADBALANCE_SRCID', which is Active/Active using source ID.
 
 
</details>

### 19. How are Distributed Firewall (DFW) rules evaluated in NSX-T?

- [ ] **A)** Bottom-up, with last rule taking precedence
- [ ] **B)** Top-down, and the first matching rule is applied
- [ ] **C)** Random order based on rule priority
- [ ] **D)** Alphabetical order of rule names

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> DFW rules are evaluated from top to bottom; the first rule that matches the traffic is applied.
 
 
</details>

### 20. Which of the following are true regarding IDS/IPS in NSX-T for VCF? (Choose two.)

- [ ] **A)** IDS/IPS requires an Advanced Threat Prevention license.
- [ ] **B)** IDS/IPS can be applied to both DFW and Gateway Firewall rules.
- [ ] **C)** IDS/IPS is always active by default on all NSX-T deployments.
- [ ] **D)** IDS/IPS does not consume any resources on Edge nodes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> IDS/IPS requires a specific license and can be attached to rules. It consumes Edge CPU/memory and is not default.
 
 
</details>

### 21. The DFW rule below shows a 'status' of 'pending'. What action is required for it to become effective?

```text
Rule ID: 1051
Source: Web-Tier
Destination: DB-Tier
Service: MSSQL (TCP 1433)
Action: Allow
Status: Pending
```

- [ ] **A)** Reboot the ESXi hosts in the cluster
- [ ] **B)** Publish the DFW policy
- [ ] **C)** Restart the NSX Manager service
- [ ] **D)** Reapply the transport node profile

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> DFW changes must be explicitly published (applied) to take effect. Status 'pending' indicates unpublished rules.
 
 
</details>

### 22. What is the minimum number of NSX Edge nodes required for high availability in a cluster?

- [ ] **A)** One
- [ ] **B)** Two
- [ ] **C)** Three
- [ ] **D)** Four

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A minimum of two Edge nodes is required for high availability, allowing one to take over if the other fails.
 
 
</details>


---

### **Operations and Troubleshooting**

### 23. Which VMware tool performs deep packet inspection and flow analytics for network performance monitoring in VCF?

- [ ] **A)** vRealize Network Insight
- [ ] **B)** vCenter Server
- [ ] **C)** NSX-T Manager dashboards
- [ ] **D)** SDDC Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> vRealize Network Insight (vRNI) provides deep packet inspection, flow analytics, and cross-domain correlation for network performance monitoring.
 
 
</details>

### 24. Which metrics can you monitor using NSX-T dashboards? (Select two.)

- [ ] **A)** Tunnel status
- [ ] **B)** Round-trip time between VMs
- [ ] **C)** Logical port statistics
- [ ] **D)** vSAN datastore throughput

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> NSX-T dashboards show tunnel status and logical port statistics; RTT and vSAN throughput are not native NSX-T dashboard metrics.
 
 
</details>

### 25. Based on the Traceflow output, which component dropped the packet?

```plaintext
Traceflow Result: Hop 1: DFW - Rule ID 1003 - Action DROP
```

- [ ] **A)** Distributed Firewall (DFW)
- [ ] **B)** Tier-1 Gateway
- [ ] **C)** Logical Switch
- [ ] **D)** Tier-0 Gateway

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Traceflow output shows a rule ID matched on the DFW with action 'DROP', indicating the Distributed Firewall dropped the packet.
 
 
</details>

### 26. What is the first step in troubleshooting north-south connectivity loss from a workload domain to an external network?

- [ ] **A)** Verify BGP peering between Tier-0 and physical spine switches
- [ ] **B)** Check NSX-T Distributed Firewall rules
- [ ] **C)** Run a packet capture on the source VM
- [ ] **D)** Review vCenter performance charts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The first step is to verify BGP peering because Tier-0 gateways exchange routes with the physical fabric for external connectivity.
 
 
</details>

### 27. Which two tools are used together to identify a network bottleneck in VCF?

- [ ] **A)** vCenter performance charts
- [ ] **B)** NSX Traceflow
- [ ] **C)** esxtop networking view
- [ ] **D)** SDDC Manager health dashboards

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> vCenter performance charts provide average metrics, while esxtop gives per-second granularity needed to spot micro-burst bottlenecks.
 
 
</details>

### 28. Review the vCenter performance chart. What does a sudden rise in network utilization coinciding with increased vSAN latency indicate?

```plaintext
vCenter Chart: Network utilization 90% (avg 5 min) | vSAN write latency 15ms (baseline 0.5ms)
```

- [ ] **A)** Network bottleneck affecting storage traffic
- [ ] **B)** Storage disk failure
- [ ] **C)** CPU overcommitment
- [ ] **D)** Memory ballooning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A simultaneous rise in network utilization and vSAN latency indicates that network congestion is starving vSAN traffic, not a storage or compute issue.
 
 
</details>

### 29. Which component must be upgraded first in an NSX-T lifecycle upgrade?

- [ ] **A)** NSX Manager cluster
- [ ] **B)** NSX Edge nodes
- [ ] **C)** Host transport nodes
- [ ] **D)** vCenter Server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The NSX Manager cluster must be upgraded first because newer Edge and host modules require a compatible manager version.
 
 
</details>

### 30. Which two pieces of information are essential for restoring an NSX Manager from backup? (Select two.)

- [ ] **A)** Backup file from the same NSX version
- [ ] **B)** The backup passphrase
- [ ] **C)** vCenter Server credentials
- [ ] **D)** SDDC Manager connectivity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The backup file must be from the same version, and the passphrase (set when backup was created) is required to decrypt the file.
 
 
</details>

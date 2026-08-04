<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Broadcom/Cloud%20Foundation%20Storage.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>VCAP - VMware Cloud Foundation Storage</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Architecture and Design](#architecture-and-design) (7 questions)
- [Implementation and Configuration](#implementation-and-configuration) (9 questions)
- [Operations and Management](#operations-and-management) (6 questions)
- [Security and Compliance](#security-and-compliance) (3 questions)
- [Troubleshooting and Optimization](#troubleshooting-and-optimization) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:00.516Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Architecture and Design | 7 |
| Implementation and Configuration | 9 |
| Operations and Management | 6 |
| Security and Compliance | 3 |
| Troubleshooting and Optimization | 5 |

---

### **Architecture and Design**

### 1. What is the minimum number of hosts required for a vSAN stretched cluster?

- [ ] **A)** 2
- [ ] **B)** 3
- [ ] **C)** 4
- [ ] **D)** 5

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A vSAN stretched cluster requires at least two hosts (one per site) plus an external witness, making two the minimum host count.
 
 
</details>

### 2. Which two are vSAN storage policy parameters?

- [ ] **A)** Primary Failures to Tolerate (PFTT)
- [ ] **B)** Number of Disk Stripes
- [ ] **C)** vCenter Server version
- [ ] **D)** Cluster node count

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> PFTT and Number of Disk Stripes are key vSAN storage policy parameters controlling availability and performance.
 
 
</details>

### 3. Refer to the code block below. What is the purpose of this ESXi command?

```bash
esxcli storage nfs list
```

- [ ] **A)** Lists NFS datastores mounted on the host
- [ ] **B)** Mounts a new NFS datastore
- [ ] **C)** Checks vSAN health status
- [ ] **D)** Configures NFS v4.1 security

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command 'esxcli storage nfs list' displays all NFS datastores currently mounted on the ESXi host.
 
 
</details>

### 4. What is the recommended free capacity headroom in a vSAN cluster for maintenance operations?

- [ ] **A)** 10%
- [ ] **B)** 20%
- [ ] **C)** 25%
- [ ] **D)** 30%

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> VCF recommends maintaining 25% free capacity in each vSAN cluster for host maintenance, rebuilds, and policy changes.
 
 
</details>

### 5. Which two are benefits of using erasure coding (RAID-5/6) over mirroring in vSAN?

- [ ] **A)** Lower capacity overhead
- [ ] **B)** Better write performance
- [ ] **C)** Lower rebuild impact
- [ ] **D)** Higher capacity efficiency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Erasure coding offers lower capacity overhead (33-50% vs 100-200%) and higher capacity efficiency, but incurs write performance penalty and slower rebuilds.
 
 
</details>

### 6. Refer to the code block. Which two pieces of information are provided by this command?

```bash
esxcli storage nfs list
```

- [ ] **A)** NFS server IP address
- [ ] **B)** vCenter Server name
- [ ] **C)** Datastore name
- [ ] **D)** VMFS volume label

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The 'esxcli storage nfs list' displays the NFS server IP and the datastore name (volume label) for each mounted NFS datastore.
 
 
</details>

### 7. What is the minimum number of hosts required for a vSAN cluster to use RAID-5 erasure coding?

- [ ] **A)** 3
- [ ] **B)** 4
- [ ] **C)** 5
- [ ] **D)** 6

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> RAID-5 erasure coding requires a minimum of 4 hosts; RAID-6 requires 6 hosts.
 
 
</details>


---

### **Implementation and Configuration**

### 8. What is the minimum number of ESXi hosts required to form a standard vSAN cluster?

- [ ] **A)** 2
- [ ] **B)** 3
- [ ] **C)** 4
- [ ] **D)** 5

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A standard vSAN cluster requires a minimum of 3 hosts to provide storage and ensure failure tolerance.
 
 
</details>

### 9. Which two network prerequisites must be met to configure vSAN within a workload domain?

- [ ] **A)** MTU 9000
- [ ] **B)** VLAN isolation from VM traffic
- [ ] **C)** Use of DHCP for IP assignment
- [ ] **D)** Multicast disabled

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> vSAN requires jumbo frames (MTU 9000) and a dedicated VLAN isolated from other traffic.
 
 
</details>

### 10. In the provided vSAN disk group configuration, which device serves as the cache tier?

```plaintext
Disk Group 1:
  Cache Tier (NVMe): vmhba0:C0:T0:L0
  Capacity Tier (SSD): vmhba0:C0:T1:L0
  Capacity Tier (SSD): vmhba0:C0:T2:L0
```

- [ ] **A)** vmhba0:C0:T0:L0
- [ ] **B)** vmhba0:C0:T1:L0
- [ ] **C)** vmhba0:C0:T2:L0
- [ ] **D)** None of the above

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The cache device is listed under Cache Tier, which is vmhba0:C0:T0:L0.
 
 
</details>

### 11. Where does the VASA Provider need to be registered to expose storage capabilities?

- [ ] **A)** ESXi host
- [ ] **B)** vCenter Server
- [ ] **C)** NSX Controller
- [ ] **D)** SDDC Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The VASA Provider is registered with vCenter Server to expose array capabilities.
 
 
</details>

### 12. Which two capabilities are provided by VASA in a vSphere environment?

- [ ] **A)** Expose array capabilities for SPBM
- [ ] **B)** Offload storage operations like snapshots
- [ ] **C)** Enable Virtual Volumes
- [ ] **D)** Provide backup integration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> VASA exposes storage capabilities for policy-based management and is required for Virtual Volumes.
 
 
</details>

### 13. What does the status \"Connected\" indicate for the VASA Provider?

```plaintext
vCenter VASA Providers:
  Provider: HPE_3PAR_VASA_Provider
  Status: Connected
  Version: 4.0
```

- [ ] **A)** Provider is running and communicating with vCenter
- [ ] **B)** Provider is registered but not responding
- [ ] **C)** Provider needs certificate update
- [ ] **D)** Provider is in maintenance mode

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> \"Connected\" indicates the VASA Provider is successfully communicating with vCenter.
 
 
</details>

### 14. Which Storage DRS mode requires administrator approval before recommendations are executed?

- [ ] **A)** Automated
- [ ] **B)** Manual
- [ ] **C)** Semi-automated
- [ ] **D)** Intelligent

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Manual mode generates recommendations but requires admin action to execute them.
 
 
</details>

### 15. Which two conditions must be met for Storage DRS to perform load balancing migrations?

- [ ] **A)** Storage vMotion license
- [ ] **B)** Shared storage between datastores
- [ ] **C)** vMotion network configured
- [ ] **D)** vSAN enabled on the cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SDRS requires storage vMotion licensing and shared storage between datastores.
 
 
</details>

### 16. Based on the SDRS settings, which threshold would trigger a load balancing operation?

```plaintext
SDRS Cluster Settings:
  Automation Level: Automated
  Space Utilization Threshold: 80%
  I/O Latency Threshold: 15 ms
  I/O Load Threshold: 25
  Invocation Frequency: 8 hours
```

- [ ] **A)** Space utilization exceeding 80%
- [ ] **B)** I/O latency above 10 ms
- [ ] **C)** I/O load threshold 20
- [ ] **D)** Invocation frequency change

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The space utilization threshold is set to 80%; exceeding it triggers evaluation.
 
 
</details>


---

### **Operations and Management**

### 17. What is the default interval (in minutes) for vSAN Skyline Health built-in health checks to run?

- [ ] **A)** 30 minutes
- [ ] **B)** 60 minutes
- [ ] **C)** 120 minutes
- [ ] **D)** 90 minutes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The document states that vSAN Skyline Health performs health checks on a configurable interval with a default of 60 minutes.
 
 
</details>

### 18. Which two tools are identified in the document as the primary monitoring tools for vSAN storage health and performance in VCF?

- [ ] **A)** vSAN Skyline Health
- [ ] **B)** vRealize Operations (with vSAN Management Pack)
- [ ] **C)** vRealize Log Insight
- [ ] **D)** vCenter Performance Charts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The playbook explicitly states: 'two primary tools: vSAN Skyline Health (formerly Skyline Health Diagnostics, now integrated into the vSphere Client as the vSAN Skyline Health dashboard) and vRealize Operations (vROps) with its vSAN Management Pack.'
 
 
</details>

### 19. An administrator runs the command `esxcli vsan network list` on an ESXi host and receives the output shown. Which statement best describes the vSAN network configuration?

```bash
~ # esxcli vsan network list
Interface
   VmkNic: vmk2
   IP Address: 192.168.10.10
   Subnet Mask: 255.255.255.0
   MAC Address: 00:50:56:ab:cd:01
   Mode: unicast
   Multicast: false
   MTU: 1500
```

- [ ] **A)** The vSAN network uses multicast mode with MTU 9000.
- [ ] **B)** The vSAN network is configured with unicast mode and MTU 1500.
- [ ] **C)** The vSAN network is using a dedicated physical NIC but no IP address.
- [ ] **D)** The vSAN network is misconfigured because multicast is false.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The output shows Mode: unicast and MTU: 1500. vSAN uses unicast by default in recent versions, and multicast being false is normal. Therefore, the configuration is correct with unicast mode and MTU 1500.
 
 
</details>

### 20. At what default capacity utilization deviation (in percentage) does vSAN trigger proactive rebalancing?

- [ ] **A)** 10%
- [ ] **B)** 20%
- [ ] **C)** 30%
- [ ] **D)** 15%

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The document states: 'When the deviation for any disk group exceeds the threshold set by the advanced parameter RebalanceThreshold (default 20%), the system flags a potential rebalance.'
 
 
</details>

### 21. Which of the following are true about the role of SDDC Manager in storage component lifecycle management for VCF workload domains? (Select two)

- [ ] **A)** It can be bypassed by using vCenter directly for upgrades.
- [ ] **B)** It orchestrates upgrades in a strict sequence.
- [ ] **C)** It only manages compute, not storage.
- [ ] **D)** It enforces pre-flight checks before upgrades.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> The playbook explains that SDDC Manager is the central orchestrator, enforcing a strict sequence of upgrades and running pre-flight checks. Directly using vCenter for upgrades is unsupported.
 
 
</details>

### 22. The vSAN Health dashboard displays the status shown above. Based on this output, which health categories are in a warning state? (Select all that apply)

```plaintext
vSAN Health Service - Cluster Health
   Hardware Compatibility: Green
   Network: Yellow (Warning)
   Data: Yellow (Warning)
   Performance Service: Green
```

- [ ] **A)** Hardware Compatibility
- [ ] **B)** Network
- [ ] **C)** Data
- [ ] **D)** Performance Service

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> The output shows Network and Data as Yellow (Warning). Hardware Compatibility and Performance Service are Green. Therefore, the Network and Data categories are in warning state.
 
 
</details>


---

### **Security and Compliance**

### 23. What is the primary method for encrypting vSAN datastores in VMware Cloud Foundation?

- [ ] **A)** vSAN Native Encryption using TPM
- [ ] **B)** vSAN Encryption with an external KMS
- [ ] **C)** VM-level encryption via vSphere
- [ ] **D)** Storage DRS encryption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> vSAN encryption with an external KMS is the primary method for encrypting vSAN datastores, providing key separation and compliance.
 
 
</details>

### 24. Which two privileges are required for a user to apply a storage policy to a VM on a vSAN datastore? (Select two.)

- [ ] **A)** Datastore.AllocateSpace
- [ ] **B)** StorageProfile.Apply
- [ ] **C)** Datastore.Browse
- [ ] **D)** StorageProfile.Create

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> To apply a storage policy, a user needs Datastore.AllocateSpace on the target datastore and StorageProfile.Apply privilege.
 
 
</details>

### 25. An administrator runs the following command. What does the output indicate about the VMDK object?

```text
vsan.storage_policy_compliance -object vmdk-123
Output: LockExpiration: 2025-01-01T00:00:00Z
```

- [ ] **A)** The object has a retention lock applied.
- [ ] **B)** The object is encrypted with an external KMS.
- [ ] **C)** The object is non-compliant with the storage policy.
- [ ] **D)** The object is undergoing a rebuild.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The output shows a lock expiration timestamp, indicating a retention lock is set on the VMDK object.
 
 
</details>


---

### **Troubleshooting and Optimization**

### 26. In vSAN Original Storage Architecture (OSA), what is the maximum number of disk groups allowed per ESXi host?

- [ ] **A)** Up to 5 disk groups per host
- [ ] **B)** Up to 2 disk groups per host
- [ ] **C)** Up to 3 disk groups per host
- [ ] **D)** Only 1 disk group per host

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In vSAN OSA, each ESXi host can support up to five disk groups. This is a key architectural constraint; more disk groups increase parallelism but consume more memory.
 
 
</details>

### 27. Which of the following statements about vSAN capacity thresholds and alarms are correct? (Select two.)

- [ ] **A)** vSAN triggers a warning at 80% usage.
- [ ] **B)** vSAN triggers a critical alarm at 95% usage.
- [ ] **C)** At 100% capacity, vSAN enters a read-only mode for all objects.
- [ ] **D)** The warning at 80% means immediate hardware addition is required.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> vSAN issues a warning at 80% utilization and a critical alarm at 95%. At 100%, some objects may become read-only, not all. The 80% warning is proactive; analyze reclaimable space before adding hardware.
 
 
</details>

### 28. An administrator runs 'esxcli vsan storage list' and sees that a disk shows 'Not eligible for vSAN'. Which is the most likely cause based on the output shown below?

```bash
esxcli vsan storage list
   Device: naa.5000c500a1b2c3d4
   Display Name: Local SSD Disk (naa.5000c500a1b2c3d4)
   Is SSD: true
   VSAN Eligible: false
   VSAN Eligibility Reason: Not HCL qualified
```

- [ ] **A)** The disk is not HCL qualified for the vSAN version.
- [ ] **B)** The disk is already used as a cache device in another disk group.
- [ ] **C)** The disk has been partitioned with a VMFS datastore.
- [ ] **D)** The disk is too small to serve as a capacity device.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The most common reason for 'Not eligible for vSAN' is that the disk is not listed on the VMware Compatibility Guide (HCL). Other reasons like existing partitions are possible but the output typically indicates HCL failure first.
 
 
</details>

### 29. What is the primary difference between vSAN OSA and ESA in terms of disk group structure?

- [ ] **A)** ESA uses only NVMe devices and allows only one disk group per host with no separate cache tier.
- [ ] **B)** ESA supports up to five disk groups per host, each with a dedicated cache device.
- [ ] **C)** OSA requires all devices to be NVMe and supports only one disk group per host.
- [ ] **D)** In ESA, capacity devices are HDDs while cache devices are SSDs.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ESA is designed for all-NVMe clusters, with a single disk group per host that combines cache and capacity in the same NVMe devices – there is no separate cache tier. OSA uses a cache + capacity model and supports up to five disk groups.
 
 
</details>

### 30. Which of the following are valid attributes in a vSAN storage policy? (Select two.)

- [ ] **A)** Number of Failures to Tolerate (FTT)
- [ ] **B)** Number of Disk Stripes per Object
- [ ] **C)** Host Cache Size
- [ ] **D)** Disk Group Count

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> FTT and Striping are explicit vSAN storage policy attributes. Host Cache Size and Disk Group Count are not policy settings; they are host-level or cluster-level configurations.
 
 
</details>

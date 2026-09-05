<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Nutanix/Nutanix%20Certified%20Professional%20-%20Multicloud%20Infrastructure%206" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Nutanix Certified Professional - Multicloud Infrastructure</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [AHV Virtualization](#ahv-virtualization) (6 questions)
- [Compute and Storage Management](#compute-and-storage-management) (5 questions)
- [Data Protection and Disaster Recovery](#data-protection-and-disaster-recovery) (4 questions)
- [Multicloud Integration and Migration](#multicloud-integration-and-migration) (4 questions)
- [Prism Administration](#prism-administration) (6 questions)
- [Security and Compliance](#security-and-compliance) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:44.386Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| AHV Virtualization | 6 |
| Compute and Storage Management | 5 |
| Data Protection and Disaster Recovery | 4 |
| Multicloud Integration and Migration | 4 |
| Prism Administration | 6 |
| Security and Compliance | 5 |

---

### **AHV Virtualization**

### 1. What is a critical risk when VirtIO drivers are not installed in a guest operating system during AHV VM creation?

- [ ] **A)** The VM will not appear in Prism Element.
- [ ] **B)** The VM may fail to boot or may have severely degraded I/O throughput.
- [ ] **C)** The VM will be automatically assigned a VLAN from the wrong subnet.
- [ ] **D)** The VM cannot be protected by Nutanix Categories.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> VirtIO drivers are essential for efficient networking and storage I/O in AHV. Without them, the guest may not boot or may use emulated devices with poor performance.
 
 
</details>

### 2. Which two statements about AHV bonding modes are correct?

- [ ] **A)** Active-Backup requires no configuration on the physical upstream switch.
- [ ] **B)** LACP works automatically once enabled on the AHV host.
- [ ] **C)** LACP requires matching link aggregation settings on the physical upstream switch.
- [ ] **D)** Active-Backup uses all physical NICs simultaneously to double bandwidth.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Active-Backup is simple and does not require switch configuration. LACP needs to be configured on both the AHV host and the physical switch to provide link aggregation and redundancy.
 
 
</details>

### 3. An administrator applies the metadata shown in the code block to a VM. What is this metadata primarily used for in Nutanix AHV?

```yaml
metadata:
  categories:
    - Environment: Production
    - Compliance: PCI
```

- [ ] **A)** To select the physical switch used for VM traffic.
- [ ] **B)** To trigger policy-based automation such as Flow microsegmentation or backup schedules.
- [ ] **C)** To define the VM's vCPU and memory reservation.
- [ ] **D)** To set the VM's boot order and disk controller type.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Nutanix Categories are metadata tags that can trigger automated policies, including Flow microsegmentation and backup through Nutanix Protect or Mine. They are not traditional VM tags or network settings.
 
 
</details>

### 4. Why is it a common mistake to apply a CPU or memory reservation to every VM in an AHV cluster?

- [ ] **A)** It causes the cluster to create a new bridge for each VM.
- [ ] **B)** It can result in resource fragmentation and wasted capacity.
- [ ] **C)** It prevents Nutanix Categories from being applied.
- [ ] **D)** It disables VirtIO drivers for Linux virtual machines.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Reservations guarantee resources, but applying them everywhere reduces the ability to overcommit, fragments available capacity, and lowers cluster density.
 
 
</details>

### 5. Which two functions are performed by Acropolis Dynamic Scheduling (ADS)?

- [ ] **A)** Monitors resource utilization and live-migrates VMs to balance workloads.
- [ ] **B)** Automatically creates VLANs in the physical switch.
- [ ] **C)** Prevents individual nodes from becoming resource bottlenecks.
- [ ] **D)** Replaces the need for VirtIO drivers in the guest OS.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> ADS continuously monitors resource use and live-migrates VMs to balance load, preventing any node from bottlenecking.
 
 
</details>

### 6. A VM policy is defined in the code block. What will happen when two VMs are assigned to this policy?

```yaml
placement_policy:
  type: anti-affinity
  scope: host
```

- [ ] **A)** The VMs will be placed on the same host to minimize latency.
- [ ] **B)** The VMs will be placed on different hosts to survive a host failure.
- [ ] **C)** The VMs will be placed on a host with the least storage usage.
- [ ] **D)** The VMs will be placed on the same host if they use VirtIO.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Anti-affinity rules keep specified VMs on separate hosts, reducing the blast radius of host failure. Affinity rules would place them together.
 
 
</details>


---

### **Compute and Storage Management**

### 7. What is the primary reason for integrating VirtIO drivers into a guest OS running on AHV?

- [ ] **A)** To allow efficient network and storage I/O for the virtual machine
- [ ] **B)** To enable automatic VLAN tag assignment from the host
- [ ] **C)** To configure the virtual machine's memory ballooning
- [ ] **D)** To replace the need for physical switch configuration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> VirtIO drivers are paravirtualized drivers that provide optimized I/O for network and storage devices in AHV. Without them, guests suffer degraded performance or fail to boot.
 
 
</details>

### 8. Which statements about Nutanix Categories compared with traditional VM tags are true? (Select two.)

- [ ] **A)** Categories can trigger microsegmentation policies and automated backup schedules.
- [ ] **B)** Categories are used only for organizational metadata, like traditional tags.
- [ ] **C)** Traditional tags are required for Nutanix Flow microsegmentation policies to work.
- [ ] **D)** Categories can be assigned during or after VM creation.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Nutanix Categories enable policy-based automation through Flow and Protect. They can be assigned during or after VM creation, whereas traditional tags are typically limited to organizational metadata.
 
 
</details>

### 9. Based on the provided Open vSwitch output, what does 'bond0' represent in AHV networking?

```bash
Bridge br0
    Port bond0
        Interface eth0
        Interface eth1
    Port vnet0
        tag: 100
        Interface vnet0
```

- [ ] **A)** An aggregation of physical NICs to provide link redundancy and bandwidth
- [ ] **B)** A bridge that connects VMs to the physical network
- [ ] **C)** A virtual port that provides DHCP addresses to VMs
- [ ] **D)** A VLAN tagging mechanism for tenant traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> bond0 aggregates the physical network interfaces eth0 and eth1 and is attached to the bridge br0. VMs connect to br0 through virtual ports, while bond0 handles link redundancy and bandwidth aggregation.
 
 
</details>

### 10. What is the name of the default logical bridge to which vNICs connect in AHV networking?

- [ ] **A)** br0
- [ ] **B)** bond0
- [ ] **C)** vnet0
- [ ] **D)** ovs0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The default bridge in AHV is br0. It connects physical NICs or bonds to virtual machine vNICs, acting as the central hub for network traffic.
 
 
</details>

### 11. Which statements are correct regarding LACP and Active-Backup bonding modes in AHV? (Select two.)

- [ ] **A)** LACP requires corresponding link aggregation configuration on the upstream physical switch.
- [ ] **B)** Active-Backup mode can provide link redundancy without any switch-side configuration.
- [ ] **C)** LACP can only be used for host management traffic and not for VM traffic.
- [ ] **D)** Active-Backup mode aggregates multiple links to increase available bandwidth.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> LACP is a dynamic link aggregation protocol that requires matching configuration on the upstream physical switch. Active-Backup provides failover redundancy without requiring switch configuration, but it does not aggregate bandwidth across active links.
 
 
</details>


---

### **Data Protection and Disaster Recovery**

### 12. In a Nutanix environment, what is the primary purpose of assigning Categories to virtual machines?

- [ ] **A)** Drive policy-based automation
- [ ] **B)** Only organize VMs
- [ ] **C)** Replace virtual switches
- [ ] **D)** Assign IP addresses

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Nutanix Categories trigger policy-based automation such as Flow microsegmentation or backup schedules, unlike standard tags used only for organizational metadata.
 
 
</details>

### 13. Which two statements about AHV VirtIO driver integration and guest OS performance for virtual machines are correct?

- [ ] **A)** They enable efficient storage and network I/O
- [ ] **B)** They must be installed in the guest OS
- [ ] **C)** They are preinstalled in all guest OSes
- [ ] **D)** They only improve display resolution

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VirtIO drivers are required in the guest OS for efficient AHV storage and network performance. Missing them can cause boot failures or degraded throughput.
 
 
</details>

### 14. Refer to the AHV network command shown. What is the administrator creating for VM connectivity?

```bash
acli net.create web-tier vlan=100
```

- [ ] **A)** A VLAN-tagged network segment
- [ ] **B)** A new physical switch
- [ ] **C)** A VirtIO driver package
- [ ] **D)** A Nutanix Category

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command creates a VLAN-tagged network segment that VMs can attach to, enabling proper segmentation within the AHV software-defined network.
 
 
</details>

### 15. What is the best definition of resource overcommitment in a Nutanix cluster with multiple hosts and VMs?

- [ ] **A)** Allocating more virtual resources than physically available
- [ ] **B)** Always a misconfiguration that must be removed
- [ ] **C)** A way to reduce virtual machine density
- [ ] **D)** Another term for storage compression

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Overcommitment is a managed strategy that increases ROI by allowing more virtual resources than physical capacity, but it must be monitored to protect SLAs.
 
 
</details>


---

### **Multicloud Integration and Migration**

### 16. Which statement best describes resource overcommitment in a Nutanix cluster?

- [ ] **A)** Allocating more virtual resources than physical capacity
- [ ] **B)** Reserving all resources for each workload
- [ ] **C)** Removing the need to monitor cluster capacity
- [ ] **D)** Preventing all contention between VMs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Overcommitment assigns more virtual resources than physically exist, increasing cluster density and ROI while requiring monitoring to avoid contention.
 
 
</details>

### 17. Which benefits are provided by installing VirtIO drivers in a guest operating system on AHV? Select all that apply.

- [ ] **A)** Efficient network and storage I/O for guest VMs
- [ ] **B)** Higher throughput compared with emulated devices
- [ ] **C)** Automatic VLAN tagging on the virtual switch
- [ ] **D)** Removing the need for a guest IP configuration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VirtIO provides optimized paravirtualized I/O for networking and storage, improving efficiency and throughput. It does not configure VLANs or remove IP addressing requirements.
 
 
</details>

### 18. In the AHV VM network configuration shown in the code block, which VLAN ID is assigned to the virtual NIC?

```yaml
network_adapters:
  - name: eth0
    bridge: br0
    vlan: 120
    ip: 192.168.20.10
```

- [ ] **A)** 120
- [ ] **B)** br0
- [ ] **C)** 192.168.20.10
- [ ] **D)** eth0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block shows the guest vNIC is attached to br0 with VLAN ID 120, placing the VM in the corresponding broadcast domain.
 
 
</details>

### 19. What is the main purpose of Nutanix Categories when compared with traditional VM tags?

- [ ] **A)** To drive policy-based automation such as Flow and protection
- [ ] **B)** To replace VLANs and virtual switches
- [ ] **C)** To assign IP addresses automatically
- [ ] **D)** To provide only organizational metadata

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Nutanix Categories enable policy-based automation, including microsegmentation and protection rules, whereas traditional tags are generally used for organization and metadata.
 
 
</details>


---

### **Prism Administration**

### 20. What is the principal risk of assigning guaranteed resource reservations to every virtual machine in a Nutanix cluster?

- [ ] **A)** It guarantees predictable performance for every workload
- [ ] **B)** It causes resource fragmentation and wasted capacity
- [ ] **C)** It disables memory ballooning
- [ ] **D)** It allows higher overcommitment ratios

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Applying reservations to every VM guarantees performance but severely limits density. This trap leads to resource fragmentation and wasted capacity in the cluster.
 
 
</details>

### 21. Which two policy-based automation functions can be driven by Nutanix Categories?

- [ ] **A)** Triggering Flow microsegmentation policies
- [ ] **B)** Initiating backup schedules through Nutanix Protect or Mine
- [ ] **C)** Modifying physical switch VLAN trunks
- [ ] **D)** Configuring the ovs bridge on AHV hosts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Nutanix Categories are used for policy-based automation such as Flow microsegmentation and backup schedules. They are not used to modify physical switching or host bridge settings.
 
 
</details>

### 22. Review the output from the AHV host below. Which network bonding mode is configured on the bond?

```bash
ovs-vsctl list bond br0-bond0
    mode: active-backup
    lacp: off
```

- [ ] **A)** Active-Backup
- [ ] **B)** LACP
- [ ] **C)** Static trunk
- [ ] **D)** Bridge mode

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The output shows mode: active-backup and lacp: off. This confirms an Active-Backup bond is configured on the AHV host.
 
 
</details>

### 23. If VirtIO drivers are not included during a guest OS installation on AHV, what is the most likely failure?

- [ ] **A)** The VM will not appear in Prism Element
- [ ] **B)** The VM will fail to boot or will experience low I/O throughput
- [ ] **C)** The VM will automatically download VirtIO drivers
- [ ] **D)** The VM will use physical NICs instead of virtual NICs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> VirtIO drivers are essential for AHV-optimized I/O. Neglecting them during installation can lead to boot failures or degraded network and storage throughput.
 
 
</details>

### 24. Which two statements accurately compare AHV bonding modes?

- [ ] **A)** Active-Backup is simpler and does not require physical switch configuration
- [ ] **B)** LACP requires a matching link aggregation configuration on the upstream switch
- [ ] **C)** LACP is automatically enabled on all Nutanix switches
- [ ] **D)** Active-Backup provides higher bandwidth than LACP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Active-Backup requires no switch-side settings, while LACP must be matched on the upstream physical switch. LACP is not automatic and Active-Backup does not increase bandwidth.
 
 
</details>

### 25. The command output below shows an AHV networking object. What kind of object is it?

```bash
br0
    bridge-id: 8000.001122334455
    ports: eth0
        eth1
        vnet0
        vnet1
```

- [ ] **A)** Bridge
- [ ] **B)** Bond
- [ ] **C)** VLAN
- [ ] **D)** Router

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The output shows br0 with physical ports and vnet interfaces attached. This is the default AHV bridge, the central logical construct for VM connectivity.
 
 
</details>


---

### **Security and Compliance**

### 26. In Nutanix AHV, what is the primary purpose of an Anti-Affinity rule?

- [ ] **A)** To keep related VMs on the same host to reduce network latency
- [ ] **B)** To ensure redundant VMs are placed on separate hosts for high availability
- [ ] **C)** To aggregate multiple physical network links into one logical bond
- [ ] **D)** To automatically assign VLAN IDs to virtual machine networks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Anti-Affinity rules separate redundant VMs onto different hosts, reducing the blast radius of a single host failure and preserving high availability.
 
 
</details>

### 27. Which statements about Nutanix Categories are true? (Select two.)

- [ ] **A)** They are used to drive policy-based automation such as microsegmentation.
- [ ] **B)** They are identical to traditional VM tags and only provide organizational metadata.
- [ ] **C)** They can trigger automated backup schedules through Nutanix Mine or Nutanix Protect.
- [ ] **D)** They can only be assigned during VM creation and cannot be changed afterward.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Nutanix Categories enable policy-based automation like Flow microsegmentation and backup scheduling via Nutanix Mine or Protect. They are more than simple organizational tags.
 
 
</details>

### 28. Review the AHV network output provided in the code block. Which logical network construct is being displayed?

```plaintext
# ovs-vsctl show
Bridge "br0"
    Port "br0"
        Interface "br0"
            type: internal
```

- [ ] **A)** The default AHV bridge, br0
- [ ] **B)** An LACP bond configuration
- [ ] **C)** A network QoS policy
- [ ] **D)** A virtual switch port group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The ovs-vsctl output displays br0, the default AHV bridge that connects physical NICs to virtual machine interfaces for cluster networking.
 
 
</details>

### 29. What is resource overcommitment in AHV?

- [ ] **A)** Assigning more virtual resources to VMs than are physically available
- [ ] **B)** Guaranteeing every VM has dedicated physical hardware
- [ ] **C)** Disabling CPU and memory limits to increase performance
- [ ] **D)** Using reserved resources only for storage traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Resource overcommitment allocates more vCPU or RAM to VMs than physically exists, enabling higher cluster density while requiring careful monitoring to avoid contention.
 
 
</details>

### 30. Which statements accurately differentiate LACP and Active-Backup bonding in AHV? (Select two.)

- [ ] **A)** Active-Backup requires no physical switch configuration.
- [ ] **B)** LACP requires matching configuration on the upstream physical switch.
- [ ] **C)** Active-Backup provides true bandwidth aggregation.
- [ ] **D)** LACP works automatically without any switch-side changes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Active-Backup is simpler and does not require switch configuration, while LACP must be enabled on both the AHV host and the physical upstream switch.
 
 
</details>

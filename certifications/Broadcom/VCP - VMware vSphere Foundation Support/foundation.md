<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Broadcom/VMware%20Certified%20Professional%20-%20VMware%20vSphere%20Foundation%20Administrator" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>VCP - VMware vSphere Foundation Support</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Architectures and Technologies](#architectures-and-technologies) (6 questions)
- [Operations and Administration](#operations-and-administration) (8 questions)
- [Planning and Designing](#planning-and-designing) (4 questions)
- [Product Solutions and Installing](#product-solutions-and-installing) (7 questions)
- [Troubleshooting and Optimizing](#troubleshooting-and-optimizing) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:16.230Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Architectures and Technologies | 6 |
| Operations and Administration | 8 |
| Planning and Designing | 4 |
| Product Solutions and Installing | 7 |
| Troubleshooting and Optimizing | 5 |

---

### **Architectures and Technologies**

### 1. Which vSphere Foundation component functions as a bare-metal hypervisor?

- [ ] **A)** ESXi
- [ ] **B)** vCenter Server
- [ ] **C)** vSphere vMotion
- [ ] **D)** vSphere HA

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ESXi is the bare-metal hypervisor that abstracts hardware resources for VMs.
 
 
</details>

### 2. Which two components are part of vSphere Foundation?

- [ ] **A)** vSphere Replication
- [ ] **B)** vCenter Server
- [ ] **C)** NSX
- [ ] **D)** vSphere HA

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> vCenter Server and vSphere HA are Foundation; Replication and NSX require add-on licenses.
 
 
</details>

### 3. Refer to the cluster image definition in the code block. Which of the following is not included in this image?

```json
{
  "esx_version": "8.0.3",
  "vendor_addon": "DellEMC-Addon",
  "firmware": "DellEMC-Firmware",
  "components": ["vsan", "nvidia-vgpu"]
}
```

- [ ] **A)** ESXi version
- [ ] **B)** Vendor add-on
- [ ] **C)** vCenter version
- [ ] **D)** Firmware bundle

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> vLCM cluster images contain ESXi version, vendor add-ons, and firmware, but not vCenter version.
 
 
</details>

### 4. What is the minimum number of hosts required for vSAN RAID-5 erasure coding?

- [ ] **A)** 2
- [ ] **B)** 3
- [ ] **C)** 4
- [ ] **D)** 6

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> RAID-5 (3+1) requires at least 4 hosts: three for data and one for parity.
 
 
</details>

### 5. Which two statements accurately describe vSAN Express Storage Architecture (ESA)?

- [ ] **A)** Uses disk groups with cache and capacity tiers
- [ ] **B)** Eliminates the need for a dedicated cache tier
- [ ] **C)** Supports hybrid HDD and flash configurations
- [ ] **D)** Applies deduplication and compression inline

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> ESA uses a unified flash pool, no disk groups, and inline dedup/compression. Hybrid storage is not supported.
 
 
</details>

### 6. Refer to the NSX distributed firewall rule in the code block. What is the result of this rule?

```json
{
  "source": "Finance-VM",
  "destination": "HR-VM",
  "service": "HTTPS",
  "action": "DENY"
}
```

- [ ] **A)** Allows HTTPS from Finance to HR
- [ ] **B)** Denies HTTPS from Finance to HR
- [ ] **C)** Allows all traffic from Finance
- [ ] **D)** Denies all traffic from Finance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The rule explicitly denies HTTPS traffic from Finance-VM to HR-VM.
 
 
</details>


---

### **Operations and Administration**

### 7. Which tool provides real-time performance charts for immediate diagnostics in vSphere?

- [ ] **A)** vCenter Server
- [ ] **B)** VMware Skyline
- [ ] **C)** vRealize Operations
- [ ] **D)** ESXi Shell

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> vCenter Server provides real-time performance charts for the last 30 minutes. Skyline focuses on log and configuration analysis, not real-time metrics.
 
 
</details>

### 8. Which two are primary functions of VMware Skyline Health Diagnostics?

- [ ] **A)** Analyze log files for configuration issues
- [ ] **B)** Display real-time CPU utilization graphs
- [ ] **C)** Run 250+ health checks on vCenter and ESXi
- [ ] **D)** Deploy virtual machines from templates

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Skyline Health Diagnostics analyzes logs and runs 250+ health checks. Real-time CPU graphs are from vCenter, and VM deployment is not a Skyline function.
 
 
</details>

### 9. Refer to the code block; what is the correct metric threshold for high CPU ready time in vSphere?

```text
vCenter alert: CPU ready time for VM 'WebServer01' is 12% over the last 10 seconds.
```

- [ ] **A)** Greater than 5% over 10 seconds
- [ ] **B)** Greater than 10% over 30 seconds
- [ ] **C)** Greater than 2% over 5 seconds
- [ ] **D)** Greater than 20% over 1 minute

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A CPU ready value >5% (over 10 seconds) generally indicates overcommitment, as stated in the playbook.
 
 
</details>

### 10. What must be installed in a VM template for guest customization to work on Linux?

- [ ] **A)** open-vm-tools
- [ ] **B)** Sysprep files
- [ ] **C)** cloud-init scripts
- [ ] **D)** VMware Tools version 12

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> open-vm-tools (including the guest customization component) is required for Linux customization. Sysprep is for Windows; cloud-init is an alternative but not required by vSphere.
 
 
</details>

### 11. Which two actions require specific RBAC privileges beyond 'Virtual machine.Provisioning.Allow template deploy'?

- [ ] **A)** Cloning a powered-off VM
- [ ] **B)** Deploying from a template with guest customization
- [ ] **C)** Importing an OVF file
- [ ] **D)** Customizing the guest OS during deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Deploying with customization requires 'Allow customization' privilege. Customizing guest OS also needs that. Cloning uses 'Create from existing'; OVF import uses 'Import' privilege.
 
 
</details>

### 12. Read the code block; which state indicates the VM is ready for template conversion in content library?

```powershell
Get-VM -Name 'GoldImage-Windows' | Where-Object {$_.PowerState -eq 'PoweredOff'} | Set-VM -ToTemplate -Confirm:$false
```

- [ ] **A)** Powered off
- [ ] **B)** Powered on with VMware Tools
- [ ] **C)** Suspended
- [ ] **D)** Maintenance mode

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Templates in a content library must be created from powered-off VMs (or snapshots). The playbook notes that you convert a VM to a template, and it requires the VM to be powered off.
 
 
</details>

### 13. What does vSphere Lifecycle Manager (vLCM) use to define the desired state of a cluster?

- [ ] **A)** A single cluster image
- [ ] **B)** Multiple baselines
- [ ] **C)** Host profiles
- [ ] **D)** Virtual machine templates

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> vLCM uses a single image per cluster to define the exact desired state, replacing the multiple baselines of VUM.
 
 
</details>

### 14. Which two are steps in the vLCM remediation process?

- [ ] **A)** Host enters maintenance mode
- [ ] **B)** vCenter reboots
- [ ] **C)** Software and firmware updates applied
- [ ] **D)** Virtual machines are migrated to another datacenter

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> During remediation, vLCM puts the host in maintenance mode, then applies updates. vCenter does not reboot, and VMs are not migrated to another datacenter (only to other hosts in the cluster).
 
 
</details>


---

### **Planning and Designing**

### 15. What is the maximum number of hosts supported per vSphere 8 cluster?

- [ ] **A)** 32
- [ ] **B)** 64
- [ ] **C)** 96
- [ ] **D)** 128

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The maximum supported hosts per cluster in vSphere 8 is 96, as documented in the planning and design guidelines.
 
 
</details>

### 16. Which two of the following are supported storage protocols for vSphere Foundation?

- [ ] **A)** iSCSI
- [ ] **B)** NFS
- [ ] **C)** Fibre Channel
- [ ] **D)** SMB

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> vSphere Foundation supports iSCSI, NFS, and Fibre Channel as storage protocols. SMB is not a supported storage protocol for vSphere.
 
 
</details>

### 17. Based on the storage policy shown, what is the minimum number of ESXi hosts required for this vSAN cluster?

```yaml
storagePolicy:
  name: "High-Availability"
  ruleSet:
    - rule:
        property: "numberOfFailuresToTolerate"
        value: 2
    - rule:
        property: "failureToleranceMethod"
        value: "RAID-1 (Mirroring)"
```

- [ ] **A)** 3
- [ ] **B)** 4
- [ ] **C)** 5
- [ ] **D)** 6

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> For FTT=2 with mirroring, vSAN requires at least 5 hosts to ensure data availability during two concurrent failures.
 
 
</details>

### 18. Which feature must be supported by the physical network to use IP hash load balancing on a vSphere Distributed Switch?

- [ ] **A)** LACP
- [ ] **B)** Route based on source MAC hash
- [ ] **C)** MTU 9000
- [ ] **D)** Network I/O Control

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IP hash load balancing requires LACP (or EtherChannel) configuration on the physical switch to distribute traffic across multiple uplinks.
 
 
</details>


---

### **Product Solutions and Installing**

### 19. What is the primary purpose of a Kickstart file during ESXi installation?

- [ ] **A)** To automate the installation process
- [ ] **B)** To configure vCenter Server
- [ ] **C)** To manage storage for VMs
- [ ] **D)** To provide a graphical user interface

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Kickstart file automates ESXi installation by providing answers to installation prompts.
 
 
</details>

### 20. Which two prerequisites must be met before deploying the vCenter Server Appliance (VCSA)?

- [ ] **A)** NTP synchronization on the target ESXi host
- [ ] **B)** A valid DNS A record for the VCSA FQDN
- [ ] **C)** vCenter Server already installed
- [ ] **D)** A Windows-based management server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VCSA deployment requires a DNS A record and NTP synchronization to ensure proper time and name resolution.
 
 
</details>

### 21. What does the following command accomplish?

```bash
esxcli network ip interface add -i vmk2 -p 'VMkernel'
```

- [ ] **A)** Creates a new VMkernel interface
- [ ] **B)** Deletes a port group
- [ ] **C)** Sets the host's IP address
- [ ] **D)** Enables SSH access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command 'esxcli network ip interface add' creates a new VMkernel network interface.
 
 
</details>

### 22. What is the minimum number of ESXi hosts required for a standard vSAN cluster?

- [ ] **A)** 2
- [ ] **B)** 3
- [ ] **C)** 4
- [ ] **D)** 1

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A standard vSAN cluster requires a minimum of three hosts to provide redundancy and support Failures to Tolerate (FTT) policies.
 
 
</details>

### 23. Which two features are enabled by creating a vSphere cluster?

- [ ] **A)** High Availability (HA)
- [ ] **B)** Distributed Resource Scheduler (DRS)
- [ ] **C)** vSAN
- [ ] **D)** Fault Tolerance (FT)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A vSphere cluster enables HA for automatic VM restart and DRS for load balancing; vSAN and FT are additional features that can be enabled separately.
 
 
</details>

### 24. What is the purpose of the following line in a PXE boot configuration?

```config
option filename "pxelinux.0";
```

- [ ] **A)** Specifies the boot loader to download via TFTP
- [ ] **B)** Sets the DHCP lease time
- [ ] **C)** Defines the VLAN for management traffic
- [ ] **D)** Configures the host's root password

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'filename' directive in DHCP options tells the PXE client which boot loader file to download from the TFTP server.
 
 
</details>

### 25. Which port is used to access the vCenter Server Appliance Management Interface (VAMI)?

- [ ] **A)** 443
- [ ] **B)** 5480
- [ ] **C)** 80
- [ ] **D)** 22

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> VAMI is accessible via HTTPS on port 5480 for appliance-level management.
 
 
</details>


---

### **Troubleshooting and Optimizing**

### 26. What is the primary purpose of VMkernel network adapters (vmknic) in ESXi?

- [ ] **A)** Provide management network for vCenter
- [ ] **B)** Serve as backbone for ESXi host management, vMotion, provision, and fault tolerance networking
- [ ] **C)** Enable guest OS network connectivity
- [ ] **D)** Connect to physical switches via vSwitches

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> VMkernel adapters are crucial for ESXi services like management, vMotion, provision, and FT networking.
 
 
</details>

### 27. Which two statements are true about troubleshooting storage connectivity?

- [ ] **A)** esxcli storage core path list verifies path status
- [ ] **B)** APD and PDL are synonymous terms
- [ ] **C)** NFS mounts depend on VMkernel networking
- [ ] **D)** CHAP authentication is only used for Fibre Channel

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> APD and PDL differ; NFS uses VMkernel; CHAP is for iSCSI, not Fibre Channel.
 
 
</details>

### 28. Which command displays VMkernel network adapter information?

```bash
esxcli network ip interface list
```

- [ ] **A)** esxcli network ip interface list
- [ ] **B)** esxcli network vswitch standard list
- [ ] **C)** vmkping -I
- [ ] **D)** esxcli storage core path list

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command esxcli network ip interface list shows VMkernel adapter configurations.
 
 
</details>

### 29. What does a red alert in vSAN Health Service indicate?

- [ ] **A)** A warning that requires attention soon
- [ ] **B)** A critical issue that needs immediate action
- [ ] **C)** A performance degradation
- [ ] **D)** A configuration mismatch

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Red alerts in vSAN Health Service are critical and require immediate action.
 
 
</details>

### 30. Which two metrics indicate CPU contention for a virtual machine?

- [ ] **A)** High CPU usage percentage
- [ ] **B)** High CPU ready time (%RDY)
- [ ] **C)** High CPU co-stop time
- [ ] **D)** High CPU idle time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> High %RDY and co-stop time indicate CPU contention; high usage means demand satisfied.
 
 
</details>

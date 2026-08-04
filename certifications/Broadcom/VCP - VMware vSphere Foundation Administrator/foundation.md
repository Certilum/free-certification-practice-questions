<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Broadcom/VMware%20Certified%20Professional%20-%20VMware%20vSphere%20Foundation%20Administrator" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>VCP - VMware vSphere Foundation Administrator</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [VMware Aria Operations and Automation](#vmware-aria-operations-and-automation) (6 questions)
- [VMware vSAN and NSX Administration](#vmware-vsan-and-nsx-administration) (3 questions)
- [VMware vSphere Foundation Architectures and Technologies](#vmware-vsphere-foundation-architectures-and-technologies) (6 questions)
- [VMware vSphere Infrastructure Installation and Configuration](#vmware-vsphere-infrastructure-installation-and-configuration) (7 questions)
- [VMware vSphere Operational Management](#vmware-vsphere-operational-management) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:13.574Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| VMware Aria Operations and Automation | 6 |
| VMware vSAN and NSX Administration | 3 |
| VMware vSphere Foundation Architectures and Technologies | 6 |
| VMware vSphere Infrastructure Installation and Configuration | 7 |
| VMware vSphere Operational Management | 8 |

---

### **VMware Aria Operations and Automation**

### 1. What is the primary purpose of Aria Operations management packs?

- [ ] **A)** Collect data from various sources
- [ ] **B)** Deploy virtual appliances
- [ ] **C)** Manage user roles
- [ ] **D)** Configure network settings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Management packs act as adapters to pull metrics from vCenter, NSX, storage, etc., enabling unified monitoring and analytics.
 
 
</details>

### 2. Which two elements are required when configuring a vCenter adapter instance in Aria Operations?

- [ ] **A)** Display name
- [ ] **B)** Connection details
- [ ] **C)** Management pack version
- [ ] **D)** Collection schedule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> An adapter instance needs a display name and connection details (hostname, credentials). Version and schedule are not required at instance creation.
 
 
</details>

### 3. Examine the Cloud Template snippet and identify the resource type of the VM.

```yaml
resources:
  myVM:
    type: Cloud.Machine
    properties:
      image: ubuntu-20.04
      flavor: small
```

- [ ] **A)** Cloud.Machine
- [ ] **B)** Cloud.Volume
- [ ] **C)** Cloud.Network
- [ ] **D)** Cloud.Template

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The YAML shows 'type: Cloud.Machine' for the VM resource, which is the native Aria Automation type for virtual machines.
 
 
</details>

### 4. What does the Capacity Planning Engine in Aria Operations use to forecast resource usage?

- [ ] **A)** Historical data
- [ ] **B)** Real-time metrics only
- [ ] **C)** User-defined thresholds
- [ ] **D)** External API inputs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The engine uses historical data (minimum 30 days) and applies algorithms to predict future demand and time to full.
 
 
</details>

### 5. Which two are valid collection levels for a vCenter adapter in Aria Operations?

- [ ] **A)** Level 2 (Basic)
- [ ] **B)** Level 4 (Full)
- [ ] **C)** Level 1 (Minimal)
- [ ] **D)** Level 5 (Extended)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Valid levels are 2 (basic metrics) and 4 (full metrics for advanced monitoring and capacity planning). Levels 1 and 5 do not exist.
 
 
</details>

### 6. Review the alert definition snippet and choose the correct severity for disk usage exceeding 80%.

```yaml
alertDefinitions:
  - name: high-disk-usage
    severity: critical
    condition: 'resource:disk.usage.percent > 80'
```

- [ ] **A)** Critical
- [ ] **B)** Warning
- [ ] **C)** Info
- [ ] **D)** Emergency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The alert definition shows 'severity: critical' for the symptom 'disk.usage.percent > 80', matching standard capacity thresholds.
 
 
</details>


---

### **VMware vSAN and NSX Administration**

### 7. What is the minimum number of hosts required for a vSAN all-flash cluster to support erasure coding RAID-5 with 1 failure tolerance?

- [ ] **A)** 3 hosts
- [ ] **B)** 4 hosts
- [ ] **C)** 5 hosts
- [ ] **D)** 6 hosts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> RAID-5 erasure coding with FTT=1 requires a minimum of 4 hosts in a vSAN all-flash cluster. This is because erasure coding splits data into 3 data blocks and 1 parity block, requiring at least 4 hosts to store the components.
 
 
</details>

### 8. Which two components can be used as key providers for vSAN encryption?

- [ ] **A)** Key Management Server (KMS)
- [ ] **B)** Local key provider
- [ ] **C)** VMware Identity Manager
- [ ] **D)** Active Directory Certificate Services

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> vSAN encryption supports two key provider modes: a Key Management Server (KMS) compliant with KMIP 1.2, and a local key provider (simplified, non-FIPS 140-2 compliant). VMware Identity Manager and AD Certificate Services are not used for vSAN encryption key management.
 
 
</details>

### 9. An administrator runs the following command on an ESXi host. What is the purpose of this command?

```bash
esxcli vsan health cluster list
```

- [ ] **A)** Check the overall vSAN cluster health status
- [ ] **B)** List all virtual machines on the host
- [ ] **C)** Display the vSAN disk group configuration
- [ ] **D)** Test network connectivity between vSAN nodes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command 'esxcli vsan health cluster list' retrieves the vSAN health status for the entire cluster from the perspective of the local host. It is used to quickly assess vSAN health without using the vSphere Client.
 
 
</details>


---

### **VMware vSphere Foundation Architectures and Technologies**

### 10. Which component of VMware vSphere Foundation (VVF) provides centralized management of ESXi hosts and virtual machines?

- [ ] **A)** vCenter Server
- [ ] **B)** ESXi Hypervisor
- [ ] **C)** vSAN
- [ ] **D)** NSX

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> vCenter Server is the centralized management plane in VVF, providing a single point of control for ESXi hosts, virtual machines, clusters, datastores, and networking. ESXi is the hypervisor, vSAN provides storage, and NSX provides networking.
 
 
</details>

### 11. Which of the following are included in the VMware vSphere Foundation (VVF) bundle? (Select TWO.)

- [ ] **A)** vCenter Server
- [ ] **B)** Aria Automation
- [ ] **C)** vSAN
- [ ] **D)** SDDC Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> VVF includes vCenter Server, vSAN, Aria Operations for Infrastructure, and Aria Operations for Logs. Aria Automation and SDDC Manager are part of VMware Cloud Foundation (VCF), not VVF.
 
 
</details>

### 12. An administrator runs the following PowerCLI command to check the vSAN health status. What is the expected output if the vSAN cluster is healthy?

```powershell
PS C:\> Get-VsanClusterHealth -ClusterName 'ProdCluster'
```

- [ ] **A)** HealthStatus: 'Green'
- [ ] **B)** HealthStatus: 'Red'
- [ ] **C)** HealthStatus: 'Yellow'
- [ ] **D)** HealthStatus: 'Orange'

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Get-VsanClusterHealth cmdlet returns a HealthStatus property. A value of 'Green' indicates that all health checks passed and the cluster is healthy.
 
 
</details>

### 13. What is the minimum number of hosts required for a vSAN Express Storage Architecture (ESA) cluster?

- [ ] **A)** 2 hosts
- [ ] **B)** 3 hosts
- [ ] **C)** 4 hosts
- [ ] **D)** 5 hosts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> vSAN ESA requires a minimum of 3 hosts. OSA can start with 2 hosts using a witness appliance, but ESA does not support 2-node configurations.
 
 
</details>

### 14. Which two components are part of VMware Cloud Foundation (VCF) but NOT included in VMware vSphere Foundation (VVF)? (Select two.)

- [ ] **A)** NSX
- [ ] **B)** Aria Operations for Logs
- [ ] **C)** SDDC Manager
- [ ] **D)** vSAN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> VCF includes all VVF components plus NSX, Aria Automation, full Aria Operations, and SDDC Manager. Aria Operations for Logs and vSAN are already part of VVF.
 
 
</details>

### 15. A vSphere admin needs to create a vSAN storage policy with 'Failures to tolerate = 1' using RAID-5 erasure coding. What is the minimum number of hosts required in the cluster?

```powershell
New-SpbmStoragePolicy -Name 'RAID5-FTT1' -Description 'Policy with RAID5 and FTT=1' -VsanCluster -VsanErasureCodeTechnology 'RAID5' -VsanFailuresToTolerate 1
```

- [ ] **A)** 3
- [ ] **B)** 4
- [ ] **C)** 5
- [ ] **D)** 6

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> RAID-5 erasure coding with FTT=1 requires a minimum of 4 hosts to avoid a 'No Quorum' condition. The number of data components is 3 (n-1), so at least 4 hosts are needed.
 
 
</details>


---

### **VMware vSphere Infrastructure Installation and Configuration**

### 16. During an interactive ESXi installation, at which step is the root password required?

- [ ] **A)** After disk selection and before EULA acceptance
- [ ] **B)** Before disk selection and after EULA acceptance
- [ ] **C)** After the installation completes and first boot
- [ ] **D)** During the keyboard layout selection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In interactive ESXi installation, the root password is prompted after accepting the EULA and before selecting the target disk. The installer asks for root password (with confirmation) prior to disk selection step.
 
 
</details>

### 17. Which of the following are valid methods for deploying an ESXi host? (Choose two)

- [ ] **A)** Interactive installation from a CD/DVD ISO
- [ ] **B)** Stateless deployment using Auto Deploy
- [ ] **C)** Using a Windows-based vCenter Server as an installation target
- [ ] **D)** Booting from a network share without a kickstart file

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Valid methods include interactive (ISO) and Auto Deploy (stateless/stateful). Scripted installation also writes to disk, but stateless Auto Deploy is distinct. vCenter is not used to install ESXi directly.
 
 
</details>

### 18. An administrator needs to list the standard virtual switches on an ESXi host. Which command should be used?

```bash
esxcli network vswitch standard list
```

- [ ] **A)** esxcli network vswitch standard list
- [ ] **B)** esxcli network vswitch dvs vmware list
- [ ] **C)** esxcli network ip interface list
- [ ] **D)** esxcli network vswitch list

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The correct command is 'esxcli network vswitch standard list'. The other commands list distributed switches, IP interfaces, or a generic list that includes both types.
 
 
</details>

### 19. Which deployment architecture is supported for vCenter Server Appliance in vSphere 8?

- [ ] **A)** Embedded Platform Services Controller only
- [ ] **B)** External Platform Services Controller with separate vCenter Server
- [ ] **C)** Both embedded and external Platform Services Controller
- [ ] **D)** Distributed deployment with multiple Platform Services Controllers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> vSphere 8 only supports embedded deployments. The external Platform Services Controller architecture was removed. All services run within a single VCSA.
 
 
</details>

### 20. Which of the following are prerequisites for deploying a VCSA? (Choose two)

- [ ] **A)** DNS must have both forward and reverse lookup records for the planned VCSA FQDN
- [ ] **B)** The target ESXi host must have DHCP enabled
- [ ] **C)** NTP servers must be reachable from the management network
- [ ] **D)** An Active Directory domain must be configured before deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Pre-deployment checks include DNS (forward and reverse) and NTP reachability. DHCP is not recommended; static IP is required. AD configuration is optional and can be done post-deployment.
 
 
</details>

### 21. An administrator needs to enable jumbo frames (MTU 9000) for vMotion traffic. Which two steps must be performed?

```bash
esxcli network ip interface set -i vmk0 -m 9000
```

- [ ] **A)** Set MTU 9000 on the vSwitch or distributed switch
- [ ] **B)** Set MTU 9000 on the physical switch ports
- [ ] **C)** Set MTU 9000 on the VMkernel adapter dedicated to vMotion
- [ ] **D)** Enable jumbo frames on the VMkernel adapter for management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> For jumbo frames, MTU must be set on the vSwitch/dvSwitch and on the VMkernel adapter. Physical switch configuration is required but is not an action an ESXi admin performs via vSphere Client.
 
 
</details>

### 22. What is the default block size for a VMFS-6 datastore created on a LUN larger than 2 TB?

- [ ] **A)** 1 MB
- [ ] **B)** 4 MB
- [ ] **C)** 8 MB
- [ ] **D)** 2 MB

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> VMFS-6 defaults to 8 MB block size for LUNs larger than 2 TB to support larger virtual disks. This is a key fact for storage configuration.
 
 
</details>


---

### **VMware vSphere Operational Management**

### 23. Which tool provides real-time, per-second performance counters for ESXi hosts?

- [ ] **A)** vCenter Performance Charts
- [ ] **B)** esxtop
- [ ] **C)** vscsiStats
- [ ] **D)** resxtop

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> esxtop provides real-time, granular counters at the ESXi host level. vCenter Charts show aggregated historical data. vscsiStats is for virtual SCSI statistics, and resxtop is a remote version of esxtop.
 
 
</details>

### 24. Which two conditions are required for vSphere Trust Authority (vTA) to function on an ESXi host?

- [ ] **A)** TPM 2.0 chip
- [ ] **B)** UEFI Secure Boot enabled
- [ ] **C)** vCenter Server 7.0 or later
- [ ] **D)** Active Directory integration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> vTA requires a discrete or firmware TPM 2.0 and UEFI Secure Boot. While a supported vCenter version is needed, it is not a prerequisite on the host itself. AD integration is unrelated to vTA.
 
 
</details>

### 25. Refer to the command below. What does the 'c' key do in this utility?

```bash
# Run esxtop on an ESXi host
~ # esxtop
   (press 'c' to enter CPU screen)
```

- [ ] **A)** Displays CPU performance counters
- [ ] **B)** Shows memory usage statistics
- [ ] **C)** Opens disk latency metrics
- [ ] **D)** Exits the tool

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In esxtop, pressing 'c' switches to the CPU screen which shows counters like %RDY, %CSTP, etc. Other keys: 'm' for memory, 'd' for disk, 'n' for network.
 
 
</details>

### 26. What is the purpose of the 'Do not propagate to children' flag when assigning a vSphere permission?

- [ ] **A)** It prevents the permission from being inherited by child objects.
- [ ] **B)** It blocks the permission from being applied to the current object.
- [ ] **C)** It revokes the permission from the user or group.
- [ ] **D)** It forces the permission to apply to all objects globally.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Permission propagation controls whether the permission is inherited by child objects. Unchecking 'Propagate to children' means the permission applies only to the selected object and not to its descendants.
 
 
</details>

### 27. Which two actions can a vSphere alarm perform when triggered?

- [ ] **A)** Send an SNMP trap
- [ ] **B)** Execute a command on the vCenter Server
- [ ] **C)** Reboot the ESXi host
- [ ] **D)** Delete the virtual machine

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Alarms can send SNMP traps and run commands (scripts) on the vCenter Server. They cannot directly reboot hosts or delete VMs as actions.
 
 
</details>

### 28. Examine the command. What is the purpose of the 'replace' operation in this context?

```bash
# Command to replace machine SSL certificate on VCSA
certificate-manager replace --machine-ssl --cert-file new_cert.cer --key-file private.key --ca-file ca_chain.pem
```

- [ ] **A)** Replaces the vCenter Server machine SSL certificate
- [ ] **B)** Replaces the solution user certificates
- [ ] **C)** Regenerates the VMCA root certificate
- [ ] **D)** Deploys a new vCenter Server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'certificate-manager replace --machine-ssl' command is used to replace the vCenter Server's machine SSL certificate (used for HTTPS access). Solution user certificates are replaced with '--solution-user'.
 
 
</details>

### 29. What is the first step when restoring a vCenter Server from a file-based backup?

- [ ] **A)** Deploy a temporary VCSA using the Installer
- [ ] **B)** Power on the old vCenter Server
- [ ] **C)** Restore from VAMI web interface
- [ ] **D)** Attach the backup disk to a running VM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The restore process begins by deploying a temporary VCSA from the Installer ISO. You cannot restore a running vCenter; the appliance must be off. VAMI restore is only for an already deployed appliance.
 
 
</details>

### 30. Which two protocols are supported for vCenter Server file-based backup destinations?

- [ ] **A)** FTP
- [ ] **B)** SMB/CIFS
- [ ] **C)** NFS
- [ ] **D)** iSCSI

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VCSA file-based backup supports FTP, FTPS, HTTPS, SCP, and SMB/CIFS. NFS and iSCSI are not protocols handled by the backup service.
 
 
</details>

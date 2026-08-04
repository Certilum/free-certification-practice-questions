<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Broadcom/VMware%20Certified%20Professional%20-%20VMware%20Cloud%20Foundation%20Administrator" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>VCP - VMware Cloud Foundation Administrator</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Administration and Operations](#administration-and-operations) (9 questions)
- [Architecture and Design](#architecture-and-design) (6 questions)
- [Automation and Orchestration](#automation-and-orchestration) (4 questions)
- [Installation, Configuration, and Upgrade](#installation-configuration-and-upgrade) (8 questions)
- [Troubleshooting and Disaster Recovery](#troubleshooting-and-disaster-recovery) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:05.730Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Administration and Operations | 9 |
| Architecture and Design | 6 |
| Automation and Orchestration | 4 |
| Installation, Configuration, and Upgrade | 8 |
| Troubleshooting and Disaster Recovery | 3 |

---

### **Administration and Operations**

### 1. Which VCF tool provides a centralized health dashboard for workload domain components?

- [ ] **A)** SDDC Manager
- [ ] **B)** vRealize Operations
- [ ] **C)** vRealize Log Insight
- [ ] **D)** vCenter Server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SDDC Manager provides the centralized health dashboard for workload domain components.
 
 
</details>

### 2. Which of the following are key capabilities of vRealize Operations in VCF? (Choose two.)

- [ ] **A)** Capacity forecasting
- [ ] **B)** Patch compliance management
- [ ] **C)** Anomaly detection
- [ ] **D)** Log aggregation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> vROps provides capacity forecasting and anomaly detection. Patch compliance is via SDDC Manager, log aggregation via vRLI.
 
 
</details>

### 3. Which SDDC Manager health check would be triggered by a certificate expiry?

```javascript
const healthCheckTypes = ['connectivity', 'certificate', 'service', 'disk'];
```

- [ ] **A)** Connectivity check
- [ ] **B)** Service status check
- [ ] **C)** Certificate expiry check
- [ ] **D)** Disk space check

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> SDDC Manager runs certificate expiry checks as part of health monitoring.
 
 
</details>

### 4. Which VCF tool is used for centralized log correlation and search?

- [ ] **A)** vRealize Log Insight
- [ ] **B)** SDDC Manager
- [ ] **C)** vRealize Operations
- [ ] **D)** vCenter Server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> vRealize Log Insight (vRLI) aggregates logs from all VCF components.
 
 
</details>

### 5. Which two roles in SDDC Manager can create or modify workload domains? (Choose two.)

- [ ] **A)** Super Admin
- [ ] **B)** Cloud Admin
- [ ] **C)** Viewer
- [ ] **D)** Network Admin

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Super Admin and Cloud Admin can manage workload domains. Viewer is read-only, Network Admin is not a standard SDDC role.
 
 
</details>

### 6. Which command on SDDC Manager CLI reconciles a restored vCenter Server?

```bash
sudo /opt/vmware/vcf/resolve-vcenter.sh --help
```

- [ ] **A)** resolve-vcenter.sh
- [ ] **B)** vcf-resolve-vcenter.sh
- [ ] **C)** /opt/vmware/vcf/resolve-vcenter.sh
- [ ] **D)** resync-vcenter.sh

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The script /opt/vmware/vcf/resolve-vcenter.sh is used to reconcile vCenter after restore.
 
 
</details>

### 7. Which backup method is recommended for vCenter Server in VCF?

- [ ] **A)** VAMI backup
- [ ] **B)** SDDC Manager snapshot
- [ ] **C)** vSphere Data Protection
- [ ] **D)** Manual file copy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Native VAMI backup is recommended for vCenter Server as it includes the database.
 
 
</details>

### 8. Which two components are included in SDDC Manager backup? (Choose two.)

- [ ] **A)** SDDC Manager database
- [ ] **B)** Workload domain VMs
- [ ] **C)** Encrypted passwords
- [ ] **D)** vSAN disk groups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> SDDC Manager backup includes its database and encrypted passwords, not workload VMs or vSAN disk groups.
 
 
</details>

### 9. How many hosts are required in a vSAN cluster to use RAID-5 erasure coding?

```javascript
const minHosts = { 'RAID1': 2, 'RAID5': 4, 'RAID6': 6 };
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
> RAID-5 erasure coding with failures to tolerate (FTT)=1 requires a minimum of 4 hosts.
 
 
</details>


---

### **Architecture and Design**

### 10. What is the minimum number of hosts required for the Management Domain in a vSAN-based VCF deployment?

- [ ] **A)** 2
- [ ] **B)** 3
- [ ] **C)** 4
- [ ] **D)** 5

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Management Domain must include at least four hosts to provide resilience for management components.
 
 
</details>

### 11. Which of the following are true statements about Workload Domains in VCF? (Choose two)

- [ ] **A)** They can have different vSphere versions assigned.
- [ ] **B)** They share the same vCenter Server as the Management Domain.
- [ ] **C)** They are logically isolated pools of compute, storage, and network resources.
- [ ] **D)** They can be directly managed by SDDC Manager for VM-level operations.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Workload Domains can have independent vSphere versions and are isolated resource pools. They do not share vCenter with the management domain, and SDDC Manager does not manage VMs.
 
 
</details>

### 12. Examine the following NSX configuration excerpt. What is the primary function of the component being configured?

```json
{
  "display_name": "T0-GW",
  "type": "TIER0",
  "ha_mode": "ACTIVE_STANDBY",
  "edge_cluster_path": "/infra/sites/default/enforcement-points/default/edge-clusters/ec-1",
  "transit_subnets": ["192.168.100.0/24"]
}
```

- [ ] **A)** Tier-0 gateway
- [ ] **B)** Tier-1 gateway
- [ ] **C)** Distributed Firewall
- [ ] **D)** NSX Manager cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The configuration creates a Tier-0 gateway with BGP peering to external routers, which handles North-South routing.
 
 
</details>

### 13. Which storage option is mandatory for the Management Domain in a VCF 5.x deployment?

- [ ] **A)** External Fibre Channel SAN
- [ ] **B)** NFS v4.1
- [ ] **C)** vSAN
- [ ] **D)** iSCSI with VMFS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Management Domain in VCF 5.x must use vSAN as the storage layer to maintain lifecycle automation and simplicity.
 
 
</details>

### 14. Which of the following are responsibilities of SDDC Manager in VCF? (Choose two)

- [ ] **A)** Orchestrating domain-level lifecycle operations
- [ ] **B)** Managing individual virtual machines
- [ ] **C)** Deploying the initial VCF stack during bring-up
- [ ] **D)** Replacing vCenter for day-to-day cluster management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> SDDC Manager orchestrates lifecycle and initial deployment, but does not manage VMs or replace vCenter for daily operations.
 
 
</details>

### 15. Examine the following vSAN storage policy snippet. What does FTT=1 with RAID-1 imply for a VM's storage?

```json
{
  "name": "basic-mirror",
  "rule_set": [
    {
      "rule": "NumberFailuresToTolerate",
      "value": 1
    },
    {
      "rule": "Policies",
      "value": "RAID-1 Mirroring"
    }
  ]
}
```

- [ ] **A)** One host failure with full data copy
- [ ] **B)** One disk failure with erasure coding
- [ ] **C)** Two host failures with mirroring
- [ ] **D)** No failures tolerated; only one copy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> FTT=1 with RAID-1 means one mirror copy; the VM can survive one host failure without data loss.
 
 
</details>


---

### **Automation and Orchestration**

### 16. Which PowerCLI cmdlet is used to establish a connection to the SDDC Manager?

- [ ] **A)** Connect-VCF
- [ ] **B)** Connect-VIServer
- [ ] **C)** Connect-VMHost
- [ ] **D)** Connect-VCFServer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Connect-VCF is the specific cmdlet from the VMware.VCF module that authenticates to the SDDC Manager REST API.
 
 
</details>

### 17. Which two components must be registered as cloud accounts in vRealize Automation to enable dynamic network provisioning on VCF?

- [ ] **A)** vCenter Server
- [ ] **B)** NSX Manager
- [ ] **C)** vRealize Orchestrator
- [ ] **D)** vRealize Suite Lifecycle Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> vRA requires both a vCenter cloud account for compute and an NSX cloud account for dynamic network provisioning.
 
 
</details>

### 18. Review the Terraform provider block below. What is the primary purpose of the 'url' argument?

```hcl
provider "vmware/vcf" {
  username = var.vcf_username
  password = var.vcf_password
  url      = var.vcf_url
}
```

- [ ] **A)** The API endpoint of SDDC Manager
- [ ] **B)** The vCenter Server address
- [ ] **C)** The NSX Manager hostname
- [ ] **D)** The Terraform Cloud backend URL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'url' argument in the VCF provider sets the SDDC Manager's API base URL for all subsequent resource operations.
 
 
</details>

### 19. What is the first action taken by SDDC Manager when initiating an automated workload domain scale-out?

- [ ] **A)** Pre-flight validation of host inventory and cluster state
- [ ] **B)** Adding the new host to the vCenter cluster
- [ ] **C)** Configuring NSX overlay on the new host
- [ ] **D)** Rebalancing VMs via DRS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The scaling workflow begins with pre-flight validation to ensure prerequisites such as host availability and image compliance are met.
 
 
</details>


---

### **Installation, Configuration, and Upgrade**

### 20. Which temporary appliance orchestrates the initial bring-up of the VCF management domain?

- [ ] **A)** Cloud Builder
- [ ] **B)** SDDC Manager
- [ ] **C)** vCenter Server
- [ ] **D)** NSX Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Cloud Builder VM is a temporary appliance used only for the initial bring-up; SDDC Manager is deployed later.
 
 
</details>

### 21. Which two prerequisites are required before adding a workload domain in VCF?

- [ ] **A)** Healthy management domain
- [ ] **B)** Available capacity pool hosts
- [ ] **C)** Deployed Horizon Connection Server
- [ ] **D)** Configured external storage array

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The management domain must be healthy and free hosts must exist in the capacity pool.
 
 
</details>

### 22. Review the deployment parameter workbook excerpt. Which network parameter is incorrectly specified?

```json
{
  "managementPool": "10.0.0.0/24",
  "vMotionPool": "10.0.0.10/24",
  "nsxOverlayPool": "10.0.1.0/24"
}
```

- [ ] **A)** Overlapping IP pools for management and vMotion
- [ ] **B)** Missing VLAN ID for overlay transport zone
- [ ] **C)** Incorrect DNS server IP address
- [ ] **D)** MTU mismatch between hosts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Overlapping IP pools are a common DPW error; management and vMotion must use distinct pools.
 
 
</details>

### 23. What is the default HA admission control setting for the management cluster after deployment?

- [ ] **A)** Disabled
- [ ] **B)** Enabled with 1 host reservation
- [ ] **C)** Enabled with 50% memory
- [ ] **D)** Enabled with 25 CPU

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SDDC Manager enables vSphere HA with admission control disabled by default in the management domain.
 
 
</details>

### 24. Which two tasks are performed by SDDC Manager during lifecycle management?

- [ ] **A)** Running pre-checks before updates
- [ ] **B)** Creating snapshots for rollback
- [ ] **C)** Deploying Cloud Builder VM
- [ ] **D)** Manually configuring NTP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SDDC Manager automatically runs pre-checks and creates snapshots before applying updates.
 
 
</details>

### 25. A deployment fails with 'DNS resolution failure for vcenter.domain.com'. Which log file should be checked first?

```plaintext
Error: DNS resolution failure for vcenter.domain.com
```

- [ ] **A)** /opt/vmware/var/log/cloudbuilder/
- [ ] **B)** /var/log/vmware/vcf/
- [ ] **C)** /var/log/vmware/vcenter-server/
- [ ] **D)** /var/log/vmkernel

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Builder logs are stored in /opt/vmware/var/log/cloudbuilder/ for pre-validation issues.
 
 
</details>

### 26. What is the minimum number of hosts required for a vSAN cluster with RAID-5 erasure coding?

- [ ] **A)** 4
- [ ] **B)** 3
- [ ] **C)** 2
- [ ] **D)** 6

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RAID-5 erasure coding requires a minimum of 4 hosts per vSAN cluster.
 
 
</details>

### 27. Which two components are included in each VCF workload domain?

- [ ] **A)** Dedicated vCenter Server
- [ ] **B)** Dedicated NSX Manager cluster
- [ ] **C)** Cloud Builder VM
- [ ] **D)** Horizon Connection Server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Each workload domain has its own vCenter and NSX Manager; Cloud Builder is only for initial bring-up.
 
 
</details>


---

### **Troubleshooting and Disaster Recovery**

### 28. What is the recommended first step when troubleshooting a VCF issue?

- [ ] **A)** Restart SDDC Manager
- [ ] **B)** Collect evidence via log bundles
- [ ] **C)** Reboot all ESXi hosts
- [ ] **D)** Re-register NSX-T Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The troubleshooting triad emphasizes systematic evidence gathering before any remediation.
 
 
</details>

### 29. Which two components are required for a DR solution using vSphere Replication and SRM?

- [ ] **A)** vSphere Replication Appliance
- [ ] **B)** SDDC Manager
- [ ] **C)** Site Recovery Manager Server
- [ ] **D)** vSAN Witness Host

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> vSphere Replication Appliance handles replication; SRM orchestrates failover.
 
 
</details>

### 30. After examining the NSX-T edge, an administrator runs the command in the code block. What does this command verify?

```text
get logical-switches
```

- [ ] **A)** BGP peer status
- [ ] **B)** Overlay segment configuration
- [ ] **C)** Transport node health
- [ ] **D)** Firewall rules

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The command 'get logical-switches' lists all logical switches, which define overlay segments.
 
 
</details>

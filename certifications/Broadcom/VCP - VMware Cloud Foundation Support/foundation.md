<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Broadcom/VMware%20Cloud%20Foundation%20Support.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>VCP - VMware Cloud Foundation Support</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Architecture and Technologies](#architecture-and-technologies) (7 questions)
- [Installation, Configuration, and Upgrade](#installation-configuration-and-upgrade) (8 questions)
- [Operations, Monitoring, and Automation](#operations-monitoring-and-automation) (5 questions)
- [Product and Solution Planning](#product-and-solution-planning) (4 questions)
- [Troubleshooting](#troubleshooting) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:10.938Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Architecture and Technologies | 7 |
| Installation, Configuration, and Upgrade | 8 |
| Operations, Monitoring, and Automation | 5 |
| Product and Solution Planning | 4 |
| Troubleshooting | 6 |

---

### **Architecture and Technologies**

### 1. What is the primary role of SDDC Manager in VMware Cloud Foundation?

- [ ] **A)** It orchestrates lifecycle management across all workload domains.
- [ ] **B)** It provides the hypervisor for virtual machines.
- [ ] **C)** It manages storage policies for vSAN clusters.
- [ ] **D)** It performs network routing and switching.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SDDC Manager is the centralized orchestration and lifecycle management platform for the entire VCF stack, automating deployment, patching, upgrades, and certificate management.
 
 
</details>

### 2. Which components are typically deployed in the VCF management domain? (Choose two)

- [ ] **A)** SDDC Manager
- [ ] **B)** vCenter Server for management
- [ ] **C)** Production workload VMs
- [ ] **D)** NSX Edge cluster for tenant workloads

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The management domain contains all management VMs: SDDC Manager, vCenter Server, NSX Manager, and the vSAN witness. Tenant workloads run in VI workload domains.
 
 
</details>

### 3. Review the deployment specification snippet provided. What is the purpose of this JSON block in VCF?

```json
{
  "domain": {
    "type": "MANAGEMENT",
    "name": "mgmt-domain",
    "vcenter": {
      "size": "medium",
      "storage": "vsan"
    },
    "nsx": {
      "license": "eval",
      "overlay": "geneve"
    }
  },
  "hosts": ["esxi-01", "esxi-02", "esxi-03"]
}
```

- [ ] **A)** It is the depoySpec.json used during initial bring-up of VCF.
- [ ] **B)** It defines an NSX firewall rule set.
- [ ] **C)** It is a vSAN storage policy template.
- [ ] **D)** It contains credentials for SDDC Manager backup.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The depoySpec.json file is a JSON-based deployment specification used by SDDC Manager to automate the creation of the management domain during the initial bring-up process.
 
 
</details>

### 4. What is the function of VMware vSAN within a VCF architecture?

- [ ] **A)** It provides software-defined storage by pooling local disks from ESXi hosts.
- [ ] **B)** It manages virtual machine networking and security.
- [ ] **C)** It automates lifecycle operations across domains.
- [ ] **D)** It acts as the hypervisor for running VMs.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> vSAN is the software-defined storage layer in VCF, aggregating local disks from ESXi hosts into a distributed shared datastore managed through storage policies.
 
 
</details>

### 5. Which two components are integrated by SDDC Manager in a VCF workload domain? (Choose two)

- [ ] **A)** vSAN
- [ ] **B)** NSX
- [ ] **C)** VMware Horizon
- [ ] **D)** VMware Site Recovery Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Each VCF workload domain includes vSphere, vSAN, and NSX. SDDC Manager orchestrates the deployment and lifecycle of these components. Horizon and SRM are optional add-ons.
 
 
</details>

### 6. Examine the code block from a VCF orchestration script. What action is being performed?

```powershell
Add-VCFHost -DomainId "workload-domain-1" -Host "esxi-prod-05.example.com" -Credentials $cred -NetworkPool "mgmt-pool"
Start-VCFDomainCreation -DomainId "workload-domain-1"
```

- [ ] **A)** Adding a host to a workload domain via SDDC Manager.
- [ ] **B)** Upgrading the NSX Manager appliance.
- [ ] **C)** Configuring a vSAN storage policy.
- [ ] **D)** Creating a vCenter Server backup.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The PowerCLI snippet shows the 'Add-VCFHost' cmdlet, which is used by SDDC Manager to add an ESXi host to a workload domain, ensuring lifecycle consistency.
 
 
</details>

### 7. What is the purpose of an availability zone in a VCF workload domain?

- [ ] **A)** It provides failure isolation at the rack or infrastructure level.
- [ ] **B)** It separates management and tenant workloads into different domains.
- [ ] **C)** It defines the network segmentation between domains.
- [ ] **D)** It controls vSAN storage policy inheritance.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Availability zones group clusters that share common infrastructure (power, cooling, network) to prevent a single failure from affecting the entire workload domain.
 
 
</details>


---

### **Installation, Configuration, and Upgrade**

### 8. Which component is the first to be deployed during a fresh VCF installation?

- [ ] **A)** SDDC Manager VM
- [ ] **B)** vCenter Server
- [ ] **C)** VCF Builder VM
- [ ] **D)** NSX Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The VCF Builder VM is the bootstrap appliance used to deploy SDDC Manager and the management domain; it is the first component deployed.
 
 
</details>

### 9. Which of the following are required before deploying the VCF Builder VM? (Select two.)

- [ ] **A)** DNS server configured
- [ ] **B)** vCenter Server already deployed
- [ ] **C)** NTP server reachable
- [ ] **D)** License key entered

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The document lists DNS and NTP as prerequisites; the license key is entered later in the wizard, not before builder deployment.
 
 
</details>

### 10. Given the following log snippet from a failed deployment, what is the most likely cause?

```text
Pre-check: Host file entries inconsistent — SDDC Manager resolves vcenter.domain.local to 10.1.1.11 but vCenter returns 10.1.1.10.
```

- [ ] **A)** DNS misconfiguration
- [ ] **B)** Stale /etc/hosts entry on SDDC Manager
- [ ] **C)** vCenter certificate expired
- [ ] **D)** NTP drift between components

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The log shows an IP resolution mismatch – the SDDC Manager resolves the vCenter FQDN to an old IP due to a stale hosts file.
 
 
</details>

### 11. What is the correct order for upgrading VCF components?

- [ ] **A)** Management domain first, then workload domains
- [ ] **B)** Workload domains first, then management domain
- [ ] **C)** Any order is supported
- [ ] **D)** All domains simultaneously

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The management domain must be upgraded first because it hosts SDDC Manager and core management components.
 
 
</details>

### 12. Which are valid methods to obtain LCM bundles in an air-gapped VCF environment? (Select two.)

- [ ] **A)** Direct download from Broadcom portal via SDDC Manager
- [ ] **B)** Manual download from customer portal and upload via UI
- [ ] **C)** Using the vcf update download command
- [ ] **D)** Uploading the offline bundle using vcf update upload

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Offline environments require manual download and import; the download command only works with internet access.
 
 
</details>

### 13. Examine the command: 'vcf update upload /path/to/bundle.vcfb'. What does this command achieve?

```bash
vcf update upload /path/to/bundle.vcfb
```

- [ ] **A)** Downloads a bundle from the internet
- [ ] **B)** Uploads a local bundle to the SDDC Manager depot
- [ ] **C)** Installs the patch immediately
- [ ] **D)** Runs pre-checks for an update

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The vcf update upload command is used to import locally downloaded bundles into the SDDC Manager for offline upgrades.
 
 
</details>

### 14. Where is the VCF Builder VM deployed during a fresh installation?

- [ ] **A)** On the management domain's vSAN datastore
- [ ] **B)** On a prepared ESXi host using vSphere Client
- [ ] **C)** Inside the SDDC Manager VM
- [ ] **D)** On a workload domain cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The builder OVA is deployed on a single ESXi host that is already prepared and connected to the management network.
 
 
</details>

### 15. Which of the following are common causes of validation failures during a fresh VCF installation? (Select two.)

- [ ] **A)** Incorrect DNS records
- [ ] **B)** License key already used
- [ ] **C)** Missing VLAN on physical switches
- [ ] **D)** vCenter already deployed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The document highlights DNS misconfiguration and missing VLANs as common pitfalls; license issues are not mentioned as validation failures.
 
 
</details>


---

### **Operations, Monitoring, and Automation**

### 16. Which tool is the primary platform for comprehensive health and performance monitoring in VMware Cloud Foundation?

- [ ] **A)** VMware Aria Operations
- [ ] **B)** vCenter Server
- [ ] **C)** SDDC Manager
- [ ] **D)** Skyline Health

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> VMware Aria Operations is the primary monitoring platform in VCF, collecting metrics from all components via management packs.
 
 
</details>

### 17. Which two metrics indicate vSAN performance degradation according to VMware best practices?

- [ ] **A)** Read latency > 10ms
- [ ] **B)** Write latency > 5ms
- [ ] **C)** CPU ready time > 5%
- [ ] **D)** Memory ballooning > 0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Read latency above 10ms and write latency above 5ms are vSAN performance degradation indicators per VMware best practices.
 
 
</details>

### 18. What HTTP method and endpoint should be used to initiate a domain upgrade via SDDC Manager API?

```bash
curl -X POST "https://sddc-manager.example.com/v1/domains/domain-123/upgrade" \
  -H "Authorization: Bearer <token>" \
  -H "Content-Type: application/json" \
  -d '{"bundleId": "bundle-456", "scheduledTime": "2023-10-01T02:00:00Z"}'
```

- [ ] **A)** POST /v1/domains/{domainId}/upgrade
- [ ] **B)** GET /v1/domains/{domainId}/upgrade
- [ ] **C)** PUT /v1/domains/{domainId}/upgrade
- [ ] **D)** POST /v1/domains/{domainId}/start-upgrade

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The correct API to initiate a domain upgrade is POST to the /v1/domains/{domainId}/upgrade endpoint.
 
 
</details>

### 19. What is the first step when decommissioning a workload domain in VCF?

- [ ] **A)** Evacuate all virtual machines
- [ ] **B)** Delete the domain from SDDC Manager
- [ ] **C)** Remove all ESXi hosts
- [ ] **D)** Destroy the vSAN datastore

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> All VMs must be evacuated to another domain or storage before any decommissioning steps to prevent data loss.
 
 
</details>

### 20. Which two pre-checks does SDDC Manager perform before adding a host to an existing vSAN cluster?

- [ ] **A)** Verify host firmware compatibility with cluster baseline
- [ ] **B)** Validate vSAN disk group configuration on the host
- [ ] **C)** Delete existing vSAN objects on the host
- [ ] **D)** Place host in maintenance mode manually

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SDDC Manager checks host firmware compatibility and validates the vSAN disk group configuration to ensure successful integration.
 
 
</details>


---

### **Product and Solution Planning**

### 21. What is the primary source for verifying hardware compatibility when planning a VMware Cloud Foundation deployment?

- [ ] **A)** General vSphere Hardware Compatibility List (HCL)
- [ ] **B)** VMware Compatibility Guide (VCG) filtered for VCF
- [ ] **C)** Vendor-specific firmware matrix
- [ ] **D)** VMware Knowledge Base articles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> VMware Cloud Foundation requires that all hardware components be listed in the VCG with the VCF filter. The general vSphere HCL is necessary but not sufficient; VCF has additional integration testing. Vendor firmware matrices and KB articles supplement but do not replace the VCG.
 
 
</details>

### 22. Which of the following are correct statements about VCF deployment planning? (Select two.)

- [ ] **A)** SDDC Manager requires a persistent boot device such as a local SSD.
- [ ] **B)** vSAN storage traffic must operate over networks configured with jumbo frames (MTU 9000).
- [ ] **C)** The management domain can be deployed with a minimum of two hosts.
- [ ] **D)** NSX overlay transport zones use default MTU 1500 for optimal performance.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VCF 5.x+ does not support SD card or USB boot devices; a persistent local SSD is required. vSAN requires jumbo frames (MTU 9000) for replication traffic; default 1500 causes packet fragmentation. A minimum of three hosts is required for a management domain, and NSX overlay transport zones require jumbo frames (MTU 1600+) to avoid fragmentation.
 
 
</details>

### 23. In the VCF deployment plan snippet above, what is the most critical design flaw?

```yaml
vcf:
  version: 5.2
  management_domain:
    hosts: 3
    network:
      mtu: 1500
  workload_domain:
    hosts: 4
```

- [ ] **A)** The management domain is configured with only three hosts.
- [ ] **B)** The MTU for the management network is set to 1500 instead of 9000.
- [ ] **C)** The workload domain has too many hosts.
- [ ] **D)** VCF version 5.2 is not listed in the Compatibility Guide.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> VCF requires jumbo frames (MTU 9000) on management, vSAN, and overlay networks. Setting MTU to 1500 will cause packet fragmentation and severe performance issues. Three hosts in the management domain is acceptable (though four is recommended), and VCF 5.2 is a valid version. The workload domain host count is within limits.
 
 
</details>

### 24. What is the minimum number of cores per processor that must be licensed for a VCF subscription?

- [ ] **A)** 8 cores
- [ ] **B)** 16 cores
- [ ] **C)** 32 cores
- [ ] **D)** 10 cores

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> VMware licenses VCF per-core with a minimum of 16 cores per physical processor socket. Even if a CPU has fewer than 16 cores (e.g., 8 or 10), you must license 16 cores per socket. For CPUs with more than 16 cores, you license the actual core count.
 
 
</details>


---

### **Troubleshooting**

### 25. What does a yellow status on vSAN Health Service indicate?

- [ ] **A)** Healthy
- [ ] **B)** At risk or degraded
- [ ] **C)** Not applicable
- [ ] **D)** Error

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Yellow status indicates a potential issue or at-risk state, not immediate failure.
 
 
</details>

### 26. Which tools are used for vSAN health diagnostics? (Choose two)

- [ ] **A)** vSAN Skyline Health
- [ ] **B)** RVC vsan commands
- [ ] **C)** NSX Manager
- [ ] **D)** SDDC Manager LCM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> vSAN Skyline Health and RVC are designed for vSAN diagnostics.
 
 
</details>

### 27. Examine the code block. What is the underlying command used for the output?

```json
{
  "cluster-health": {
    "status": "green",
    "checks": [
      {
        "name": "Object Health",
        "status": "green"
      }
    ]
  }
}
```

- [ ] **A)** esxcli vsan cluster list
- [ ] **B)** esxcli vsan health cluster list
- [ ] **C)** esxcli vsan storage list
- [ ] **D)** esxcli vsan network list

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The JSON output with health check results corresponds to esxcli vsan health cluster list.
 
 
</details>

### 28. What is the first step in VCF troubleshooting methodology?

- [ ] **A)** Collect logs
- [ ] **B)** Identify symptom
- [ ] **C)** Remediate
- [ ] **D)** Escalate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The methodology begins with identifying the symptom from alerts or reports.
 
 
</details>

### 29. Which two components are part of NSX policy conflict diagnosis?

- [ ] **A)** Distributed Firewall rules
- [ ] **B)** Gateway Firewall rules
- [ ] **C)** vCenter alarms
- [ ] **D)** vSAN health

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Both DFW and Gateway FW rules need cross-checking for conflicts.
 
 
</details>

### 30. The code shows a log snippet. Which service generated this log?

```plaintext
2025-03-20 10:15:32 ERROR [lcm] Certificate chain validation failed during upgrade step
```

- [ ] **A)** Certificate Manager
- [ ] **B)** Lifecycle Management (LCM)
- [ ] **C)** Domain Manager
- [ ] **D)** Credential Management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The log path /var/log/vmware/vcf/lcm indicates LCM service.
 
 
</details>

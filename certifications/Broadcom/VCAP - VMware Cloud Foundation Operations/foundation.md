<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Broadcom/Cloud%20Foundation%20Operations.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>VCAP - VMware Cloud Foundation Operations</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Automation and Lifecycle Management](#automation-and-lifecycle-management) (4 questions)
- [Networking and Security](#networking-and-security) (6 questions)
- [SDDC Operations and Management](#sddc-operations-and-management) (9 questions)
- [Software-Defined Data Center (SDDC) Design and Deploy](#software-defined-data-center-sddc-design-and-deploy) (6 questions)
- [Storage and Data Protection](#storage-and-data-protection) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:57.912Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Automation and Lifecycle Management | 4 |
| Networking and Security | 6 |
| SDDC Operations and Management | 9 |
| Software-Defined Data Center (SDDC) Design and Deploy | 6 |
| Storage and Data Protection | 5 |

---

### **Automation and Lifecycle Management**

### 1. What authentication method is required for SDDC Manager API calls?

- [ ] **A)** Session cookies
- [ ] **B)** Bearer token
- [ ] **C)** Basic authentication
- [ ] **D)** OAuth 2.0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SDDC Manager API authentication uses a bearer token obtained from the /v1/tokens endpoint.
 
 
</details>

### 2. Which two prerequisites must be satisfied before deploying a workload domain with the VCF API?

- [ ] **A)** Management domain is operational
- [ ] **B)** Hosts are in AVAILABLE state
- [ ] **C)** SDDC Manager is rebooted
- [ ] **D)** NSX Manager license key is not required

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The management domain must be functional and hosts must be in AVAILABLE state before domain deployment.
 
 
</details>

### 3. Based on the provided PowerCLI snippet, what does the Get-VCFCertificate cmdlet accomplish?

```powershell
Connect-VCF -Server sddc01.example.com -User admin -Password ****
Get-VCFCertificate -DomainType MANAGEMENT
```

- [ ] **A)** To generate a new certificate signing request
- [ ] **B)** To retrieve all certificates for a given domain type
- [ ] **C)** To replace expired certificates
- [ ] **D)** To validate certificate chain

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Get-VCFCertificate retrieves certificate information for the specified domain type from SDDC Manager.
 
 
</details>

### 4. Why is Terraform preferred over Ansible for provisioning VCF resources?

- [ ] **A)** Procedural execution
- [ ] **B)** Stateful declarative management
- [ ] **C)** Better configuration management
- [ ] **D)** Simpler syntax

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Terraform is stateful and declarative, making it ideal for provisioning and lifecycle management of VCF resources.
 
 
</details>


---

### **Networking and Security**

### 5. What is the primary encapsulation protocol used by NSX-T Data Center for overlay segments?

- [ ] **A)** VXLAN
- [ ] **B)** Geneve
- [ ] **C)** STT
- [ ] **D)** NVGRE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Geneve is the encapsulation protocol used for overlay segments in NSX-T, providing flexibility and scalability.
 
 
</details>

### 6. Which two components are part of the NSX-T logical routing architecture? (Choose two)

- [ ] **A)** Tier-0 Gateway
- [ ] **B)** Tier-1 Gateway
- [ ] **C)** Distributed Firewall
- [ ] **D)** Transport Zone

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Tier-0 and Tier-1 gateways provide north-south and east-west routing respectively in NSX-T.
 
 
</details>

### 7. Review the output of the NSX CLI command. What is the operational state of the logical router?

```plaintext
Logical Router: LR-1
Type: Service Router
State: Active
```

- [ ] **A)** Active
- [ ] **B)** Standby
- [ ] **C)** Disabled
- [ ] **D)** Unknown

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The output shows 'State: Active', indicating the logical router is currently operational.
 
 
</details>

### 8. Where is the Distributed Firewall (DFW) enforced in NSX-T?

- [ ] **A)** At the virtual switch
- [ ] **B)** At the vNIC of the virtual machine
- [ ] **C)** At the Tier-1 gateway
- [ ] **D)** At the physical switch

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The DFW enforces security at the vNIC level within the ESXi hypervisor kernel for east-west traffic.
 
 
</details>

### 9. Which two methods can be used to define security group membership dynamically in NSX-T? (Choose two)

- [ ] **A)** Static IP sets
- [ ] **B)** Dynamic tags
- [ ] **C)** MAC addresses
- [ ] **D)** VM names

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Dynamic membership uses tags or VM names to include VMs automatically, enabling scalable grouping.
 
 
</details>

### 10. Refer to the Traceflow output. What does an 'Allow' action indicate?

```plaintext
Traceflow Result:
Source VM: VM-A
Destination VM: VM-B
Hop 1: Segment-1
Hop 2: DFW (Action: Allow)
Hop 3: Tier-1 Gateway (Action: Forward)
```

- [ ] **A)** East-west traffic is permitted
- [ ] **B)** The gateway firewall allowed the traffic
- [ ] **C)** A routing issue exists
- [ ] **D)** The packet was dropped

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Traceflow showing 'Action: Allow' means the Distributed Firewall permitted the packet at that hop.
 
 
</details>


---

### **SDDC Operations and Management**

### 11. What action does SDDC Manager carry out prior to staging an upgrade bundle?

- [ ] **A)** Prerequisites check
- [ ] **B)** Performance tuning
- [ ] **C)** Capacity planning
- [ ] **D)** Backup verification

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SDDC Manager runs pre-checks including disk space, DNS, and DRS before staging bundles.
 
 
</details>

### 12. Which two tools are used for capacity planning in VCF according to the playbook?

- [ ] **A)** vRealize Operations
- [ ] **B)** SDDC Manager
- [ ] **C)** vCenter Server
- [ ] **D)** VMware Update Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> vROps predicts trending; SDDC Manager provides initial sizing data. vCenter only shows real-time stats.
 
 
</details>

### 13. Examine the command below. What is its purpose?

```bash
vcf-backup-restore --restore --backup-file /share/backup.bkp
```

- [ ] **A)** Restore SDDC Manager from backup
- [ ] **B)** Take a snapshot of vCenter
- [ ] **C)** Upgrade NSX Manager
- [ ] **D)** Back up vCenter database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command 'vcf-backup-restore --restore' performs SDDC Manager restoration.
 
 
</details>

### 14. Which component must be restored first after a disaster in VCF?

- [ ] **A)** SDDC Manager
- [ ] **B)** Workload domain vCenter
- [ ] **C)** NSX Manager
- [ ] **D)** vSAN datastore

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SDDC Manager must be restored first to re-establish management plane and inventory.
 
 
</details>

### 15. Which two are required to create a proactive alert from Log Insight to vROps?

- [ ] **A)** Log Insight Management Pack for vROps
- [ ] **B)** Custom log query in Log Insight
- [ ] **C)** vCenter syslog configuration
- [ ] **D)** SNMP trap receiver in vROps

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The management pack and a custom alert-in-log query enable the integration.
 
 
</details>

### 16. Read the SNIPPET. What is the purpose of the 'scoped' attribute?

```json
{
  "role": "Security Operator",
  "scope": "Org: Tenant-A"
}
```

- [ ] **A)** Restricts NSX role to a specific tenant organization
- [ ] **B)** Enables global admin privileges
- [ ] **C)** Defines the NSX Manager cluster size
- [ ] **D)** Sets the firewall rule priority

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'scoped' attribute ties an NSX role to a specific tenant organization for RBAC.
 
 
</details>

### 17. What is the correct order for upgrading components in a VCF management domain?

- [ ] **A)** SDDC Manager first, then vCenter, ESXi, NSX
- [ ] **B)** vCenter first, then ESXi, NSX, SDDC Manager
- [ ] **C)** NSX first, then vCenter, ESXi, SDDC Manager
- [ ] **D)** ESXi first, then vCenter, NSX, SDDC Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SDDC Manager must be upgraded before domain components; then vCenter, ESXi, and NSX.
 
 
</details>

### 18. Which two metrics indicate CPU contention in a VCF cluster?

- [ ] **A)** CPU ready time > 5%
- [ ] **B)** Memory swap rate > 0 KB/s
- [ ] **C)** High vSAN latency
- [ ] **D)** Elevated co-stop time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CPU ready time over 5% and co-stop time indicate vCPU scheduling contention.
 
 
</details>

### 19. Examine this vLCM image. What does it define?

```yaml
image: "ESXi-7.0U3-20328353"
addons:
  - "firmware-7.0-addon"
  - "driver-nic-addon"
```

- [ ] **A)** ESXi base image and add-ons
- [ ] **B)** vCenter version and build
- [ ] **C)** NSX edge cluster topology
- [ ] **D)** vSAN disk group configuration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The image includes a base ESXi version with firmware and driver add-ons for vLCM.
 
 
</details>


---

### **Software-Defined Data Center (SDDC) Design and Deploy**

### 20. What is the primary purpose of requirement categorization in SDDC design?

- [ ] **A)** Functional vs. Non-functional
- [ ] **B)** Hardware vs. Software
- [ ] **C)** Availability vs. Performance
- [ ] **D)** Logical vs. Physical

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> It separates what the SDDC must do from performance characteristics, guiding component mapping.
 
 
</details>

### 21. Which components are part of a VI workload domain? (Select two)

- [ ] **A)** vCenter Server
- [ ] **B)** NSX Manager
- [ ] **C)** vRealize Operations
- [ ] **D)** vSAN without policy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VI workload domains have their own vCenter and NSX Manager; vRealize Operations is in management domain.
 
 
</details>

### 22. What does the 'managementPool' parameter define in the deployment manifest?

```json
{"managementPool": {"vlanId": 100, "subnet": "10.10.0.0/21"}}
```

- [ ] **A)** Defines VLAN for management traffic
- [ ] **B)** Defines VLAN for workload traffic
- [ ] **C)** Defines storage network
- [ ] **D)** Defines vMotion network

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The management pool provides network parameters for the management cluster during initial bring-up.
 
 
</details>

### 23. What is the recommended minimum MTU for an NSX stretched cluster?

- [ ] **A)** 1500
- [ ] **B)** 1600
- [ ] **C)** 9000
- [ ] **D)** 1400

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> NSX stretched clusters require MTU of at least 1600 bytes to accommodate Geneve headers.
 
 
</details>

### 24. Which two are vSAN storage policy capabilities? (Select two)

- [ ] **A)** Failures to Tolerate (FTT)
- [ ] **B)** Stripe Width
- [ ] **C)** Encryption
- [ ] **D)** IOPS Limit

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> FTT and Stripe Width are core vSAN policy rules; encryption is a separate service.
 
 
</details>

### 25. What does the API call GET /v1/workflows?status=FAILED return?

```http
GET /v1/workflows?status=FAILED
```

- [ ] **A)** List of failed workflows
- [ ] **B)** List of all workflows
- [ ] **C)** Workflow ID
- [ ] **D)** Error logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> It filters workflows with status FAILED, helping identify deployment issues.
 
 
</details>


---

### **Storage and Data Protection**

### 26. What does the 'Number of Failures to Tolerate' (PFTT) attribute in a vSAN storage policy define?

- [ ] **A)** The maximum number of concurrent host, disk, or network failures the object can survive while remaining accessible.
- [ ] **B)** The percentage of flash cache capacity reserved for the VMDK.
- [ ] **C)** The number of disk groups across which each replica is striped.
- [ ] **D)** The percentage of the virtual disk size that is thick-provisioned.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PFTT defines how many concurrent failures the object can tolerate. Other options describe cache reservation, stripe width, or object space reservation.
 
 
</details>

### 27. Which two Failure Tolerance Methods (FTM) are supported by vSAN for creating storage policies?

- [ ] **A)** RAID-1 (Mirroring)
- [ ] **B)** RAID-5 (Erasure Coding 3+1)
- [ ] **C)** RAID-0 (Striping)
- [ ] **D)** RAID-10 (Stripe of Mirrors)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> vSAN supports RAID-1 (mirroring) and RAID-5/6 erasure coding. RAID-0 and RAID-10 are not native FTM options.
 
 
</details>

### 28. Examine the output from the vSAN health service: 'Object: db-vm.vmdk, Policy: FTT=1, Stripe Width=4, Compliance: Non-Compliant'. What is the most likely cause of non-compliance?

```plaintext
Object: db-vm.vmdk
Policy: FTT=1, Stripe Width=4
Compliance: Non-Compliant
```

- [ ] **A)** The cluster has fewer than 4 disk groups, making stripe width unsatisfiable.
- [ ] **B)** The cluster has fewer than 4 hosts to satisfy FTT=1.
- [ ] **C)** Object Space Reservation is set too high.
- [ ] **D)** Cache Reservation is not set for the VM.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Stripe width cannot exceed the number of disk groups in the cluster. Insufficient disk groups cause non-compliance.
 
 
</details>

### 29. What is the primary purpose of vSAN HCI Mesh?

- [ ] **A)** To enable cross-cluster storage consumption by mounting remote vSAN datastores.
- [ ] **B)** To provide synchronous replication between two sites for disaster recovery.
- [ ] **C)** To encrypt data at rest using a Key Management Server.
- [ ] **D)** To guarantee I/O performance with Quality of Service policies.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> HCI Mesh allows a vSAN cluster to access another cluster's datastore as a remote datastore, enabling capacity federation.
 
 
</details>

### 30. Which two components are required to configure a vSAN stretched cluster?

- [ ] **A)** A witness host in a third location
- [ ] **B)** Low-latency network links (<5 ms RTT) between sites
- [ ] **C)** A dedicated Key Management Server for encryption
- [ ] **D)** Identical storage capacity in both sites

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A stretched cluster requires a witness for quorum and low-latency links for synchronous replication. KMS and identical capacities are not mandatory.
 
 
</details>

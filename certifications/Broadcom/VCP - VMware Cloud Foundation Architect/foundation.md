<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Broadcom/VMware%20Certified%20Professional%20-%20VMware%20Cloud%20Foundation%20Architect" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>VCP - VMware Cloud Foundation Architect</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Architecture and Design](#architecture-and-design) (7 questions)
- [Deploy and Configure](#deploy-and-configure) (6 questions)
- [Management and Operations](#management-and-operations) (6 questions)
- [Security and Compliance](#security-and-compliance) (6 questions)
- [Troubleshooting and Optimization](#troubleshooting-and-optimization) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:08.302Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Architecture and Design | 7 |
| Deploy and Configure | 6 |
| Management and Operations | 6 |
| Security and Compliance | 6 |
| Troubleshooting and Optimization | 5 |

---

### **Architecture and Design**

### 1. What is the first step in designing a VMware Cloud Foundation (VCF) architecture based on business requirements?

- [ ] **A)** Requirement gathering and mapping
- [ ] **B)** Selecting the hardware vendors
- [ ] **C)** Deploying SDDC Manager
- [ ] **D)** Configuring vSAN storage policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The first step is gathering and mapping business requirements to technical decisions, as documented in the VMware Cloud Foundation Design Guide.
 
 
</details>

### 2. Which of the following are key design constructs for organizing resources in VCF? (Choose two)

- [ ] **A)** Workload Domain
- [ ] **B)** Availability Zone
- [ ] **C)** Resource Pool
- [ ] **D)** vSphere Cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Workload domains provide policy-driven boundaries; resource pools enable fine-grained resource allocation within clusters. Availability zones and clusters are also used but not as primary organizational constructs for resource isolation.
 
 
</details>

### 3. Refer to the command output. Which VCF component is being updated first according to the lifecycle sequence shown?

```text
Upgrade Sequence:
1. SDDC Manager (v4.5 -> v5.0)
2. vCenter Server
3. ESXi hosts (with vSAN)
4. NSX
```

- [ ] **A)** SDDC Manager
- [ ] **B)** vCenter Server
- [ ] **C)** ESXi hosts
- [ ] **D)** NSX Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SDDC Manager is always upgraded first because it orchestrates all subsequent component upgrades.
 
 
</details>

### 4. What is the primary role of SDDC Manager in VCF lifecycle management?

- [ ] **A)** It orchestrates upgrades and patches across all workload domains
- [ ] **B)** It provides storage policies for vSAN
- [ ] **C)** It manages NSX distributed firewall rules
- [ ] **D)** It balances workloads across clusters

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SDDC Manager is the brain of VCF, responsible for lifecycle operations including patching and upgrades.
 
 
</details>

### 5. Which statements are true about VCF workload domains? (Choose two)

- [ ] **A)** Each workload domain can have its own vCenter Server
- [ ] **B)** Workload domains always stretch across multiple sites
- [ ] **C)** Management and tenant workloads can be placed in the same domain without restrictions
- [ ] **D)** A VCF instance supports up to 25 workload domains

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Workload domains can have dedicated vCenter Servers; VCF supports up to 25 workload domains per instance. They are not required to be stretched, and management components should be separate from tenant workloads.
 
 
</details>

### 6. Considering the vSAN topology snippet, which cluster type requires a separate witness appliance?

```text
vSAN Cluster Types:
- Standard: single site, no witness
- Stretched: two active sites + witness
- Two-node: two hosts + witness
```

- [ ] **A)** Stretched cluster
- [ ] **B)** Standard cluster
- [ ] **C)** vSAN single-host cluster
- [ ] **D)** Federated cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A vSAN stretched cluster uses a witness appliance in a third location to maintain quorum if one site fails.
 
 
</details>

### 7. What is the main purpose of an availability zone in a VCF workload domain?

- [ ] **A)** Fault isolation across different failure domains
- [ ] **B)** Fine-grained resource control for VMs
- [ ] **C)** Multi-tenancy through separate vCenter Servers
- [ ] **D)** Lifecycle management automation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Availability zones group clusters to provide fault isolation, ensuring workloads survive failure of a physical infrastructure component.
 
 
</details>


---

### **Deploy and Configure**

### 8. What is the initial step performed by SDDC Manager in the management domain bring-up workflow?

- [ ] **A)** Deploy vCenter Server
- [ ] **B)** Validate prerequisites
- [ ] **C)** Configure vSAN storage
- [ ] **D)** Deploy NSX Manager appliances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The bring-up workflow begins with prerequisite validation including DNS, NTP, and network connectivity.
 
 
</details>

### 9. Which two statements correctly describe characteristics of the management workload domain in VCF?

- [ ] **A)** CPU overcommit ratio of 4:1 is recommended for optimal performance
- [ ] **B)** No overcommit on CPU or memory is applied
- [ ] **C)** Typical cluster size ranges from 3 to 4 nodes
- [ ] **D)** Storage policy uses RAID-5 to reduce costs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Management domains require guaranteed resources with no overcommit and are typically 3-4 nodes for high availability.
 
 
</details>

### 10. Review the following NSX-T Tier-0 gateway configuration snippet. What high availability mode is defined?

```json
{
  "high_availability_mode": "ACTIVE_ACTIVE",
  "stateful_services": false
}
```

- [ ] **A)** Active-Standby
- [ ] **B)** Active-Active
- [ ] **C)** Standalone
- [ ] **D)** Dynamic Active-Passive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 'ACTIVE_ACTIVE' high availability mode supports stateless routing only.
 
 
</details>

### 11. In a vSAN stretched cluster, what is the maximum number of site failures the primary Failures to Tolerate (FTT) setting can protect against?

- [ ] **A)** 0
- [ ] **B)** 1
- [ ] **C)** 2
- [ ] **D)** 3

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Stretched clusters support only one site failure at the primary level due to two data sites plus witness.
 
 
</details>

### 12. Which two prerequisites are essential for integrating a third-party hardware management system with SDDC Manager?

- [ ] **A)** The hardware management system must be registered as a vCenter extension
- [ ] **B)** The hardware management API must be reachable from the SDDC Manager network
- [ ] **C)** Out-of-band management network connectivity is required for server discovery
- [ ] **D)** All compute nodes must have identical firmware versions at the time of registration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> SDDC Manager uses the hardware API for discovery and firmware checks; OOB network must be separate from production traffic.
 
 
</details>

### 13. The SDDC Manager bring-up wizard returns the error shown. What is the likely root cause?

```text
Error: Failed to resolve FQDN for management vCenter. Ensure DNS records are configured correctly.
```

- [ ] **A)** Incorrect NTP server configuration
- [ ] **B)** Missing DNS A/PTR records for the management vCenter FQDN
- [ ] **C)** Invalid ESXi root credentials
- [ ] **D)** Firewall blocking port 443 to the vCenter

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The error explicitly states DNS resolution failure; verifying forward/reverse DNS records is the required step.
 
 
</details>


---

### **Management and Operations**

### 14. Which VCF component acts as the single control plane for all upgrade and patching activities?

- [ ] **A)** SDDC Manager
- [ ] **B)** vCenter Server
- [ ] **C)** NSX Manager
- [ ] **D)** vSphere Replication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SDDC Manager is the single control plane that orchestrates all upgrade and patching activities across the VCF stack, eliminating individual component management.
 
 
</details>

### 15. Which two are critical aspects of VCF lifecycle management? (Select two)

- [ ] **A)** Upgrade sequence from management domain to workload domains
- [ ] **B)** Using any version regardless of BOM
- [ ] **C)** Certificate rotation is optional
- [ ] **D)** Pre-upgrade health checks are mandatory

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> The upgrade must start with the management domain, and pre-upgrade health checks are mandatory to prevent failures during the lifecycle operation.
 
 
</details>

### 16. Examine the following API call. What does it do? (Single Choice)

```bash
curl -X GET https://sddc-manager.example.com/v1/tasks/1234-5678 -H 'Authorization: Bearer token'
```

- [ ] **A)** Initiate an upgrade
- [ ] **B)** Check task status
- [ ] **C)** Rotate certificates
- [ ] **D)** Delete a workload domain

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The API call is a GET request to /v1/tasks/{taskId} which retrieves the status of a previously submitted task, such as an upgrade.
 
 
</details>

### 17. During a VCF lifecycle upgrade, which component must be upgraded first?

- [ ] **A)** ESXi hosts
- [ ] **B)** vCenter Server
- [ ] **C)** SDDC Manager
- [ ] **D)** NSX Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The SDDC Manager must be upgraded first to avoid API mismatch and ensure it can manage the new component versions.
 
 
</details>

### 18. Which two tools are commonly used to monitor resource utilization in VCF? (Select two)

- [ ] **A)** vRealize Operations
- [ ] **B)** vSphere Replication
- [ ] **C)** Site Recovery Manager
- [ ] **D)** vCenter Server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> vRealize Operations provides predictive analytics and vCenter Server offers real-time performance charts for resource utilization monitoring.
 
 
</details>

### 19. Analyze the alert definition snippet. Which two components are involved? (Multiple Select)

```json
{
  "alertDefinition": {
    "name": "vCenter and vSAN Health",
    "symptoms": [
      { "property": "vCenter:HostConnectionState", "condition": "not equal to connected" },
      { "property": "vSAN:DiskLatency", "condition": "> 10ms" }
    ]
  }
}
```

- [ ] **A)** vCenter
- [ ] **B)** vSAN
- [ ] **C)** NSX
- [ ] **D)** SDDC Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The alert definition includes symptoms for vCenter (e.g., host connection state) and vSAN (e.g., disk latency), indicating both components are monitored.
 
 
</details>


---

### **Security and Compliance**

### 20. What is the core philosophy of a zero-trust security model as implemented by NSX Distributed Firewall?

- [ ] **A)** Never trust, always verify. No entity is trusted by default.
- [ ] **B)** Trust but verify all network traffic.
- [ ] **C)** Block all inbound traffic and allow all outbound traffic.
- [ ] **D)** Use micro-segmentation to isolate workloads only.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The zero-trust model operates on \"never trust, always verify\" without implicit trust.
 
 
</details>

### 21. Which two characteristics accurately describe the NSX Distributed Firewall in VCF?

- [ ] **A)** It operates at the hypervisor kernel level.
- [ ] **B)** It requires a physical firewall appliance.
- [ ] **C)** It enforces policies at wire speed without hair-pinning.
- [ ] **D)** It only filters north-south traffic.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> DFW is hypervisor-based, operates at kernel level, and enforces east-west traffic.
 
 
</details>

### 22. Which NSX feature prevents IP/MAC address spoofing in a zero-trust environment?

```json
{"spoofguard_policy": {"enabled": true, "mode": "VM_and_MAC_spoofing"}}
```

- [ ] **A)** SpoofGuard
- [ ] **B)** Identity Firewall
- [ ] **C)** IDS/IPS
- [ ] **D)** Distributed Firewall

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SpoofGuard validates source IP against assigned IP, preventing spoofing.
 
 
</details>

### 23. In VCF SDDC Manager, which built-in role can configure identity sources and perform domain join?

- [ ] **A)** SUPER_ADMIN
- [ ] **B)** ADMIN
- [ ] **C)** USER
- [ ] **D)** AUDITOR

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Only SUPER_ADMIN has privileges for identity source configuration and domain join.
 
 
</details>

### 24. Which two prerequisites must be met before enabling vSAN encryption in VCF?

- [ ] **A)** A key management server (KMS) registered with vCenter
- [ ] **B)** All ESXi hosts must have TPM 2.0 for key caching
- [ ] **C)** vMotion encryption must be enabled
- [ ] **D)** The vSAN cluster must be in a stretched configuration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> vSAN encryption requires a KMS and TPM for key caching.
 
 
</details>

### 25. Which tool provides pre-built dashboards and alerts for regulatory compliance in VCF?

```bash
loginsight-cli install_content_pack --pack PCI-DSS.v1.0.0.pak
```

- [ ] **A)** vRealize Log Insight with compliance packs
- [ ] **B)** vCenter Server with default logging
- [ ] **C)** NSX Manager audit logs
- [ ] **D)** SDDC Manager compliance dashboard

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Compliance packs in Log Insight provide mapped controls and alerts.
 
 
</details>


---

### **Troubleshooting and Optimization**

### 26. What is the most common cause of VCF deployment failure?

- [ ] **A)** Environmental issues like DNS or NTP misconfiguration
- [ ] **B)** A bug in the VCF software code
- [ ] **C)** Insufficient CPU resources on the management domain hosts
- [ ] **D)** Corruption of the SDDC Manager database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Over 70% of VCF deployment failures are due to environmental issues such as time synchronization (NTP) drift, DNS record problems, or incorrect switch MTU settings.
 
 
</details>

### 27. Which tools or commands can be used to verify NSX-T overlay connectivity? (Choose two.)

- [ ] **A)** nsxdi-cli
- [ ] **B)** get tunnel command
- [ ] **C)** Standard ping utility
- [ ] **D)** esxtop command

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The nsxdi-cli and the get tunnel command are specifically designed for NSX-T troubleshooting. Standard ping only tests Layer 3 reachability, and esxtop is for performance monitoring.
 
 
</details>

### 28. An architect needs to collect logs for a problem that spans both the management domain and a VI workload domain. Which Skyline Health Diagnostics scope should be used?

```bash
sddc-manager collect-logs --scope full
```

- [ ] **A)** Single host
- [ ] **B)** Cluster
- [ ] **C)** Workload domain
- [ ] **D)** Full VCF instance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> The full VCF instance scope collects logs from all domains and is required for cross-domain correlation, as the SDDC Manager coordinates external services.
 
 
</details>

### 29. Which DRS rule enforcement level ensures that VMs are always placed on a specific host group?

- [ ] **A)** Must run on hosts in group
- [ ] **B)** Should run on hosts in group
- [ ] **C)** Must not run on hosts in group
- [ ] **D)** VM-to-VM anti-affinity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'Must run on hosts in group' rule is a mandatory constraint that DRS will never violate, ensuring VMs are always placed on the specified host group.
 
 
</details>

### 30. Which of the following are valid sources of log data for conducting a multi-domain root cause analysis in VCF? (Choose three.)

- [ ] **A)** SDDC Manager logs
- [ ] **B)** vCenter Server logs
- [ ] **C)** ESXi hostd logs
- [ ] **D)** Aria Operations performance charts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> SDDC Manager logs track lifecycle operations, vCenter logs record events and tasks, and hostd logs provide host-level details. Aria Operations charts are aggregated metrics, not raw log data.
 
 
</details>

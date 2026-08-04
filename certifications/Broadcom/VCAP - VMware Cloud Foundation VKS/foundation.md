<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Broadcom/Cloud%20Foundation%20VKS.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>VCAP - VMware Cloud Foundation VKS</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Kubernetes Workload Management with VKS](#kubernetes-workload-management-with-vks) (7 questions)
- [Troubleshooting, Optimization, and Lifecycle Management](#troubleshooting-optimization-and-lifecycle-management) (6 questions)
- [VMware Cloud Foundation Architecture and Design](#vmware-cloud-foundation-architecture-and-design) (8 questions)
- [VMware Cloud Foundation Deployment and Configuration](#vmware-cloud-foundation-deployment-and-configuration) (9 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:03.109Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Kubernetes Workload Management with VKS | 7 |
| Troubleshooting, Optimization, and Lifecycle Management | 6 |
| VMware Cloud Foundation Architecture and Design | 8 |
| VMware Cloud Foundation Deployment and Configuration | 9 |

---

### **Kubernetes Workload Management with VKS**

### 1. What is the foundational layer of VKS that manages workload clusters?

- [ ] **A)** Supervisor Cluster
- [ ] **B)** vSphere Namespace
- [ ] **C)** VKS Cluster Plan
- [ ] **D)** NSX Load Balancer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Supervisor Cluster is the Kubernetes control plane that runs on ESXi and manages workload clusters in VKS.
 
 
</details>

### 2. Which of the following are required for deploying a VKS cluster? (Select all that apply)

- [ ] **A)** Enabled Supervisor Cluster
- [ ] **B)** Configured NSX networking
- [ ] **C)** vSphere Namespace with resource quotas
- [ ] **D)** A pre-deployed external load balancer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> VKS requires a Supervisor Cluster, NSX networking, and a vSphere Namespace; the load balancer is integrated via NSX.
 
 
</details>

### 3. Complete the command to log in to the Supervisor Cluster: 'kubectl vsphere login --server=[blank] --vsphere-username=admin'

```bash
kubectl vsphere login --server=[blank] --vsphere-username=admin
```

- [ ] **A)** vcenter.example.com
- [ ] **B)** Supervisor Cluster API server IP
- [ ] **C)** Namespace name
- [ ] **D)** VKS cluster name

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The kubectl vsphere login command requires the API server IP of the Supervisor Cluster.
 
 
</details>

### 4. What is the purpose of a VKS Cluster Plan?

- [ ] **A)** To specify the Kubernetes version for the cluster
- [ ] **B)** To define the cluster topology, node pools, and VM class
- [ ] **C)** To manage user permissions and RBAC
- [ ] **D)** To configure network policies for the cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Cluster Plans are templates that specify the cluster’s topology, including control plane size, worker node configurations, and VM class.
 
 
</details>

### 5. Which statements are true about VKS cluster upgrades? (Select all that apply)

- [ ] **A)** Upgrades are triggered by modifying the cluster YAML and reapplying
- [ ] **B)** The tanzu cluster upgrade command is used for upgrades
- [ ] **C)** The Supervisor Cluster must be at the same or newer version than the VKS cluster
- [ ] **D)** Worker nodes are upgraded before control plane nodes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> VKS upgrades are declarative via YAML; the Supervisor Cluster version must be compatible; control plane upgrades first.
 
 
</details>

### 6. In the VKS cluster YAML, which field specifies the plan to use? Refer to the code block.

```yaml
apiVersion: run.tanzu.vmware.com/v1alpha1
kind: VksCluster
metadata:
  name: my-cluster
spec:
  plan: small
  version: v1.27
  nodePools:
  - name: worker-pool
    replicas: 3
```

- [ ] **A)** spec.plan
- [ ] **B)** spec.version
- [ ] **C)** spec.nodePools
- [ ] **D)** spec.storagePolicy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The plan is referenced under spec.plan in the VKS cluster manifest.
 
 
</details>

### 7. Which component provides persistent storage for containerized applications in VKS?

- [ ] **A)** NFS datastores
- [ ] **B)** vSAN
- [ ] **C)** External SAN arrays
- [ ] **D)** Local host storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> vSAN provides hyper-converged storage that integrates with VKS via the CSI driver for persistent volumes.
 
 
</details>


---

### **Troubleshooting, Optimization, and Lifecycle Management**

### 8. What is the initial step recommended when troubleshooting a VCF deployment failure?

- [ ] **A)** Check the Hardware Compatibility List (HCL)
- [ ] **B)** Review SDDC Manager logs
- [ ] **C)** Run pre-validation checklists
- [ ] **D)** Restart NSX services

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> VCF includes a built-in pre-validation tool that checks DNS, NTP, network, and hardware compatibility. Skipping this is a common cause of deployment failures.
 
 
</details>

### 9. Which of the following are common causes of VCF deployment failures? (Choose three)

- [ ] **A)** DNS resolution failures
- [ ] **B)** Certificate expiry
- [ ] **C)** Hardware compatibility issues
- [ ] **D)** Insufficient vSAN deduplication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> DNS failures, expired certificates, and hardware incompatibility are frequent root causes. vSAN deduplication settings do not typically cause deployment failures.
 
 
</details>

### 10. Examine the following log snippet from SDDC Manager: 'Failed to deploy vCenter Server. Reason: SSH timeout.' What is the most likely root cause?

```plaintext
Error: SSH connection timeout to vCenter appliance at 192.168.1.100:22
```

- [ ] **A)** Firewall blocking SSH
- [ ] **B)** vCenter appliance failed to power on due to insufficient datastore space
- [ ] **C)** Incorrect SSH credentials
- [ ] **D)** NSX manager not reachable

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The SSH timeout is a symptom of the vCenter OVF appliance not powering on, often due to insufficient datastore space. Checking datastore capacity should be the first step.
 
 
</details>

### 11. Which of the following is true about vSAN snapshots in the context of backup?

- [ ] **A)** They provide crash-consistent backups suitable for long-term retention
- [ ] **B)** They are stored on the same datastore and impact performance
- [ ] **C)** They can replace vSphere Replication for DR
- [ ] **D)** They automatically export to external storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> vSAN snapshots are crash-consistent but stored on the same datastore, consuming space and affecting performance. They are not a substitute for proper backup.
 
 
</details>

### 12. Which VCF components require separate backup procedures? (Choose three)

- [ ] **A)** SDDC Manager
- [ ] **B)** vCenter Server
- [ ] **C)** NSX Manager
- [ ] **D)** Workload VMs via agent backup

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Each management component (SDDC Manager, vCenter, NSX) has its own backup method. Workload VMs are backed up by external tools and are not specific management components.
 
 
</details>

### 13. A PersistentVolumeClaim (PVC) remains in 'Pending' status. The output of 'kubectl get pvc my-pvc -o yaml' shows an event 'no matching StorageClass'. What is the most likely cause?

```yaml
apiVersion: v1
kind: PersistentVolumeClaim
metadata:
  name: my-pvc
spec:
  accessModes:
    - ReadWriteOnce
  resources:
    requests:
      storage: 10Gi
  storageClassName: gold

```

- [ ] **A)** StorageClass 'gold' does not exist in the cluster
- [ ] **B)** The pod using the PVC is not scheduled
- [ ] **C)** vSAN datastore is full
- [ ] **D)** The namespace has a resource quota

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The event 'no matching StorageClass' indicates that the StorageClass referenced in the PVC spec (e.g., 'gold') is not defined. This is a common VKS issue.
 
 
</details>


---

### **VMware Cloud Foundation Architecture and Design**

### 14. What is the minimum number of hosts required for a vSAN cluster with Failures to Tolerate (FTT) = 1?

- [ ] **A)** 2
- [ ] **B)** 3
- [ ] **C)** 4
- [ ] **D)** 5

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> For vSAN FTT=1, the minimum number of hosts is 2n+1 = 3, where n is the number of failures to tolerate (1).
 
 
</details>

### 15. Which components are part of the VCF management domain? (Select two.)

- [ ] **A)** SDDC Manager
- [ ] **B)** vSAN datastore for management data
- [ ] **C)** Workload VMs
- [ ] **D)** NSX Edge nodes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The management domain hosts SDDC Manager, vCenter Server, NSX Manager, and the vSAN datastore for management data. Workload VMs and NSX Edge nodes are part of workload domains.
 
 
</details>

### 16. An architect is configuring a vSAN storage policy. The requirement is to tolerate one failure with space efficiency. Which erasure coding algorithm is indicated by the code shown?

```bash
vmkfstools -C --policy "(('hostFailuresToTolerate' i1) ('erasureCoding' i1))"
```

- [ ] **A)** RAID-5
- [ ] **B)** RAID-6
- [ ] **C)** RAID-1
- [ ] **D)** RAID-0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> vSAN policy with FTT=1 using erasure coding applies RAID-5 (3+1), which tolerates one failure and provides space efficiency.
 
 
</details>

### 17. What is the maximum number of vCenter Servers that can be managed by a single SDDC Manager instance?

- [ ] **A)** 5
- [ ] **B)** 10
- [ ] **C)** 15
- [ ] **D)** 20

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> According to VCF validated design, SDDC Manager can manage up to 10 vCenter Server instances.
 
 
</details>

### 18. Which two types of traffic must be separated into distinct VLANs in a VCF design?

- [ ] **A)** vMotion traffic
- [ ] **B)** Management traffic
- [ ] **C)** Internet browsing traffic
- [ ] **D)** Backup traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VCF recommends separate VLANs for management, vMotion, vSAN, and overlay traffic to prevent Layer 2 conflicts.
 
 
</details>

### 19. An administrator runs the command shown to check vSAN cluster health. What does the 'Hosts with connectivity issues' field indicate?

```bash
esxcli vsan health cluster list
Hosts with connectivity issues: 0
```

- [ ] **A)** All hosts are communicating properly
- [ ] **B)** One host is disconnected
- [ ] **C)** vSAN network is misconfigured
- [ ] **D)** Hosts with issues are ignored

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A value of 0 for hosts with connectivity issues indicates that all hosts in the vSAN cluster have network connectivity to each other.
 
 
</details>

### 20. What is the role of SDDC Manager in VCF?

- [ ] **A)** Managing virtual machine storage policies
- [ ] **B)** Orchestrating lifecycle management of VCF components
- [ ] **C)** Providing compute virtualization
- [ ] **D)** Performing network micro-segmentation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SDDC Manager handles deployment, patching, and upgrade orchestration for VCF infrastructure components.
 
 
</details>

### 21. Which two features are available in vSphere that provide VM availability?

- [ ] **A)** vSphere High Availability (HA)
- [ ] **B)** vSphere Fault Tolerance (FT)
- [ ] **C)** vSphere Distributed Resource Scheduler (DRS)
- [ ] **D)** vSphere vMotion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> vSphere HA restarts VMs after host failure; FT provides continuous availability via a shadow VM.
 
 
</details>


---

### **VMware Cloud Foundation Deployment and Configuration**

### 22. Which component is used only for the initial bring-up of the management domain in VCF?

- [ ] **A)** Cloud Builder
- [ ] **B)** SDDC Manager
- [ ] **C)** vCenter Server
- [ ] **D)** NSX Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Builder is temporary; SDDC Manager persists for lifecycle management.
 
 
</details>

### 23. Which two prerequisites must be met before deploying SDDC Manager? (Choose two.)

- [ ] **A)** Valid DNS forward and reverse records
- [ ] **B)** NTP time synchronization
- [ ] **C)** VMware vCenter already installed
- [ ] **D)** External load balancer configured

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DNS PTR records and NTP are mandatory for Cloud Builder pre-checks.
 
 
</details>

### 24. Review the snippet from the Cloud Builder log. What caused the failure?

```plaintext
Pre-check failed: Reverse DNS resolution for 10.1.0.10 returned no PTR record.
```

- [ ] **A)** Missing PTR record for IP 10.1.0.10
- [ ] **B)** Incorrect VLAN ID assigned
- [ ] **C)** vCenter password too short
- [ ] **D)** Insufficient ESXi hosts in cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The log clearly indicates reverse DNS lookup failure for the management IP.
 
 
</details>

### 25. After Cloud Builder completes, which tool handles ongoing lifecycle operations?

- [ ] **A)** SDDC Manager
- [ ] **B)** Cloud Builder
- [ ] **C)** vCenter Server
- [ ] **D)** NSX Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SDDC Manager is persistent and manages all lifecycle operations.
 
 
</details>

### 26. Which two services are hosted by SDDC Manager after deployment? (Choose two.)

- [ ] **A)** LCM repository for VCF bundles
- [ ] **B)** Certificate management via VMCA
- [ ] **C)** vCenter database backup
- [ ] **D)** NSX load balancer configuration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SDDC Manager hosts a local repository and manages certificates through VMCA.
 
 
</details>

### 27. A vSphere administrator tries to manually change the root password on an ESXi host. What is the impact on SDDC Manager?

```plaintext
vpxd_service on esxi1.vcf.local: password changed via CLI instead of SDDC Manager.
```

- [ ] **A)** Inventory becomes out-of-sync
- [ ] **B)** SDDC Manager automatically updates
- [ ] **C)** Password rotation is disabled
- [ ] **D)** No impact occurs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Manual password changes break the password vault and future lifecycle operations.
 
 
</details>

### 28. What defines the data redundancy and placement for VMs on a vSAN cluster?

- [ ] **A)** Storage policy
- [ ] **B)** Cluster DRS rules
- [ ] **C)** vSphere HA settings
- [ ] **D)** Host profile

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A vSAN storage policy determines redundancy, striping, and reservation for VM objects.
 
 
</details>

### 29. Which two vSAN storage policy settings directly affect availability? (Choose two.)

- [ ] **A)** Failures to Tolerate (FTT)
- [ ] **B)** Strip Width
- [ ] **C)** Object Space Reservation
- [ ] **D)** Erasure Coding vs Mirroring

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> FTT and the choice between mirroring and erasure coding set the redundancy level.
 
 
</details>

### 30. A VM with a storage policy requiring FTT=2 becomes inaccessible after a host failure. The cluster initially had 5 hosts. What is the most likely cause?

```plaintext
vSAN compliance view: VM objects report 'Inaccessible'. Cluster hosts: 4 (one failed).
```

- [ ] **A)** Insufficient hosts remain to meet FTT=2
- [ ] **B)** vSAN capacity is full
- [ ] **C)** Network connectivity lost to remaining hosts
- [ ] **D)** vCenter is not responding

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> FTT=2 with mirroring requires at least 5 hosts; losing one reduces to 4, breaking compliance.
 
 
</details>

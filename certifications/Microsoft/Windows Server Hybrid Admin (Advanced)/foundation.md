<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Windows%20Server%20Hybrid%20Admin%20(Core).png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Windows Server Hybrid Admin (Advanced)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Implement and manage Windows Server high availability](#implement-and-manage-windows-server-high-availability) (4 questions)
- [Implement disaster recovery](#implement-disaster-recovery) (3 questions)
- [Migrate servers and workloads](#migrate-servers-and-workloads) (7 questions)
- [Monitor and troubleshoot Windows Server environments](#monitor-and-troubleshoot-windows-server-environments) (7 questions)
- [Secure Windows Server on-premises and hybrid infrastructures](#secure-windows-server-on-premises-and-hybrid-infrastructures) (9 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:53:00.646Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Implement and manage Windows Server high availability | 4 |
| Implement disaster recovery | 3 |
| Migrate servers and workloads | 7 |
| Monitor and troubleshoot Windows Server environments | 7 |
| Secure Windows Server on-premises and hybrid infrastructures | 9 |

---

### **Implement and manage Windows Server high availability**

### 1. What is the primary purpose of implementing Failover Clustering in a Windows Server environment for production workloads?

- [ ] **A)** Restarts failing services on another cluster node
- [ ] **B)** Balances web traffic across multiple web servers
- [ ] **C)** Replicates virtual machines to a secondary site
- [ ] **D)** Centralizes DNS management for the cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Failover Clustering keeps services and applications available by automatically moving them to another cluster node when a node fails.
 
 
</details>

### 2. Which of the following is required before configuring a traditional two-node Windows Server failover cluster? (Select all that apply.)

- [ ] **A)** At least two Windows Server cluster nodes
- [ ] **B)** Shared storage available to all nodes
- [ ] **C)** Active Directory domain membership for all nodes
- [ ] **D)** Azure subscription linked to the cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A traditional failover cluster requires multiple servers, shared storage, and Active Directory domain membership. An Azure subscription is not required for an on-premises failover cluster.
 
 
</details>

### 3. You execute the following PowerShell command on a Windows Server failover cluster. Which quorum configuration does it apply?

```powershell
Set-ClusterQuorum -DiskOnly "Cluster Disk 1"
```

- [ ] **A)** No majority: disk only
- [ ] **B)** Node majority
- [ ] **C)** Node and disk majority
- [ ] **D)** Node and file share majority

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The `-DiskOnly` parameter configures the No Majority: Disk Only quorum model, which uses a designated cluster disk as the quorum witness.
 
 
</details>

### 4. What is the primary purpose of Storage Spaces Direct when it is used in Windows Server high availability deployments?

- [ ] **A)** Creates software-defined storage from local cluster disks
- [ ] **B)** Balances network traffic among web servers
- [ ] **C)** Replicates virtual machines to Azure
- [ ] **D)** Provides DNS services for failover clusters

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Storage Spaces Direct pools local disks across failover cluster nodes to provide highly available, software-defined storage without a traditional SAN.
 
 
</details>


---

### **Implement disaster recovery**

### 5. What is the main purpose of Azure Site Recovery in a hybrid Windows Server environment?

- [ ] **A)** Business continuity and disaster recovery by replicating virtual machines to Azure
- [ ] **B)** Long-term archival backup with versioning
- [ ] **C)** Real-time server performance monitoring
- [ ] **D)** Centralized DNS and Active Directory management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Site Recovery supports disaster recovery by replicating workloads and enabling failover and failback in hybrid environments.
 
 
</details>

### 6. Which two components are required to configure Hyper-V Replica between two Windows Server hosts?

- [ ] **A)** A primary Hyper-V host
- [ ] **B)** A replica Hyper-V host
- [ ] **C)** An Azure Active Directory tenant
- [ ] **D)** An Azure Site Recovery vault

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Hyper-V Replica is built into Windows Server and copies VMs from a primary host to a replica host; it does not require Azure AD or a Site Recovery vault.
 
 
</details>

### 7. Examine the PowerShell script in the code block. What action does the last cmdlet perform in the disaster recovery workflow?

```powershell
$vault = Get-AzRecoveryServicesVault -Name 'ContosoVault'
$container = Get-AzRecoveryServicesAsrProtectionContainer -Vault $vault
$item = Get-AzRecoveryServicesAsrReplicationProtectedItem -ProtectionContainer $container
Start-AzRecoveryServicesAsrUnplannedFailoverJob -ReplicationProtectedItem $item -Direction PrimaryToRecovery
```

- [ ] **A)** It starts an unplanned failover to the recovery location
- [ ] **B)** It deletes the current recovery point
- [ ] **C)** It pauses replication to the primary site
- [ ] **D)** It creates a new Recovery Services vault

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Start-AzRecoveryServicesAsrUnplannedFailoverJob begins an unplanned failover for a protected item to the configured recovery location.
 
 
</details>


---

### **Migrate servers and workloads**

### 8. What is the primary purpose of Azure Migrate when preparing Windows Server workloads for cloud migration?

- [ ] **A)** Create and manage Azure Active Directory users
- [ ] **B)** Discover, assess, and migrate on-premises servers and workloads
- [ ] **C)** Configure network security between Azure virtual networks
- [ ] **D)** Monitor the performance of cloud-native applications

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Azure Migrate is a centralized hub for discovering, assessing, and migrating on-premises servers and workloads to Azure. It provides readiness assessment, sizing, and migration tools for Windows Server workloads.
 
 
</details>

### 9. Which two tools are built into the Azure Migrate hub for assessing and migrating Windows Server workloads?

- [ ] **A)** Azure Migrate: Discovery and Assessment
- [ ] **B)** Azure Migrate: Server Migration
- [ ] **C)** Azure Backup Center
- [ ] **D)** Azure Cost Management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure Migrate includes Discovery and Assessment for readiness and sizing, and Server Migration for orchestrating the migration of VMs and workloads to Azure.
 
 
</details>

### 10. An administrator runs the script in the code block. What action does the script perform in a migration project?

```powershell
Connect-AzAccount
New-AzMigrateProject -Name "MigrationProject" -ResourceGroupName "RG-Migration" -Location "EastUS"
```

- [ ] **A)** Connects to Azure and creates a new Azure Migrate project
- [ ] **B)** Starts replication of a Windows Server VM
- [ ] **C)** Installs the Azure Migrate appliance on-premises
- [ ] **D)** Uploads a VHD to a storage account

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Connect-AzAccount authenticates to Azure and New-AzMigrateProject creates an Azure Migrate project in the specified resource group and region.
 
 
</details>

### 11. Which service provides continuous replication and failover for Windows Server VMs being migrated from on-premises to Azure?

- [ ] **A)** Azure Backup
- [ ] **B)** Azure Site Recovery
- [ ] **C)** Azure Policy
- [ ] **D)** Azure Resource Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Azure Site Recovery replicates on-premises workloads to Azure and supports failover and test failover, which is commonly used for Windows Server migration.
 
 
</details>

### 12. Which two source environments are supported by Azure Migrate: Server Migration tool when migrating Windows Server VMs to Azure?

- [ ] **A)** VMware VMs
- [ ] **B)** Hyper-V VMs
- [ ] **C)** Azure virtual machine scale sets
- [ ] **D)** Azure Container Instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure Migrate Server Migration supports migrating VMware VMs and Hyper-V VMs to Azure, as well as physical and other virtualized servers.
 
 
</details>

### 13. An administrator executes the PowerShell commands in the code block as part of an Azure Site Recovery migration. What action is being performed?

```powershell
$vault = Get-AzRecoveryServicesVault -Name "vaultName" -ResourceGroupName "rgName"
$item = Get-AzRecoveryServicesAsrReplicationProtectedItem -FriendlyName "WS2019"
Start-AzRecoveryServicesAsrTestFailoverJob -ReplicationProtectedItem $item -Direction PrimaryToRecovery
```

- [ ] **A)** A test failover of a replicated Windows Server VM
- [ ] **B)** A full production failover and final migration
- [ ] **C)** Creation of a Recovery Services vault
- [ ] **D)** Removal of a replication policy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Start-AzRecoveryServicesAsrTestFailoverJob starts a test failover to validate the migration and disaster recovery configuration without impacting production.
 
 
</details>

### 14. Before uploading an on-premises Windows Server disk to Azure, which VHD format must be used?

- [ ] **A)** Dynamically expanding VHD
- [ ] **B)** Fixed-size VHD
- [ ] **C)** VHDX with differential snapshots
- [ ] **D)** Fixed-size VHDX

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Azure requires a fixed-size VHD file when uploading an on-premises virtual disk for VM migration. VHDX and dynamic disks are not supported for direct upload.
 
 
</details>


---

### **Monitor and troubleshoot Windows Server environments**

### 15. Which Windows Server tool captures performance counters in real time or from saved logs?

- [ ] **A)** Performance Monitor
- [ ] **B)** Task Manager
- [ ] **C)** Device Manager
- [ ] **D)** Services console

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Performance Monitor is the built-in Windows Server tool for viewing and logging performance counters, both live and from saved Data Collector Sets.
 
 
</details>

### 16. Which of the following are standard Event Viewer logs in Windows Server? (Select all that apply.)

- [ ] **A)** Application
- [ ] **B)** Security
- [ ] **C)** System
- [ ] **D)** Network

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The default Windows Server Event Viewer logs are Application, Security, Setup, System, and Forwarded Events; no Network log exists by default.
 
 
</details>

### 17. Review the PowerShell command in the code block. What is its purpose?

```powershell
Get-WinEvent -LogName Application -MaxEvents 20 | Where-Object { $_.LevelDisplayName -eq 'Error' }
```

- [ ] **A)** Show the most recent Error events from the Application log
- [ ] **B)** Delete the most recent Application log Error events
- [ ] **C)** Export all Application Error events to a CSV file
- [ ] **D)** List the newest 20 applications installed on the server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command gets up to 20 newest events from the Application log and filters them for events classified as Error.
 
 
</details>

### 18. Which Windows Server tool shows detailed real-time CPU, memory, disk, and network activity per process?

- [ ] **A)** Resource Monitor
- [ ] **B)** Performance Monitor
- [ ] **C)** Task Manager
- [ ] **D)** Server Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Resource Monitor (resmon.exe) offers detailed real-time data for CPU, memory, disk, and network, including per-process information.
 
 
</details>

### 19. Which of the following are built-in tools for monitoring Windows Server performance? (Select all that apply.)

- [ ] **A)** Task Manager
- [ ] **B)** Resource Monitor
- [ ] **C)** Performance Monitor
- [ ] **D)** Device Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Task Manager, Resource Monitor, and Performance Monitor are all native monitoring tools; Device Manager is used for hardware device management.
 
 
</details>

### 20. Review the PowerShell code in the code block. What does it return?

```powershell
Get-Service | Where-Object { $_.Status -eq 'Running' } | Sort-Object DisplayName
```

- [ ] **A)** Running services sorted by display name
- [ ] **B)** Stopped services with errors
- [ ] **C)** All installed services in order
- [ ] **D)** Only services with a manual startup type

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Get-Service retrieves all services, Where-Object selects running services, and Sort-Object orders them by DisplayName.
 
 
</details>

### 21. Which Event Viewer severity level indicates a possible problem that is not yet critical?

- [ ] **A)** Warning
- [ ] **B)** Error
- [ ] **C)** Critical
- [ ] **D)** Information

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Warning events indicate that an issue may occur or has occurred but has not yet caused a critical system failure.
 
 
</details>


---

### **Secure Windows Server on-premises and hybrid infrastructures**

### 22. Which technology isolates Windows Server domain credentials in a virtualized security environment to help prevent credential theft?

- [ ] **A)** Windows Defender Credential Guard
- [ ] **B)** BitLocker Drive Encryption
- [ ] **C)** Local Administrator Password Solution
- [ ] **D)** Windows Defender Firewall

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Windows Defender Credential Guard uses Virtualization-Based Security to isolate domain credentials so malware cannot access them.
 
 
</details>

### 23. Which of the following are Windows Server features that help protect credential data? (Select all that apply.)

- [ ] **A)** Windows Defender Credential Guard
- [ ] **B)** Local Administrator Password Solution
- [ ] **C)** Remote Desktop Services
- [ ] **D)** DNS Admin Service

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Credential Guard isolates secrets in VBS, while LAPS randomizes local administrator passwords. Remote Desktop Services and DNS Admin do not protect credential data.
 
 
</details>

### 24. An administrator runs the following PowerShell command on a Windows Server. What type of domain controller is being deployed?

```powershell
Install-ADDSDomainController
  -NoGlobalCatalog
  -ReadOnlyReplica
  -DomainName contoso.com
  -SiteName Default-First-Site
```

- [ ] **A)** Read-only domain controller (RODC)
- [ ] **B)** Writable domain controller
- [ ] **C)** Child domain
- [ ] **D)** Global catalog server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The -ReadOnlyReplica parameter creates a read-only domain controller, while -NoGlobalCatalog prevents the RODC from hosting the global catalog.
 
 
</details>

### 25. Where does Windows Local Administrator Password Solution store the local administrator password for member servers?

- [ ] **A)** In a confidential attribute on the computer object
- [ ] **B)** In the registry of the domain controller
- [ ] **C)** In a Group Policy preferences file
- [ ] **D)** In the SYSVOL folder

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> LAPS stores the password in an AD computer object attribute, ms-Mcs-AdmPwd, and only authorized users can retrieve it.
 
 
</details>

### 26. Which of the following are recommended practices for securing Active Directory identity infrastructure? (Select all that apply.)

- [ ] **A)** Require LDAP signing or LDAPS
- [ ] **B)** Deploy read-only domain controllers at unsecured sites
- [ ] **C)** Allow LAN Manager authentication
- [ ] **D)** Disable SMB signing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> LDAP signing/channel binding stops tampering, and RODCs limit exposure at untrusted sites. LM authentication and disabling SMB signing weaken security.
 
 
</details>

### 27. An administrator runs the following PowerShell command. What type of service account is being created?

```powershell
New-ADServiceAccount
  -Name svcApp
  -GroupManagedServiceAccount
  -DNSHostName svcApp.contoso.com
  -PrincipalsAllowedToRetrieveManagedPassword Server01$
```

- [ ] **A)** Group Managed Service Account (gMSA)
- [ ] **B)** Managed Service Account (MSA)
- [ ] **C)** Virtual account
- [ ] **D)** User account

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The -GroupManagedServiceAccount parameter creates a gMSA, which automatically manages passwords and can be used across multiple servers.
 
 
</details>

### 28. What does Just Enough Administration (JEA) in Windows Server allow administrators to do?

- [ ] **A)** Grant least-privilege administrative access through constrained PowerShell endpoints
- [ ] **B)** Encrypt volumes on domain controllers
- [ ] **C)** Replace Active Directory domain controllers
- [ ] **D)** Automate Windows Server installation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> JEA limits administrators to specific cmdlets and tasks through constrained PowerShell session configurations, applying least-privilege.
 
 
</details>

### 29. Which of the following are components of Microsoft Defender for Identity? (Select all that apply.)

- [ ] **A)** Sensors installed on domain controllers
- [ ] **B)** Microsoft 365 Defender portal
- [ ] **C)** Azure Arc agent
- [ ] **D)** Azure AD Connect sync engine

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Defender for Identity uses domain controller sensors and delivers alerts in the Microsoft 365 Defender portal. Azure Arc and Azure AD Connect are not core components.
 
 
</details>

### 30. An administrator assigns a policy to an Azure Arc-enabled Windows Server using the JSON below. What is the administrator assigning?

```json
{
  "properties": {
    "policyDefinitionId": "/providers/Microsoft.Authorization/policyDefinitions/azureSecurityBaseline",
    "parameters": {
      "effect": {
        "value": "AuditIfNotExists"
      }
    },
    "scope": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/rg/providers/Microsoft.HybridCompute/machines/Server01"
  }
}
```

- [ ] **A)** An Azure Policy assignment
- [ ] **B)** An Azure RBAC role assignment
- [ ] **C)** An Azure AD conditional access policy
- [ ] **D)** An Azure Blueprint artifact

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The JSON assigns a policy definition to a machine scope, which is how Azure Policy applies a security baseline to Azure Arc-enabled servers.
 
 
</details>

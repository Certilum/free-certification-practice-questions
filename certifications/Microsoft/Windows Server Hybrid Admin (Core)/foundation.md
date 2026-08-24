<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Windows%20Server%20Hybrid%20Admin%20(Core).png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Windows Server Hybrid Admin (Core)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Deploy and manage Active Directory Domain Services (AD DS) in on-premises and cloud environments](#deploy-and-manage-active-directory-domain-services-ad-ds-in-on-premises-and-cloud-environments) (11 questions)
- [Implement and manage an on-premises and hybrid networking infrastructure](#implement-and-manage-an-on-premises-and-hybrid-networking-infrastructure) (6 questions)
- [Manage Windows Servers and workloads in a hybrid environment](#manage-windows-servers-and-workloads-in-a-hybrid-environment) (3 questions)
- [Manage storage and file services](#manage-storage-and-file-services) (6 questions)
- [Manage virtual machines and containers](#manage-virtual-machines-and-containers) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:53:06.521Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Deploy and manage Active Directory Domain Services (AD DS) in on-premises and cloud environments | 11 |
| Implement and manage an on-premises and hybrid networking infrastructure | 6 |
| Manage Windows Servers and workloads in a hybrid environment | 3 |
| Manage storage and file services | 6 |
| Manage virtual machines and containers | 4 |

---

### **Deploy and manage Active Directory Domain Services (AD DS) in on-premises and cloud environments**

### 1. Which MMC snap-in is used to manage Active Directory sites, subnets, and the replication topology?

- [ ] **A)** Active Directory Sites and Services
- [ ] **B)** Active Directory Users and Computers
- [ ] **C)** Active Directory Domains and Trusts
- [ ] **D)** Active Directory Administrative Center

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Active Directory Sites and Services manages sites, subnets, and replication topology. The other consoles manage objects, domains, or AD administrative tasks.
 
 
</details>

### 2. Which of the following are valid Active Directory Domain Services directory partitions? (Choose all that apply.)

- [ ] **A)** Schema partition
- [ ] **B)** Configuration partition
- [ ] **C)** Domain partition
- [ ] **D)** SYSVOL partition

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Schema, configuration, and domain partitions are valid AD DS directory partitions; application partitions also exist. SYSVOL is a replicated folder, not a partition.
 
 
</details>

### 3. A server is prepared with the AD DS role. Examine the script in the code block. What AD DS component is created when you run it?

```powershell
Install-WindowsFeature -Name AD-DomainServices -IncludeManagementTools; Install-ADDSForest -DomainName contoso.com -DomainNetbiosName CONTOSO -ForestMode WinThreshold -DomainMode WinThreshold -InstallDns $true
```

- [ ] **A)** A new forest root domain
- [ ] **B)** A child domain
- [ ] **C)** An additional domain controller in an existing domain
- [ ] **D)** A read-only domain controller

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Install-ADDSForest creates a new forest root domain. Child domains, replica domain controllers, and RODCs require different installation parameters.
 
 
</details>

### 4. What is the default tombstone lifetime for Active Directory objects on Windows Server?

- [ ] **A)** 30 days
- [ ] **B)** 60 days
- [ ] **C)** 180 days
- [ ] **D)** 365 days

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The default tombstone lifetime is 180 days. This period is used by replication to ensure deletions are replicated before tombstones are removed.
 
 
</details>

### 5. Which two Active Directory FSMO roles are forest-wide? (Choose all that apply.)

- [ ] **A)** Schema Master
- [ ] **B)** Domain Naming Master
- [ ] **C)** RID Master
- [ ] **D)** PDC Emulator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Schema Master and Domain Naming Master are forest-wide roles. RID Master, PDC Emulator, and Infrastructure Master are domain-wide roles.
 
 
</details>

### 6. The PowerShell command in the code block is executed in the contoso.com domain. Which FSMO role is transferred?

```powershell
Move-ADDirectoryServerOperationMasterRole -Identity DC01 -OperationMasterRole SchemaMaster
```

- [ ] **A)** Schema Master
- [ ] **B)** Domain Naming Master
- [ ] **C)** RID Master
- [ ] **D)** PDC Emulator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The OperationMasterRole value SchemaMaster moves the schema master to DC01. Other roles are moved with different values.
 
 
</details>

### 7. Where are AD-integrated DNS zones such as ForestDNSZones stored?

- [ ] **A)** Application partition
- [ ] **B)** Schema partition
- [ ] **C)** Configuration partition
- [ ] **D)** Domain partition

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AD-integrated DNS zones are stored in application partitions. The other partition types serve schema, configuration, or domain data.
 
 
</details>

### 8. Which administrative tasks are performed by using Active Directory Sites and Services? (Choose all that apply.)

- [ ] **A)** Create and manage AD DS sites
- [ ] **B)** Link sites and configure replication cost
- [ ] **C)** Assign subnets to sites
- [ ] **D)** Create DNS zones

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Sites and Services controls sites, subnets, and site links. DNS zone management is performed by DNS Manager or PowerShell.
 
 
</details>

### 9. The code block contains a diagnostic command. Which AD DS subsystem does it test?

```cmd
dcdiag /test:replications
```

- [ ] **A)** Active Directory replication
- [ ] **B)** DNS zone transfer
- [ ] **C)** Group Policy application
- [ ] **D)** Kerberos authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> dcdiag /test:replications validates Active Directory replication between domain controllers. It does not test DNS, GPO, or Kerberos.
 
 
</details>

### 10. Which FSMO role is responsible for assigning RID pools to domain controllers?

- [ ] **A)** RID Master
- [ ] **B)** Schema Master
- [ ] **C)** PDC Emulator
- [ ] **D)** Infrastructure Master

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The RID Master distributes RID pools to domain controllers. The schema, PDC, and infrastructure roles perform different functions.
 
 
</details>

### 11. Which characteristics apply to a Read-Only Domain Controller? (Choose all that apply.)

- [ ] **A)** The Active Directory database is read-only on the RODC.
- [ ] **B)** An RODC can be placed in locations with lower physical security.
- [ ] **C)** Password hashes are not cached for all users by default.
- [ ] **D)** An RODC should be used as the schema master in the forest.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> RODCs hold read-only databases, are suited to branch offices, and use a password replication policy. RODCs do not host FSMO roles.
 
 
</details>


---

### **Implement and manage an on-premises and hybrid networking infrastructure**

### 12. Which network component in Windows Server forwards IP packets between different subnets and can perform network address translation?

- [ ] **A)** IP router
- [ ] **B)** Layer 2 switch
- [ ] **C)** Network bridge
- [ ] **D)** Packet filter

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A router operates at Layer 3 and forwards IP packets between subnets. NAT is commonly implemented on routers to translate private and public addresses.
 
 
</details>

### 13. Which two functions are provided by a DHCP server in a Windows Server network environment?

- [ ] **A)** Assigns IP addresses to clients
- [ ] **B)** Registers DNS records for clients
- [ ] **C)** Blocks unwanted network traffic
- [ ] **D)** Encrypts network communications

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DHCP servers dynamically assign IP addresses and can register client DNS records. Packet filtering and encryption are provided by firewalls or IPsec, not DHCP.
 
 
</details>

### 14. Review the PowerShell output in the code block. What IP address is currently assigned to the network adapter?

```powershell
Get-NetIPAddress -InterfaceAlias 'Ethernet0' | Format-Table IPAddress, InterfaceAlias, AddressFamily

IPAddress     InterfaceAlias AddressFamily
----------     -------------- ------------
10.10.0.25     Ethernet0      IPv4

```

- [ ] **A)** IP address 10.10.0.25
- [ ] **B)** IP address 10.10.0.1
- [ ] **C)** IP address 192.168.1.10
- [ ] **D)** IP address 172.16.0.25

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Format-Table output shows the Ethernet0 adapter has IPv4 address 10.10.0.25. The other values in the output represent different network elements.
 
 
</details>

### 15. Which DNS record type is used to resolve a host name to an IPv6 address in Windows Server DNS?

- [ ] **A)** AAAA record
- [ ] **B)** A record
- [ ] **C)** CNAME record
- [ ] **D)** PTR record

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IPv6 host addresses are stored in AAAA DNS records. A records are for IPv4, CNAME records are aliases, and PTR records handle reverse lookups.
 
 
</details>

### 16. Which two tools can an administrator use to view and configure network adapters on Windows Server?

- [ ] **A)** Network Connections (ncpa.cpl)
- [ ] **B)** PowerShell Get-NetAdapter cmdlet
- [ ] **C)** Active Directory Users and Computers
- [ ] **D)** Disk Management console

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Network Connections provides a GUI for adapters, and Get-NetAdapter is the PowerShell cmdlet for viewing and configuring adapter settings. The other tools are unrelated.
 
 
</details>

### 17. The command in the code block configures a network interface. What IP address is set by this command?

```powershell
New-NetIPAddress -InterfaceAlias 'Ethernet0' -IPAddress 192.168.1.50 -PrefixLength 24 -DefaultGateway 192.168.1.1
```

- [ ] **A)** IP address 192.168.1.50
- [ ] **B)** IP address 192.168.1.1
- [ ] **C)** IP address 192.168.1.0
- [ ] **D)** Subnet mask 255.255.255.0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> New-NetIPAddress assigns the IP address specified by the -IPAddress parameter. Therefore, the Ethernet0 interface receives 192.168.1.50.
 
 
</details>


---

### **Manage Windows Servers and workloads in a hybrid environment**

### 18. Your organization uses both on-premises Windows Servers and Azure virtual machines. You need a centralized way to manage these servers as Azure resources without migrating them. Which service should you use?

- [ ] **A)** Azure Arc
- [ ] **B)** Azure Migrate
- [ ] **C)** Azure Site Recovery
- [ ] **D)** Windows Admin Center

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Arc enables existing Windows Servers outside Azure to be represented as Azure resources. This allows governance such as Azure Policy and RBAC through the Azure portal. The other options do not provide this capability.
 
 
</details>

### 19. Which two options are valid management tools for Windows Server workloads in a hybrid environment?

- [ ] **A)** Azure Arc
- [ ] **B)** Windows Admin Center
- [ ] **C)** Azure Cognitive Services
- [ ] **D)** Azure DevOps

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure Arc provides management and governance for Windows Server workloads outside Azure. Windows Admin Center is a browser-based management console for Windows Servers. Azure Cognitive Services and Azure DevOps are not server management tools.
 
 
</details>

### 20. An administrator runs the PowerShell script shown in the code block. What Azure service is being used to manage the on-premises Windows Server?

```powershell
Connect-AzAccount
New-AzConnectedMachine -Name "SQL01" -ResourceGroupName "RG-HYBRID" -SubscriptionId "1a2b3c4d-1234-4321-8765-1a2b3c4d5e6f" -Location "eastus"
```

- [ ] **A)** Azure Arc
- [ ] **B)** Azure Automation
- [ ] **C)** Azure Update Management
- [ ] **D)** Azure Monitor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The New-AzConnectedMachine cmdlet is part of the Azure Connected Machine module and is used to register an on-premises Windows Server with Azure Arc.
 
 
</details>


---

### **Manage storage and file services**

### 21. Which Windows Server feature creates storage pools from physical disks to provide software-defined storage?

- [ ] **A)** Storage Spaces
- [ ] **B)** Storage Replica
- [ ] **C)** Data Deduplication
- [ ] **D)** Failover Clustering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Storage Spaces lets you pool physical storage and create virtual disks with resiliency. Storage Replica is for replication, Data Deduplication reduces data footprint, and Failover Clustering is for high availability.
 
 
</details>

### 22. Which of the following are included in the File and iSCSI Services role? Select all that apply.

- [ ] **A)** File Server
- [ ] **B)** DFS Namespaces
- [ ] **C)** DNS Server
- [ ] **D)** iSCSI Target Server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> File and iSCSI Services includes File Server, DFS Namespaces, DFS Replication, File Server Resource Manager, NFS, and iSCSI Target Server. DNS Server is a separate role, not part of this role.
 
 
</details>

### 23. Review the PowerShell cmdlet in the code block. What is the primary purpose of this command?

```powershell
New-SmbShare -Name "DataShare" -Path "D:\Shares\Data" -FullAccess "CONTOSO\Users"
```

- [ ] **A)** Create a new SMB file share
- [ ] **B)** Delete an existing SMB file share
- [ ] **C)** Set NTFS permissions on the folder
- [ ] **D)** Create a DFS namespace

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The New-SmbShare cmdlet creates a new SMB file share. It does not delete shares, modify NTFS permissions, or create DFS namespaces.
 
 
</details>

### 24. Which Windows Server feature reduces storage costs by identifying and removing duplicate data at the block level?

- [ ] **A)** Data Deduplication
- [ ] **B)** Storage Replica
- [ ] **C)** BitLocker
- [ ] **D)** Volume Shadow Copy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Data Deduplication finds duplicated chunks and stores a single copy. Storage Replica replicates data, BitLocker encrypts, and Volume Shadow Copy creates snapshots.
 
 
</details>

### 25. Which features are supported by SMB 3.1.1 in Windows Server? Select all that apply.

- [ ] **A)** SMB Encryption
- [ ] **B)** SMB Multichannel
- [ ] **C)** SMB Direct over RDMA
- [ ] **D)** FTP tunneling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> SMB 3.1.1 includes SMB Encryption, SMB Multichannel, and SMB Direct over RDMA. FTP tunneling is not an SMB feature.
 
 
</details>

### 26. Look at the PowerShell cmdlet in the code block. What is the purpose of this command?

```powershell
Get-SmbShare | Where-Object Name -eq "DataShare"
```

- [ ] **A)** List all SMB shares on the server
- [ ] **B)** Create a new SMB share
- [ ] **C)** Delete an SMB share
- [ ] **D)** Set SMB share permissions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Get-SmbShare cmdlet retrieves SMB shares. The Where-Object filter limits the output to shares named DataShare, but the overall purpose is to list SMB shares.
 
 
</details>


---

### **Manage virtual machines and containers**

### 27. What is the default isolation mode used by Windows containers on a Windows Server host?

- [ ] **A)** Process isolation
- [ ] **B)** Hyper-V isolation
- [ ] **C)** Virtual Machine isolation
- [ ] **D)** Kernel isolation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> By default, Windows containers use process isolation, in which the container shares the host kernel and processes are separated by namespaces.
 
 
</details>

### 28. Which two essential components must be installed or present on a Windows Server host to run Windows containers?

- [ ] **A)** Container host
- [ ] **B)** Container image
- [ ] **C)** Container registry
- [ ] **D)** Container orchestrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A container host runs the container engine, and a container image supplies the application and OS files. A registry stores images, and an orchestrator is optional.
 
 
</details>

### 29. When a Windows Server administrator runs the command in the code block, what information is returned?

```bash
docker ps
```

- [ ] **A)** IDs and names of running containers
- [ ] **B)** Pulled images and their sizes
- [ ] **C)** Stopped containers and exit codes
- [ ] **D)** Container host configuration details

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> docker ps lists the IDs, names, and status of containers currently running on the host. It does not display images, stopped containers, or host configuration details.
 
 
</details>

### 30. Besides the Containers feature, what additional Windows Server role is required to run Hyper-V isolated Windows containers?

- [ ] **A)** Hyper-V role
- [ ] **B)** Failover Clustering
- [ ] **C)** Network Policy and Access Services
- [ ] **D)** Windows Deployment Services

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Hyper-V isolation requires the Hyper-V role, which supplies the lightweight VM boundary used to isolate each Windows container.
 
 
</details>

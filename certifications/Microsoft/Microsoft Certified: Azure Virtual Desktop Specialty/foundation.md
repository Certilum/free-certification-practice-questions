<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Microsoft%20Certified-%20Azure%20Virtual%20Desktop%20Specialty.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Microsoft Certified: Azure Virtual Desktop Specialty</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Monitor and maintain an Azure Virtual Desktop infrastructure](#monitor-and-maintain-an-azure-virtual-desktop-infrastructure) (4 questions)
- [Plan and implement an Azure Virtual Desktop infrastructure](#plan-and-implement-an-azure-virtual-desktop-infrastructure) (14 questions)
- [Plan and implement identity and security](#plan-and-implement-identity-and-security) (5 questions)
- [Plan and implement user environments and apps](#plan-and-implement-user-environments-and-apps) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-11T02:42:24.948Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Monitor and maintain an Azure Virtual Desktop infrastructure | 4 |
| Plan and implement an Azure Virtual Desktop infrastructure | 14 |
| Plan and implement identity and security | 5 |
| Plan and implement user environments and apps | 7 |

---

### **Monitor and maintain an Azure Virtual Desktop infrastructure**

### 1. Which Azure service provides a global view of Azure service availability, including Azure Virtual Desktop, across regions?

- [ ] **A)** Azure Service Health
- [ ] **B)** Resource Health
- [ ] **C)** Azure Monitor
- [ ] **D)** Log Analytics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Service Health gives a global view of Azure service availability, including AVD. Resource Health reports only on individual resources, such as a session host VM.
 
 
</details>

### 2. Which two actions are required to send AVD user connection events to Log Analytics? (Choose two.)

- [ ] **A)** Enable diagnostic settings on the host pool
- [ ] **B)** Create a Log Analytics workspace
- [ ] **C)** Deploy Azure Monitor Agent on session hosts
- [ ] **D)** Configure Azure Service Health alerts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Host pool diagnostic settings send connection events to Log Analytics, and the workspace stores them. The agent collects OS performance data, not AVD connection events.
 
 
</details>

### 3. Examine the KQL query in the code block. Which Log Analytics table does it query?

```kusto
WVDDiagnostics
| where ActivityType == "Connection"
| where State == "Failed"
| summarize count() by bin(TimeGenerated, 15m)
```

- [ ] **A)** WVDDiagnostics
- [ ] **B)** WVDCheckpoints
- [ ] **C)** WVDErrors
- [ ] **D)** InsightsMetrics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query starts from the WVDDiagnostics table and filters Connection activity with a failed state to count failures over time.
 
 
</details>

### 4. Which Log Analytics table records the successful phases of an Azure Virtual Desktop session establishment?

- [ ] **A)** WVDCheckpoints
- [ ] **B)** WVDDiagnostics
- [ ] **C)** InsightsMetrics
- [ ] **D)** Perf

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> WVDCheckpoints records the successful stages of session establishment. WVDDiagnostics is used for errors and other activity types, not successful phase tracing.
 
 
</details>


---

### **Plan and implement an Azure Virtual Desktop infrastructure**

### 5. In Azure Virtual Desktop, a host pool is the main compute boundary for user sessions. What does this resource contain?

- [ ] **A)** A collection of session host VMs
- [ ] **B)** A layer that publishes RemoteApps
- [ ] **C)** A container for FSLogix profiles
- [ ] **D)** An identity provider for users

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A host pool is the compute container holding session host virtual machines. Workspaces publish applications, and FSLogix stores profiles separately.
 
 
</details>

### 6. A user reports that an Azure Virtual Desktop resource is not visible and cannot be launched. Which two assignments are required to fix this issue?

- [ ] **A)** Application group assignment
- [ ] **B)** Workspace visibility
- [ ] **C)** Host pool registration token
- [ ] **D)** Storage account key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A user needs workspace visibility to see resources and application group assignment to launch them. Registration tokens and storage keys do not grant user access.
 
 
</details>

### 7. An administrator uses the Azure CLI command shown in the code block. Which Azure Virtual Desktop resource is created by this command?

```bash
az desktopvirtualization hostpool create --name Pool01 --resource-group RG-AVD --host-pool-type Pooled --load-balancer-type BreadthFirst --max-session-limit 5
```

- [ ] **A)** A pooled host pool with breadth-first load balancing
- [ ] **B)** A personal host pool with automatic assignment
- [ ] **C)** A workspace with two application groups
- [ ] **D)** A registered session host VM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command creates a pooled host pool with breadth-first load balancing and a maximum session limit of five. It does not create a workspace or session host.
 
 
</details>

### 8. A business requires each user to have a dedicated session host virtual machine. Which Azure Virtual Desktop host pool type should the architect select?

- [ ] **A)** Personal host pool
- [ ] **B)** Pooled host pool
- [ ] **C)** Validation host pool
- [ ] **D)** Hybrid host pool

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A personal host pool assigns a dedicated session host to each user. Pooled host pools share session hosts across many users.
 
 
</details>

### 9. Which two statements accurately describe how FSLogix profile containers function in Azure Virtual Desktop?

- [ ] **A)** Stored as VHDX on SMB shares
- [ ] **B)** Mounted at sign-in and dismounted at sign-out
- [ ] **C)** Used only in personal host pools
- [ ] **D)** Requires Azure AD Domain Services

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> FSLogix stores profiles in VHDX files on SMB shares. Containers are attached at sign-in and detached at sign-out.
 
 
</details>

### 10. The registry snippet shown in the code block is about to be applied to a session host. Which FSLogix behavior is enabled by this configuration?

```powershell
[HKEY_LOCAL_MACHINE\SOFTWARE\FSLogix\Profiles]
"Enabled"=dword:00000001
"VHDLocations"="\\storageaccount.file.core.windows.net\profiles"
```

- [ ] **A)** Enables profiles and sets the VHD location
- [ ] **B)** Disables profile containers
- [ ] **C)** Creates a storage account
- [ ] **D)** Configures the Office container only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The registry key enables FSLogix profiles and sets the VHDLocations UNC path that session hosts use to mount profile containers.
 
 
</details>

### 11. In an Azure Virtual Desktop deployment, what is the role of a workspace in relation to application groups?

- [ ] **A)** It presents application groups to users
- [ ] **B)** It stores session host VMs
- [ ] **C)** It manages load balancing
- [ ] **D)** It provides domain authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A workspace is the presentation layer that makes application groups visible to clients. It does not store VMs or manage sessions.
 
 
</details>

### 12. Which two network practices should be implemented when deploying session hosts for Azure Virtual Desktop?

- [ ] **A)** Allow outbound HTTPS to AVD endpoints
- [ ] **B)** Block inbound RDP from the internet
- [ ] **C)** Place session hosts on the domain controller subnet
- [ ] **D)** Allow inbound RDP from all public IPs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Session hosts need outbound HTTPS to AVD endpoints and should block direct inbound internet RDP because reverse connect is used.
 
 
</details>

### 13. The command in the code block changes the load-balancing type of an Azure Virtual Desktop host pool. Which user session behavior will result?

```bash
az desktopvirtualization hostpool update --name Pool01 --resource-group RG-AVD --load-balancer-type DepthFirst
```

- [ ] **A)** New sessions fill one host before moving to the next
- [ ] **B)** New sessions spread evenly across all hosts
- [ ] **C)** The pool becomes a personal host pool
- [ ] **D)** All session hosts start automatically

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Depth-first load balancing sends new sessions to a host until its maximum session limit is reached before using the next host.
 
 
</details>

### 14. Which Azure Virtual Desktop load-balancing algorithm should be selected when the goal is to minimize the number of active session hosts?

- [ ] **A)** Depth-first
- [ ] **B)** Breadth-first
- [ ] **C)** Round robin
- [ ] **D)** Random distribution

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Depth-first minimizes the number of running hosts by filling each host to its session limit before using another host.
 
 
</details>

### 15. Which two software components must be installed on a session host to support registration with the Azure Virtual Desktop control plane?

- [ ] **A)** AVD Agent
- [ ] **B)** Bootloader
- [ ] **C)** FSLogix Agent
- [ ] **D)** Azure Backup Extension

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The AVD Agent communicates with the control plane, and the Bootloader handles side-by-side upgrades of the agent.
 
 
</details>

### 16. An administrator executes the PowerShell command in the code block. What does this command generate for the Azure Virtual Desktop host pool?

```powershell
$token = New-AzWvdRegistrationInfo -HostPoolName 'Pool01' -ResourceGroupName 'RG-AVD' -ExpirationTime (Get-Date).AddDays(30)
```

- [ ] **A)** A registration token valid for 30 days
- [ ] **B)** A new host pool in the resource group
- [ ] **C)** An Azure Active Directory account
- [ ] **D)** A storage account SAS token

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command generates registration information with a token used to register session hosts to the named host pool before it expires.
 
 
</details>

### 17. Which profile container solution is recommended for maintaining user settings in Azure Virtual Desktop pooled and personal host pools?

- [ ] **A)** FSLogix profile containers
- [ ] **B)** Windows roaming profiles
- [ ] **C)** Local user profiles
- [ ] **D)** OneDrive Known Folder Move

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> FSLogix profile containers are the recommended profile solution for AVD, providing persistent profiles in pooled and personal host pools.
 
 
</details>

### 18. Which two fully managed Azure storage services are commonly recommended for hosting FSLogix profile containers?

- [ ] **A)** Azure Files
- [ ] **B)** Azure NetApp Files
- [ ] **C)** Local temporary disk
- [ ] **D)** Azure Blob storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure Files and Azure NetApp Files are fully managed SMB-based storage services commonly used for FSLogix profile containers.
 
 
</details>


---

### **Plan and implement identity and security**

### 19. Which Microsoft service provides a fully managed domain in Azure for AVD session hosts without requiring you to manage domain controllers?

- [ ] **A)** Microsoft Entra Domain Services
- [ ] **B)** Active Directory Domain Services on Azure VMs
- [ ] **C)** Microsoft Entra ID
- [ ] **D)** On-premises Active Directory Domain Services

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Microsoft Entra Domain Services is the managed domain service that supports domain join and Kerberos/NTLM authentication without requiring domain controller management.
 
 
</details>

### 20. Which two components are required to synchronize on-premises AD DS users so they can authenticate through Microsoft Entra Domain Services?

- [ ] **A)** Microsoft Entra Connect
- [ ] **B)** Password Hash Synchronization
- [ ] **C)** Pass-Through Authentication
- [ ] **D)** Active Directory Federation Services

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Hybrid users must be synchronized by Microsoft Entra Connect, and Password Hash Synchronization must be enabled to supply password hashes for the managed domain.
 
 
</details>

### 21. An administrator prepares the Entra Connect configuration shown. What must be changed before Microsoft Entra Domain Services can authenticate hybrid AVD users?

```json
{
  "syncMethod": "PassThroughAuthentication",
  "syncPasswordHashes": false,
  "scopedOUs": ["OU=AVDUsers,DC=contoso,DC=com"]
}
```

- [ ] **A)** Enable Password Hash Synchronization
- [ ] **B)** Switch to Active Directory Federation Services
- [ ] **C)** Disable OU scoping
- [ ] **D)** Set sync method to Seamless SSO only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Entra DS requires password hashes for Kerberos/NTLM, so Password Hash Synchronization must be enabled; pass-through authentication alone is insufficient.
 
 
</details>

### 22. Which RBAC role must be assigned to a Microsoft Entra ID group at the application group scope so users can access published AVD resources?

- [ ] **A)** Desktop Virtualization User
- [ ] **B)** Desktop Virtualization Reader
- [ ] **C)** Desktop Virtualization Session Host Operator
- [ ] **D)** Virtual Machine User Login

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Desktop Virtualization User role includes the data actions required to discover and launch published desktops and RemoteApps when scoped to the application group.
 
 
</details>

### 23. Which two tasks can be performed by an administrator who has the Desktop Virtualization Session Host Operator role on a host pool?

- [ ] **A)** Place session hosts in drain mode
- [ ] **B)** Log off active user sessions
- [ ] **C)** Delete the host pool
- [ ] **D)** Assign RBAC roles to other users

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> This role supports session host and user session management at the host pool scope but does not allow deleting host pools or delegating access.
 
 
</details>


---

### **Plan and implement user environments and apps**

### 24. Where must FSLogix profile containers be stored in an Azure Virtual Desktop pooled environment?

- [ ] **A)** A central SMB 3.0 file share
- [ ] **B)** The local disk of each session host
- [ ] **C)** A standard Azure Blob container as the primary store
- [ ] **D)** A mapped drive letter on the session host

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> FSLogix profile containers must be on a central SMB 3.0 share such as Azure Files or NetApp Files; local disks and mapped drives are unsupported.
 
 
</details>

### 25. Which storage provider types are supported in FSLogix Cloud Cache locations? Select all that apply.

- [ ] **A)** azureFiles
- [ ] **B)** azureBlob
- [ ] **C)** samba
- [ ] **D)** netapp

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> Cloud Cache supports azureFiles, azureBlob, samba, and netapp as provider types for replicating profile containers.
 
 
</details>

### 26. Review the registry excerpt. What additional prerequisite must be satisfied for FSLogix to mount profiles from the configured location?

```registry
HKLM\SOFTWARE\FSLogix\Profiles
EnableFSLogix = 1
VHDLocations = "\\storageaccount.file.core.windows.net\profiles"
```

- [ ] **A)** SMB 3.0 share with identity-based authentication
- [ ] **B)** Cloud Cache locations must be configured before mounting
- [ ] **C)** The Office 365 container must be enabled
- [ ] **D)** The profile share must be an Azure Blob container

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> FSLogix requires an SMB 3.0 share with identity-based authentication for the configured UNC path; Cloud Cache and ODFC are optional.
 
 
</details>

### 27. What is true about the built-in application group created with an AVD host pool?

- [ ] **A)** It is a Desktop group publishing the full desktop; one per host pool
- [ ] **B)** It is a RemoteApp group that can be created multiple times
- [ ] **C)** It automatically appears to users without workspace registration
- [ ] **D)** It can be converted to a RemoteApp group after creation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Every host pool has one built-in Desktop application group. It still requires workspace registration and user assignment to appear.
 
 
</details>

### 28. Which steps are required for a user to see and launch a RemoteApp in the AVD feed? Select all that apply.

- [ ] **A)** Assign the user the Desktop Virtualization User role on the application group
- [ ] **B)** Register the application group to a workspace
- [ ] **C)** Grant the user read or Desktop Virtualization User access on the workspace
- [ ] **D)** Add the user to the host pool's built-in role for direct RDP access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> AVD feed access requires an application group assignment, workspace registration, and workspace-level access; host pool role assignment is not enough.
 
 
</details>

### 29. An administrator runs the PowerShell command shown. What must be true of the target application group for this command to succeed?

```powershell
Add-AzWvdApplication -ResourceGroupName "rg-avd" -GroupName "AppGroup-Prod" -Name "Excel" -FilePath "C:\Program Files\Microsoft Office\root\Office16\EXCEL.EXE" -IconPath "C:\Program Files\Microsoft Office\root\Office16\EXCEL.EXE" -IconIndex 0
```

- [ ] **A)** It must be a RemoteApp application group
- [ ] **B)** It must be a Desktop application group
- [ ] **C)** It must be an MSIX app attach package group
- [ ] **D)** It must be the built-in default Desktop group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Add-AzWvdApplication is used to publish individual applications and is valid only inside a RemoteApp application group.
 
 
</details>

### 30. Which storage option is recommended for hosting MSIX app attach packages?

- [ ] **A)** Azure Files premium share accessible over SMB
- [ ] **B)** Standard Azure Blob container
- [ ] **C)** Local disk on each session host
- [ ] **D)** The same share used for FSLogix profiles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MSIX app attach should use a premium Azure Files share over SMB; the profile share is separate and Blob or local storage is unsupported.
 
 
</details>

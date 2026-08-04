<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Microsoft%20Certified-%20Azure%20Administrator%20Associate.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Microsoft Certified: Azure Administrator Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Deploy and manage Azure compute resources](#deploy-and-manage-azure-compute-resources) (8 questions)
- [Implement and manage storage](#implement-and-manage-storage) (6 questions)
- [Implement and manage virtual networking](#implement-and-manage-virtual-networking) (4 questions)
- [Manage Azure identities and governance](#manage-azure-identities-and-governance) (8 questions)
- [Monitor and maintain Azure resources](#monitor-and-maintain-azure-resources) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:37.352Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Deploy and manage Azure compute resources | 8 |
| Implement and manage storage | 6 |
| Implement and manage virtual networking | 4 |
| Manage Azure identities and governance | 8 |
| Monitor and maintain Azure resources | 4 |

---

### **Deploy and manage Azure compute resources**

### 1. Which Azure compute offering provides full control over the operating system, applications, and configuration as an IaaS service?

- [ ] **A)** Azure virtual machine
- [ ] **B)** Virtual machine scale set
- [ ] **C)** Azure Container Instances
- [ ] **D)** Azure App Service

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A virtual machine is Azure's IaaS offering that provides control over the OS and applications. A scale set is a collection of identical VMs, but the definition of a single VM emphasizes full configuration control.
 
 
</details>

### 2. Which two statements correctly describe Azure Virtual Machine Scale Sets (VMSS)?

- [ ] **A)** A VMSS can automatically scale out and scale in based on metrics such as CPU or custom metrics.
- [ ] **B)** A VMSS requires each instance to run a different operating system image.
- [ ] **C)** VMSS instances are identical and are often placed behind an Azure Load Balancer or Application Gateway.
- [ ] **D)** A VMSS provides built-in disaster recovery replication to a secondary region.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> VMSS deploys identical VMs and supports autoscaling based on metrics. It is commonly integrated with load balancers or application gateways. It does not require different images and does not provide built-in disaster recovery.
 
 
</details>

### 3. What does running this Azure CLI command accomplish?

```bash
az vm create --resource-group RG1 --name VM1 --image UbuntuLTS --admin-username azureuser --generate-ssh-keys
```

- [ ] **A)** Creates a Linux virtual machine and generates SSH keys
- [ ] **B)** Creates a Windows virtual machine with a password
- [ ] **C)** Creates a virtual machine scale set
- [ ] **D)** Deletes an existing virtual machine and its SSH keys

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command creates an Ubuntu Linux VM and uses --generate-ssh-keys to create SSH keys for authentication.
 
 
</details>

### 4. Which high availability option provides physical separation within an Azure region by using separate buildings and offers a 99.99% VM SLA?

- [ ] **A)** Availability Zones
- [ ] **B)** Availability Sets
- [ ] **C)** Recovery Services vault
- [ ] **D)** Azure Site Recovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Availability Zones are physically separate locations within an Azure region and provide a 99.99% SLA for VMs. Availability Sets protect against failures inside a single datacenter.
 
 
</details>

### 5. Which two statements about Azure Backup are true?

- [ ] **A)** Azure Backup can provide automated failover to a secondary region.
- [ ] **B)** Azure Backup stores recovery points in a Recovery Services vault.
- [ ] **C)** Azure Backup supports soft delete by default to protect against accidental deletion.
- [ ] **D)** Azure Backup replicates VMs continuously with a recovery point objective of seconds.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Azure Backup stores recovery points in a Recovery Services vault and has soft delete enabled by default. Automated failover and continuous replication are features of Azure Site Recovery.
 
 
</details>

### 6. What is the purpose of the Bicep code shown?

```bicep
resource storageAccount 'Microsoft.Storage/storageAccounts@2023-01-01' = {
  name: 'mystorageaccount'
  location: resourceGroup().location
  sku: {
    name: 'Standard_LRS'
  }
  kind: 'StorageV2'
}
```

- [ ] **A)** Deploys a storage account with locally redundant storage
- [ ] **B)** Deploys a virtual machine with a public IP
- [ ] **C)** Deploys an App Service plan
- [ ] **D)** Deploys a virtual network and subnet

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Bicep code declares a Microsoft.Storage/storageAccounts resource with the Standard_LRS SKU and StorageV2 kind, so it deploys a storage account.
 
 
</details>

### 7. Which is the minimum App Service plan tier required for autoscaling?

- [ ] **A)** Free
- [ ] **B)** Basic
- [ ] **C)** Standard
- [ ] **D)** Isolated

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Autoscaling is available from the Standard App Service plan tier and above. Basic supports only manual scaling, and Free does not support autoscaling.
 
 
</details>

### 8. Which two statements about App Service deployment slots are correct?

- [ ] **A)** Deployment slots are available in Standard, Premium, and Isolated tiers.
- [ ] **B)** Swapping between slots is performed with zero downtime.
- [ ] **C)** Deployment slots are automatically created in the Free tier.
- [ ] **D)** Slot-sticky settings are moved to the other slot during a swap.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Deployment slots are available from Standard tier upward and swapping can be done with zero downtime. Slot-sticky settings remain with their original slot and are not moved during a swap.
 
 
</details>


---

### **Implement and manage storage**

### 9. Which storage account kind is the recommended default when you need support for blobs, files, queues, tables, and all access tiers?

- [ ] **A)** General-purpose v2
- [ ] **B)** BlobStorage
- [ ] **C)** FileStorage
- [ ] **D)** BlockBlobStorage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> General-purpose v2 is the recommended default because it supports all storage services and all access tiers.
 
 
</details>

### 10. Which replication options are supported for premium block blob and premium Azure file share accounts?

- [ ] **A)** Locally Redundant Storage (LRS)
- [ ] **B)** Zone-Redundant Storage (ZRS)
- [ ] **C)** Geo-Redundant Storage (GRS)
- [ ] **D)** Read-Access Geo-Redundant Storage (RA-GRS)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Premium block blob and premium file share accounts only support LRS and ZRS; GRS and RA-GRS are not available.
 
 
</details>

### 11. Review the Azure CLI command in the code block. If a blob is uploaded without an explicit access tier, which tier will be assigned?

```azurecli
az storage account create --name examstorage112 --resource-group rg-112 --location eastus --sku Standard_LRS --kind StorageV2 --access-tier Hot

```

- [ ] **A)** Hot
- [ ] **B)** Cool
- [ ] **C)** Archive
- [ ] **D)** Premium

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The account is created with --access-tier Hot, so blobs uploaded without an explicit tier use the Hot tier.
 
 
</details>

### 12. Which storage replication option provides 11 nines of durability?

- [ ] **A)** Locally Redundant Storage (LRS)
- [ ] **B)** Zone-Redundant Storage (ZRS)
- [ ] **C)** Geo-Redundant Storage (GRS)
- [ ] **D)** Geo-Zone-Redundant Storage (GZRS)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> LRS copies data three times in a single datacenter and provides 11 nines durability.
 
 
</details>

### 13. Which two statements about Azure Blob storage access tiers are correct?

- [ ] **A)** Cool tier has a 30-day minimum storage duration.
- [ ] **B)** Archive tier can require up to 15 hours to retrieve a blob.
- [ ] **C)** Archive tier is an account-level setting.
- [ ] **D)** Hot tier has the lowest storage cost per GB.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Cool has a 30-day minimum, Archive rehydration can take up to 15 hours; Archive is blob-level and Hot has highest storage cost.
 
 
</details>

### 14. The code block generates a SAS token for a container. Which permissions does the token grant?

```azurecli
az storage container generate-sas --account-name examstorage112 --name docs --permissions rl --expiry 2025-12-31T23:59:00Z --https-only

```

- [ ] **A)** Read and List
- [ ] **B)** Read and Write
- [ ] **C)** Write and Delete
- [ ] **D)** Full control

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The --permissions rl parameter grants read (r) and list (l) access only.
 
 
</details>


---

### **Implement and manage virtual networking**

### 15. How many usable IP addresses does a /24 Azure subnet provide after Azure reserves its required addresses?

- [ ] **A)** 251
- [ ] **B)** 256
- [ ] **C)** 253
- [ ] **D)** 252

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure reserves five IP addresses per subnet, so a /24 subnet with 256 total addresses leaves 251 usable addresses.
 
 
</details>

### 16. Which two statements correctly describe VNet peering behavior in Azure?

- [ ] **A)** VNet peering is non-transitive by default.
- [ ] **B)** Global peering connects VNets across Azure regions.
- [ ] **C)** Peering requires overlapping address spaces.
- [ ] **D)** Peered VNets share the same DNS servers automatically.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VNet peering is non-transitive and can be regional or global. Overlapping address spaces prevent peering, and DNS configuration is not automatically shared.
 
 
</details>

### 17. You run the subnet creation command shown in the code block. What is the direct result of this command?

```bash
az network vnet subnet create \
  --name GatewaySubnet \
  --resource-group RG1 \
  --vnet-name VNet1 \
  --address-prefixes 10.0.0.0/27
```

- [ ] **A)** Creates a /27 subnet with 27 usable addresses.
- [ ] **B)** Creates a /27 subnet with 32 usable addresses.
- [ ] **C)** Delegates the subnet to Azure Container Instances.
- [ ] **D)** Creates a /27 subnet with 5 usable addresses.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command creates a subnet named GatewaySubnet using a /27 prefix. A /27 has 32 total addresses; Azure reserves five, leaving 27 usable.
 
 
</details>

### 18. Which Network Watcher tool verifies the allow or deny decision for a single packet based on effective NSG rules?

- [ ] **A)** IP Flow Verify
- [ ] **B)** Next Hop
- [ ] **C)** Connection Monitor
- [ ] **D)** Packet Capture

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IP Flow Verify evaluates a single packet against NSGs and routes, returning the allow or deny decision and the rule that caused it.
 
 
</details>


---

### **Manage Azure identities and governance**

### 19. Which Azure AD object serves as the identity for an application to authenticate and access Azure resources?

- [ ] **A)** Service principal
- [ ] **B)** User
- [ ] **C)** Security group
- [ ] **D)** Management group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Service principals are Azure AD identities created for applications, services, and automation tools to authenticate to Azure resources.
 
 
</details>

### 20. Which two membership types can be configured for Azure AD groups?

- [ ] **A)** Assigned
- [ ] **B)** Dynamic
- [ ] **C)** Security
- [ ] **D)** Microsoft 365

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure AD groups support assigned and dynamic membership. Security and Microsoft 365 are group types, not membership types.
 
 
</details>

### 21. What is the effect of the command shown in the code block?

```azurecli
az role assignment create --assignee user@contoso.com --role Contributor --scope /subscriptions/12345/resourceGroups/Finance
```

- [ ] **A)** Assigns the Contributor role to a user at the Finance resource group
- [ ] **B)** Creates a new custom role named Contributor
- [ ] **C)** Creates a new Azure AD group
- [ ] **D)** Applies an Azure Policy to the subscription

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This Azure CLI command creates a role assignment that grants the specified user the Contributor role at the Finance resource group scope.
 
 
</details>

### 22. Which Azure capability should you use to enforce a rule that virtual machines can only be deployed in West Europe?

- [ ] **A)** Azure Policy
- [ ] **B)** Azure RBAC
- [ ] **C)** Azure AD roles
- [ ] **D)** Management groups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Policy enforces resource configuration rules, such as allowed locations, using effects like Deny. RBAC controls identity permissions, not resource properties.
 
 
</details>

### 23. Which two built-in RBAC roles can delegate access by assigning roles to other users?

- [ ] **A)** Owner
- [ ] **B)** User Access Administrator
- [ ] **C)** Contributor
- [ ] **D)** Reader

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Only Owner and User Access Administrator can manage role assignments. Contributor can manage resources but cannot delegate access.
 
 
</details>

### 24. What is the effect of the command shown in the code block?

```azurecli
az account management-group subscription add --management-group-id Production --subscription 12345678-1234-1234-1234-123456789012
```

- [ ] **A)** Adds a subscription to the Production management group
- [ ] **B)** Creates a new management group named Production
- [ ] **C)** Deletes the Production management group
- [ ] **D)** Assigns an Azure policy to the subscription

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command adds the specified subscription to the Production management group, making it a child of that group.
 
 
</details>

### 25. Which Azure AD role must be assigned at the root management group scope to delegate tenant-wide RBAC management?

- [ ] **A)** User Access Administrator
- [ ] **B)** Global Administrator
- [ ] **C)** Application Administrator
- [ ] **D)** Password Administrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> User Access Administrator at the root scope is needed to assign roles and manage tenant-wide RBAC.
 
 
</details>

### 26. Which two statements about Azure Policy are correct?

- [ ] **A)** A Deny effect can block creation of non-compliant resources.
- [ ] **B)** Azure Policy evaluates resource configuration, not user permissions.
- [ ] **C)** A Deny effect can prevent resource deletion.
- [ ] **D)** Policy assignments are not inherited by child scopes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure Policy enforces configuration rules and can block non-compliant creation with Deny, but it cannot block deletion and assignments inherit to child scopes.
 
 
</details>


---

### **Monitor and maintain Azure resources**

### 27. Which Azure service provides the foundational monitoring platform for collecting, analyzing, and acting on telemetry from cloud and hybrid environments?

- [ ] **A)** Azure Monitor
- [ ] **B)** Azure Advisor
- [ ] **C)** Azure Service Health
- [ ] **D)** Azure Cost Management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Monitor is the foundational monitoring platform for Azure, providing telemetry collection, analysis, and alerts for cloud and hybrid resources.
 
 
</details>

### 28. Which of the following action types can be configured in an Azure action group? Select all that apply.

- [ ] **A)** Email
- [ ] **B)** SMS
- [ ] **C)** Webhook
- [ ] **D)** Azure Policy assignment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Action groups support email, SMS, voice, webhook, ITSM, Azure Function, Logic App, and Automation runbook actions. Azure Policy assignment is not an action group action type.
 
 
</details>

### 29. Examine the KQL query in the code block. What is the output of this sign-in log query?

```kql
SigninLogs
| where ResultType != 0
| summarize count() by bin(TimeGenerated, 15m)
```

- [ ] **A)** Failed sign-ins grouped into 15-minute intervals
- [ ] **B)** Successful sign-ins grouped into 15-minute intervals
- [ ] **C)** All sign-ins where ResultType is zero
- [ ] **D)** A count of all sign-in events by user

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query filters SigninLogs to non-zero ResultType values, then uses summarize count() by bin(TimeGenerated, 15m) to count failed sign-ins in 15-minute intervals.
 
 
</details>

### 30. Which component of Azure Service Health provides the health state of an individual Azure resource, such as a specific virtual machine?

- [ ] **A)** Resource Health
- [ ] **B)** Azure Status
- [ ] **C)** Service Health
- [ ] **D)** Azure Advisor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Resource Health gives status for individual Azure resources such as a VM. Azure Status and Service Health focus on platform and subscription-level events.
 
 
</details>

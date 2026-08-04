<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Microsoft%20Certified%3A%20Azure%20Fundamentals" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Microsoft Certified: Azure Fundamentals</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Describe Azure architecture and services](#describe-azure-architecture-and-services) (13 questions)
- [Describe Azure management and governance](#describe-azure-management-and-governance) (7 questions)
- [Describe cloud concepts](#describe-cloud-concepts) (10 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:39.897Z |
| Domains | 3 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Describe Azure architecture and services | 13 |
| Describe Azure management and governance | 7 |
| Describe cloud concepts | 10 |

---

### **Describe Azure architecture and services**

### 1. What is the main function of a resource group in Azure?

- [ ] **A)** To define geographical boundaries for data residency
- [ ] **B)** To provide high availability within a region
- [ ] **C)** To logically group related resources for lifecycle management
- [ ] **D)** To encrypt data at rest

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> A resource group is a logical container that holds related resources, enabling shared lifecycle and management.
 
 
</details>

### 2. Which of the following are PaaS compute services in Azure? (Choose all that apply)

- [ ] **A)** Azure Virtual Machines
- [ ] **B)** Azure App Service
- [ ] **C)** Azure Functions
- [ ] **D)** Azure Container Instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C, D**
 
> 💡  **Explanation** 
> 
> Azure App Service, Functions, and Container Instances are all managed platform services abstracting underlying infrastructure.
 
 
</details>

### 3. Examine the ARM template. What Azure resource does it create?

```json
{
  "$schema": "https://schema.management.azure.com/schemas/2019-04-01/deploymentTemplate.json#",
  "contentVersion": "1.0.0.0",
  "resources": [
    {
      "type": "Microsoft.Network/virtualNetworkGateways",
      "apiVersion": "2022-01-01",
      "name": "myVpnGateway",
      "properties": {
        "gatewayType": "Vpn",
        "vpnType": "RouteBased"
      }
    }
  ]
}
```

- [ ] **A)** Azure Virtual Network
- [ ] **B)** Azure VPN Gateway
- [ ] **C)** Azure Load Balancer
- [ ] **D)** Azure DNS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The template deploys a virtual network gateway of type 'Vpn', which is an Azure VPN Gateway.
 
 
</details>

### 4. Which service should you use to migrate a legacy app needing full OS control?

- [ ] **A)** Azure Functions
- [ ] **B)** Azure App Service
- [ ] **C)** Azure Virtual Machines
- [ ] **D)** Azure Container Instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Virtual Machines provide full control over the OS and software, suitable for legacy migrations.
 
 
</details>

### 5. Select the correct statements about Azure Load Balancer.

- [ ] **A)** Operates at Layer 7
- [ ] **B)** Distributes traffic across backend resources
- [ ] **C)** Supports health probes
- [ ] **D)** Provides SSL termination

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Load Balancer works at Layer 4, distributes traffic, and uses health probes to remove unhealthy instances.
 
 
</details>

### 6. In the CLI command, which redundancy option is specified?

```bash
az storage account create --name mystorage --resource-group myrg --sku Standard_GRS --kind StorageV2
```

- [ ] **A)** Locally Redundant Storage (LRS)
- [ ] **B)** Geo-Redundant Storage (GRS)
- [ ] **C)** Zone-Redundant Storage (ZRS)
- [ ] **D)** Read-Access Geo-Redundant Storage (RA-GRS)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The SKU Standard_GRS specifies Geo-Redundant Storage, which replicates data to a secondary region.
 
 
</details>

### 7. Which service offers a private, dedicated network connection to Azure?

- [ ] **A)** Azure VPN Gateway
- [ ] **B)** Azure ExpressRoute
- [ ] **C)** Azure Application Gateway
- [ ] **D)** Azure DNS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> ExpressRoute establishes a private connection to Azure, not using the public internet, offering higher reliability and lower latency.
 
 
</details>

### 8. Select the Azure Storage redundancy options that enable reading from the secondary region.

- [ ] **A)** Locally Redundant Storage (LRS)
- [ ] **B)** Read-Access Geo-Redundant Storage (RA-GRS)
- [ ] **C)** Geo-Redundant Storage (GRS)
- [ ] **D)** Read-Access Geo-Zone Redundant Storage (RA-GZRS)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> RA-GRS and RA-GZRS both allow read access to the secondary region, while GRS and GZRS do not.
 
 
</details>

### 9. Based on the connection string, which database service is targeted?

```text
Server=tcp:myserver.database.windows.net,1433;Database=mydb;User Id=admin;Password=pass;
```

- [ ] **A)** Azure Cosmos DB
- [ ] **B)** Azure SQL Database
- [ ] **C)** Azure Database for MySQL
- [ ] **D)** Azure Synapse Analytics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The connection string format 'Server=tcp:*.database.windows.net' is typical for Azure SQL Database.
 
 
</details>

### 10. Which storage service is best for storing large binary objects?

- [ ] **A)** Azure Blob Storage
- [ ] **B)** Azure Disk Storage
- [ ] **C)** Azure Files
- [ ] **D)** Azure Queue Storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Blob Storage is optimized for massive amounts of unstructured object data such as images, videos, and backups.
 
 
</details>

### 11. Select the correct statements regarding Azure Cosmos DB.

- [ ] **A)** It is a globally distributed database service
- [ ] **B)** It supports only the SQL API
- [ ] **C)** It offers tunable consistency levels
- [ ] **D)** It provides single-digit millisecond latency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Cosmos DB is globally distributed, offers multiple consistency models, guarantees low latency, and supports multiple APIs.
 
 
</details>

### 12. What does this CLI command do in terms of access management?

```bash
az role assignment create --assignee user@contoso.com --role Contributor --resource-group myrg
```

- [ ] **A)** Assigns the Reader role to the user
- [ ] **B)** Assigns the Contributor role to the user at resource group scope
- [ ] **C)** Assigns the Owner role to the user
- [ ] **D)** Removes all role assignments for the user

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The command assigns the Contributor role to the specified user for the specified resource group.
 
 
</details>

### 13. For petabyte-scale analytics, which Azure database service is recommended?

- [ ] **A)** Azure SQL Database
- [ ] **B)** Azure Database for PostgreSQL
- [ ] **C)** Azure Cosmos DB
- [ ] **D)** Azure Synapse Analytics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> Synapse Analytics is purpose-built for massive parallel processing and petabyte-scale analytics, unlike OLTP databases.
 
 
</details>


---

### **Describe Azure management and governance**

### 14. An administrator runs the following Azure CLI command: `az policy assignment create --name 'DenyUnmanagedDisks' --policy 'abc123' --scope /subscriptions/00000000-0000-0000-0000-000000000000`. What is the effect of this command?

```bash
az policy assignment create --name 'DenyUnmanagedDisks' --policy 'abc123' --scope /subscriptions/00000000-0000-0000-0000-000000000000
```

- [ ] **A)** It creates a new policy definition
- [ ] **B)** It assigns an existing policy definition to the specified subscription scope
- [ ] **C)** It modifies the policy definition's effect to 'Deny'
- [ ] **D)** It removes all previous policy assignments from the subscription

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The command assigns an existing policy definition (referenced by ID 'abc123') to the subscription scope. A policy assignment enforces the policy's rules (e.g., Deny unmanaged disks) on resources within that scope.
 
 
</details>

### 15. A developer runs the following Azure CLI command: `az group create --name MyResourceGroup --location eastus`. What is the result of this command?

```bash
az group create --name MyResourceGroup --location eastus
```

- [ ] **A)** It deploys a set of Azure resources into a new resource group
- [ ] **B)** It creates a new, empty resource group in the East US region
- [ ] **C)** It creates a virtual machine named MyResourceGroup
- [ ] **D)** It creates a management group for organizing subscriptions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The command creates a new resource group named 'MyResourceGroup' in the 'eastus' location. Resource groups are logical containers for resources and do not contain any resources at creation time unless specified.
 
 
</details>

### 16. An administrator creates a policy definition with the following JSON: it checks if the resource location is in a list of allowed regions. What type of effect would block non-compliant resource creation?

```json
{
  "policyRule": {
    "if": {
      "not": {
        "field": "location",
        "in": ["eastus", "westus"]
      }
    },
    "then": {
      "effect": "Deny"
    }
  }
}
```

- [ ] **A)** Audit
- [ ] **B)** Deny
- [ ] **C)** Append
- [ ] **D)** DeployIfNotExists

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 'Deny' effect blocks resource creation or update if the condition is met. 'Audit' only logs non-compliance but allows creation. 'Append' adds fields and 'DeployIfNotExists' deploys additional resources.
 
 
</details>

### 17. Which Azure tool provides automated recommendations to improve cost, security, reliability, performance, and operational excellence?

- [ ] **A)** Azure Monitor
- [ ] **B)** Azure Advisor
- [ ] **C)** Azure Service Health
- [ ] **D)** Azure Cost Management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Azure Advisor is a built-in recommendation engine that provides suggestions in five categories: cost, security, reliability, performance, and operational excellence. Azure Monitor collects telemetry, Service Health reports platform issues, and Cost Management tracks billing.
 
 
</details>

### 18. Which of the following are benefits of using Azure management groups? (Choose all that apply.)

- [ ] **A)** They allow applying policies across multiple subscriptions at once.
- [ ] **B)** They can directly contain Azure resources such as VMs.
- [ ] **C)** They enable inheritance of RBAC assignments to all subscriptions in the hierarchy.
- [ ] **D)** They can be nested up to six levels deep for organizational structure.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Management groups are containers for subscriptions only, not resources. They allow policy and RBAC inheritance across all subscriptions in the hierarchy and can be nested up to six levels.
 
 
</details>

### 19. An administrator runs the following Azure PowerShell cmdlet: `Get-AzResourceGroup -Name MyResourceGroup`. What information does this command retrieve?

```powershell
Get-AzResourceGroup -Name MyResourceGroup
```

- [ ] **A)** It deletes the specified resource group and all its resources
- [ ] **B)** It returns the properties (name, location, tags) of the specified resource group
- [ ] **C)** It creates a new resource group with that name
- [ ] **D)** It lists all virtual machines inside the resource group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The `Get-AzResourceGroup` cmdlet retrieves information about one or more resource groups. Here it targets a specific resource group by name and returns its metadata such as location, tags, and provisioning state.
 
 
</details>

### 20. How can you prevent accidental deletion of an Azure resource group and all its resources?

- [ ] **A)** Assign the Reader role to all users
- [ ] **B)** Apply a CanNotDelete lock on the resource group
- [ ] **C)** Use Azure Policy to deny delete operations
- [ ] **D)** Add a tag named 'DoNotDelete'

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A CanNotDelete lock prevents deletion of the resource group and all resources within it. Locks override RBAC permissions, so even an Owner cannot delete. RBAC roles and Azure Policy cannot prevent deletion of existing resources.
 
 
</details>


---

### **Describe cloud concepts**

### 21. Which cloud computing benefit ensures that applications remain operational even if one component fails by using redundant infrastructure across multiple availability zones?

- [ ] **A)** High availability
- [ ] **B)** Scalability
- [ ] **C)** Security
- [ ] **D)** Governance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> High availability (HA) is the ability of a system to remain operational despite component failures. Azure achieves HA through redundancy across Availability Zones (physically separate datacenters within a region). Scalability deals with capacity adjustment, security with protection, and governance with policies and compliance.
 
 
</details>

### 22. Which of the following Azure services are classified as Platform-as-a-Service (PaaS)? (Select all that apply.)

- [ ] **A)** Azure App Service
- [ ] **B)** Azure Virtual Machines
- [ ] **C)** Azure SQL Database
- [ ] **D)** Microsoft 365

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Azure App Service and Azure SQL Database are PaaS services because they provide a managed platform where customers deploy applications or databases without managing the underlying OS. Azure VMs are IaaS (customer manages OS). Microsoft 365 is SaaS.
 
 
</details>

### 23. Refer to the code block. Which cloud service model does the command represent?

```bash
az vm create --resource-group MyRG --name MyVM --image UbuntuLTS --size Standard_B1s --admin-username azureuser
```

- [ ] **A)** Infrastructure-as-a-Service (IaaS)
- [ ] **B)** Platform-as-a-Service (PaaS)
- [ ] **C)** Software-as-a-Service (SaaS)
- [ ] **D)** On-premises virtualization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command 'az vm create' deploys a virtual machine, which is an IaaS resource. The customer manages the OS, middleware, and applications on that VM, while Azure manages the physical host and hypervisor.
 
 
</details>

### 24. In the shared responsibility model for cloud security, which of the following is the responsibility of the cloud customer when using Infrastructure-as-a-Service (IaaS)?

- [ ] **A)** Patching the operating system running inside the virtual machine
- [ ] **B)** Securing the physical datacenter
- [ ] **C)** Maintaining the hypervisor
- [ ] **D)** Replacing failed network switches

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In IaaS, the cloud provider manages the physical infrastructure (datacenter, servers, network, hypervisor). The customer is responsible for everything inside the VM, including the operating system, applications, data, and network security configurations.
 
 
</details>

### 25. Which of the following are characteristics of the consumption-based (pay-as-you-go) pricing model? (Select all that apply.)

- [ ] **A)** No upfront capital expenditure required
- [ ] **B)** Costs increase linearly with resource usage
- [ ] **C)** You are billed a fixed monthly fee regardless of usage
- [ ] **D)** Resources must be pre-provisioned for peak demand to avoid overspending

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The consumption-based model shifts costs from CapEx to OpEx: you pay only for what you use, with no upfront investment. Costs increase with usage, but you can reduce them by scaling down. Fixed fees are typical of reserved capacity, not pay-as-you-go. Pre-provisioning for peak is a traditional on-premises approach; cloud allows dynamic scaling.
 
 
</details>

### 26. Examine the code block. This Azure Policy definition enforces a rule. Which cloud concept does this rule primarily support?

```json
{
  "if": {
    "field": "location",
    "notIn": ["eastus", "westus"]
  },
  "then": {
    "effect": "deny"
  }
}
```

- [ ] **A)** Governance
- [ ] **B)** High availability
- [ ] **C)** Scalability
- [ ] **D)** Disaster recovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Policy is a governance tool that enforces organizational rules (e.g., requiring tags or restricting regions) to ensure compliance and consistency. It does not directly provide high availability, scalability, or disaster recovery.
 
 
</details>

### 27. Which cloud deployment model is characterized by a single-tenant environment that can be hosted on-premises or by a third-party provider exclusively for one organization?

- [ ] **A)** Private cloud
- [ ] **B)** Public cloud
- [ ] **C)** Hybrid cloud
- [ ] **D)** Multi-cloud

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A private cloud is dedicated to a single organization, providing maximum control over security and compliance. It can be hosted on-premises or in a third-party datacenter as long as the infrastructure is not shared (single-tenant).
 
 
</details>

### 28. Which of the following are considerations or challenges of using cloud services that organizations must plan for? (Select all that apply.)

- [ ] **A)** Vendor lock-in
- [ ] **B)** Unpredictable costs if not properly monitored
- [ ] **C)** Automatic compliance with all regulations
- [ ] **D)** Elimination of all security responsibilities

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Cloud computing introduces risks such as vendor lock-in (dependency on a specific provider), cost variability without governance, and compliance complexity under the shared responsibility model. The provider does not automatically make you compliant, and security responsibilities are shared, not eliminated.
 
 
</details>

### 29. Analyze the code block. Which concept does this infrastructure deployment primarily illustrate?

```bicep
resource vm1 'Microsoft.Compute/virtualMachines@2023-03-01' = {
  name: 'vm-zone1'
  location: resourceGroup().location
  zones: ['1']
  properties: { ... }
}
resource vm2 'Microsoft.Compute/virtualMachines@2023-03-01' = {
  name: 'vm-zone2'
  location: resourceGroup().location
  zones: ['2']
  properties: { ... }
}
```

- [ ] **A)** High availability
- [ ] **B)** Scalability
- [ ] **C)** Governance
- [ ] **D)** Cost management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Bicep code deploys two virtual machines in separate availability zones (zone1 and zone2) behind a load balancer. This architecture is designed to provide high availability by ensuring that if one zone fails, the VM in the other zone continues serving traffic.
 
 
</details>

### 30. Which cloud service model provides the customer with the most control over the operating system and network configuration?

- [ ] **A)** Infrastructure-as-a-Service (IaaS)
- [ ] **B)** Platform-as-a-Service (PaaS)
- [ ] **C)** Software-as-a-Service (SaaS)
- [ ] **D)** Function-as-a-Service (FaaS)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IaaS gives customers the highest level of control over the operating system, networking, and storage. PaaS abstracts the OS and runtime, while SaaS and FaaS provide even less control. IaaS is suitable when full OS customization is required.
 
 
</details>

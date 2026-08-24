<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Azure%20Solutions%20Architect%20Expert.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Azure Solutions Architect Expert</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Design business continuity solutions](#design-business-continuity-solutions) (5 questions)
- [Design data storage solutions](#design-data-storage-solutions) (6 questions)
- [Design identity, governance, and monitoring solutions](#design-identity-governance-and-monitoring-solutions) (9 questions)
- [Design infrastructure solutions](#design-infrastructure-solutions) (10 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:52:50.613Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Design business continuity solutions | 5 |
| Design data storage solutions | 6 |
| Design identity, governance, and monitoring solutions | 9 |
| Design infrastructure solutions | 10 |

---

### **Design business continuity solutions**

### 1. Which Azure service is the native orchestration solution for workload replication, failover, and failback in a disaster recovery design?

- [ ] **A)** Azure Site Recovery
- [ ] **B)** Azure Backup
- [ ] **C)** Azure Storage
- [ ] **D)** Azure Monitor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Site Recovery performs continuous replication and automated failover/failback, while Azure Backup provides point-in-time data protection.
 
 
</details>

### 2. Which two statements correctly describe Read-Access Geo-Redundant Storage (RA-GRS)?

- [ ] **A)** Read access to data in the secondary region
- [ ] **B)** Write access to the secondary region
- [ ] **C)** Asynchronous replication to a paired secondary region
- [ ] **D)** Synchronous replication to two secondary regions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> RA-GRS provides read-only access to asynchronously replicated data in a paired secondary region, after local synchronous replication in the primary.
 
 
</details>

### 3. The code block contains Azure CLI commands for configuring a backup management entity. Which entity is being provisioned?

```bash
az backup vault create --name myRecoveryVault --resource-group rg-bcdr --location eastus
az backup vault backup-properties set --name myRecoveryVault --resource-group rg-bcdr --backup-storage-redundancy GeoRedundant
```

- [ ] **A)** Recovery Services Vault
- [ ] **B)** Backup Vault
- [ ] **C)** Site Recovery Vault
- [ ] **D)** Storage Sync Service

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The commands use the Azure CLI backup vault group, which provisions a Recovery Services Vault for Azure Backup workloads.
 
 
</details>

### 4. What does Recovery Point Objective (RPO) define in a business continuity plan?

- [ ] **A)** Maximum acceptable data loss measured in time
- [ ] **B)** Maximum duration of downtime after a disaster
- [ ] **C)** Minimum time required to test backups
- [ ] **D)** Time interval for automatic failover

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RPO is the maximum acceptable data loss expressed as time; RTO is the maximum acceptable duration of downtime.
 
 
</details>

### 5. Which two capabilities are provided by Azure Site Recovery?

- [ ] **A)** Continuous replication to a secondary location
- [ ] **B)** Orchestrated failover and failback
- [ ] **C)** Long-term compliance archiving
- [ ] **D)** Immutable storage for audit logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure Site Recovery focuses on replication and orchestrated failover or failback; long-term archiving is handled by Azure Backup.
 
 
</details>


---

### **Design data storage solutions**

### 6. Which Azure Cosmos DB consistency level provides the strongest data consistency guarantee for globally distributed applications?

- [ ] **A)** Strong
- [ ] **B)** Bounded Staleness
- [ ] **C)** Eventual
- [ ] **D)** Session

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Strong consistency provides the strongest data guarantee by ensuring reads always return the latest committed write in Azure Cosmos DB.
 
 
</details>

### 7. Which two Azure Storage redundancy options replicate your data to a secondary Azure region for disaster recovery? Select two.

- [ ] **A)** Locally redundant storage (LRS)
- [ ] **B)** Geo-redundant storage (GRS)
- [ ] **C)** Geo-zone-redundant storage (GZRS)
- [ ] **D)** Zone-redundant storage (ZRS)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Geo-redundant storage (GRS) and geo-zone-redundant storage (GZRS) replicate data to a secondary Azure region, while LRS and ZRS do not.
 
 
</details>

### 8. The code block shows a JSON document with user preferences and order details. Which Azure service should store this semi-structured document with global low-latency access?

```json
{
  "userId": "12345",
  "name": "Jane Doe",
  "preferences": {
    "theme": "dark",
    "language": "en"
  },
  "orders": [
    { "orderId": "A1", "total": 25.5 }
  ]
}
```

- [ ] **A)** Azure Cosmos DB
- [ ] **B)** Azure SQL Database
- [ ] **C)** Azure Blob Storage
- [ ] **D)** Azure Data Factory

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Cosmos DB is the recommended multi-model NoSQL service for globally distributed, schema-less JSON documents that require low-latency access.
 
 
</details>

### 9. Which feature must be enabled when creating an Azure Storage account to support Azure Data Lake Storage Gen2 functions?

- [ ] **A)** Hierarchical namespace
- [ ] **B)** Soft delete
- [ ] **C)** Blob versioning
- [ ] **D)** Infrastructure encryption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The hierarchical namespace must be enabled during Azure Storage account creation because it cannot be added later to an existing standard storage account.
 
 
</details>

### 10. Which two access control mechanisms can be used to secure Azure Storage accounts and their data? Select two.

- [ ] **A)** Role-Based Access Control (RBAC)
- [ ] **B)** Shared Access Signatures (SAS)
- [ ] **C)** Azure SQL firewall rules
- [ ] **D)** Azure Databricks clusters

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> RBAC and Shared Access Signatures are Azure Storage security mechanisms that control access to data without exposing account keys.
 
 
</details>

### 11. The SQL query in the code block uses joins to combine relational data. Which Azure data architecture is best suited to run this workload?

```sql
SELECT OrderID, CustomerName
FROM Orders
INNER JOIN Customers ON Orders.CustomerID = Customers.CustomerID;
```

- [ ] **A)** Azure SQL Database
- [ ] **B)** Azure Cosmos DB
- [ ] **C)** Azure Blob Storage
- [ ] **D)** Azure Data Lake Storage Gen2

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure SQL Database is designed for structured relational data with SQL joins, foreign keys, and ACID transactional guarantees.
 
 
</details>


---

### **Design identity, governance, and monitoring solutions**

### 12. Which Microsoft Entra ID capability applies context-aware access rules based on user, device, location, and risk signals?

- [ ] **A)** Conditional Access
- [ ] **B)** Azure Policy
- [ ] **C)** Privileged Identity Management
- [ ] **D)** Management Groups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Conditional Access is the Entra ID engine that evaluates contextual signals before granting access. Azure Policy and management groups address governance, and PIM governs privileged roles.
 
 
</details>

### 13. Which two capabilities are core components of Microsoft Entra ID Privileged Identity Management (PIM)? Select two.

- [ ] **A)** Just-in-time privileged role activation
- [ ] **B)** Time-bound role assignments with approval workflows
- [ ] **C)** Continuous enforcement of resource tags
- [ ] **D)** Blocking legacy authentication protocols by default

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> PIM provides just-in-time, time-bound access to privileged roles. Tag enforcement is Azure Policy, and conditional access controls legacy authentication.
 
 
</details>

### 14. The policy rule in the code block defines a condition and an effect. Which effect blocks resource creation outside approved regions?

```json
{
  "if": {
    "field": "location",
    "notIn": ["eastus", "westus"]
  },
  "then": { "effect": "Deny" }
}
```

- [ ] **A)** Deny
- [ ] **B)** Audit
- [ ] **C)** DeployIfNotExists
- [ ] **D)** Append

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Deny prevents the resource creation request when the policy condition is met. Audit only logs compliance, while DeployIfNotExists and Append modify existing or new resources.
 
 
</details>

### 15. Which Microsoft Entra ID synchronization method validates users by sending the on-premises password hash to Microsoft Entra ID for authentication?

- [ ] **A)** Password Hash Synchronization
- [ ] **B)** Pass-Through Authentication
- [ ] **C)** Active Directory Federation Services
- [ ] **D)** Azure Policy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Password Hash Synchronization replicates password hashes to Microsoft Entra ID and validates sign-in in the cloud. Pass-through and federation validate on-premises.
 
 
</details>

### 16. Which two actions are correctly implemented with Azure Policy rather than Azure RBAC? Select two.

- [ ] **A)** Enforcing mandatory tags on resources
- [ ] **B)** Restricting resource creation to approved Azure regions
- [ ] **C)** Granting a user Contributor access to a resource group
- [ ] **D)** Reviewing user access to applications with access reviews

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure Policy governs resource configuration, such as tags and allowed regions. RBAC grants identity permissions, and access reviews belong to identity governance.
 
 
</details>

### 17. The command in the code block creates which Azure governance structure?

```bash
az account management-group create --name Contoso --display-name Contoso
```

- [ ] **A)** Management Group
- [ ] **B)** Azure Policy Initiative
- [ ] **C)** Log Analytics Workspace
- [ ] **D)** Resource Group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Azure CLI command creates a management group, which can organize subscriptions and inherit policy and RBAC assignments.
 
 
</details>

### 18. Which Azure service acts as the central data plane for collecting and analyzing telemetry from Azure and hybrid resources?

- [ ] **A)** Azure Monitor
- [ ] **B)** Azure Application Insights
- [ ] **C)** Log Analytics
- [ ] **D)** Microsoft Sentinel

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Monitor is the unified monitoring pipeline. Application Insights provides APM, Log Analytics stores logs, and Sentinel is a SIEM.
 
 
</details>

### 19. Which two components are required in an Azure Monitor alerting strategy? Select two.

- [ ] **A)** An alert rule that defines a condition
- [ ] **B)** An action group that receives notifications
- [ ] **C)** A management group hierarchy
- [ ] **D)** A connection string from Application Insights

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> An alert rule defines the signal and condition, and an action group defines the notification or automated response. The other options do not directly form the alert strategy.
 
 
</details>

### 20. In which Azure Monitor component should you run the query shown in the code block?

```kql
AzureDiagnostics
| where TimeGenerated > ago(1d)
| summarize Count = count() by Resource
```

- [ ] **A)** Log Analytics workspace
- [ ] **B)** Azure Policy
- [ ] **C)** Privileged Identity Management
- [ ] **D)** Management Group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Log Analytics workspaces store and query Azure log data using KQL. The other choices are governance or identity tools.
 
 
</details>


---

### **Design infrastructure solutions**

### 21. Which Azure compute service provides the highest level of control over the operating system and underlying hardware configuration?

- [ ] **A)** Virtual Machines
- [ ] **B)** Azure App Service
- [ ] **C)** Azure Container Instances
- [ ] **D)** Azure Kubernetes Service

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Virtual Machines are an IaaS service that gives architects full control over the operating system and underlying hardware, making them ideal for custom configurations and legacy migrations.
 
 
</details>

### 22. Which two statements accurately describe Azure App Service?

- [ ] **A)** Fully managed PaaS for web apps and APIs
- [ ] **B)** Built-in scaling tiers and integrated SSL
- [ ] **C)** Absolute control over the OS kernel
- [ ] **D)** Best for isolated batch tasks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure App Service is a fully managed PaaS with built-in scaling and SSL. OS kernel control belongs to VMs, and isolated batch tasks are a fit for Container Instances.
 
 
</details>

### 23. An architect runs the command in the code block to deploy a container. Which Azure compute service is being used?

```bash
az container create --resource-group RG1 --name web-app-1 --image nginx --ports 80
```

- [ ] **A)** Azure Container Instances
- [ ] **B)** Azure Kubernetes Service
- [ ] **C)** Azure App Service
- [ ] **D)** Virtual Machines

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses az container create, which is the Azure CLI command for Azure Container Instances, the fastest managed option for running containers.
 
 
</details>

### 24. Which Azure compute capability provides centralized management and auto-scaling of identical virtual machines for fault-tolerant architectures?

- [ ] **A)** Virtual Machine Scale Sets
- [ ] **B)** Azure App Service
- [ ] **C)** Azure Container Instances
- [ ] **D)** Azure Kubernetes Service

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Virtual Machine Scale Sets manage identical VMs, support custom scaling based on metrics, and provide automatic healing across Availability Zones.
 
 
</details>

### 25. Which two statements correctly describe Azure Load Balancer?

- [ ] **A)** Layer 4 TCP and UDP balancing
- [ ] **B)** SSL termination and URL routing
- [ ] **C)** Internal and public-facing endpoints
- [ ] **D)** FQDN-based outbound filtering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Azure Load Balancer operates at Layer 4 and supports internal or public endpoints. SSL termination and URL routing belong to Application Gateway, and FQDN filtering belongs to Azure Firewall.
 
 
</details>

### 26. The code block contains an inbound rule that denies traffic to a database port from a specific subnet. Which Azure component is defined by this configuration?

```json
{
  "name": "DenySQLFromWebSubnet",
  "properties": {
    "priority": 100,
    "direction": "Inbound",
    "access": "Deny",
    "protocol": "Tcp",
    "destinationPortRange": "1433",
    "sourceAddressPrefix": "10.0.1.0/24"
  }
}
```

- [ ] **A)** Network Security Group
- [ ] **B)** Azure Firewall
- [ ] **C)** Application Gateway
- [ ] **D)** Azure DNS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The rule filters by source IP, protocol, port, and direction at the network layer, which is characteristic of a Network Security Group.
 
 
</details>

### 27. Which Azure service provides centralized stateful inspection from Layer 4 through Layer 7 with FQDN filtering and threat intelligence?

- [ ] **A)** Azure Firewall
- [ ] **B)** Network Security Group
- [ ] **C)** Azure Load Balancer
- [ ] **D)** Application Gateway

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Firewall is a managed cloud security service that provides centralized Layer 4 through Layer 7 inspection, FQDN filtering, and threat intelligence.
 
 
</details>

### 28. Which two capabilities are provided by Azure Application Gateway?

- [ ] **A)** Layer 7 HTTP and HTTPS management
- [ ] **B)** Cookie affinity and URL path routing
- [ ] **C)** TCP and UDP packet forwarding
- [ ] **D)** FQDN filtering and threat intelligence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Application Gateway is a dedicated Layer 7 web traffic load balancer with cookie affinity, URL path routing, and WAF; TCP/UDP forwarding belongs to Load Balancer.
 
 
</details>

### 29. The command in the code block creates a hub-side VNet peering. Which parameter must be added to the spoke-side peering so the spoke can use the hub gateway?

```bash
az network vnet peering create --name HubToSpoke --resource-group HubRG --vnet-name HubVNet --remote-vnet SpokeVNet --allow-vnet-access
```

- [ ] **A)** --use-remote-gateways
- [ ] **B)** --allow-forwarded-traffic
- [ ] **C)** --allow-gateway-transit
- [ ] **D)** --no-wait

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> For a spoke VNet to reach on-premises through a hub gateway, the spoke-side peering must enable the use of remote gateways.
 
 
</details>

### 30. Which statement best describes Azure DNS Private Zones?

- [ ] **A)** DNS within VNets without custom servers
- [ ] **B)** Forces traffic through a security appliance
- [ ] **C)** Balances TCP and UDP traffic
- [ ] **D)** Filters traffic by fully qualified domains

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure DNS Private Zones provide reliable DNS resolution inside virtual networks and across peered networks without the need for custom DNS server deployments.
 
 
</details>

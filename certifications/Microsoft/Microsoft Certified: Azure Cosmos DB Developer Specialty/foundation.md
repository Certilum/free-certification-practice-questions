<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Microsoft%20Certified%20-%20Azure%20Cosmos%20DB%20Developer%20Specialty.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Microsoft Certified: Azure Cosmos DB Developer Specialty</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Design and implement data distribution](#design-and-implement-data-distribution) (2 questions)
- [Design and implement data models](#design-and-implement-data-models) (11 questions)
- [Integrate an Azure Cosmos DB solution](#integrate-an-azure-cosmos-db-solution) (3 questions)
- [Maintain an Azure Cosmos DB solution](#maintain-an-azure-cosmos-db-solution) (8 questions)
- [Optimize an Azure Cosmos DB solution](#optimize-an-azure-cosmos-db-solution) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-11T02:42:22.288Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Design and implement data distribution | 2 |
| Design and implement data models | 11 |
| Integrate an Azure Cosmos DB solution | 3 |
| Maintain an Azure Cosmos DB solution | 8 |
| Optimize an Azure Cosmos DB solution | 6 |

---

### **Design and implement data distribution**

### 1. Which consistency level is not supported when an Azure Cosmos DB account has multiple write regions enabled?

- [ ] **A)** Strong
- [ ] **B)** Session
- [ ] **C)** Eventual
- [ ] **D)** Consistent Prefix

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Strong consistency is not supported with multiple write regions because it requires synchronous global ordering. Only Session, Consistent Prefix, and Eventual are supported in this scenario.
 
 
</details>

### 2. Which statements about the failover priority list for an Azure Cosmos DB single-write multi-region account are correct? Select all that apply.

- [ ] **A)** One region must be assigned priority 0 as the current write region.
- [ ] **B)** Every region must have a unique integer failover priority.
- [ ] **C)** The list is used to route read requests to the nearest region.
- [ ] **D)** Automatic failover is enabled by default when a region is added.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The priority list designates the write region and failover order; priorities must be unique. It does not control read routing, and automatic failover is not enabled by default.
 
 
</details>


---

### **Design and implement data models**

### 3. Which option states the maximum size of a single document in Azure Cosmos DB?

- [ ] **A)** 1 MB
- [ ] **B)** 2 MB
- [ ] **C)** 4 MB
- [ ] **D)** 10 GB

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The maximum item size in Azure Cosmos DB is 2 MB. Documents that exceed this limit must be redesigned using splitting or referencing.
 
 
</details>

### 4. Which two statements about denormalization in Azure Cosmos DB are true?

- [ ] **A)** Data duplication is acceptable and often needed for efficient reads.
- [ ] **B)** The change feed can synchronize duplicated data.
- [ ] **C)** Normalization is the primary design goal.
- [ ] **D)** Use server-side JOINs across containers to avoid duplication.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Denormalization reduces round trips and RU cost. Cosmos DB intentionally duplicates data, and the change feed can keep copies synchronized.
 
 
</details>

### 5. Review the stored procedure in the code block. What is required for it to update multiple documents in one transaction?

```javascript
function updateMultipleDocuments() {
    var context = getContext();
    var collection = context.getCollection();
    // process documents
}
```

- [ ] **A)** All documents must share the same partition key value.
- [ ] **B)** All documents must be in different containers.
- [ ] **C)** All documents must have the same id.
- [ ] **D)** All documents must be indexed manually.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Stored procedures in Azure Cosmos DB execute within a single logical partition. Therefore, every document updated atomically must have the same partition key value.
 
 
</details>

### 6. What is the primary purpose of a partition key in Azure Cosmos DB?

- [ ] **A)** To route items to physical partitions
- [ ] **B)** To set the consistency level
- [ ] **C)** To define the indexing mode
- [ ] **D)** To enforce unique ids globally

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The partition key determines the logical partition and is hashed to route items to the correct physical partition for storage and queries.
 
 
</details>

### 7. Which two characteristics should a good partition key have?

- [ ] **A)** High cardinality
- [ ] **B)** Even distribution of data and throughput
- [ ] **C)** Low number of distinct values
- [ ] **D)** Frequent value changes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A good partition key has many unique values and spreads both storage and request traffic evenly across physical partitions.
 
 
</details>

### 8. Which two statements about the indexing policy shown in the code block are correct?

```json
{
  "indexingMode": "consistent",
  "automatic": true,
  "includedPaths": [
    {"path": "/name/?"}
  ],
  "excludedPaths": [
    {"path": "/description/*"}
  ]
}
```

- [ ] **A)** The /name property is indexed.
- [ ] **B)** The /description property can still be queried, but may require a scan.
- [ ] **C)** The /description property cannot be queried.
- [ ] **D)** The indexing mode is set to None.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Included paths index the /name property. Excluded paths remove /description from the index, but queries can still run through full scans, although less efficiently.
 
 
</details>

### 9. Which consistency level is the default for most Azure Cosmos DB SDK operations?

- [ ] **A)** Strong
- [ ] **B)** Bounded staleness
- [ ] **C)** Session
- [ ] **D)** Eventual

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Session consistency is the default for most SDK calls and provides read-your-writes within a client session.
 
 
</details>

### 10. Which two consistency levels are not supported when the account has multiple write regions?

- [ ] **A)** Strong
- [ ] **B)** Bounded staleness
- [ ] **C)** Session
- [ ] **D)** Eventual

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Strong and Bounded staleness require a single write region. Multi-region write accounts support Session, Consistent prefix, and Eventual.
 
 
</details>

### 11. Which query can be efficiently served by the composite index in the code block?

```json
[
  {"path": "/tenantId", "order": "ascending"},
  {"path": "/timestamp", "order": "descending"}
]
```

- [ ] **A)** WHERE tenantId = @tenant ORDER BY timestamp DESC
- [ ] **B)** WHERE tenantId = @tenant ORDER BY timestamp ASC
- [ ] **C)** SELECT * FROM c ORDER BY tenantId, timestamp
- [ ] **D)** SELECT * FROM c WHERE timestamp > @time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Composite indexes must match the equality property order and sort direction. This index has tenantId ascending and timestamp descending, so that query pattern matches.
 
 
</details>

### 12. What is the maximum storage size for a single logical partition?

- [ ] **A)** 10 GB
- [ ] **B)** 20 GB
- [ ] **C)** 30 GB
- [ ] **D)** 2 MB

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Each logical partition can store up to 20 GB. Exceeding this limit makes the container unable to accept writes to that partition.
 
 
</details>

### 13. Which two statements about hot partitions are correct?

- [ ] **A)** A hot partition can cause throttling even when total throughput is not exhausted.
- [ ] **B)** Normalized RU Consumption at 100% can indicate a hot partition.
- [ ] **C)** TotalRequests is the most reliable metric for detecting hot partitions.
- [ ] **D)** Hot partitions affect storage only, not throughput.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Hot partitions are identified by per-partition metrics such as Normalized RU Consumption. TotalRequests alone can hide partition-level imbalance and throttling.
 
 
</details>


---

### **Integrate an Azure Cosmos DB solution**

### 14. What is the primary purpose of the lease container in an Azure Functions Cosmos DB trigger?

- [ ] **A)** Stores checkpoints and processing state
- [ ] **B)** Stores the original source documents
- [ ] **C)** Caches query results for repeat reads
- [ ] **D)** Temporarily stores output binding data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The lease container keeps checkpoints and work distribution metadata so the Change Feed Processor can resume and coordinate processing across instances.
 
 
</details>

### 15. Which two statements accurately describe the behavior of Change Feed modes in Azure Cosmos DB containers?

- [ ] **A)** Latest mode does not include delete operations
- [ ] **B)** All versions and deletes must be enabled at container creation
- [ ] **C)** Latest mode includes all intermediate changes for each item
- [ ] **D)** All versions and deletes mode is the default for existing containers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Latest mode exposes only the most recent update per item and omits deletes. Full fidelity mode must be enabled at container creation and includes delete operations.
 
 
</details>

### 16. Review the container settings in the code block. What is the result of the analyticalStoreTtl value specified?

```json
{
  "id": "orders",
  "partitionKey": "/customerId",
  "analyticalStoreTtl": -1,
  "defaultTtl": 2592000
}
```

- [ ] **A)** It enables unlimited retention for the analytical store
- [ ] **B)** It disables the analytical store for this container
- [ ] **C)** It retains analytical data for one year
- [ ] **D)** It sets the transactional store TTL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A value of -1 for analyticalStoreTtl enables the analytical store and retains all historical analytical versions indefinitely.
 
 
</details>


---

### **Maintain an Azure Cosmos DB solution**

### 17. Which statement best describes encryption at rest for an Azure Cosmos DB account?

- [ ] **A)** All data is encrypted automatically with AES-256 and cannot be disabled.
- [ ] **B)** Encryption at rest must be enabled per container.
- [ ] **C)** Encryption at rest applies only to SQL API data.
- [ ] **D)** Encryption at rest can be turned off to improve performance.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cosmos DB encrypts all data at rest by default using AES-256. The encryption is mandatory, applies to every API, and requires no configuration.
 
 
</details>

### 18. Which statements about data plane RBAC for Azure Cosmos DB are true?

- [ ] **A)** RBAC uses Microsoft Entra ID tokens.
- [ ] **B)** A role assignment can be scoped to a single container.
- [ ] **C)** RBAC replaces the need to configure consistency levels.
- [ ] **D)** RBAC supports all Cassandra API operations.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Data plane RBAC uses Microsoft Entra ID tokens and supports container-level scopes. It does not alter consistency levels and is not fully supported for all APIs.
 
 
</details>

### 19. In the Azure CLI restore command shown, which parameter must be added to restore the account to a specific point in time?

```bash
az cosmosdb restore --resource-group target-rg --name restored-account --source-database-account-name source-account
```

- [ ] **A)** --restore-timestamp
- [ ] **B)** --backup-interval
- [ ] **C)** --retention-period
- [ ] **D)** --throughput

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The --restore-timestamp parameter specifies the UTC time for point-in-time restore. Other parameters configure backup or throughput, not restore time.
 
 
</details>

### 20. What is the default backup mode for a new Azure Cosmos DB account?

- [ ] **A)** Periodic backup
- [ ] **B)** Continuous backup
- [ ] **C)** Customer-managed key backup
- [ ] **D)** No backup

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cosmos DB defaults to periodic backup, with configurable interval and retention. Continuous backup must be explicitly enabled.
 
 
</details>

### 21. Which of the following are diagnostic log categories for Azure Cosmos DB?

- [ ] **A)** DataPlaneRequests
- [ ] **B)** MongoRequests
- [ ] **C)** ControlPlaneRequests
- [ ] **D)** AzureActivity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> DataPlaneRequests, MongoRequests, and ControlPlaneRequests are Cosmos DB diagnostic categories. AzureActivity is the subscription-level activity log, not a Cosmos DB diagnostic category.
 
 
</details>

### 22. Which value should be supplied for the --scope parameter in this RBAC role assignment command to limit access to a single container?

```bash
az cosmosdb sql role assignment create --account-name demo --resource-group rg --role-definition-id <id> --principal-id <object-id> --scope <scope>
```

- [ ] **A)** Full container resource ID
- [ ] **B)** Database resource ID
- [ ] **C)** Cosmos DB account resource ID
- [ ] **D)** Subscription resource ID

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The scope for a role assignment determines the accessible resource. A container resource ID restricts the principal to that specific container.
 
 
</details>

### 23. Which network feature gives a Cosmos DB account a private IP address inside a virtual network?

- [ ] **A)** Private endpoint
- [ ] **B)** IP firewall
- [ ] **C)** Service tag
- [ ] **D)** TLS 1.2

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A private endpoint assigns a private IP from a VNet subnet and uses Private Link. IP firewalls and service tags do not provide a private IP.
 
 
</details>

### 24. Which requirements must be met before configuring customer-managed keys for Azure Cosmos DB?

- [ ] **A)** Key Vault soft delete and purge protection enabled
- [ ] **B)** System-assigned managed identity with crypto permissions
- [ ] **C)** Public network access enabled
- [ ] **D)** Continuous backup enabled

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CMK requires purge protection and a managed identity with wrap and unwrap permissions. It does not require public access or continuous backup.
 
 
</details>


---

### **Optimize an Azure Cosmos DB solution**

### 25. Which Azure Monitor metric shows the percentage of provisioned throughput consumed by a Cosmos DB container?

- [ ] **A)** NormalizedRUConsumption
- [ ] **B)** TotalRequestUnits
- [ ] **C)** ServerSideLatency
- [ ] **D)** ReplicationLatency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NormalizedRUConsumption divides consumed RU by provisioned capacity and supports filters by physical partition, making it the correct metric for throughput saturation.
 
 
</details>

### 26. Which two Azure Monitor platform metrics are available for an Azure Cosmos DB account?

- [ ] **A)** TotalRequests
- [ ] **B)** TotalRequestUnits
- [ ] **C)** CDBPartitionKeyRUConsumption
- [ ] **D)** QueryRuntimeStatistics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> TotalRequests and TotalRequestUnits are account-level platform metrics published to Azure Monitor. PartitionKeyRUConsumption is a diagnostic log, and QueryRuntimeStatistics is a log table, not a metric.
 
 
</details>

### 27. Review the following KQL query run against the CDBDataPlaneRequests table. What does the query identify?

```kql
CDBDataPlaneRequests
| where TimeGenerated > ago(1h)
| where StatusCode == 429
| summarize Count = count() by PartitionKeyRangeId
| top 1 by Count
```

- [ ] **A)** Most throttled partition range
- [ ] **B)** Total Request Units consumed
- [ ] **C)** Fastest queries by latency
- [ ] **D)** Replication lag between regions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query filters for status code 429 and groups by PartitionKeyRangeId, so it surfaces the physical partition range responsible for the most throttled requests.
 
 
</details>

### 28. Which metric measures the maximum replication delay between a source region and a target region?

- [ ] **A)** ReplicationLatency
- [ ] **B)** ServerSideLatency
- [ ] **C)** NormalizedRUConsumption
- [ ] **D)** TotalRequests

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ReplicationLatency, also known as MaxReplicationLag, measures the maximum lag between a source and target region for multi-region accounts.
 
 
</details>

### 29. Which two resource-specific diagnostic log tables should be enabled to analyze expensive queries and partition-level RU consumption?

- [ ] **A)** CDBDataPlaneRequests
- [ ] **B)** CDBQueryRuntimeStatistics
- [ ] **C)** CDBControlPlaneRequests
- [ ] **D)** CDBMetering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CDBDataPlaneRequests captures per-request RU charges, status codes, and partition range IDs; CDBQueryRuntimeStatistics exposes query text, index hit ratio, and retrieved document counts.
 
 
</details>

### 30. Review the following indexing policy. What is the effect of this configuration?

```json
{
  "indexingMode": "consistent",
  "automatic": true,
  "includedPaths": [
    { "path": "/*" }
  ],
  "excludedPaths": [
    { "path": "/clientLogs/*" }
  ]
}
```

- [ ] **A)** Excludes unqueried paths from the index
- [ ] **B)** Disables indexing for the container
- [ ] **C)** Adds a composite index
- [ ] **D)** Indexes only string properties

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The excludedPath removes /clientLogs/* from the index while the rest of the policy remains consistent, lowering write RU and storage for unqueried data.
 
 
</details>

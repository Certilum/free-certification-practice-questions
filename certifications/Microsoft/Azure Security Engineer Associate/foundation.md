<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Azure%20Security%20Engineer%20Associate.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Azure Security Engineer Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Secure Azure using Microsoft Defender for Cloud and Microsoft Sentinel](#secure-azure-using-microsoft-defender-for-cloud-and-microsoft-sentinel) (10 questions)
- [Secure Identity and Access](#secure-identity-and-access) (6 questions)
- [Secure compute, storage, and databases](#secure-compute-storage-and-databases) (7 questions)
- [Secure networking](#secure-networking) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:52:45.569Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Secure Azure using Microsoft Defender for Cloud and Microsoft Sentinel | 10 |
| Secure Identity and Access | 6 |
| Secure compute, storage, and databases | 7 |
| Secure networking | 7 |

---

### **Secure Azure using Microsoft Defender for Cloud and Microsoft Sentinel**

### 1. What is the primary purpose of Microsoft Defender for Cloud?

- [ ] **A)** Cloud security posture management and workload protection
- [ ] **B)** Security information and event management
- [ ] **C)** Domain name system filtering
- [ ] **D)** Virtual private network gateway

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Microsoft Defender for Cloud is a cloud-native security posture management and workload protection platform that helps secure cloud resources.
 
 
</details>

### 2. Which resources can be protected by Microsoft Defender for Cloud enhanced security plans? (Select all that apply.)

- [ ] **A)** Virtual machines
- [ ] **B)** Azure SQL databases
- [ ] **C)** Azure Kubernetes Service clusters
- [ ] **D)** Microsoft 365 mailboxes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Enhanced security plans in Microsoft Defender for Cloud protect compute, data, and services such as VMs, SQL databases, and Kubernetes clusters; mailboxes are covered by Microsoft 365 Defender.
 
 
</details>

### 3. The code block contains a KQL query. Which statement correctly describes the query output?

```kql
SecurityEvent
| where TimeGenerated > ago(24h)
| summarize count() by Account
| top 10 by count_
```

- [ ] **A)** Top 10 accounts with the most security events in the last 24 hours
- [ ] **B)** Security events with a severity higher than 10
- [ ] **C)** All security events from the last 10 days
- [ ] **D)** A list of computers unavailable in the last 24 hours

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query filters the last 24 hours of SecurityEvent data, counts events per account, and returns the top 10 accounts by count.
 
 
</details>

### 4. What kind of solution is Microsoft Sentinel?

- [ ] **A)** Cloud-native SIEM and SOAR solution
- [ ] **B)** Cloud access security broker
- [ ] **C)** Web application firewall
- [ ] **D)** Container orchestration platform

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Microsoft Sentinel is a cloud-native SIEM and SOAR solution that provides intelligent security analytics and automated response across the enterprise.
 
 
</details>

### 5. Which of the following are built-in data connectors in Microsoft Sentinel? (Select all that apply.)

- [ ] **A)** Azure Active Directory
- [ ] **B)** Office 365
- [ ] **C)** Azure Activity
- [ ] **D)** SQL Server Management Studio

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Microsoft Sentinel provides built-in connectors for Azure AD, Office 365, Azure Activity, and many others; SQL Server Management Studio is not a data source connector.
 
 
</details>

### 6. The KQL query in the code block is run in Microsoft Sentinel. What does it produce?

```kql
SecurityAlert
| where TimeGenerated >= ago(7d)
| summarize count() by Severity
| render piechart
```

- [ ] **A)** A pie chart showing the count of alerts by severity
- [ ] **B)** A bar chart of alerts over time
- [ ] **C)** A table of all security alerts
- [ ] **D)** A line chart of alerts by workspace

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query counts SecurityAlert records by Severity and renders a pie chart, giving a visual distribution of alert severity.
 
 
</details>

### 7. What does the secure score in Microsoft Defender for Cloud indicate?

- [ ] **A)** Security posture based on completed recommendations
- [ ] **B)** Number of workloads currently running
- [ ] **C)** Volume of security logs ingested
- [ ] **D)** Number of active alerts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Secure score aggregates the status of security recommendations, measuring how well an organization has improved its security posture.
 
 
</details>

### 8. Which of the following are SOAR capabilities provided by Microsoft Sentinel? (Select all that apply.)

- [ ] **A)** Playbooks
- [ ] **B)** Automation rules
- [ ] **C)** Incident management
- [ ] **D)** Network packet capture

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Microsoft Sentinel SOAR uses playbooks, automation rules, and incident management to orchestrate and automate investigations; packet capture is not a Sentinel feature.
 
 
</details>

### 9. The KQL query in the code block is intended to identify which information?

```kql
Heartbeat
| summarize count() by Computer
| where count_ > 10
```

- [ ] **A)** Computers with more than 10 heartbeat records
- [ ] **B)** Computers with fewer than 10 heartbeat records
- [ ] **C)** The 10 most recent heartbeat records
- [ ] **D)** Heartbeats that occurred in the last 10 minutes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query groups heartbeat records by computer and keeps only computers whose count is greater than 10.
 
 
</details>

### 10. Which Azure service is used as the data store for Microsoft Sentinel?

- [ ] **A)** Log Analytics workspace
- [ ] **B)** Azure Data Lake Storage
- [ ] **C)** Azure SQL Database
- [ ] **D)** Blob storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Microsoft Sentinel is built on top of Log Analytics workspaces, where logs and alerts are stored and queried.
 
 
</details>


---

### **Secure Identity and Access**

### 11. What is Microsoft Entra ID (formerly Azure Active Directory) used for in Azure?

- [ ] **A)** Cloud identity and access management
- [ ] **B)** Domain name system (DNS) hosting
- [ ] **C)** Virtual machine snapshot backup
- [ ] **D)** Network packet filtering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Microsoft Entra ID is Microsoft's cloud-based identity and access management service. It supports authentication, single sign-on, and application access control.
 
 
</details>

### 12. Which of the following are capabilities of Microsoft Entra ID? (Select all that apply.)

- [ ] **A)** Conditional Access
- [ ] **B)** Identity Protection
- [ ] **C)** Privileged Identity Management
- [ ] **D)** Azure Traffic Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Conditional Access, Identity Protection, and Privileged Identity Management are all Microsoft Entra ID capabilities. Azure Traffic Manager is a networking service.
 
 
</details>

### 13. The command in the code block is executed by an administrator. What is the result?

```bash
az ad user create --display-name "Aisha Patel" --user-principal-name "aisha@contoso.com" --password "P@ssw0rd123!"
```

- [ ] **A)** Creates a new user in Microsoft Entra ID
- [ ] **B)** Creates an Azure resource group
- [ ] **C)** Assigns a Contributor role
- [ ] **D)** Deletes an application registration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> the command az ad user create provisions a new user object in Microsoft Entra ID. It does not manage Azure infrastructure roles or resource groups.
 
 
</details>

### 14. What is a service principal in Microsoft Entra ID?

- [ ] **A)** An identity created for an application
- [ ] **B)** A virtual machine image
- [ ] **C)** A global Azure region
- [ ] **D)** A storage account key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A service principal is the identity that an application uses to access Azure resources. It can be used for authentication and authorization.
 
 
</details>

### 15. Which of the following are Azure AD/Entra ID multi-factor authentication verification methods? (Select all that apply.)

- [ ] **A)** Mobile app notification
- [ ] **B)** Phone call
- [ ] **C)** OATH hardware token
- [ ] **D)** Email confirmation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Microsoft Entra ID MFA supports mobile app notifications, phone calls, SMS, and OATH tokens. Email is not an MFA verification method for interactive sign-in.
 
 
</details>

### 16. An administrator defines the Conditional Access policy in the code block. What does this policy require?

```json
{
  "conditions": {
    "applications": {
      "includeApplications": ["All"]
    }
  },
  "grantControls": {
    "operator": "OR",
    "builtInControls": ["Mfa"]
  }
}
```

- [ ] **A)** Multi-factor authentication for all included cloud apps
- [ ] **B)** Blocking all application sign-ins
- [ ] **C)** A mandatory password change
- [ ] **D)** Requiring a hybrid Azure AD join

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy includes all applications and configures MFA as a grant control. It does not block access, require a password change, or enforce device join.
 
 
</details>


---

### **Secure compute, storage, and databases**

### 17. Which Microsoft Azure service provides centralized security management and advanced threat protection across cloud workloads?

- [ ] **A)** Microsoft Defender for Cloud
- [ ] **B)** Azure Sentinel
- [ ] **C)** Azure Monitor
- [ ] **D)** Azure Policy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Microsoft Defender for Cloud provides centralized security posture management and advanced threat protection for cloud workloads, making it the correct answer.
 
 
</details>

### 18. Which two of the following are recommended security practices for securing an Azure Storage account?

- [ ] **A)** Require secure transfer for the storage account
- [ ] **B)** Disable public blob access
- [ ] **C)** Allow all IP addresses through the storage firewall
- [ ] **D)** Store account keys in application source code

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Requiring secure transfer enforces HTTPS, and disabling public blob access prevents anonymous access. Allowing all IPs and embedding keys increases exposure.
 
 
</details>

### 19. The following Azure CLI command creates a storage account. Which security configuration is being applied by this command?

```bash
az storage account create --name secstore01 --resource-group rg-sec --location eastus --sku Standard_LRS --allow-blob-public-access false --min-tls-version TLS1_2
```

- [ ] **A)** Disables public blob access and requires TLS 1.2
- [ ] **B)** Enables Azure AD authentication and disables TLS
- [ ] **C)** Configures a private endpoint only
- [ ] **D)** Stores storage account keys in Azure Key Vault

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses --allow-blob-public-access false to block anonymous access and --min-tls-version TLS1_2 to require secure TLS connections.
 
 
</details>

### 20. Which Azure SQL Database feature encrypts a database and its backups without requiring changes to the application?

- [ ] **A)** Transparent Data Encryption
- [ ] **B)** Always Encrypted
- [ ] **C)** Dynamic Data Masking
- [ ] **D)** Auditing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Transparent Data Encryption encrypts SQL Server, Azure SQL Database, and backup files at rest while requiring no change to application code.
 
 
</details>

### 21. Which two statements about Azure managed identities are true?

- [ ] **A)** They provide an automatically managed identity in Azure AD
- [ ] **B)** They allow applications to authenticate without storing credentials
- [ ] **C)** They require a client secret to be stored in source code
- [ ] **D)** They can only be assigned to on-premises virtual machines

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Managed identities are backed by Azure AD service principals and remove the need to manage credentials. They are used by Azure resources, not on-premises VMs.
 
 
</details>

### 22. Consider the following Azure CLI command. What is the primary purpose of this command?

```bash
az sql db create --resource-group rg-sec --server sqlsrvsec --name contosodb --service-objective S0 --no-wait
```

- [ ] **A)** Provisions a new Azure SQL database in an existing server
- [ ] **B)** Creates a new Azure SQL logical server
- [ ] **C)** Deletes an existing Azure SQL database
- [ ] **D)** Scales a database to a higher service tier

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command includes az sql db create and a server name, indicating it creates a new database in an existing logical SQL server.
 
 
</details>

### 23. Which Azure Storage feature prevents Blob data from being modified or deleted for a specified time interval?

- [ ] **A)** Immutability policies
- [ ] **B)** Soft delete
- [ ] **C)** Shared access signatures
- [ ] **D)** Storage account failover

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Immutability policies enforce WORM storage, preventing blobs from being modified or deleted for the configured retention period.
 
 
</details>


---

### **Secure networking**

### 24. Which Azure resource uses security rules to allow or deny inbound and outbound network traffic for subnets and network interfaces?

- [ ] **A)** Network Security Group
- [ ] **B)** Azure Firewall
- [ ] **C)** Azure DDoS Protection
- [ ] **D)** Azure Bastion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Network Security Group filters traffic with security rules assigned to subnets or network interfaces. Azure Firewall is a separate cloud-delivered network security service.
 
 
</details>

### 25. Which two abilities are provided by an Azure Network Security Group?

- [ ] **A)** Filter traffic based on source IP and port
- [ ] **B)** Apply allow and deny rules at subnet or NIC level
- [ ] **C)** Provide SQL injection attack protection
- [ ] **D)** Automatically encrypt all network packets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Network Security Groups enforce allow and deny rules based on IP, port, and protocol at the subnet or NIC level. SQL injection protection is a Web Application Firewall feature, not an NSG function.
 
 
</details>

### 26. Refer to the command in the code block. What does this command accomplish?

```bash
az network nsg rule create --resource-group RG --nsg-name MyNsg --name WebRule --priority 100 --access Allow --direction Inbound --protocol Tcp --source-address-prefixes * --source-port-ranges * --destination-address-prefixes 10.0.0.4 --destination-port-ranges 80
```

- [ ] **A)** Allows inbound TCP traffic to port 80 for a specific IP address
- [ ] **B)** Blocks outbound TCP traffic to all destinations
- [ ] **C)** Creates a virtual network with a new subnet
- [ ] **D)** Deletes an existing network security group rule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command creates an inbound security rule that allows TCP traffic on port 80 to the destination IP 10.0.0.4 from any source.
 
 
</details>

### 27. Which Azure service provides continuous monitoring and mitigation for volumetric network DDoS attacks?

- [ ] **A)** Azure DDoS Protection
- [ ] **B)** Azure Firewall
- [ ] **C)** Network Security Group
- [ ] **D)** Azure Front Door

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure DDoS Protection provides always-on traffic monitoring and mitigation for volumetric DDoS attacks. Azure Firewall and NSGs focus on traffic filtering rather than DDoS defense.
 
 
</details>

### 28. Which two statements accurately describe Azure DDoS Protection?

- [ ] **A)** Always-on traffic monitoring and mitigation
- [ ] **B)** Protects Azure resources from volumetric DDoS attacks
- [ ] **C)** Replaces private endpoint encryption
- [ ] **D)** Generates public SSL certificates

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure DDoS Protection continuously monitors traffic and mitigates volumetric attacks. It does not replace encryption or issue SSL certificates.
 
 
</details>

### 29. Refer to the command in the code block. What is the command doing?

```bash
az network vnet subnet update --resource-group RG --vnet-name VNet --name SubnetA --network-security-group MyNsg
```

- [ ] **A)** Attaches an NSG to the named subnet
- [ ] **B)** Creates a new virtual network
- [ ] **C)** Removes all rules from an NSG
- [ ] **D)** Assigns a public IP address to a VM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command updates the subnet named SubnetA in VNet by associating the network security group MyNsg with that subnet.
 
 
</details>

### 30. Which Azure service creates a managed jump host for securely connecting to virtual machines without public endpoints?

- [ ] **A)** Azure Bastion
- [ ] **B)** Azure DNS
- [ ] **C)** Traffic Manager
- [ ] **D)** Network Watcher

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Bastion is a fully managed service that provides secure and seamless RDP and SSH access to virtual machines directly from the Azure portal without public IPs.
 
 
</details>

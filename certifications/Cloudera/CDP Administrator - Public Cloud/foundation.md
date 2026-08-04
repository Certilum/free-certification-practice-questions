<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cloudera/CDP%20Administrator%20-%20Public%20Cloud" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>CDP Administrator - Public Cloud</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Automation and Operations](#automation-and-operations) (4 questions)
- [CDP Public Cloud Architecture](#cdp-public-cloud-architecture) (4 questions)
- [High Availability and Disaster Recovery](#high-availability-and-disaster-recovery) (5 questions)
- [Installation and Configuration](#installation-and-configuration) (6 questions)
- [Security and Governance](#security-and-governance) (6 questions)
- [Troubleshooting and Monitoring](#troubleshooting-and-monitoring) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:13.806Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Automation and Operations | 4 |
| CDP Public Cloud Architecture | 4 |
| High Availability and Disaster Recovery | 5 |
| Installation and Configuration | 6 |
| Security and Governance | 6 |
| Troubleshooting and Monitoring | 5 |

---

### **Automation and Operations**

### 1. Which paradigm does the Terraform provider for Cloudera use to manage CDP resources?

- [ ] **A)** Declarative
- [ ] **B)** Imperative
- [ ] **C)** Procedural
- [ ] **D)** Functional

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Terraform follows declarative configuration where you define the desired state, not the steps. Cloudera Manager API is imperative.
 
 
</details>

### 2. Which two authentication methods are supported for the Cloudera Manager REST API?

- [ ] **A)** OAuth2 with client credentials
- [ ] **B)** API keys generated from Management Console
- [ ] **C)** SSH key pairs
- [ ] **D)** SAML assertions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The CM API supports OAuth2 (client ID/secret) and API keys. SSH and SAML are not used.
 
 
</details>

### 3. Refer to the Terraform code block. Which resource type is used to create a CDP Data Lake?

```hcl
resource "cloudera_datalake" "example" {
  name = "my-datalake"
  environment = cloudera_environment.env.id
}
```

- [ ] **A)** cloudera_environment
- [ ] **B)** cloudera_datalake
- [ ] **C)** cloudera_datahub
- [ ] **D)** cloudera_cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The resource cloudera_datalake is used to manage Data Lakes in the Terraform provider.
 
 
</details>

### 4. Which type of upgrade updates nodes one at a time to maintain service availability?

- [ ] **A)** Rolling upgrade
- [ ] **B)** Express upgrade
- [ ] **C)** Full downtime upgrade
- [ ] **D)** Blue-green upgrade

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Rolling upgrades update nodes one at a time, keeping services available. Express stops all services.
 
 
</details>


---

### **CDP Public Cloud Architecture**

### 5. What is the name of the shared layer that provides consistent security, governance, and metadata management across all CDP services?

- [ ] **A)** Data Hub
- [ ] **B)** Data Engineering
- [ ] **C)** Shared Data Experience (SDX)
- [ ] **D)** Data Warehouse

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Shared Data Experience (SDX) layer provides consistent security, governance, and metadata across all CDP services.
 
 
</details>

### 6. Which two prerequisites must be met before creating a CDP environment in AWS?

- [ ] **A)** Two private subnets in different Availability Zones
- [ ] **B)** A dedicated internet gateway for each subnet
- [ ] **C)** A cross-account IAM role with trust from Cloudera control plane
- [ ] **D)** A single public subnet for all nodes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> CDP requires at least two private subnets across two AZs and a cross-account IAM role that the control plane can assume.
 
 
</details>

### 7. An administrator runs the command shown below and receives the output. What is the most likely cause of the environment status?

```json
{
  "environment": {
    "status": "DISCONNECTED",
    "statusMessage": "No telemetry received for over 30 minutes."
  }
}
```

- [ ] **A)** Control plane outage
- [ ] **B)** Data plane lost outbound internet access
- [ ] **C)** Incorrect IAM role configuration
- [ ] **D)** Missing private hosted zone

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The environment became DISCONNECTED because the data plane cannot reach the control plane, likely due to lost outbound internet access.
 
 
</details>

### 8. Which CDP service provides a fully managed Spark experience where users cannot access cluster nodes?

- [ ] **A)** Data Hub
- [ ] **B)** Data Engineering (CDE)
- [ ] **C)** Data Warehouse (CDW)
- [ ] **D)** Machine Learning (CML)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Data Engineering (CDE) provides a fully managed Spark environment where users submit jobs without cluster access.
 
 
</details>


---

### **High Availability and Disaster Recovery**

### 9. What is an Availability Zone in the context of cloud infrastructure?

- [ ] **A)** A physically separate location with independent power, networking, and cooling.
- [ ] **B)** A logical partition of a VPC with identical resources.
- [ ] **C)** A single data center with redundant power and cooling.
- [ ] **D)** A cloud region's primary data center with high availability.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An Availability Zone is a physically isolated data center with independent power, networking, and cooling, used to distribute workloads for fault tolerance.
 
 
</details>

### 10. Which of the following are required for a fault-tolerant CDP control plane deployment across AZs? (Select two.)

- [ ] **A)** Cloudera Manager and SDX services must be deployed across at least two AZs.
- [ ] **B)** Explicit AZ mappings must be configured for Data Hub clusters using templates.
- [ ] **C)** All services must be deployed in three AZs with equal node distribution.
- [ ] **D)** The control plane can be deployed in a single AZ if managed services are used.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The document states that control plane services must span at least two AZs and explicit AZ mappings for Data Hub clusters are required for enterprise deployments.
 
 
</details>

### 11. In the provided DistCp command, what does the `-bandwidth` parameter control?

```bash
distcp -update -skipcrccheck -bandwidth 100 /data/important/.snapshot/snapshot_20250304_1200 s3a://backup-bucket/hdfs-backups/20250304/
```

- [ ] **A)** It throttles the network bandwidth used during the copy to avoid saturating the network.
- [ ] **B)** It specifies the size of files to be copied.
- [ ] **C)** It sets the number of parallel threads for copying.
- [ ] **D)** It compresses the data during transfer.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The `-bandwidth` parameter limits the average bandwidth (in MB/s) used by DistCp to prevent network saturation.
 
 
</details>

### 12. Where are HBase snapshots initially stored before being exported to a backup location?

- [ ] **A)** In the HDFS directory of the HBase installation.
- [ ] **B)** In the cloud object store associated with the cluster.
- [ ] **C)** In the HBase Write-Ahead Logs directory.
- [ ] **D)** In a temporary location that is cleared after export.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> HBase snapshots are stored in HDFS under the HBase installation directory; they must be explicitly exported to a backup location for DR.
 
 
</details>

### 13. Which components of the Shared Data Experience (SDX) require separate replication across regions for DR? (Select two.)

- [ ] **A)** Ranger policies
- [ ] **B)** Apache Atlas metadata
- [ ] **C)** Hive table data stored in S3
- [ ] **D)** Kafka topic configurations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Ranger policies and Atlas metadata require manual export/import; cloud storage replication covers data but not these SDX components.
 
 
</details>


---

### **Installation and Configuration**

### 14. Which component is the core deployment engine for CDP Public Cloud environments?

- [ ] **A)** Cloudbreak
- [ ] **B)** Cloudera Manager
- [ ] **C)** Terraform
- [ ] **D)** Apache Atlas

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloudbreak is the core deployment engine that automates provisioning of CDP Public Cloud environments, including Data Lakes and Data Hubs.
 
 
</details>

### 15. Which tools are used for provisioning CDP Public Cloud environments? (Select two.)

- [ ] **A)** Cloudbreak
- [ ] **B)** Cloudera Manager
- [ ] **C)** Terraform
- [ ] **D)** Apache Ranger

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Cloudbreak is the native provisioning engine, while Terraform can be used via Cloudera-provided modules for infrastructure-as-code.
 
 
</details>

### 16. Review the CDP CLI command below. Which action does it perform?

```bash
cdp environments create-aws-environment --environment-name myenv --region us-east-1 --credential-arn arn:aws:iam::123456789012:role/my-role
```

- [ ] **A)** Creates a new CDP environment on AWS
- [ ] **B)** Creates a new Data Hub cluster
- [ ] **C)** Describes a Data Lake
- [ ] **D)** Updates Ranger policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command 'cdp environments create-aws-environment' is used to create a new CDP environment in AWS.
 
 
</details>

### 17. What is the primary role of HDFS in CDP Public Cloud?

- [ ] **A)** Persistent storage for data lake
- [ ] **B)** Intermediate scratch space for YARN and Spark
- [ ] **C)** Replication of data for durability
- [ ] **D)** Resource management and scheduling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In CDP Public Cloud, HDFS is primarily used for intermediate data such as YARN logs and Spark shuffle, while persistent data is stored in cloud object stores.
 
 
</details>

### 18. Which configurations are required to enable Hive ACID transactions? (Select two.)

- [ ] **A)** hive.support.concurrency=true
- [ ] **B)** hive.execution.engine=mr
- [ ] **C)** hive.txn.manager=org.apache.hadoop.hive.ql.lockmgr.DbTxnManager
- [ ] **D)** dfs.replication=3

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Hive ACID requires concurrency support and the DbTxnManager. MapReduce engine is not recommended and dfs.replication is irrelevant for cloud storage.
 
 
</details>

### 19. Examine the YARN configuration snippet. What auxiliary service is being enabled?

```xml
<property>
  <name>yarn.nodemanager.aux-services</name>
  <value>spark_shuffle</value>
</property>
```

- [ ] **A)** Spark shuffle service
- [ ] **B)** MapReduce shuffle service
- [ ] **C)** Hive LLAP service
- [ ] **D)** Kafka service

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The property 'yarn.nodemanager.aux-services' with value 'spark_shuffle' enables the Spark external shuffle service on YARN NodeManagers.
 
 
</details>


---

### **Security and Governance**

### 20. Which component in CDP Public Cloud is responsible for fine-grained authorization and auditing of data access?

- [ ] **A)** Apache Ranger
- [ ] **B)** Apache Knox
- [ ] **C)** Apache Atlas
- [ ] **D)** Kerberos

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Apache Ranger is the component that provides fine-grained authorization policies and audit logging across CDP services. Knox is an authentication gateway, Atlas handles metadata, and Kerberos handles service-to-service authentication.
 
 
</details>

### 21. Which two components are primarily responsible for user and service authentication in CDP Public Cloud? (Choose two.)

- [ ] **A)** Kerberos
- [ ] **B)** Apache Ranger
- [ ] **C)** Apache Knox
- [ ] **D)** Apache Atlas

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Kerberos authenticates services internally, while Knox authenticates external users via LDAP or SSO. Ranger authorizes; Atlas classifies metadata.
 
 
</details>

### 22. Review the Knox topology configuration snippet below. Which authentication provider is being used?

```xml
<topology>
  <gateway>
    <provider>
      <role>authentication</role>
      <name>LdapProvider</name>
      <enabled>true</enabled>
      <param>
        <name>ldapRealm</name>
        <value>com.my.realm</value>
      </param>
    </provider>
  </gateway>
</topology>
```

- [ ] **A)** LDAP authentication
- [ ] **B)** Kerberos authentication
- [ ] **C)** SAML authentication
- [ ] **D)** Shiro static authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The presence of <param name='ldapRealm'/> and <provider>LdapProvider</provider> indicates LDAP authentication is configured.
 
 
</details>

### 23. What is the purpose of Apache Knox in CDP Public Cloud?

- [ ] **A)** A reverse proxy gateway that provides a single entry point for REST API calls and handles authentication
- [ ] **B)** A fine-grained authorization engine for Hive and HBase
- [ ] **C)** A metadata repository for data lineage and classification
- [ ] **D)** A Kerberos Key Distribution Center (KDC) for the cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Knox is a reverse proxy that terminates external connections, authenticates users, and forwards requests to internal services. It does not perform fine-grained authorization or store metadata.
 
 
</details>

### 24. Which two statements about encryption in CDP Public Cloud are correct? (Choose two.)

- [ ] **A)** Encryption at rest for cloud object stores uses provider-managed or customer-managed keys
- [ ] **B)** HDFS encryption zones are managed by Apache Atlas
- [ ] **C)** TLS 1.2 is the minimum version enforced for service-to-service communication
- [ ] **D)** Cloud KMS key rotation automatically re-encrypts all existing data in the bucket

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> CDP uses cloud KMS for object store encryption and enforces TLS 1.2+. HDFS zones are managed by Ranger KMS, not Atlas. Key rotation affects only new writes.
 
 
</details>

### 25. Examine the audit log entry below. Which component generated this log?

```json
{
  "user": "janedoe",
  "resource": "default.customers.ssn",
  "action": "SELECT",
  "result": "Denied",
  "timestamp": "2025-03-01T14:30:00Z"
}
```

- [ ] **A)** Apache Ranger
- [ ] **B)** Apache Atlas
- [ ] **C)** Apache Knox
- [ ] **D)** Kerberos KDC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The log shows user, resource, action, and result (Allow/Deny), which is typical of Ranger audit events. Atlas audits metadata changes, Knox audits gateway access, and Kerberos logs ticket events.
 
 
</details>


---

### **Troubleshooting and Monitoring**

### 26. When a DataLake creation times out, what is the first step to diagnose the issue?

- [ ] **A)** Verify VPC/subnet routing and security group inbound/outbound rules
- [ ] **B)** Restart the DataLake services
- [ ] **C)** Check the YARN Resource Manager for queue capacity
- [ ] **D)** Update the FreeIPA certificate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In CDP Public Cloud, the first step is to check network-level configurations such as security groups and routing, as misconfigured firewall rules are a common cause of deployment failures.
 
 
</details>

### 27. Which of the following are common symptoms of resource contention in YARN?

- [ ] **A)** Job stays in ACCEPTED state
- [ ] **B)** Container allocation delays
- [ ] **C)** High network latency
- [ ] **D)** Kerberos authentication failures

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Resource contention in YARN often causes jobs to remain in ACCEPTED state and containers to be allocated slowly due to insufficient queue capacity or memory.
 
 
</details>

### 28. Examine the following command: `nc -zv hive-metastore.service.consul 9083`. What is its primary purpose?

```bash
nc -zv hive-metastore.service.consul 9083
```

- [ ] **A)** Verifies network connectivity to the Hive Metastore Thrift port
- [ ] **B)** Checks the status of the Hive Metastore service
- [ ] **C)** Tests Kerberos authentication
- [ ] **D)** Monitors YARN container allocation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The `nc -zv` command performs a port scan to check if the specified port (9083 for Hive Metastore) is reachable from the client, which is the first step in diagnosing connection failures.
 
 
</details>

### 29. Which Cloudera Manager alert severity indicates that immediate action is required?

- [ ] **A)** CRITICAL
- [ ] **B)** IMPORTANT
- [ ] **C)** INFORMATIONAL
- [ ] **D)** WARNING

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CRITICAL alerts in Cloudera Manager signify that a service or host is in a state requiring immediate action to prevent outage.
 
 
</details>

### 30. Which of the following are sources of monitoring data in CDP Public Cloud?

- [ ] **A)** Cloudera Manager alerts
- [ ] **B)** Cloud provider metrics
- [ ] **C)** Service logs
- [ ] **D)** CDP CLI commands

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Monitoring in CDP Public Cloud relies on Cloudera Manager alerts for stack health, cloud provider metrics for infrastructure, and logs for forensic analysis.
 
 
</details>

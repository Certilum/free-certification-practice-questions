<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cloudera/CDP%20Administrator%20-%20Private%20Cloud%20Base" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>CDP Administrator - Private Cloud Base</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Administration](#administration) (8 questions)
- [Backup and Disaster Recovery](#backup-and-disaster-recovery) (3 questions)
- [Installation and Configuration](#installation-and-configuration) (6 questions)
- [Monitoring and Logging](#monitoring-and-logging) (4 questions)
- [Security and Access Control](#security-and-access-control) (6 questions)
- [Troubleshooting and Optimization](#troubleshooting-and-optimization) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:11.229Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Administration | 8 |
| Backup and Disaster Recovery | 3 |
| Installation and Configuration | 6 |
| Monitoring and Logging | 4 |
| Security and Access Control | 6 |
| Troubleshooting and Optimization | 3 |

---

### **Administration**

### 1. What is the primary resource negotiation component in CDP Private Cloud Base?

- [ ] **A)** YARN
- [ ] **B)** HDFS
- [ ] **C)** MapReduce
- [ ] **D)** Cloudera Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> YARN is the resource negotiator that manages container allocation across the cluster.
 
 
</details>

### 2. Which two methods can be used to define resource pools in CDP Private Cloud Base?

- [ ] **A)** fair-scheduler.xml
- [ ] **B)** capacity-scheduler.xml
- [ ] **C)** hdfs-site.xml
- [ ] **D)** yarn-site.xml

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Fair Scheduler uses fair-scheduler.xml; Capacity Scheduler uses capacity-scheduler.xml.
 
 
</details>

### 3. In the YARN configuration snippet, which setting enables hard memory limits for containers?

```xml
<property><name>yarn.nodemanager.linux-container-executor.cgroups.memory.enabled</name><value>true</value></property>
```

- [ ] **A)** yarn.nodemanager.linux-container-executor.cgroups.memory.enabled
- [ ] **B)** yarn.scheduler.maximum-allocation-mb
- [ ] **C)** yarn.nodemanager.resource.memory-mb
- [ ] **D)** yarn.app.mapreduce.am.resource.mb

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The property enables cgroups-based memory limits, preventing OOM kills.
 
 
</details>

### 4. What is the default HDFS block size in CDP Private Cloud Base?

- [ ] **A)** 128 MB
- [ ] **B)** 64 MB
- [ ] **C)** 256 MB
- [ ] **D)** 512 MB

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The default HDFS block size is 128 MB, configurable via dfs.blocksize.
 
 
</details>

### 5. Which two mechanisms does YARN provide to isolate resources at the kernel level?

- [ ] **A)** CPU shares
- [ ] **B)** Memory limits
- [ ] **C)** Disk I/O rate
- [ ] **D)** Network bandwidth

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> cgroups provide CPU shares and memory limits for YARN container isolation.
 
 
</details>

### 6. In the fair-scheduler.xml snippet, what does the <minResources> element define?

```xml
<pool name="production"><minResources>1024 mb,1 vcores</minResources><maxResources>8192 mb,8 vcores</maxResources></pool>
```

- [ ] **A)** Guaranteed minimum resources for the pool
- [ ] **B)** Maximum allowed resources for the pool
- [ ] **C)** Current resource usage
- [ ] **D)** Preemption threshold

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> <minResources> ensures the pool receives at least that amount under contention.
 
 
</details>

### 7. Which built-in Cloudera Manager role can start and stop services but not change configurations?

- [ ] **A)** Operator
- [ ] **B)** Full Administrator
- [ ] **C)** Limited Administrator
- [ ] **D)** Read-Only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Operator role can start/stop services and view dashboards but cannot modify configurations.
 
 
</details>

### 8. Which two features are enforced by Cloudera Manager for internal users?

- [ ] **A)** Password complexity
- [ ] **B)** Password expiration
- [ ] **C)** Account lockout
- [ ] **D)** Multi-factor authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CM enforces password complexity and expiration for internal users; lockout is configurable but not default.
 
 
</details>


---

### **Backup and Disaster Recovery**

### 9. What is the most critical component of a Cloudera Manager backup?

- [ ] **A)** The Cloudera Manager Server database
- [ ] **B)** The parcel cache on each host
- [ ] **C)** The /etc/hosts file
- [ ] **D)** The root HDFS directory

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Cloudera Manager Server database stores all cluster metadata; without it, the cluster cannot be restored.
 
 
</details>

### 10. Which components are included in the backup created by the cloudera-manager-backup script?

- [ ] **A)** A database dump of the CM Server database
- [ ] **B)** The Cloudera Manager Server configuration directory
- [ ] **C)** Agent configuration files
- [ ] **D)** Deployment descriptor JSON files

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> The script bundles the database dump, server config, agent configs, and deployment descriptors into a tarball.
 
 
</details>

### 11. Which flag creates a full backup using the cloudera-manager-backup script?

```bash
/opt/cloudera/cm/bin/cloudera-manager-backup <flag>
```

- [ ] **A)** --full
- [ ] **B)** --incremental
- [ ] **C)** --complete
- [ ] **D)** --all

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The --full flag tells the script to create a complete backup of the database and all configuration files.
 
 
</details>


---

### **Installation and Configuration**

### 12. What is the recommended value for the kernel parameter vm.swappiness on CDP Private Cloud Base data nodes?

- [ ] **A)** 0
- [ ] **B)** 1
- [ ] **C)** 60
- [ ] **D)** 100

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Cloudera recommends setting vm.swappiness to 1 to minimize swapping and improve HDFS performance on data nodes.
 
 
</details>

### 13. Which storage practices are recommended by Cloudera for CDP Private Cloud Base? (Select all that apply)

- [ ] **A)** Use JBOD (Just a Bunch of Disks) for HDFS data disks
- [ ] **B)** Use RAID 10 for data disks to improve performance
- [ ] **C)** Mount data disks with the noatime option
- [ ] **D)** Place /var/log on the root partition without separate volume

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> JBOD and noatime mounts are recommended. RAID adds complexity and is not needed because HDFS provides redundancy.
 
 
</details>

### 14. Based on the command in the code block, which OS parameter is being configured?

```bash
echo 'vm.swappiness=1' >> /etc/sysctl.conf && sysctl -p
```

- [ ] **A)** vm.swappiness
- [ ] **B)** vm.max_map_count
- [ ] **C)** net.core.somaxconn
- [ ] **D)** transparent_hugepage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command sets vm.swappiness to 1, which is the recommended value for CDP data nodes.
 
 
</details>

### 15. What distribution mechanism does Cloudera use for CDP service binaries?

- [ ] **A)** RPM packages
- [ ] **B)** Parcels
- [ ] **C)** DEB packages
- [ ] **D)** Container images

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Cloudera uses self-contained parcels (tarballs) to distribute CDP services, allowing version switching without OS package conflicts.
 
 
</details>

### 16. Which of the following are prerequisites that must be fulfilled before installing CDP Private Cloud Base? (Select all that apply)

- [ ] **A)** Configure DNS with forward and reverse hostname resolution
- [ ] **B)** Synchronize clocks across all nodes using NTP
- [ ] **C)** Set SELinux to permissive mode or disable it
- [ ] **D)** Install Cloudera Manager Server on every node

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> DNS, NTP, and disabling SELinux (or permissive) are prerequisites. CM Server is installed on only one host, not all nodes.
 
 
</details>

### 17. The command in the code block is used to perform which action?

```bash
systemctl start cloudera-scm-server
```

- [ ] **A)** Start the Cloudera Manager Server
- [ ] **B)** Start the Cloudera Manager Agent
- [ ] **C)** Restart all cluster services
- [ ] **D)** Initialize the Cloudera Manager database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command `systemctl start cloudera-scm-server` launches the Cloudera Manager Server service.
 
 
</details>


---

### **Monitoring and Logging**

### 18. What are the four severity levels for alerts in Cloudera Manager?

- [ ] **A)** Critical, Warning, Informational, Unknown
- [ ] **B)** Critical, High, Medium, Low
- [ ] **C)** Fatal, Error, Warn, Info
- [ ] **D)** Emergency, Alert, Critical, Error

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloudera Manager defines Critical, Warning, Informational, and Unknown severity levels for alerts.
 
 
</details>

### 19. Which notification channels are supported for Cloudera Manager alerts?

- [ ] **A)** Email
- [ ] **B)** SNMP traps
- [ ] **C)** Custom webhooks
- [ ] **D)** JMS queues

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Cloudera Manager supports email, SNMP traps, and custom webhooks for alert notifications.
 
 
</details>

### 20. Examine the log4j configuration snippet for HDFS. What log level is set for the HDFS audit logger?

```properties
log4j.logger.org.apache.hadoop.hdfs.server.namenode.AuditLogger=INFO,RFAAUDIT
```

- [ ] **A)** INFO
- [ ] **B)** DEBUG
- [ ] **C)** WARN
- [ ] **D)** ERROR

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet `log4j.logger.org.apache.hadoop.hdfs.server.namenode.AuditLogger=INFO,RFAAUDIT` sets the level to INFO.
 
 
</details>

### 21. What is the default retention period for raw metric data in Cloudera Manager?

- [ ] **A)** 31 days
- [ ] **B)** 7 days
- [ ] **C)** 90 days
- [ ] **D)** 180 days

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloudera Manager retains raw metric data for 31 days by default.
 
 
</details>


---

### **Security and Access Control**

### 22. Which authentication mechanism is mandatory for secure CDP Private Cloud Base clusters?

- [ ] **A)** Kerberos
- [ ] **B)** LDAP
- [ ] **C)** SAML
- [ ] **D)** RADIUS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Kerberos is mandatory for secure CDP clusters because Hadoop services rely on it for mutual authentication.
 
 
</details>

### 23. Which two mechanisms are used for authentication in CDP Private Cloud Base? (Choose two.)

- [ ] **A)** Kerberos
- [ ] **B)** LDAP
- [ ] **C)** RADIUS
- [ ] **D)** SAML

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The two primary mechanisms are Kerberos for strong authentication and LDAP as an identity repository.
 
 
</details>

### 24. Complete the command to create a Kerberos principal for the HDFS service on node1.example.com in realm EXAMPLE.COM.

```bash
kadmin.local: addprinc -randkey hdfs/____@____
```

- [ ] **A)** hdfs/node1.example.com@EXAMPLE.COM
- [ ] **B)** node1.example.com/hdfs@EXAMPLE.COM
- [ ] **C)** HDFS/node1.example.com@EXAMPLE.COM
- [ ] **D)** hn/node1.example.com@EXAMPLE.COM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Service principals are formatted as service/fully.qualified.domain@REALM, e.g., hdfs/node1.example.com@EXAMPLE.COM.
 
 
</details>

### 25. What is the default port for Cloudera Manager Agent non-secure communication?

- [ ] **A)** 7182
- [ ] **B)** 7180
- [ ] **C)** 7184
- [ ] **D)** 7183

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The default non-secure port for Cloudera Manager Agent is 7182; secure is 7184.
 
 
</details>

### 26. Which two services provide centralized authorization in CDP Private Cloud Base? (Choose two.)

- [ ] **A)** Apache Sentry
- [ ] **B)** Apache Ranger
- [ ] **C)** Apache Knox
- [ ] **D)** Apache Atlas

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CDP supports both Apache Sentry (legacy) and Apache Ranger (recommended) for authorization.
 
 
</details>

### 27. Complete the statement: Apache Ranger stores audit logs in ____ by default.

```text
Ranger Admin stores audit logs in _____ by default.
```

- [ ] **A)** Solr
- [ ] **B)** HDFS
- [ ] **C)** MySQL
- [ ] **D)** Kafka

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Ranger audit logs are stored in Apache Solr by default; they can be exported to HDFS.
 
 
</details>


---

### **Troubleshooting and Optimization**

### 28. What is the first step in diagnosing a common cluster issue according to Cloudera best practices?

- [ ] **A)** Restart the service immediately
- [ ] **B)** Check Cloudera Manager health and events
- [ ] **C)** Run hdfs fsck /
- [ ] **D)** Check system logs on each node

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The logical workflow starts with identifying the symptom and gathering evidence from Cloudera Manager health and events before deeper analysis.
 
 
</details>

### 29. Which of the following are common troubleshooting traps? (Select two)

- [ ] **A)** Restarting the service as the first action
- [ ] **B)** Always checking system logs first
- [ ] **C)** Ignoring Cloudera Manager event history
- [ ] **D)** Using Cloudera Manager for all diagnostics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Restarting destroys evidence; ignoring event history loses context. Both are listed as common traps in the playbook.
 
 
</details>

### 30. Examine the following HDFS fsck output. Which issue does it indicate?

```text
Status: HEALTHY
Total size:    1000000000 B
Total dirs:    100
Total files:   500
Total symlinks: 0
Total blocks (validated): 480
Minimally replicated blocks: 480
Over-replicated blocks: 0
Under-replicated blocks: 0
Mis-replicated blocks: 0
Default replication factor: 3
Average block replication: 2.8
Missing blocks: 5
Corrupt blocks: 0
```

- [ ] **A)** NameNode is in safe mode
- [ ] **B)** DataNode heartbeat lost
- [ ] **C)** Block corruption or missing blocks
- [ ] **D)** Disk space is full

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Missing blocks indicate data corruption or unreplicated blocks, a common HDFS issue.
 
 
</details>

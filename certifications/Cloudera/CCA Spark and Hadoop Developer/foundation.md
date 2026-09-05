<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cloudera/CCA%20Spark%20and%20Hadoop%20Developer.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>CCA Spark and Hadoop Developer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Cluster Management](#cluster-management) (1 questions)
- [Data Analysis](#data-analysis) (2 questions)
- [Data Ingestion](#data-ingestion) (1 questions)
- [Data Processing](#data-processing) (3 questions)
- [Data Storage](#data-storage) (2 questions)
- [Security](#security) (1 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 10 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:19.681Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Cluster Management | 1 |
| Data Analysis | 2 |
| Data Ingestion | 1 |
| Data Processing | 3 |
| Data Storage | 2 |
| Security | 1 |

---

### **Cluster Management**

### 1. In a Cloudera deployment, what is the role of Apache Atlas in relation to Apache Ranger for security enforcement?

- [ ] **A)** Atlas enforces access policies by blocking users from reading files, while Ranger stores metadata tags.
- [ ] **B)** Atlas classifies and tags data assets, and this metadata synchronizes to Ranger so it can enforce tag-based access policies.
- [ ] **C)** Ranger sends security policies to Atlas, and Atlas enforces them at the file system level.
- [ ] **D)** Atlas and Ranger are independent; Atlas manages user roles, and Ranger manages metadata.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Atlas manages metadata and classification; it does not enforce access. Tags flow from Atlas to Ranger, which then enforces tag-based access policies (TBAC).
 
 
</details>


---

### **Data Analysis**

### 2. Which Cloudera component is responsible for defining and enforcing access control policies?

- [ ] **A)** Apache Ranger
- [ ] **B)** Apache Atlas
- [ ] **C)** Apache Hive
- [ ] **D)** Apache Spark

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Ranger is the centralized security administration tool used to define and enforce access policies. Atlas handles metadata management, while Hive and Spark are data processing engines.
 
 
</details>

### 3. Which statements correctly describe Apache Atlas' role in security and governance? (Select all that apply.)

- [ ] **A)** Atlas provides data classification and lineage tracking.
- [ ] **B)** Atlas enforces access policies by blocking unauthorized reads.
- [ ] **C)** Atlas tags are synced to Ranger for tag-based policy execution.
- [ ] **D)** Atlas receives policies from Ranger to manage metadata.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Atlas is a governance and metadata tool used for classification, lineage, and cataloging. Tags flow from Atlas to Ranger to inform policies; Atlas itself cannot enforce or block access.
 
 
</details>


---

### **Data Ingestion**

### 4. Which Apache Hadoop component is used to centrally define and enforce access policies for data resources?

- [ ] **A)** Ranger
- [ ] **B)** Atlas
- [ ] **C)** Kerberos
- [ ] **D)** HiveServer2

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Ranger is the centralized security administration tool used to define and enforce access policies. Atlas manages metadata, Kerberos handles authentication, and HiveServer2 is a service principal.
 
 
</details>


---

### **Data Processing**

### 5. Which component in the Hadoop ecosystem is used to define and enforce access policies?

- [ ] **A)** Ranger
- [ ] **B)** Atlas
- [ ] **C)** HDFS
- [ ] **D)** Hive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Ranger is the centralized security administration tool used to define and enforce access policies. Atlas is a metadata management framework and does not enforce access. HDFS and Hive are not policy enforcement tools.
 
 
</details>

### 6. Which statements correctly describe Apache Atlas? (Select all that apply.)

- [ ] **A)** Atlas is primarily a metadata management framework for data classification, lineage tracking, and cataloging.
- [ ] **B)** Atlas can enforce access policies by blocking users from reading sensitive files.
- [ ] **C)** Tag metadata in Atlas can be synchronized to Ranger to enable tag-based access control.
- [ ] **D)** Metadata flows from Ranger to Atlas so Ranger classifications can update Atlas tags.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Atlas is a governance and metadata tool that classifies data, tracks lineage, and catalogs assets. It cannot enforce security. Atlas metadata, including tags, flows to Ranger to inform tag-based policies, not the other way around.
 
 
</details>

### 7. A developer creates a Ranger policy with a tag condition, as shown in the snippet. Where are the tag definitions managed and synchronized from?

```json
{
  "name": "tag_policy_pii",
  "service": "tag_service",
  "tags": ["PII"],
  "users": ["analyst"],
  "accesses": ["read"]
}
```

- [ ] **A)** Atlas
- [ ] **B)** Ranger
- [ ] **C)** HDFS
- [ ] **D)** YARN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet represents a tag-based Ranger policy. Tags are defined and maintained in Atlas, then synchronized to Ranger so policies can be enforced based on data classifications such as PII.
 
 
</details>


---

### **Data Storage**

### 8. In a Cloudera deployment, which component is responsible for defining and enforcing access control policies?

- [ ] **A)** Apache Ranger
- [ ] **B)** Apache Atlas
- [ ] **C)** Apache Hive
- [ ] **D)** Apache Spark

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Ranger is the centralized security administration tool used to define and enforce access policies. Atlas is a metadata management framework and does not enforce security.
 
 
</details>

### 9. Which statements correctly describe the integration between Apache Atlas and Apache Ranger?

- [ ] **A)** When a user tags an asset in Atlas, that metadata can be synchronized to Ranger for tag-based policies.
- [ ] **B)** Ranger sends metadata tags to Atlas to enforce classification-based access control.
- [ ] **C)** Atlas can block users from reading a file if they are not authorized.
- [ ] **D)** Ranger can execute policies based on Atlas tags rather than specific file paths or table names.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Metadata flows from Atlas to Ranger: Atlas tags such as 'PII' are synchronized to Ranger, which can then enforce policies based on those tags. Atlas is purely a governance and metadata tool and cannot block access, and metadata does not flow from Ranger to Atlas.
 
 
</details>


---

### **Security**

### 10. In a Cloudera environment, which component is responsible for defining and enforcing access policies, and which component serves as the metadata management framework?

- [ ] **A)** Ranger enforces access policies; Atlas manages metadata, classification, and lineage.
- [ ] **B)** Atlas enforces access policies; Ranger manages metadata, classification, and lineage.
- [ ] **C)** Ranger manages metadata and lineage; Atlas enforces access policies.
- [ ] **D)** Both Ranger and Atlas enforce access policies collaboratively.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Ranger is the centralized security administration tool used to define and enforce access policies, while Atlas is the metadata management framework used for data classification, lineage tracking, and cataloging. Together, they ensure security follows the data.
 
 
</details>

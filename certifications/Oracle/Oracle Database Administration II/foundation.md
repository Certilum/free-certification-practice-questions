<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Oracle%20Database%20Administration%20I.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Oracle Database Administration II</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Application PDBs](#application-pdbs) (3 questions)
- [Backup and Recovery](#backup-and-recovery) (6 questions)
- [Database Duplication](#database-duplication) (2 questions)
- [Flashback Technologies](#flashback-technologies) (2 questions)
- [Multitenant Architecture](#multitenant-architecture) (5 questions)
- [Multitenant Security](#multitenant-security) (3 questions)
- [Patching and Upgrades](#patching-and-upgrades) (4 questions)
- [Performance and Tuning](#performance-and-tuning) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:46:28.674Z |
| Domains | 8 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Application PDBs | 3 |
| Backup and Recovery | 6 |
| Database Duplication | 2 |
| Flashback Technologies | 2 |
| Multitenant Architecture | 5 |
| Multitenant Security | 3 |
| Patching and Upgrades | 4 |
| Performance and Tuning | 5 |

---

### **Application PDBs**

### 1. What is an application PDB?

- [ ] **A)** A PDB that is created inside an application root
- [ ] **B)** A PDB that is created directly in the CDB root
- [ ] **C)** A PDB that does not belong to a container
- [ ] **D)** A PDB used only for backup and recovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An application PDB is a pluggable database that belongs to an application root in an application container. It is not plugged into the CDB root directly.
 
 
</details>

### 2. Which of the following are valid components of an Oracle application container? (Select all that apply.)

- [ ] **A)** Application root
- [ ] **B)** Application PDBs
- [ ] **C)** Application seed
- [ ] **D)** CDB root

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> An application container is composed of an application root and can include application PDBs and an application seed. The CDB root is above all application containers and is not a component of one.
 
 
</details>

### 3. You run the statement shown in the code block while connected to the root of the CDB. What component is created?

```sql
CREATE PLUGGABLE DATABASE sales_app AS APPLICATION CONTAINER ADMIN USER sa_admin IDENTIFIED BY Password123;
```

- [ ] **A)** An application root
- [ ] **B)** An application PDB
- [ ] **C)** An application seed
- [ ] **D)** A CDB root

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The AS APPLICATION CONTAINER clause creates a PDB that acts as the application root. It does not by itself create an application seed or an application PDB.
 
 
</details>


---

### **Backup and Recovery**

### 4. What is an application PDB in an Oracle multitenant environment?

- [ ] **A)** A pluggable database inside an application container
- [ ] **B)** A database that replaces the CDB root
- [ ] **C)** A PDB that is permanently read-only
- [ ] **D)** A file set shared by every PDB

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An application PDB is a pluggable database that belongs to an application container inside a CDB. It shares common objects managed through the application root.
 
 
</details>

### 5. Which two statements are true about application PDBs?

- [ ] **A)** They belong to an application container
- [ ] **B)** Application changes from the app root can be synchronized into them
- [ ] **C)** They are standalone databases outside the CDB
- [ ] **D)** They must always remain in mount mode

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> An application PDB is a member of an application container. One key benefit is synchronizing application changes such as updates and patches from the application root to application PDBs.
 
 
</details>

### 6. Refer to the RMAN command in the code block. What is the outcome of running this command?

```rman
BACKUP PLUGGABLE DATABASE app_pdb1;
```

- [ ] **A)** A backup of the application PDB named app_pdb1
- [ ] **B)** A backup of all PDBs in the CDB
- [ ] **C)** A backup of the CDB root only
- [ ] **D)** A backup of the application seed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RMAN uses BACKUP PLUGGABLE DATABASE with a PDB name to back up one specific pluggable database, including an application PDB.
 
 
</details>

### 7. What is the purpose of the application root in an application container?

- [ ] **A)** It acts as the root for common objects and app PDBs
- [ ] **B)** It stores the archived redo logs for all CDBs
- [ ] **C)** It creates the control file for the CDB
- [ ] **D)** It replaces the recovery catalog

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An application root is a PDB that serves as the container root for the application container. It stores common objects that can be shared by application PDBs.
 
 
</details>

### 8. Which two conditions are required before performing an online RMAN backup of an application PDB?

- [ ] **A)** The CDB must be in ARCHIVELOG mode
- [ ] **B)** The PDB must be accessible to RMAN
- [ ] **C)** The PDB must be unplugged first
- [ ] **D)** All other PDBs must be shut down

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Online RMAN backups need archive log mode so redo can be used for recovery. RMAN also must be able to access the target application PDB.
 
 
</details>

### 9. Refer to the RMAN command in the code block. What will RMAN display after this command is run?

```rman
LIST BACKUP OF PLUGGABLE DATABASE app_pdb1;
```

- [ ] **A)** Backups recorded for app_pdb1
- [ ] **B)** Backups recorded for the entire CDB
- [ ] **C)** Tablespace usage in app_pdb1
- [ ] **D)** The current status of the application seed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> LIST BACKUP OF PLUGGABLE DATABASE shows backup information for a particular PDB, making it useful for checking backups that exist for app_pdb1.
 
 
</details>


---

### **Database Duplication**

### 10. When a DBA reviews an Oracle multitenant database, which description best identifies an application PDB?

- [ ] **A)** Created inside an application container
- [ ] **B)** Used solely as a CDB seed
- [ ] **C)** Configured only for Oracle Cloud
- [ ] **D)** Mounted as a read-only report store

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An application PDB is created inside an application container. It is not just a seed, a cloud-only object, or a read-only reporting store.
 
 
</details>

### 11. Which statements below correctly describe how application PDBs relate to the application container in Oracle multitenant databases? Select all that apply.

- [ ] **A)** They are kept inside an application container.
- [ ] **B)** They hold data and metadata for an application.
- [ ] **C)** They are placed directly in the CDB root without a parent application container.
- [ ] **D)** They can be created only from a non-CDB backup.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Application PDBs belong to an application container and store application-specific data and metadata. They do not live directly in the CDB root and are not limited to non-CDB backups.
 
 
</details>


---

### **Flashback Technologies**

### 12. Within the context of Oracle multitenant architecture, which statement best describes an Application PDB in a CDB?

- [ ] **A)** PDB inside an application root
- [ ] **B)** Root of the CDB container
- [ ] **C)** Stand-alone PDB without an application root
- [ ] **D)** Template used for creating PDBs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An Application PDB belongs to an application root and is part of an application container, not the CDB root or a seed template.
 
 
</details>

### 13. Within an Oracle application container, which two statements about Application PDBs are true? (Choose two.)

- [ ] **A)** PDB under an application root
- [ ] **B)** Container root of the CDB
- [ ] **C)** Shares common objects from its application root
- [ ] **D)** Never synchronized with its application root

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Application PDBs are contained in the application root and use common application objects installed there; they can also be synchronized with the app root.
 
 
</details>


---

### **Multitenant Architecture**

### 14. In an Oracle multitenant container database, which type of container is the home for an application PDB?

- [ ] **A)** Application container
- [ ] **B)** CDB root
- [ ] **C)** ASM disk group
- [ ] **D)** Recovery catalog

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An application PDB is a PDB that is created in an application container, not in the CDB root, ASM, or recovery catalog.
 
 
</details>

### 15. Which two statements about application PDBs in an Oracle multitenant container database environment are correct?

- [ ] **A)** They are created inside an application container.
- [ ] **B)** They can only be used by the CDB root.
- [ ] **C)** They can be opened and closed independently.
- [ ] **D)** They do not need a data dictionary.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Application PDBs live inside an application container. Like other PDBs, they can be opened and closed independently; they also maintain a data dictionary.
 
 
</details>

### 16. Review the SQL code block and identify what container type is created by the statement.

```sql
CREATE PLUGGABLE DATABASE app_container
  ADMIN USER app_admin IDENTIFIED BY Oracle_123
  AS APPLICATION CONTAINER;
```

- [ ] **A)** Application container
- [ ] **B)** Application PDB
- [ ] **C)** Regular PDB
- [ ] **D)** CDB root

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The AS APPLICATION CONTAINER clause makes the new PDB an application container in which application PDBs can later be created.
 
 
</details>

### 17. In an Oracle application container, which container component stores the application common objects used by application PDBs?

- [ ] **A)** Application root
- [ ] **B)** Each application PDB
- [ ] **C)** CDB root
- [ ] **D)** Online redo log

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The application root is the container component that stores application common objects and makes them available to application PDBs.
 
 
</details>

### 18. When an administrator creates an application PDB, which two statements are true in an Oracle multitenant database?

- [ ] **A)** Connect to the application root.
- [ ] **B)** Connect to the CDB root.
- [ ] **C)** Application container must already exist.
- [ ] **D)** PDB is created outside an application container.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> An application PDB is created by connecting to the application root and creating a PDB inside an existing application container.
 
 
</details>


---

### **Multitenant Security**

### 19. Which statement correctly defines what an application PDB is in an Oracle Multitenant container database environment?

- [ ] **A)** A PDB inside an application container
- [ ] **B)** A PDB that stores only CDB backups
- [ ] **C)** A PDB detached from all containers
- [ ] **D)** A replacement for the CDB root

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An application PDB is a pluggable database that belongs to an application container. It stores user data and can share application common objects with other PDBs in that container.
 
 
</details>

### 20. Which two statements about application PDBs are true in an Oracle multitenant container database environment?

- [ ] **A)** They live in application containers
- [ ] **B)** They can share application common objects
- [ ] **C)** They cannot be opened or closed
- [ ] **D)** They are copies of CDB root

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Application PDBs belong to an application container and can mount application common objects used in application installs. They are normal PDBs and can be opened and closed as needed.
 
 
</details>

### 21. Review the SQL command in the code block. An administrator connected to an application root in Oracle Multitenant executes it. What happens?

```sql
ALTER PLUGGABLE DATABASE app_pdb1 APPLICATION BEGIN;
```

- [ ] **A)** Starts an application change transaction
- [ ] **B)** Shuts down the named PDB
- [ ] **C)** Unplugs the named PDB
- [ ] **D)** Deletes common application metadata

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The APPLICATION BEGIN clause opens a transaction for application maintenance. Application installs or upgrades place operations between this command and APPLICATION END before changes become permanent or are rolled back.
 
 
</details>


---

### **Patching and Upgrades**

### 22. What is an application PDB in an Oracle multitenant environment?

- [ ] **A)** A regular PDB plugged into an application root that contains application data and metadata
- [ ] **B)** The root container that stores Oracle metadata for all PDBs
- [ ] **C)** A PDB created only for storing Oracle patch bundles
- [ ] **D)** A seed PDB used to create new application roots

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An application PDB is a PDB that is plugged into an application root. It participates in the application container and contains application-specific data and metadata.
 
 
</details>

### 23. Which containers are part of an application container?

- [ ] **A)** Application root
- [ ] **B)** Application seed
- [ ] **C)** Application PDB
- [ ] **D)** CDB root

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> An application container consists of an application root, an application seed, and application PDBs. The CDB root is the root of the entire multitenant container database and is not part of an application container.
 
 
</details>

### 24. The code block shows a SQL statement. What kind of container is created when the statement is executed?

```sql
CREATE PLUGGABLE DATABASE app_root AS APPLICATION CONTAINER ADMIN USER app_admin IDENTIFIED BY password;
```

- [ ] **A)** Application root
- [ ] **B)** Application PDB
- [ ] **C)** Application seed
- [ ] **D)** CDB root

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The clause AS APPLICATION CONTAINER creates an application root, which is the parent container for an application container.
 
 
</details>

### 25. Which statement best describes an application seed?

- [ ] **A)** A template used to create application PDBs
- [ ] **B)** A copy of CDB$ROOT used to create new CDBs
- [ ] **C)** A special PDB used only for application patching
- [ ] **D)** A database link required for application upgrades

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The application seed is a template PDB in the application container. It is used as a base for creating new application PDBs.
 
 
</details>


---

### **Performance and Tuning**

### 26. Which statement best defines an application PDB when it is created inside an Oracle multitenant application container?

- [ ] **A)** A PDB using an application root
- [ ] **B)** A PDB containing the whole CDB
- [ ] **C)** A PDB created automatically by RMAN
- [ ] **D)** A PDB that stores only AWR data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An application PDB belongs to an application container and shares application metadata through its application root.
 
 
</details>

### 27. Which two resource dimensions can a CDB resource plan allocate among application PDBs?

- [ ] **A)** CPU usage
- [ ] **B)** I/O usage
- [ ] **C)** SCN value
- [ ] **D)** Alert log size

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A CDB resource plan can control resource allocation across PDBs, including CPU and I/O. SCN values and alert log sizes are not managed resources.
 
 
</details>

### 28. Examine the CREATE PLUGGABLE DATABASE statement in the code block. What type of container is created by this command?

```sql
CREATE PLUGGABLE DATABASE app_root AS APPLICATION CONTAINER ADMIN USER app_admin IDENTIFIED BY Password123;
```

- [ ] **A)** Application root
- [ ] **B)** Application seed
- [ ] **C)** Application PDB
- [ ] **D)** OS file system

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The clause AS APPLICATION CONTAINER creates an application root, which is a PDB that can contain application PDBs.
 
 
</details>

### 29. Which statement is true about the application seed inside an application container?

- [ ] **A)** Template for app PDBs
- [ ] **B)** Storage for alert logs
- [ ] **C)** Backup of CDB root
- [ ] **D)** Repository for optimizer stats

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An application seed acts as a template that helps Oracle create application PDBs consistently within an application container.
 
 
</details>

### 30. Which two sections of an AWR PDB report are most useful when diagnosing an application PDB performance problem?

- [ ] **A)** Top SQL statements
- [ ] **B)** Wait event statistics
- [ ] **C)** RMAN backup schedule
- [ ] **D)** Password profile settings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> AWR PDB reports include workload, SQL, and wait event data that help diagnose database performance issues.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Oracle%20Database%20Administration%20I.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Oracle Database Administration I</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Configuring Oracle Net Services](#configuring-oracle-net-services) (3 questions)
- [Managing Database Instances](#managing-database-instances) (4 questions)
- [Managing Storage](#managing-storage) (4 questions)
- [Managing Undo](#managing-undo) (3 questions)
- [Managing Users, Roles and Privileges](#managing-users-roles-and-privileges) (5 questions)
- [Moving Data](#moving-data) (3 questions)
- [SQL Fundamentals for DBA](#sql-fundamentals-for-dba) (3 questions)
- [Understanding Oracle Database Architecture](#understanding-oracle-database-architecture) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:46:26.079Z |
| Domains | 8 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Configuring Oracle Net Services | 3 |
| Managing Database Instances | 4 |
| Managing Storage | 4 |
| Managing Undo | 3 |
| Managing Users, Roles and Privileges | 5 |
| Moving Data | 3 |
| SQL Fundamentals for DBA | 3 |
| Understanding Oracle Database Architecture | 5 |

---

### **Configuring Oracle Net Services**

### 1. Which statement best describes the purpose of the tnsnames.ora file on an Oracle Net client?

- [ ] **A)** Maps connect identifiers to connect descriptors.
- [ ] **B)** Stores listener protocol endpoints.
- [ ] **C)** Contains encrypted client authentication data.
- [ ] **D)** Controls database instance resource limits.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> tnsnames.ora is the local naming configuration file. It allows a client to use a net service name or connect identifier that resolves to a valid connect descriptor.
 
 
</details>

### 2. Which two statements correctly describe Oracle Net Listener responsibilities? (Select two.)

- [ ] **A)** Accepts and forwards client connection requests.
- [ ] **B)** Stores all database user passwords.
- [ ] **C)** May service several database instances.
- [ ] **D)** Optimizes SQL execution plans.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Oracle Net Listener receives initial connection requests and redirects or forwards them to a database service. One listener process can support multiple database instances through service registration.
 
 
</details>

### 3. The code block shows a configuration entry. Which file stores this entry on a dedicated Oracle Net listener host?

```text
LISTENER =
  (DESCRIPTION =
    (ADDRESS = (PROTOCOL = TCP)(HOST = sales-svr1)(PORT = 1521)))

```

- [ ] **A)** listener.ora
- [ ] **B)** tnsnames.ora
- [ ] **C)** sqlnet.ora
- [ ] **D)** orapwd.ora

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A listener.ora file holds the listener name and its protocol addresses. The example defines a listener named LISTENER using TCP on port 1521.
 
 
</details>


---

### **Managing Database Instances**

### 4. Which Oracle utility is the primary tool for moving logical data and metadata between databases or schemas?

- [ ] **A)** Oracle Data Pump
- [ ] **B)** SQL*Loader
- [ ] **C)** RMAN
- [ ] **D)** Automatic Workload Repository

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Oracle Data Pump is the primary tool for logical data movement and metadata. SQL*Loader loads external files, RMAN handles physical backups, and AWR collects performance statistics.
 
 
</details>

### 5. Which types of objects can be moved with Oracle Data Pump?

- [ ] **A)** Table data and metadata
- [ ] **B)** Entire schemas
- [ ] **C)** Oracle home binary files
- [ ] **D)** Database alert log files

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Oracle Data Pump operates on logical objects, including table data and schemas. It does not move operating system files such as Oracle home binaries or alert logs.
 
 
</details>

### 6. Examine the SQL command. What is the effect of executing the statement?

```sql
CREATE OR REPLACE DIRECTORY dp_dir AS '/u01/app/oracle/dp';
```

- [ ] **A)** An Oracle directory object for dump files
- [ ] **B)** A physical operating system directory
- [ ] **C)** A table named DP_DIR
- [ ] **D)** A database backup job

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CREATE DIRECTORY creates a database directory object that points to an operating system location. It does not create the OS directory, a table, or a backup job.
 
 
</details>

### 7. What is the output of a Data Pump export job called?

- [ ] **A)** Dump file set
- [ ] **B)** Control file
- [ ] **C)** Parameter file
- [ ] **D)** Redo log file

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Data Pump Export writes logical copies of selected objects into a dump file set. Import later reads that dump file set to recreate the objects.
 
 
</details>


---

### **Managing Storage**

### 8. Which Oracle Database utility creates a portable dump file set containing data and metadata for movement to another database?

- [ ] **A)** Oracle Data Pump Export
- [ ] **B)** SQL*Loader utility
- [ ] **C)** Oracle Recovery Manager
- [ ] **D)** Directory object

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Oracle Data Pump Export writes data and metadata into dump files that can be copied and imported into another Oracle database.
 
 
</details>

### 9. Which two types of content are saved in a dump file generated by Oracle Data Pump Export?

- [ ] **A)** Database table data
- [ ] **B)** Parameter file values
- [ ] **C)** Schema object definitions
- [ ] **D)** Instance startup settings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Data Pump Export captures logical table data and metadata that describes schemas, including definitions of tables, indexes, constraints, and other objects.
 
 
</details>

### 10. Examine the command shown in the code block. Which Oracle Database utility is invoked by this command?

```bash
expdp hr/hr@orcl SCHEMAS=hr DIRECTORY=data_pump_dir DUMPFILE=hr_schema.dmp
```

- [ ] **A)** Oracle Data Pump Export
- [ ] **B)** Oracle Data Pump Import
- [ ] **C)** SQL*Loader utility
- [ ] **D)** Oracle Recovery Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The expdp command is the command-line client for Oracle Data Pump Export, used here to move the hr schema into a dump file.
 
 
</details>

### 11. Which Oracle Database feature allows SQL to read data from an operating-system file without loading it into the database?

- [ ] **A)** External table feature
- [ ] **B)** Directory object
- [ ] **C)** SQL*Loader utility
- [ ] **D)** Materialized view

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An external table keeps rows in a flat file but exposes the file to SQL, allowing data to be selected without first loading it.
 
 
</details>


---

### **Managing Undo**

### 12. Which Oracle utility is used to move data between Oracle databases by creating a binary dump file set?

- [ ] **A)** SQL*Loader
- [ ] **B)** Oracle Data Pump
- [ ] **C)** External tables
- [ ] **D)** Recovery Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Oracle Data Pump Export creates a binary dump file set; Data Pump Import later reads that file set and moves objects and data into another Oracle database.
 
 
</details>

### 13. Which two statements are true about SQL*Loader? (Choose two.)

- [ ] **A)** It is invoked with the sqlldr command.
- [ ] **B)** It uses a control file to describe the input data format.
- [ ] **C)** It can be used only for Data Pump dump files.
- [ ] **D)** It automatically creates all target tables and indexes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SQL*Loader loads data from external flat files into an Oracle database. It is started with sqlldr and uses a control file to interpret the input data.
 
 
</details>

### 14. You run the command shown in the code block. What is the expected result in the target database?

```bash
impdp system/oracle@ORCL DIRECTORY=data_pump_dir DUMPFILE=hr.dmp SCHEMAS=hr CONTENT=METADATA_ONLY
```

- [ ] **A)** Creates schema metadata but no table data.
- [ ] **B)** Imports rows into existing tables only.
- [ ] **C)** Drops the imported schema objects before loading them.
- [ ] **D)** Creates a backup of the dump file set.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CONTENT=METADATA_ONLY parameter tells Data Pump Import to restore object definitions only. No table rows are loaded into the target schema.
 
 
</details>


---

### **Managing Users, Roles and Privileges**

### 15. In Oracle Database, which definition best describes what a privilege is compared to other security objects?

- [ ] **A)** Right to execute SQL or access objects
- [ ] **B)** Encryption rule for stored passwords
- [ ] **C)** Storage limit assigned to a tablespace
- [ ] **D)** Backup schedule configured by an administrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A privilege is the right to run a particular SQL statement or to access another schema's object. Privileges are security grants, not encryption, storage, or backup settings.
 
 
</details>

### 16. In Oracle Database, which of the following are classified as system privileges? Select all that apply.

- [ ] **A)** CREATE SESSION
- [ ] **B)** ALTER SYSTEM
- [ ] **C)** UPDATE ON hr.employees
- [ ] **D)** CREATE TABLE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> CREATE SESSION, ALTER SYSTEM, and CREATE TABLE are system privileges. UPDATE ON hr.employees applies to a specific table, so it is an object privilege.
 
 
</details>

### 17. Look at the GRANT command shown in the code block. What category of privileges is being granted to user SCOTT?

```sql
GRANT SELECT, INSERT ON hr.departments TO scott;
```

- [ ] **A)** Object privileges
- [ ] **B)** System privileges
- [ ] **C)** Role privileges
- [ ] **D)** Resource privileges

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The SELECT and INSERT privileges are granted on the hr.departments table. Privileges on a specific object are object privileges rather than system privileges.
 
 
</details>

### 18. In a CREATE USER statement for an Oracle user, what is the function of the DEFAULT TABLESPACE clause?

- [ ] **A)** Sets where permanent objects are stored
- [ ] **B)** Sets where temporary sort data is stored
- [ ] **C)** Sets where undo data is recorded
- [ ] **D)** Sets how often the password must change

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The DEFAULT TABLESPACE clause establishes where the user's permanent objects, such as tables and indexes, are stored when no tablespace is named.
 
 
</details>

### 19. Which of the following statements about Oracle roles are true? Select all that apply.

- [ ] **A)** A role is a named group of privileges
- [ ] **B)** Roles can include both system and object privileges
- [ ] **C)** Roles simplify privilege administration
- [ ] **D)** Roles cannot be granted to other roles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A role is a named set of privileges and can be granted to users or other roles. Roles contain system and object privileges and reduce the number of individual GRANT statements.
 
 
</details>


---

### **Moving Data**

### 20. Which Oracle tool is designed for logical data movement between Oracle databases?

- [ ] **A)** Oracle Data Pump
- [ ] **B)** SQL*Loader
- [ ] **C)** Recovery Manager (RMAN)
- [ ] **D)** Automatic Storage Management (ASM)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Oracle Data Pump performs logical exports and imports using dump files. SQL*Loader loads external files; Recovery Manager is used for physical backup.
 
 
</details>

### 21. Which two command-line clients are used for Oracle Data Pump operations? (Choose two.)

- [ ] **A)** expdp
- [ ] **B)** impdp
- [ ] **C)** sqlldr
- [ ] **D)** rman

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> expdp starts a Data Pump export and impdp starts a Data Pump import. sqlldr and rman are used by SQL*Loader and Recovery Manager instead.
 
 
</details>

### 22. View the Data Pump command shown in the code block. What operation is the command performing?

```bash
expdp hr/hr_password@orclpdb DIRECTORY=dp_dir DUMPFILE=hr_schema.dmp LOGFILE=exp_hr.log SCHEMAS=hr
```

- [ ] **A)** It imports the HR schema
- [ ] **B)** It exports the HR schema
- [ ] **C)** It creates a directory object
- [ ] **D)** It loads external table data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Because the command starts with expdp and includes SCHEMAS=hr, it performs a Data Pump schema export for the HR schema.
 
 
</details>


---

### **SQL Fundamentals for DBA**

### 23. Which Data Pump command-line client is used to export data and metadata to a dump file?

- [ ] **A)** impdp
- [ ] **B)** expdp
- [ ] **C)** SQL*Loader
- [ ] **D)** RMAN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> expdp is Oracle Data Pump's export client. It writes schema objects and data to a dump file set; impdp performs the import direction.
 
 
</details>

### 24. Which Oracle utilities or features are commonly used to move data into or out of an Oracle database? Select all that apply.

- [ ] **A)** Data Pump export and import
- [ ] **B)** Automatic Storage Management
- [ ] **C)** External tables
- [ ] **D)** SQL*Loader

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Data Pump, SQL*Loader, and external tables are standard Oracle options for moving data into or out of a database. ASM manages storage but does not move logical data.
 
 
</details>

### 25. Examine the Data Pump export command in the code block. What does the schema parameter limit the export to?

```bash
expdp system/password@ORCL DIRECTORY=data_pump_dir DUMPFILE=hr_dump.dmp SCHEMAS=hr
```

- [ ] **A)** The objects in the specified schema are overwritten in the target database.
- [ ] **B)** The entire database is exported without object filtering.
- [ ] **C)** Only the objects owned by the specified schema are unloaded.
- [ ] **D)** The specified schema is created and then removed during the export.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The SCHEMAS parameter identifies the schema owner. Only objects owned by that schema are written to the dump file; other schemas are not exported.
 
 
</details>


---

### **Understanding Oracle Database Architecture**

### 26. In the context of moving data between Oracle databases, what is Oracle Data Pump primarily designed to accomplish?

- [ ] **A)** High-speed server-side export and import of logical data
- [ ] **B)** Physical backup of database data files
- [ ] **C)** Network traffic monitoring and tuning
- [ ] **D)** Storage reallocation within tablespaces

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Oracle Data Pump runs on the database server and moves logical data and metadata in dump file sets.
 
 
</details>

### 27. Within Oracle Database administration, which two statements correctly describe the behavior and purpose of SQL*Loader?

- [ ] **A)** Loads data from external files into tables
- [ ] **B)** Uses a control file to define loading rules
- [ ] **C)** Used for logical database export
- [ ] **D)** Performs recovery after media failure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SQL*Loader reads data from external files and loads it into Oracle tables using a control file. It is not an export or recovery tool.
 
 
</details>

### 28. Examine the command in the code block and identify which Oracle Database utility is being invoked.

```bash
#!/bin/bash
impdp admin/password@ORCL DIRECTORY=DATA_PUMP_DIR DUMPFILE=hr.dmp SCHEMAS=hr
```

- [ ] **A)** Oracle Data Pump Import
- [ ] **B)** Oracle Data Pump Export
- [ ] **C)** SQL*Loader
- [ ] **D)** Recovery Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The impdp command starts Oracle Data Pump Import, which reads a dump file set and loads objects into an Oracle database.
 
 
</details>

### 29. Before running a Data Pump job, which database object identifies the operating system directory for dump files?

- [ ] **A)** Directory object
- [ ] **B)** Tablespace
- [ ] **C)** Profile
- [ ] **D)** Synonym

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A directory object stores the operating system path where Data Pump reads or writes files. The user must be granted read and write privileges on it.
 
 
</details>

### 30. During an Oracle Data Pump export job, which two file types are normally generated on the server?

- [ ] **A)** Dump file set
- [ ] **B)** Log file
- [ ] **C)** Control file
- [ ] **D)** Oracle Net configuration file

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Data Pump creates dump files containing data and metadata and a log file that records the job's progress. Control files and Oracle Net files are not part of Data Pump.
 
 
</details>

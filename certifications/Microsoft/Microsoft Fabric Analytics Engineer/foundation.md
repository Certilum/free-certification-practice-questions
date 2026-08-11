<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/microsoft-certified-associate-badge.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Microsoft Fabric Analytics Engineer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Explore and analyze data](#explore-and-analyze-data) (6 questions)
- [Implement and manage semantic models](#implement-and-manage-semantic-models) (7 questions)
- [Plan, implement, and manage a solution for data analytics](#plan-implement-and-manage-a-solution-for-data-analytics) (4 questions)
- [Prepare and serve data](#prepare-and-serve-data) (13 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-11T02:42:32.860Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Explore and analyze data | 6 |
| Implement and manage semantic models | 7 |
| Plan, implement, and manage a solution for data analytics | 4 |
| Prepare and serve data | 13 |

---

### **Explore and analyze data**

### 1. Which visual type should you choose when your exploration scenario requires a multi-dimensional comparison across several fields?

- [ ] **A)** Matrix
- [ ] **B)** Scatter chart
- [ ] **C)** Line chart
- [ ] **D)** Pie chart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A matrix supports multi-dimensional comparisons, making it the best selection when the exploration must compare values across several fields.
 
 
</details>

### 2. Power BI maintains several principal filter levels. Which of the following are included in that set?

- [ ] **A)** Visual-level filter
- [ ] **B)** Page-level filter
- [ ] **C)** Report-level filter
- [ ] **D)** Slicer-level filter

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Power BI has three principal filter levels: visual, page, and report. Slicers act as page-level filters rather than a separate level.
 
 
</details>

### 3. The DAX query shown in the code block is executed against a semantic model. What output should it produce?

```dax
EVALUATE
CALCULATETABLE(Product, Product[Color] = "Red")
```

- [ ] **A)** Only product rows where Color is Red
- [ ] **B)** A scalar value for total product count
- [ ] **C)** An error because CALCULATETABLE is invalid
- [ ] **D)** An empty table with no rows

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CALCULATETABLE evaluates a table expression under modified filter conditions, so the query returns only the product rows where Color is Red.
 
 
</details>

### 4. Which Fabric AI capability should you use to automatically find statistically unusual changes in a time-series line chart?

- [ ] **A)** Anomaly Detection
- [ ] **B)** Key Influencers
- [ ] **C)** Decomposition Tree
- [ ] **D)** Smart Narrative

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Anomaly Detection uses time-series analysis on a line chart to identify data points that fall outside expected ranges and can explain their causes.
 
 
</details>

### 5. In a Microsoft Fabric environment, which of the following must be in place before Copilot can be used by analysts?

- [ ] **A)** Paid Fabric capacity of F64 or higher
- [ ] **B)** Power BI Premium capacity of P1 or higher
- [ ] **C)** Copilot enabled by the tenant admin
- [ ] **D)** DirectQuery mode for every semantic model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Copilot requires premium Fabric or Power BI capacity, tenant admin enablement, and appropriate user licenses. A DirectQuery model is not required.
 
 
</details>

### 6. The DAX query in the code block uses a variable to calculate a measure. What result is returned?

```dax
EVALUATE
VAR Total = [Sales Amount]
RETURN {Total}
```

- [ ] **A)** A single-row table containing the total sales amount
- [ ] **B)** Every row from the Sales table
- [ ] **C)** A syntax error because VAR is invalid
- [ ] **D)** A persistent measure named Total

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The VAR stores the Sales Amount measure, and the RETURN block returns a single-row table containing that value.
 
 
</details>


---

### **Implement and manage semantic models**

### 7. What is an enterprise semantic model in Microsoft Fabric and Power BI?

- [ ] **A)** A centrally managed metadata layer that provides consistent measures, relationships, and security
- [ ] **B)** A single Power BI report visual used by one team
- [ ] **C)** A OneLake folder that stores raw transaction files
- [ ] **D)** A Power Query transformation that cleans data for a single notebook

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An enterprise semantic model is a governed, shared metadata layer that centralizes measures, relationships, hierarchies, and security so reports consume consistent business logic.
 
 
</details>

### 8. Which storage modes are supported by semantic models in Microsoft Fabric?

- [ ] **A)** Import
- [ ] **B)** Direct Lake
- [ ] **C)** DirectQuery
- [ ] **D)** Live Query

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Fabric semantic models support Import, DirectQuery, and the Fabric-specific Direct Lake mode. Live Query is not a distinct storage mode.
 
 
</details>

### 9. Examine the DAX code in the code block. What kind of calculation does this measure perform?

```dax
Sales YTD = TOTALYTD([Total Sales], 'Date'[Date])
```

- [ ] **A)** Year-to-date total sales
- [ ] **B)** Same period last year sales
- [ ] **C)** Moving annual average
- [ ] **D)** Ranking of sales by region

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TOTALYTD calculates the year-to-date total of a measure and uses the date column in the model's date table.
 
 
</details>

### 10. Direct Lake reads data directly from which source?

- [ ] **A)** Delta-parquet tables in OneLake
- [ ] **B)** External SQL Server databases
- [ ] **C)** Azure Blob Storage containers
- [ ] **D)** SharePoint lists

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Direct Lake is Fabric-specific and reads delta-parquet files directly from OneLake without importing data or querying the source directly.
 
 
</details>

### 11. Which two security mechanisms can be configured directly in a Fabric semantic model?

- [ ] **A)** Row-level security (RLS)
- [ ] **B)** Object-level security (OLS)
- [ ] **C)** Transport Layer Security (TLS)
- [ ] **D)** Multi-factor authentication (MFA)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> RLS filters rows and OLS hides tables or columns. TLS and MFA are related to connectivity and identity, not model authorization.
 
 
</details>

### 12. The expression in the code block uses USERELATIONSHIP. What is its purpose inside the measure?

```dax
CALCULATE([Total Sales], USERELATIONSHIP('Orders'[ShipDate], 'Date'[Date]))
```

- [ ] **A)** It activates an inactive relationship for the duration of the calculation
- [ ] **B)** It creates a new physical relationship between tables
- [ ] **C)** It deletes an existing relationship from the model
- [ ] **D)** It changes the storage mode of the related tables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> USERELATIONSHIP temporarily activates an inactive relationship during a CALCULATE evaluation so a measure can use an alternate date or dimension relationship.
 
 
</details>

### 13. What does high cardinality mean in a semantic model column?

- [ ] **A)** It contains many distinct values
- [ ] **B)** It contains a large number of rows
- [ ] **C)** It is part of many measures
- [ ] **D)** It is connected to many source tables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cardinality refers to the number of distinct values in a column. High cardinality can increase dictionary size and reduce compression efficiency.
 
 
</details>


---

### **Plan, implement, and manage a solution for data analytics**

### 14. Which Microsoft Fabric workload is specifically designed to handle streaming and event-based data for low-latency analytics?

- [ ] **A)** Real-Time Intelligence
- [ ] **B)** Data Warehouse
- [ ] **C)** Data Engineering
- [ ] **D)** Data Factory

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Real-Time Intelligence uses KQL and is optimized for streaming, event data with sub-second latency. Data Engineering and Data Warehouse handle batch or high-concurrency relational workloads.
 
 
</details>

### 15. Which characteristics indicate that a Data Warehouse is the correct workload in Fabric? (Select all that apply.)

- [ ] **A)** SQL-first analytics and high-concurrency queries
- [ ] **B)** Curated, relational, read-optimized data
- [ ] **C)** Raw JSON, images, and unstructured logs
- [ ] **D)** T-SQL queries from end users

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Data Warehouse serves curated relational data to SQL consumers with high concurrency. Raw unstructured data belongs in a Lakehouse, not a Warehouse.
 
 
</details>

### 16. Review the query shown in the code block. Which query language is being used in the Fabric SQL analytics endpoint?

```sql
SELECT ProductID, SUM(Amount) AS TotalSales
FROM Sales
GROUP BY ProductID;
```

- [ ] **A)** T-SQL
- [ ] **B)** KQL
- [ ] **C)** DAX
- [ ] **D)** Spark SQL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The SELECT statement is standard T-SQL, which is the interface for Fabric Warehouse and SQL analytics endpoints.
 
 
</details>

### 17. Where is a Microsoft Fabric workspace placed when no specific domain is assigned during creation?

- [ ] **A)** In the default domain defined by the admin
- [ ] **B)** Outside all domains
- [ ] **C)** In a temporary unmanaged domain
- [ ] **D)** It remains unassigned until a domain admin approves

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Every workspace belongs to a domain; if none is specified, it is placed in the tenant's default domain.
 
 
</details>


---

### **Prepare and serve data**

### 18. Which component is the primary data movement engine inside a Microsoft Fabric pipeline?

- [ ] **A)** Copy Activity
- [ ] **B)** Dataflow Gen2
- [ ] **C)** Shortcut
- [ ] **D)** Notebook

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: **
 
> 💡  **Explanation** 
> 
> The Copy Activity is described as the foundation of data movement inside a Fabric pipeline.
 
 
</details>

### 19. Which of the following are supported external source types for OneLake shortcuts?

- [ ] **A)** Azure Data Lake Storage Gen2
- [ ] **B)** Amazon S3
- [ ] **C)** On-premises SQL Server
- [ ] **D)** Azure Blob Storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: **
 
> 💡  **Explanation** 
> 
> Fabric shortcuts support ADLS Gen2, Amazon S3, Google Cloud Storage, Dataverse, and other Fabric locations. They do not support on-premises SQL Server or Azure Blob Storage as direct shortcut targets.
 
 
</details>

### 20. What is the outcome when the notebook code below is executed?

```python
df = spark.read.table("Sales")
filtered = df.filter("Region = 'West'")
filtered.select("CustomerID", "Amount")
```

- [ ] **A)** No data is read or written because no action is invoked
- [ ] **B)** The first five rows of the DataFrame are displayed
- [ ] **C)** The filtered data is written to a table
- [ ] **D)** An error occurs because a transform cannot be chained

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: **
 
> 💡  **Explanation** 
> 
> PySpark transformations such as filter and select are lazy. An action is required before Spark reads or writes data.
 
 
</details>

### 21. Which file format is required for tables hosted in both Fabric lakehouses and warehouses?

- [ ] **A)** Delta Lake
- [ ] **B)** CSV
- [ ] **C)** JSON
- [ ] **D)** Avro

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: **
 
> 💡  **Explanation** 
> 
> Both lakehouses and warehouses in Fabric rely on OneLake and use Delta Lake as the mandatory table format.
 
 
</details>

### 22. Which statements accurately describe Dataflows Gen2 in Microsoft Fabric?

- [ ] **A)** They provide a low-code Power Query experience
- [ ] **B)** They are suitable for self-service data preparation
- [ ] **C)** They are ideal for orchestrating thousands of files at scale
- [ ] **D)** They support joins, custom columns, and filtering before load

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: **
 
> 💡  **Explanation** 
> 
> Dataflows Gen2 are low-code Power Query tools suited to self-service prep. They are not designed to replace the Copy Activity for heavy orchestrated movement.
 
 
</details>

### 23. What kind of operation is implemented by the SQL code shown below?

```sql
MERGE INTO gold.Orders AS t
USING silver.Orders AS s
ON t.OrderId = s.OrderId
WHEN MATCHED THEN UPDATE SET t.Amount = s.Amount
WHEN NOT MATCHED THEN INSERT (OrderId, Amount) VALUES (s.OrderId, s.Amount);
```

- [ ] **A)** Upsert or merge
- [ ] **B)** Full refresh
- [ ] **C)** Schema drift detection
- [ ] **D)** High-watermark query

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: **
 
> 💡  **Explanation** 
> 
> The code uses a MERGE statement to update matching rows and insert new rows, which is an upsert pattern.
 
 
</details>

### 24. What is the main purpose of the Bronze layer in a medallion architecture?

- [ ] **A)** Raw, unmodified source data
- [ ] **B)** Cleansed and conformed data
- [ ] **C)** Business-ready aggregates
- [ ] **D)** Final semantic model tables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: **
 
> 💡  **Explanation** 
> 
> The Bronze layer is the landing zone for raw, unmodified data and should preserve original source values.
 
 
</details>

### 25. Which practices help optimize Spark transformations in Fabric notebooks?

- [ ] **A)** Broadcasting a small dimension table
- [ ] **B)** Using coalesce() to reduce partitions without a full shuffle
- [ ] **C)** Filtering rows before performing a join
- [ ] **D)** Calling collect() to send all data to the driver before aggregation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: **
 
> 💡  **Explanation** 
> 
> Broadcast joins, coalesce, and early filtering reduce shuffle and data movement. collect() is risky and inefficient for large data.
 
 
</details>

### 26. Why is coalesce() the preferred choice in this write operation?

```python
df = spark.read.table("raw_events")
df = df.filter("OrderDate >= '2024-01-01'")
df.coalesce(4).write.mode("overwrite").format("delta").saveAsTable("silver_events")
```

- [ ] **A)** It reduces partition count without a full shuffle
- [ ] **B)** It increases the number of partitions for better parallelism
- [ ] **C)** It guarantees sorted file output
- [ ] **D)** It caches the DataFrame in memory before writing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: **
 
> 💡  **Explanation** 
> 
> coalesce() merges partitions on the same executors without a full shuffle, making it more efficient for reducing partition count.
 
 
</details>

### 27. What is a OneLake shortcut in Microsoft Fabric?

- [ ] **A)** A logical reference to external data without copying it
- [ ] **B)** A physical copy of data moved into the lakehouse
- [ ] **C)** A transformation layer that cleans external data
- [ ] **D)** A scheduled pipeline that loads data daily

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: **
 
> 💡  **Explanation** 
> 
> Shortcuts are virtual references to external data. They do not move or transform data.
 
 
</details>

### 28. Which statements about views in Fabric Warehouse are true?

- [ ] **A)** Views are virtual objects and store no data
- [ ] **B)** Views can hide sensitive columns and rows
- [ ] **C)** Views are materialized and can be indexed
- [ ] **D)** Views always reflect the current data in their base tables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: **
 
> 💡  **Explanation** 
> 
> Views are saved SELECT queries, do not store data, can enforce security, and reflect current base table data. They cannot be indexed like materialized views.
 
 
</details>

### 29. What type of object is created by the SQL statement below?

```sql
CREATE FUNCTION dbo.GetOrders(@CustomerID INT)
RETURNS TABLE
AS RETURN
SELECT OrderID, OrderDate, Amount
FROM Sales.Orders
WHERE CustomerID = @CustomerID;
```

- [ ] **A)** Inline table-valued function
- [ ] **B)** Stored procedure
- [ ] **C)** View
- [ ] **D)** Materialized view

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: **
 
> 💡  **Explanation** 
> 
> The code uses CREATE FUNCTION with RETURNS TABLE and a single RETURN SELECT statement, which defines an inline table-valued function.
 
 
</details>

### 30. Which statement about the Lakehouse SQL analytics endpoint is true?

- [ ] **A)** It is read-only and cannot run DML statements
- [ ] **B)** It supports INSERT, UPDATE, and DELETE operations
- [ ] **C)** It stores a separate copy of the data
- [ ] **D)** It requires a scheduled refresh to show new files

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: **
 
> 💡  **Explanation** 
> 
> The Lakehouse SQL analytics endpoint is read-only. Writes must be performed through Spark, Dataflows, or pipelines.
 
 
</details>

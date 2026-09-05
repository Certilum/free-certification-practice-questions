<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Microsoft%20Certified-%20Power%20BI%20Data%20Analyst%20Associate.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Microsoft Certified: Power BI Data Analyst Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Manage and secure Power BI](#manage-and-secure-power-bi) (4 questions)
- [Model the data](#model-the-data) (8 questions)
- [Prepare the data](#prepare-the-data) (9 questions)
- [Visualize and analyze the data](#visualize-and-analyze-the-data) (9 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:18.731Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Manage and secure Power BI | 4 |
| Model the data | 8 |
| Prepare the data | 9 |
| Visualize and analyze the data | 9 |

---

### **Manage and secure Power BI**

### 1. Which storage mode loads data into the Power BI in-memory engine to provide the fastest analytical performance?

- [ ] **A)** Import mode
- [ ] **B)** DirectQuery
- [ ] **C)** Composite Model
- [ ] **D)** Live Connection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Import mode copies data into the Power BI in-memory engine, maximizing query speed and DAX functionality, and needs scheduled refresh to remain current.
 
 
</details>

### 2. Which of the following are valid Power BI data source privacy levels? Select all that apply.

- [ ] **A)** Public
- [ ] **B)** Organizational
- [ ] **C)** Private
- [ ] **D)** Isolated

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Power BI privacy levels are Public, Organizational, and Private. They control how data sources can be combined to prevent unintended data leakage.
 
 
</details>

### 3. Review the Power Query M code in the code block. What is the result of the Unpivoted Columns step?

```m
let
    Source = Excel.Workbook(File.Contents("sales.xlsx"), null, true),
    Sales_Table = Source{[Item="Sales",Kind="Table"]}[Data],
    #"Changed Type" = Table.TransformColumnTypes(Sales_Table,{{"Product", type text}, {"Q1", type number}, {"Q2", type number}, {"Q3", type number}, {"Q4", type number}}),
    #"Unpivoted Columns" = Table.UnpivotOtherColumns(#"Changed Type", {"Product"}, "Quarter", "Sales"),
    #"Renamed Columns" = Table.RenameColumns(#"Unpivoted Columns", {{"Quarter", "Period"}})
in
    #"Renamed Columns"
```

- [ ] **A)** Converts quarter columns into an attribute-value pair of Quarter and Sales
- [ ] **B)** Converts rows into columns to improve readability
- [ ] **C)** Deletes the Product column from the table
- [ ] **D)** Joins the table horizontally with another table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Unpivoting creates a normalized table by turning multiple columns into attribute-value pairs, increasing row count and enabling easier analysis.
 
 
</details>

### 4. Which connection type is used specifically to connect to Analysis Services or Power BI datasets?

- [ ] **A)** Live Connection
- [ ] **B)** DirectQuery
- [ ] **C)** Import mode
- [ ] **D)** Composite Model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Live Connection targets Analysis Services or Power BI datasets. DirectQuery connects to relational databases by sending native queries.
 
 
</details>


---

### **Model the data**

### 5. Which storage mode loads data into the Power BI in-memory engine for the fastest analytical query performance?

- [ ] **A)** Import mode
- [ ] **B)** DirectQuery mode
- [ ] **C)** Live Connection mode
- [ ] **D)** Composite model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Import mode loads data into the VertiPaq in-memory engine, making it the most common mode for high-speed analytical queries.
 
 
</details>

### 6. Which options correctly characterize DirectQuery storage mode? Select all that apply.

- [ ] **A)** Leaves data in source system
- [ ] **B)** Sends real-time queries to source
- [ ] **C)** Loads columns into VertiPaq memory
- [ ] **D)** Works only in Power Query Desktop

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DirectQuery leaves data in the source system and sends real-time queries to the source. It does not load data into memory and is not limited to Power Query Desktop.
 
 
</details>

### 7. Review the M code in the block. What action does this applied step perform in Power Query?

```m
= Table.UnpivotOtherColumns(#"Changed Type", {"Country"}, "Attribute", "Value")
```

- [ ] **A)** Converts wide columns into rows
- [ ] **B)** Stacks queries vertically
- [ ] **C)** Joins tables horizontally
- [ ] **D)** Renames selected columns

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Table.UnpivotOtherColumns function unpivots specified columns, converting wide attribute columns into additional rows and forming a long, normalized table.
 
 
</details>

### 8. Which privacy level should be selected for a sensitive source that must not be mixed with other data sources?

- [ ] **A)** Private privacy level
- [ ] **B)** Public privacy level
- [ ] **C)** Organizational privacy level
- [ ] **D)** No privacy level

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Private is the most restrictive privacy level and can help prevent data leakage across data sources during merging and query folding.
 
 
</details>

### 9. Which categories are displayed by Column Quality in Power Query? Select all that apply.

- [ ] **A)** Valid value percentage
- [ ] **B)** Error value percentage
- [ ] **C)** Empty value percentage
- [ ] **D)** Unique value percentage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Column Quality displays the percentage of Valid, Error, and Empty values in each column. Unique is not one of the categories shown by Column Quality.
 
 
</details>

### 10. Examine the M code in the code block. Which statements are correct about this transformation? Select all that apply.

```m
= Table.Combine({#"Orders 2023", #"Orders 2024"})
```

- [ ] **A)** Stacks rows vertically
- [ ] **B)** Keeps duplicate rows
- [ ] **C)** Joins tables horizontally
- [ ] **D)** Removes duplicate rows

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Table.Combine appends tables vertically, preserving duplicates in the result. It does not perform a horizontal join and does not eliminate duplicate rows.
 
 
</details>

### 11. What kind of data source is DirectQuery intended for in contrast to Live Connection?

- [ ] **A)** Relational databases
- [ ] **B)** Power BI datasets
- [ ] **C)** Analysis Services models
- [ ] **D)** Excel workbooks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> DirectQuery is intended for relational databases, while Live Connection is specifically for Analysis Services models or Power BI datasets. They are not identical.
 
 
</details>

### 12. Which statements are correct about data refresh requirements? Select all that apply.

- [ ] **A)** Requires gateway for on-premises refresh
- [ ] **B)** Cloud-to-cloud refresh needs no gateway
- [ ] **C)** Gateway is needed for every refresh
- [ ] **D)** Gateway is never used for DirectQuery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> An On-premises Data Gateway is required when the source is on-premises, but cloud-to-cloud refresh generally needs no gateway. DirectQuery can also require a gateway for on-premises sources.
 
 
</details>


---

### **Prepare the data**

### 13. What is the most common Power BI storage mode used to load data into the in-memory engine?

- [ ] **A)** Import Mode
- [ ] **B)** DirectQuery
- [ ] **C)** Live Connection
- [ ] **D)** Composite Model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Import Mode is the most common storage mode because it loads data into the Power BI in-memory engine, VertiPaq, for high-speed querying.
 
 
</details>

### 14. Which statements accurately describe DirectQuery in Power BI?

- [ ] **A)** It leaves the data in the source system.
- [ ] **B)** It sends queries to the source in real time.
- [ ] **C)** It loads the full data set into VertiPaq.
- [ ] **D)** It is the same as a Live Connection.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DirectQuery leaves source data in place and sends real-time queries to the source, so it is not imported into VertiPaq and should not be confused with Live Connection.
 
 
</details>

### 15. Review the code in the code block. Which applied step is executed last in this Power Query M query?

```powerquery
let
    Source = Sql.Database("Server01", "AdventureWorks"),
    Sales = Source{[Schema="Sales", Item="Orders"]}[Data],
    #"Changed Type" = Table.TransformColumnTypes(Sales, {{"OrderDate", type date}, {"Amount", type number}}),
    #"Filtered Rows" = Table.SelectRows(#"Changed Type", each [Amount] > 1000)
in
    #"Filtered Rows"
```

- [ ] **A)** Source
- [ ] **B)** Changed Type
- [ ] **C)** Filtered Rows
- [ ] **D)** SelectRows

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The M query starts with Source, then changes data types, and finally filters rows. Filtered Rows is therefore the last applied step.
 
 
</details>

### 16. Why is it critical to select the correct built-in connector when importing data into Power BI?

- [ ] **A)** It determines metadata availability and transformation methods.
- [ ] **B)** It determines the visual layout of reports.
- [ ] **C)** It decides which DAX functions are available.
- [ ] **D)** It removes the need to profile data.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The selected connector determines the level of metadata available and the methods available for subsequent data transformation in Power Query.
 
 
</details>

### 17. Which two elements must be configured when Power BI analyzes how a data source is accessed?

- [ ] **A)** Authentication method, such as OAuth2 or Windows
- [ ] **B)** Privacy level, such as Public or Organizational
- [ ] **C)** Applied Step sequence
- [ ] **D)** In-memory engine size

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Connecting to a data source requires configuring authentication methods such as OAuth2 or Windows, and privacy levels such as Public or Organizational.
 
 
</details>

### 18. What transformation does the code in the code block apply to the source table?

```powerquery
let
    Source = Excel.CurrentWorkbook(){[Name="Sales"]}[Content],
    #"Unpivoted Other Columns" = Table.UnpivotOtherColumns(Source, {"Country"}, "Attribute", "Value")
in
    #"Unpivoted Other Columns"
```

- [ ] **A)** It merges two tables horizontally.
- [ ] **B)** It appends two tables vertically.
- [ ] **C)** It unpivots columns into attribute-value pairs.
- [ ] **D)** It duplicates the source table.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The M code uses Table.UnpivotOtherColumns, which converts wide columns into attribute-value pairs, a critical structural transformation.
 
 
</details>

### 19. How does a Live Connection differ from DirectQuery in Power BI?

- [ ] **A)** It is used specifically for Analysis Services or Power BI datasets.
- [ ] **B)** It always imports data into VertiPaq.
- [ ] **C)** It connects directly to relational databases.
- [ ] **D)** It mixes DirectQuery and Import in one model.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Live Connection is specifically for Analysis Services or Power BI datasets, while DirectQuery is for relational databases.
 
 
</details>

### 20. Which two statements are true when refreshing an on-premises data source in Power BI?

- [ ] **A)** An On-premises Data Gateway is required for scheduled refreshes.
- [ ] **B)** On-premises source credentials are managed with the data source, not the gateway.
- [ ] **C)** Every connection in Power BI requires a gateway even if the source is in the cloud.
- [ ] **D)** Personal gateway mode is ideal for departmental shared report refreshes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> An On-premises Data Gateway is non-negotiable for scheduled refresh of on-premises data, and source credentials belong with the data source, not the gateway.
 
 
</details>

### 21. What operation is performed by the Power Query code in the code block?

```powerquery
let
    Source = Sql.Database("Server01", "Data Warehouse"),
    dbo_Products = Source{[Schema="dbo", Item="Products"]}[Data],
    dbo_Sales = Source{[Schema="dbo", Item="Sales"]}[Data],
    #"Merged Queries" = Table.NestedJoin(dbo_Sales, {"ProductID"}, dbo_Products, {"ProductID"}, "Products", JoinKind.LeftOuter)
in
    #"Merged Queries"
```

- [ ] **A)** It merges queries horizontally on a common key.
- [ ] **B)** It appends queries vertically.
- [ ] **C)** It unpivots selected columns.
- [ ] **D)** It replaces null values.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code uses Table.NestedJoin, which merges two tables horizontally based on a common ProductID key, similar to a SQL Join.
 
 
</details>


---

### **Visualize and analyze the data**

### 22. Which storage mode loads data into the Power BI in-memory engine and requires scheduled refreshes to stay current?

- [ ] **A)** Import mode
- [ ] **B)** DirectQuery
- [ ] **C)** Live Connection
- [ ] **D)** Composite Model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Import mode copies data into VertiPaq, Power BI's in-memory engine. It enables fast queries and full DAX usage but requires scheduled refreshes to keep information current.
 
 
</details>

### 23. Which of the following accurately describe DirectQuery storage mode? Select all that apply.

- [ ] **A)** Data stays in the original source system.
- [ ] **B)** Queries are sent to the source system in real time.
- [ ] **C)** Data is compressed and loaded into VertiPaq.
- [ ] **D)** DirectQuery removes all query load from the source system.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DirectQuery does not import data. It leaves data in the source system and sends native queries to it for real-time access, which can add latency and does not reduce source workload.
 
 
</details>

### 24. Refer to the code block. What transformation is performed on the source table?

```m
let
    Source = #table(type table [Country = text, "2020" = text, "2021" = text], {
        {"USA", "100", "150"},
        {"UK", "80", "120"}
    }),
    #"Unpivoted Other Columns" = Table.UnpivotOtherColumns(Source, {"Country"}, "Year", "Sales")
in
    #"Unpivoted Other Columns"
```

- [ ] **A)** Turns wide columns into attribute-value rows
- [ ] **B)** Adds rows from another table
- [ ] **C)** Combines tables using a key column
- [ ] **D)** Changes column data types

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Unpivoting transforms wide tables with values spread across multiple columns into a normalized long format with attribute and value columns.
 
 
</details>

### 25. Which Power Query profiling tool visually reports the Valid, Error, and Empty percentages of each column?

- [ ] **A)** Column Quality
- [ ] **B)** Column Distribution
- [ ] **C)** Column Profile
- [ ] **D)** Value Distribution

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Column Quality provides a high-level visual summary of each column, showing the percentage of values that are Valid, Error, or Empty.
 
 
</details>

### 26. Which options are valid privacy levels in Power BI? Select all that apply.

- [ ] **A)** Public
- [ ] **B)** Organizational
- [ ] **C)** Private
- [ ] **D)** Shared

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Power BI privacy levels are Public, Organizational, and Private. Shared is not a valid data privacy level.
 
 
</details>

### 27. Refer to the code block. What operation is performed after the Orders and Details tables are created?

```m
let
    Orders = Table.FromRows(
        {
            {1, "Active"},
            {2, "Closed"}
        },
        type table [OrderID = number, Status = text]
    ),
    Details = Table.FromRows(
        {
            {1, "A"},
            {1, "B"}
        },
        type table [OrderID = number, Detail = text]
    ),
    MergedQueries = Table.NestedJoin(Orders, {"OrderID"}, Details, {"OrderID"}, "Details", JoinKind.LeftOuter),
    FilteredRows = Table.SelectRows(MergedQueries, each [Status] = "Active")
in
    FilteredRows
```

- [ ] **A)** A horizontal merge based on OrderID
- [ ] **B)** A vertical append
- [ ] **C)** A column unpivot
- [ ] **D)** A row-level filter

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Table.NestedJoin joins tables horizontally using a common key, similar to a SQL JOIN. In this example the key is OrderID.
 
 
</details>

### 28. Which Power Query tool provides Min, Max, Average, Standard Deviation, and row count for a selected column?

- [ ] **A)** Column Profile
- [ ] **B)** Column Quality
- [ ] **C)** Column Distribution
- [ ] **D)** Value Distribution

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Column Profile is a deep-dive tool that shows statistics such as Min, Max, Average, Standard Deviation, and Count for a column.
 
 
</details>

### 29. In which scenarios is DirectQuery an appropriate choice? Select all that apply.

- [ ] **A)** Dataset is larger than the available memory
- [ ] **B)** Near-real-time data is required
- [ ] **C)** Full DAX capability with no limitations is required
- [ ] **D)** Source database workload should be minimized

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DirectQuery handles very large data sets and near-real-time updates. However, it can introduce latency, place load on the source system, and limit certain DAX features.
 
 
</details>

### 30. Refer to the code block. The filter removes empty string values. Which missing-value problem remains?

```m
let
    Source = Table.FromRows(
        {
            {"1", "North"},
            {"2", ""},
            {"3", null},
            {"4", "South"}
        },
        type table [CustomerID = text, Region = text]
    ),
    #"Filtered Rows" = Table.SelectRows(Source, each [Region] <> "")
in
    #"Filtered Rows"
```

- [ ] **A)** Rows with null Region values remain
- [ ] **B)** Rows with empty string Region values remain
- [ ] **C)** Rows with duplicate CustomerID remain
- [ ] **D)** All rows with missing Region are removed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In Power Query M, null is not equal to an empty string. The filter [Region] <> \"\" removes empty strings but leaves null values in the result.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Microsoft%20Certified-%20Power%20Platform%20Functional%20Consultant%20Associate.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Microsoft Certified: Power Platform Functional Consultant Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Analyze data](#analyze-data) (4 questions)
- [Build Power Apps](#build-power-apps) (9 questions)
- [Build Power Automate](#build-power-automate) (5 questions)
- [Configure the data model](#configure-the-data-model) (5 questions)
- [Create a Power Platform solution](#create-a-power-platform-solution) (5 questions)
- [Implement Power Virtual Agents chatbots](#implement-power-virtual-agents-chatbots) (2 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:23.833Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Analyze data | 4 |
| Build Power Apps | 9 |
| Build Power Automate | 5 |
| Configure the data model | 5 |
| Create a Power Platform solution | 5 |
| Implement Power Virtual Agents chatbots | 2 |

---

### **Analyze data**

### 1. When you need to display a metric over a continuous period of time, which chart type is the most appropriate to select?

- [ ] **A)** Line chart
- [ ] **B)** Bar chart
- [ ] **C)** Pie chart
- [ ] **D)** Scatter plot

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Line charts are used for temporal trends, while bar charts are better for categorical comparisons.
 
 
</details>

### 2. Which two statements correctly describe the difference between standard and premium connectors in the Power Platform?

- [ ] **A)** SharePoint and OneDrive are included with standard licensing.
- [ ] **B)** SQL Server and HTTP require premium licensing.
- [ ] **C)** All connectors are included with standard licensing.
- [ ] **D)** Premium connectors are included with basic Power Platform licensing.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Standard connectors, such as SharePoint and OneDrive, are included with basic licensing; premium connectors, such as SQL Server and HTTP, require additional licensing.
 
 
</details>

### 3. The Power Query expression in the code block is used in a dataflow. Which type of data source is it referencing?

```powerquery
let
    Source = Sql.Database("localhost", "AdventureWorks"),
    Data = Source{[Schema="dbo", Item="Customers"]}[Data]
in
    Data
```

- [ ] **A)** On-premises SQL Server
- [ ] **B)** SharePoint Online
- [ ] **C)** Dataverse
- [ ] **D)** REST API

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Sql.Database function targets SQL Server. For an on-premises SQL Server, an On-premises Data Gateway is required to make it available to cloud services.
 
 
</details>

### 4. A report is being designed to compare many product categories. Which chart type should be avoided in this scenario?

- [ ] **A)** Pie chart
- [ ] **B)** Line chart
- [ ] **C)** Bar chart
- [ ] **D)** Scatter plot

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Pie Chart Pitfall states that a pie chart with too many categories obscures the ability to compare relative values effectively.
 
 
</details>


---

### **Build Power Apps**

### 5. In Power BI, which visual type is most appropriate for showing a trend over time?

- [ ] **A)** Line chart
- [ ] **B)** Pie chart
- [ ] **C)** Bar chart
- [ ] **D)** Scatter chart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Line charts are recommended for temporal trends; bar charts are for categorical comparisons. Pie charts show parts of a whole and can obscure comparisons.
 
 
</details>

### 6. Which of the following are standard connectors that are included with basic Power Platform licensing?

- [ ] **A)** SharePoint
- [ ] **B)** OneDrive
- [ ] **C)** SQL Server
- [ ] **D)** Azure DevOps

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SharePoint and OneDrive are standard connectors. SQL Server and Azure DevOps are premium connectors and require additional Power Platform licensing.
 
 
</details>

### 7. The code block configures a visual with order date and sales amount. Which business question is this visual best suited to answer?

```json
{
  "visual": "line",
  "x": "OrderDate",
  "y": "SalesAmount"
}
```

- [ ] **A)** How sales change over time
- [ ] **B)** How sales compare across product categories
- [ ] **C)** What proportion of total sales each product represents
- [ ] **D)** Whether two numeric variables are correlated

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A line chart with a date field and a measure is ideal for analyzing changes over time, not categorical comparison or proportion.
 
 
</details>

### 8. What is the primary difference between a Power BI dashboard and a detailed report in the Power BI Service?

- [ ] **A)** Dashboard is single-page; report is multi-page
- [ ] **B)** Report is single-page; dashboard is multi-page
- [ ] **C)** Dashboards are for raw data entry
- [ ] **D)** Terms are interchangeable

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A report provides detailed multi-page views of data. A dashboard is a single-page, high-level overview used for monitoring critical metrics.
 
 
</details>

### 9. Which actions support effective visual hierarchy and layout on a Power Apps canvas?

- [ ] **A)** Use size and color for KPIs
- [ ] **B)** Place secondary data above KPIs
- [ ] **C)** Position KPIs prominently
- [ ] **D)** Avoid overloading the canvas

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Visual hierarchy uses size, color, and position to emphasize KPIs and reduce cognitive overload. Secondary data should not outrank primary KPIs.
 
 
</details>

### 10. The code block describes a connection to a data source located behind a corporate firewall. Which component provides the secure bridge?

```json
{
  "dataSource": "OnPremises SQL Server",
  "connection": "Secure Bridge"
}
```

- [ ] **A)** On-premises Data Gateway
- [ ] **B)** Dataverse Virtual Table
- [ ] **C)** Custom Connector
- [ ] **D)** Dataflow

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The On-premises Data Gateway works as a secure bridge between cloud services and on-premises data, avoiding the need for complex VPN configurations.
 
 
</details>

### 11. What does the Dataverse Virtual Tables feature allow you to do with data stored in external sources?

- [ ] **A)** Surface external data without moving it
- [ ] **B)** Copy external data into Dataverse
- [ ] **C)** Transform data using Power Query Online
- [ ] **D)** Create custom REST API connectors

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Virtual Tables surface external data within Dataverse without copying or moving the data, reducing duplication and storage costs.
 
 
</details>

### 12. Which two statements describe common traps when making Power Platform architecture choices?

- [ ] **A)** Selecting Dataflows to avoid data duplication
- [ ] **B)** Overlooking On-premises Data Gateway requirement
- [ ] **C)** Using line charts for temporal trends
- [ ] **D)** Using Model-driven dashboards for operational views

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Common traps include using Dataflows when duplication is a concern and overlooking the Data Gateway for on-premises sources. Line charts and model-driven dashboards are appropriate in their contexts.
 
 
</details>

### 13. The code block describes an API endpoint that has no pre-built connector. What should be created to use this endpoint?

```json
{
  "endpoint": "https://api.example.com/v1/orders",
  "authentication": "OAuth2"
}
```

- [ ] **A)** Custom Connector
- [ ] **B)** Dataflow
- [ ] **C)** On-premises Data Gateway
- [ ] **D)** Dataverse Virtual Table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Custom Connectors are designed when no pre-built connector exists for a REST API. They require understanding authentication methods like OAuth 2.0 and endpoint structure.
 
 
</details>


---

### **Build Power Automate**

### 14. Which chart type is best for showing temporal trends?

- [ ] **A)** Line chart
- [ ] **B)** Bar chart
- [ ] **C)** Pie chart
- [ ] **D)** Scatter chart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Line charts are ideal for temporal trends because they emphasize changes over a continuous time interval. Use bar charts for categorical comparisons.
 
 
</details>

### 15. Which of the following connectors are classified as Standard connectors included with basic Power Platform licensing?

- [ ] **A)** SharePoint
- [ ] **B)** OneDrive
- [ ] **C)** SQL Server
- [ ] **D)** HTTP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SharePoint and OneDrive are Standard connectors included with basic licensing. SQL Server and HTTP are Premium connectors that require additional licensing.
 
 
</details>

### 16. You are reviewing a Power Automate flow. Review the connector name in the trigger shown in the code block. What is true about this connector?

```json
{"triggers":{"When_an_item_is_created":{"inputs":{"host":{"connectionName":"shared_sql"}}}}}
```

- [ ] **A)** It requires a Premium license
- [ ] **B)** It is included with basic licensing
- [ ] **C)** It is a custom connector
- [ ] **D)** It uses Dataverse Virtual Tables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> shared_sql indicates SQL Server, a Premium connector. Using it without the appropriate license can cause unexpected costs.
 
 
</details>

### 17. What is the primary distinction between a dashboard and a report in Power BI?

- [ ] **A)** Dashboard is a single-page high-level overview
- [ ] **B)** Dashboard contains detailed multi-page data
- [ ] **C)** Report is a single-page overview
- [ ] **D)** Report is limited to real-time task lists

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A report is a detailed multi-page view, while a dashboard is a single-page high-level overview used for monitoring critical metrics.
 
 
</details>

### 18. Which statements about Dataverse Virtual Tables are correct?

- [ ] **A)** They surface external data without copying it
- [ ] **B)** They provide a unified view across sources
- [ ] **C)** They reduce duplication and storage costs
- [ ] **D)** They perform ETL using Power Query Online

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Virtual Tables create a window to external data without physical movement, reducing duplication. Dataflows, not virtual tables, use Power Query Online for ETL.
 
 
</details>


---

### **Configure the data model**

### 19. Which chart type is most appropriate for showing a sales trend over a twelve-month period?

- [ ] **A)** Bar chart
- [ ] **B)** Line chart
- [ ] **C)** Pie chart
- [ ] **D)** Scatter chart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Line charts are designed to show temporal trends, making them the correct choice for time-series data such as a 12-month sales trend.
 
 
</details>

### 20. Which two statements accurately describe standard vs premium connectors? Choose two.

- [ ] **A)** Standard connectors such as SharePoint and OneDrive are included with basic Power Platform licensing.
- [ ] **B)** Premium connectors such as SQL Server and HTTP require additional licensing.
- [ ] **C)** Standard connectors include SQL Server and HTTP with no additional cost.
- [ ] **D)** All connectors are free when used inside Dataverse Virtual Tables.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Standard connectors are included with basic Power Platform licensing, while Premium connectors such as SQL Server, HTTP, and Azure DevOps require additional licensing.
 
 
</details>

### 21. Review the JSON definition. Based on the actions listed, which Power Platform component is being configured to move and transform data into Dataverse?

```json
{
  "name": "CustomerETL",
  "source": "SQL Server",
  "destination": "Dataverse",
  "actions": ["Extract", "Transform", "Load"]
}
```

- [ ] **A)** Dataflow
- [ ] **B)** Virtual Table
- [ ] **C)** Custom Connector
- [ ] **D)** On-premises Data Gateway

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Dataflows use Power Query Online to extract, transform, and load data into Dataverse, matching the ETL actions shown in the definition.
 
 
</details>

### 22. Which feature allows you to access and query data from an external SQL Server directly inside Dataverse without moving or duplicating the data?

- [ ] **A)** Dataverse Virtual Table
- [ ] **B)** Dataflow
- [ ] **C)** Custom Connector
- [ ] **D)** On-premises Data Gateway

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Dataverse Virtual Tables surface external data within Dataverse without physically copying it, reducing duplication and storage costs.
 
 
</details>

### 23. Which two options describe common traps when building Power Platform data integration solutions? Choose two.

- [ ] **A)** Selecting Dataflows when the requirement is to avoid data duplication.
- [ ] **B)** Assuming a cloud service can access a local SQL Server without an On-premises Data Gateway.
- [ ] **C)** Using Virtual Tables to reduce storage costs by avoiding data copies.
- [ ] **D)** Choosing Power BI for advanced analytical reporting.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Dataflows physically copy data, so they should not be used when the goal is to avoid duplication. Also, cloud services cannot natively access on-premises SQL Server without the Data Gateway.
 
 
</details>


---

### **Create a Power Platform solution**

### 24. Which chart type should be used to display data that changes over a continuous period of time?

- [ ] **A)** Line chart
- [ ] **B)** Bar chart
- [ ] **C)** Pie chart
- [ ] **D)** Scatter chart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Line charts are best for showing trends over time; bar charts are better for categorical comparisons.
 
 
</details>

### 25. According to the playbook, which two statements correctly describe a dashboard as defined in Power Platform concepts?

- [ ] **A)** Single-page high-level overview
- [ ] **B)** Used for monitoring critical metrics
- [ ] **C)** Detailed multi-page view of data
- [ ] **D)** Designed for deep-dive analysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A dashboard is a single-page high-level overview for monitoring key metrics; reports provide detailed multi-page views.
 
 
</details>

### 26. A consultant is creating a custom connector for a REST API. Review the authentication configuration in the code block. Which authentication type is being used?

```json
{
  "authentication": {
    "type": "oauth2",
    "authorizationUrl": "https://login.microsoftonline.com/common/oauth2/v2.0/authorize",
    "tokenUrl": "https://login.microsoftonline.com/common/oauth2/v2.0/token",
    "scopes": ["https://api.example.com/.default"]
  }
}
```

- [ ] **A)** OAuth 2.0
- [ ] **B)** API Key
- [ ] **C)** Basic Authentication
- [ ] **D)** Anonymous

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block shows an OAuth 2.0 configuration with authorization and token URLs, commonly used for secured REST APIs.
 
 
</details>

### 27. What is the primary role of the On-premises Data Gateway in a Power Platform solution?

- [ ] **A)** Secure bridge between cloud and on-premises data
- [ ] **B)** Physically migrates data to Dataverse
- [ ] **C)** Replaces VPN in all cases
- [ ] **D)** Only works for SharePoint data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The On-premises Data Gateway securely connects cloud-based Power Platform services to local data without complex VPN setups.
 
 
</details>

### 28. According to the playbook, which two statements correctly describe Dataverse Virtual Tables and their behavior?

- [ ] **A)** Surfaces external data without moving it
- [ ] **B)** Reduces duplication and storage costs
- [ ] **C)** Physically copies external data into Dataverse
- [ ] **D)** Requires gateway for all external sources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Virtual tables provide a unified view of external data without physical copy, reducing duplication and storage costs.
 
 
</details>


---

### **Implement Power Virtual Agents chatbots**

### 29. Which chart type best displays data changes over time?

- [ ] **A)** Line chart
- [ ] **B)** Bar chart
- [ ] **C)** Pie chart
- [ ] **D)** Scatter chart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Line charts are best for temporal trends; bar charts compare categories, and pie charts show parts of a whole.
 
 
</details>

### 30. Which of the following are known traps to avoid with data integration and connectors? (Select all that apply.)

- [ ] **A)** Selecting Dataflows to avoid data duplication
- [ ] **B)** Assuming cloud services can natively access on-premises SQL
- [ ] **C)** Confusing Custom Connectors with Dataflows
- [ ] **D)** Using line charts for temporal trends

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Dataflows physically copy data; on-premises data needs a gateway; Custom Connectors are for APIs, not data movement.
 
 
</details>

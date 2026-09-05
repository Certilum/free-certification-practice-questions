<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Snowflake/SnowPro%20Advanced-%20Data%20Analyst.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>SnowPro Advanced: Data Analyst</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Data Analysis](#data-analysis) (10 questions)
- [Data Ingestion and Data Preparation](#data-ingestion-and-data-preparation) (5 questions)
- [Data Presentation and Data Visualization](#data-presentation-and-data-visualization) (8 questions)
- [Data Transformation and Data Modeling](#data-transformation-and-data-modeling) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:48:10.858Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Data Analysis | 10 |
| Data Ingestion and Data Preparation | 5 |
| Data Presentation and Data Visualization | 8 |
| Data Transformation and Data Modeling | 7 |

---

### **Data Analysis**

### 1. How do aggregate functions differ from window statistical functions in Snowflake?

- [ ] **A)** Aggregate functions collapse multiple rows into a single summary row, while window functions retain the original row identity.
- [ ] **B)** Window functions collapse multiple rows into a single summary row, while aggregate functions retain the original row identity.
- [ ] **C)** Both return exactly one row for each input group and hide row-level details.
- [ ] **D)** Both preserve every input row exactly as it appears in the source table.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Aggregate functions such as AVG reduce rows to one summary row. Window functions compute across rows related to the current row and preserve granularity.
 
 
</details>

### 2. Which of the following are descriptive statistics that quantify central tendency and dispersion? Select all that apply.

- [ ] **A)** Mean
- [ ] **B)** Median
- [ ] **C)** Variance
- [ ] **D)** Clustering depth

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Mean and median describe central tendency, while variance measures dispersion. Clustering depth is a performance and optimization metric, not a descriptive statistic.
 
 
</details>

### 3. The SQL statement in the code block calculates a percentile. What kind of result does it return?

```sql
SELECT PERCENTILE_CONT(0.5) WITHIN GROUP (ORDER BY amount) AS median_estimate
FROM orders;
```

- [ ] **A)** A continuously interpolated value that may not be an actual value in the dataset.
- [ ] **B)** A discrete value guaranteed to exist in the dataset.
- [ ] **C)** The row number of the median record.
- [ ] **D)** A boolean value that states whether interpolation was required.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PERCENTILE_CONT returns a continuous or interpolated percentile value, which may not exist as an actual row value. PERCENTILE_DISC is used when an actual existing value is required.
 
 
</details>

### 4. What is returned by the CORR function in Snowflake?

- [ ] **A)** The correlation coefficient between two numeric variables.
- [ ] **B)** The covariance of two numeric variables.
- [ ] **C)** The variance of one numeric variable.
- [ ] **D)** The median of two numeric variables.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CORR returns the correlation coefficient, which measures the strength and direction of the linear relationship between two numeric variables.
 
 
</details>

### 5. When should an analyst choose VAR_SAMP instead of VAR_POP? Select all that apply.

- [ ] **A)** When the data is a random sample of a larger population.
- [ ] **B)** When the data contains every member of the entire population.
- [ ] **C)** When the goal is to compute an unbiased estimate of the population variance.
- [ ] **D)** When the exact variance of the collected population is required.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> VAR_SAMP is used for sample data and produces an unbiased estimate of the population variance. VAR_POP is used when the dataset represents the entire population.
 
 
</details>

### 6. The code block uses RANK() as a window function. How are tied sales values handled?

```sql
SELECT product, sales,
       RANK() OVER (ORDER BY sales DESC) AS sales_rank
FROM products;
```

- [ ] **A)** Tied rows receive the same rank, and the next rank contains a gap.
- [ ] **B)** Tied rows receive the same rank, and the next rank has no gap.
- [ ] **C)** Each tied row receives a unique sequential row number.
- [ ] **D)** Tied rows are skipped and do not receive a rank.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RANK() assigns the same rank to tied rows and leaves gaps in the following rank values. DENSE_RANK() would not leave gaps.
 
 
</details>

### 7. What is the main purpose of micro-partition pruning in Snowflake?

- [ ] **A)** To skip reading irrelevant micro-partitions using selective filters on well-chosen columns.
- [ ] **B)** To merge all micro-partitions into one large partition after every query.
- [ ] **C)** To create materialized views automatically for all tables.
- [ ] **D)** To increase warehouse size before running a query.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Micro-partition pruning allows the Cloud Services layer to skip unnecessary partitions when queries use highly selective filters on columns with good cardinality or clustering.
 
 
</details>

### 8. Which conditions suggest that a Clustering Key might be beneficial for a large Snowflake table? Select all that apply.

- [ ] **A)** The table has a high clustering depth.
- [ ] **B)** Frequent queries filter or join on a column with poor data distribution.
- [ ] **C)** The table's data distribution has become poor over time.
- [ ] **D)** The table is only used for long-term archival and is rarely queried.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Clustering keys are useful when large tables have high clustering depth, poor data distribution, or frequent queries on specific filter or join columns.
 
 
</details>

### 9. The query in the code block performs a highly selective point lookup on a massive orders table. Which Snowflake feature is designed to optimize this pattern?

```sql
SELECT * FROM orders WHERE order_id = 12345;
```

- [ ] **A)** Search Optimization Service
- [ ] **B)** Clustering Key
- [ ] **C)** Materialized View
- [ ] **D)** Larger warehouse

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Search Optimization Service accelerates highly selective and non-contiguous point lookups, while clustering is better suited for range scans.
 
 
</details>

### 10. What does data spilling to local or remote disk indicate in a Query Profile?

- [ ] **A)** Intermediate query results exceeded the available memory and were written to disk.
- [ ] **B)** The query did not use any micro-partitions.
- [ ] **C)** The query result was too large to return to the user.
- [ ] **D)** The table is not compressed.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Data spilling occurs when intermediate results exceed the memory available to the warehouse. It can be caused by insufficient warehouse size or poorly written SQL.
 
 
</details>


---

### **Data Ingestion and Data Preparation**

### 11. What is the primary result of using an aggregate function such as AVG or STDDEV in a query?

- [ ] **A)** It collapses multiple rows into a single summary row.
- [ ] **B)** It preserves the original row identity and granularity.
- [ ] **C)** It adds a new column to every row without reducing row count.
- [ ] **D)** It sorts all rows by the computed value.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Aggregate functions summarize many rows into one result. Window functions, by contrast, preserve row-level detail.
 
 
</details>

### 12. Which statements about sample-based and population-based variance functions are correct?

- [ ] **A)** VAR_POP should be used when analyzing a complete population.
- [ ] **B)** VAR_SAMP should be used when the dataset is a sample.
- [ ] **C)** VAR_SAMP always returns a smaller value than VAR_POP.
- [ ] **D)** VAR_POP and VAR_SAMP are interchangeable.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Use VAR_SAMP for sample data and VAR_POP for complete populations. Choosing the wrong variant can lead to biased statistical inference.
 
 
</details>

### 13. Examine the SQL query in the code block. What does the output reveal about the table being profiled?

```sql
SELECT COUNT(*) AS total_rows,
       COUNT(score) AS non_null_scores,
       AVG(score) AS avg_score
FROM survey_responses;
```

- [ ] **A)** COUNT(column) returns the number of rows where that column is not NULL.
- [ ] **B)** COUNT(*) returns the number of rows where the column is not NULL.
- [ ] **C)** AVG(column) treats NULL values as zero.
- [ ] **D)** COUNT(column) returns the same result as COUNT(*) regardless of NULLs.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> COUNT(*) counts all rows, while COUNT(column) ignores NULLs. AVG also ignores NULLs and does not treat them as zero.
 
 
</details>

### 14. Which function should an analyst use to return a percentile value that actually exists in the dataset?

- [ ] **A)** PERCENTILE_DISC
- [ ] **B)** PERCENTILE_CONT
- [ ] **C)** CUME_DIST
- [ ] **D)** PERCENT_RANK

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PERCENTILE_DISC returns a non-interpolated value from the input set, while PERCENTILE_CONT returns an interpolated value.
 
 
</details>

### 15. Which Snowflake functions can be used to measure the strength and direction of a linear relationship between two numeric variables?

- [ ] **A)** CORR
- [ ] **B)** COVAR_POP
- [ ] **C)** COVAR_SAMP
- [ ] **D)** STDDEV

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> CORR returns the correlation coefficient, and COVAR_POP/COVAR_SAMP measure covariance. STDDEV measures the spread of one variable.
 
 
</details>


---

### **Data Presentation and Data Visualization**

### 16. Which type of function collapses multiple input rows into a single summary result?

- [ ] **A)** Aggregate function
- [ ] **B)** Window function
- [ ] **C)** Ranking function
- [ ] **D)** Scaling function

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Aggregate functions like AVG and STDDEV collapse multiple rows into a single summary row, unlike window functions which preserve row identity.
 
 
</details>

### 17. Which statements about using VAR_POP versus VAR_SAMP are correct?

- [ ] **A)** Use VAR_SAMP when the data represents a sample.
- [ ] **B)** Use VAR_POP when analyzing a complete population.
- [ ] **C)** VAR_POP on sample data can cause biased inference.
- [ ] **D)** VAR_POP is always preferred over VAR_SAMP.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> VAR_SAMP is for sample data and VAR_POP is for a full population. Choosing VAR_POP for a sample will lead to biased statistical inference.
 
 
</details>

### 18. Refer to the code block. Which function in the query returns an interpolated percentile value?

```sql
SELECT PERCENTILE_CONT(0.5) WITHIN GROUP (ORDER BY salary) AS cont_median,
       PERCENTILE_DISC(0.5) WITHIN GROUP (ORDER BY salary) AS disc_median
FROM employees;
```

- [ ] **A)** PERCENTILE_CONT
- [ ] **B)** PERCENTILE_DISC
- [ ] **C)** MEDIAN
- [ ] **D)** AVG

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PERCENTILE_CONT returns a continuous interpolated result, while PERCENTILE_DISC returns an actual value from the dataset.
 
 
</details>

### 19. Which statistical metric identifies the most frequently occurring value in a dataset?

- [ ] **A)** Mode
- [ ] **B)** Mean
- [ ] **C)** Median
- [ ] **D)** Variance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The mode is a descriptive statistic that quantifies the central tendency by identifying the most frequent value in a dataset.
 
 
</details>

### 20. Which statements accurately describe NULL handling by most Snowflake statistical functions?

- [ ] **A)** Most statistical functions ignore NULLs.
- [ ] **B)** COALESCE can be used to handle NULLs explicitly.
- [ ] **C)** Ignoring NULLs can skew the perceived distribution.
- [ ] **D)** NULLs are treated as zero in most statistical functions.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Most statistical functions ignore NULLs, so analysts should use COALESCE or similar logic to avoid an inaccurate representation of data distribution.
 
 
</details>

### 21. Refer to the code block. Which window frame clause is used in the running total?

```sql
SELECT order_date,
       amount,
       SUM(amount) OVER (ORDER BY order_date ROWS BETWEEN UNBOUNDED PRECEDING AND CURRENT ROW) AS running_total
FROM orders;
```

- [ ] **A)** ROWS
- [ ] **B)** RANGE
- [ ] **C)** GROUPS
- [ ] **D)** DEFAULT

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query uses ROWS BETWEEN UNBOUNDED PRECEDING AND CURRENT ROW, which defines a cumulative window frame with the ROWS clause.
 
 
</details>

### 22. Which Snowflake function returns the correlation coefficient between two numeric variables?

- [ ] **A)** CORR
- [ ] **B)** COVAR_POP
- [ ] **C)** COVAR_SAMP
- [ ] **D)** STDDEV

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CORR returns the correlation coefficient, which measures the strength and direction of the linear relationship between two numeric variables.
 
 
</details>

### 23. Which statements about clustering keys in Snowflake are correct?

- [ ] **A)** They physically reorder data in a table.
- [ ] **B)** They should align with common filter or join predicates.
- [ ] **C)** A high clustering depth indicates poor data distribution.
- [ ] **D)** They are the preferred optimization for single-value point lookups.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Clustering keys physically reorder data, align with frequent predicates, and a high clustering depth suggests poor distribution. Point lookups are better handled by Search Optimization Service.
 
 
</details>


---

### **Data Transformation and Data Modeling**

### 24. What is the primary difference between aggregate functions and window statistical functions in Snowflake?

- [ ] **A)** Aggregate functions collapse multiple rows into a single summary row, while window functions preserve original row granularity.
- [ ] **B)** Window functions collapse multiple rows into a single summary row, while aggregate functions preserve original row granularity.
- [ ] **C)** Both aggregate and window functions preserve the original row identity in all cases.
- [ ] **D)** Aggregate functions are used only for ranking, while window functions are used only for averaging.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Aggregate functions like AVG and STDDEV reduce a set of rows to one summary result. Window statistical functions calculate values across rows related to the current row and retain the original row-level detail.
 
 
</details>

### 25. Which of the following Snowflake functions can be classified as descriptive statistics for quantifying central tendency or dispersion? (Select all that apply.)

- [ ] **A)** AVG
- [ ] **B)** MEDIAN
- [ ] **C)** VAR_SAMP
- [ ] **D)** CORR

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> AVG and MEDIAN are central tendency metrics, while VAR_SAMP measures dispersion around the mean. CORR measures the linear relationship between two variables, not univariate descriptive statistics.
 
 
</details>

### 26. Review the SQL snippet. What does the function used in this query return for the requested percentile?

```sql
SELECT PERCENTILE_CONT(0.5) WITHIN GROUP (ORDER BY sales_amount) AS median_cont FROM orders;
```

- [ ] **A)** It returns an interpolated value between the two closest rows when the percentile falls between them.
- [ ] **B)** It returns the nearest actual existing value from the dataset.
- [ ] **C)** It returns NULL if the percentile is not an exact row match.
- [ ] **D)** It returns the sum of all values divided by the number of rows.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PERCENTILE_CONT is a continuous percentile function. It interpolates between values, so the result may not exist in the dataset.
 
 
</details>

### 27. An analyst is working with a random sample of customer transactions rather than the full population. Which variance function should be used to avoid biased statistical inference?

- [ ] **A)** VAR_POP
- [ ] **B)** VAR_SAMP
- [ ] **C)** STDDEV_POP
- [ ] **D)** COVAR_POP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> VAR_SAMP computes sample variance, which is appropriate when the data represents a subset of a larger population. Using VAR_POP on a sample would underestimate variance and produce biased inference.
 
 
</details>

### 28. Which statements about PERCENTILE_CONT and PERCENTILE_DISC are true? (Select all that apply.)

- [ ] **A)** PERCENTILE_CONT can return an interpolated value that does not exist in the dataset.
- [ ] **B)** PERCENTILE_DISC always returns an actual value from the dataset.
- [ ] **C)** PERCENTILE_DISC interpolates between two rows when the percentile falls between them.
- [ ] **D)** PERCENTILE_CONT returns only existing values from the dataset.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> PERCENTILE_CONT interpolates and may return values not in the dataset; PERCENTILE_DISC returns one of the actual existing values.
 
 
</details>

### 29. Review the SQL snippet. When two employees have the same sales value, how do the two ranking columns differ?

```sql
SELECT employee_id, sales, RANK() OVER (ORDER BY sales DESC) AS rnk, DENSE_RANK() OVER (ORDER BY sales DESC) AS dense_rnk FROM employees;
```

- [ ] **A)** The RANK column leaves gaps after ties, while DENSE_RANK does not leave gaps.
- [ ] **B)** The DENSE_RANK column leaves gaps after ties, while RANK does not.
- [ ] **C)** Both columns produce identical values for all rows, including ties.
- [ ] **D)** RANK ignores ties and assigns a unique number to every row.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RANK() skips the next rank after tied rows, creating gaps. DENSE_RANK() assigns consecutive ranks without gaps.
 
 
</details>

### 30. How does Snowflake's micro-partition pruning reduce the amount of data scanned by a query?

- [ ] **A)** Using highly selective filters in the WHERE clause so the Cloud Services layer can prune micro-partitions.
- [ ] **B)** Always declaring every column as a clustering key.
- [ ] **C)** Disabling the Cloud Services layer for large scans.
- [ ] **D)** Applying a materialized view to every query automatically.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Snowflake stores metadata for micro-partitions. Highly selective filters allow the Cloud Services layer to prune partitions and scan only relevant data.
 
 
</details>

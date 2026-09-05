<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/NVIDIA/NVIDIA-Certified%20Associate%3A%20Accelerated%20Data%20Science" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>NVIDIA Certified Associate - Accelerated Data Science</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Advance Data Structures](#advance-data-structures) (4 questions)
- [Data Manipulation and Preparation](#data-manipulation-and-preparation) (7 questions)
- [Data Science Pipelines and Workflow Automation](#data-science-pipelines-and-workflow-automation) (3 questions)
- [Descriptive Analysis and Visualization](#descriptive-analysis-and-visualization) (3 questions)
- [Foundations of Accelerated Data Science](#foundations-of-accelerated-data-science) (3 questions)
- [Introductory MLOps Practices](#introductory-mlops-practices) (3 questions)
- [Machine Learning With NVIDIA RAPIDS](#machine-learning-with-nvidia-rapids) (5 questions)
- [Software and Environment Management](#software-and-environment-management) (2 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:34.183Z |
| Domains | 8 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Advance Data Structures | 4 |
| Data Manipulation and Preparation | 7 |
| Data Science Pipelines and Workflow Automation | 3 |
| Descriptive Analysis and Visualization | 3 |
| Foundations of Accelerated Data Science | 3 |
| Introductory MLOps Practices | 3 |
| Machine Learning With NVIDIA RAPIDS | 5 |
| Software and Environment Management | 2 |

---

### **Advance Data Structures**

### 1. What is the primary advantage of using cuDF's optimized readers, such as read_parquet, for data ingestion?

- [ ] **A)** They use GPU kernels to parallelize file parsing directly into GPU memory
- [ ] **B)** They convert all numeric values to float64 before loading
- [ ] **C)** They store the data on disk to avoid using GPU memory
- [ ] **D)** They require the data to be in CSV format

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> cuDF readers leverage GPU kernels to parse and load data in parallel into VRAM, reducing ingestion time compared to CPU-based loading.
 
 
</details>

### 2. Which methods can you use to quickly inspect a cuDF DataFrame after loading it? (Select all that apply.)

- [ ] **A)** .head()
- [ ] **B)** .tail()
- [ ] **C)** .info()
- [ ] **D)** .plot()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> .head(), .tail(), and .info() are DataFrame inspection methods used to examine rows, structure, and schema before expensive GPU operations.
 
 
</details>

### 3. Review the code block. What does the printed output represent?

```python
import cudf

df = cudf.read_parquet("sensor_data.parquet")
print(df.dtypes)

```

- [ ] **A)** The column names and their data types
- [ ] **B)** The first five rows of the DataFrame
- [ ] **C)** Summary statistics for numeric columns
- [ ] **D)** The total memory usage of the GPU

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> .dtypes returns a Series containing the dtype of each column, enabling schema verification before further GPU processing.
 
 
</details>

### 4. What is the primary purpose of downcasting numeric columns in a cuDF DataFrame?

- [ ] **A)** To reduce the memory footprint so more data fits in GPU VRAM
- [ ] **B)** To increase the mathematical precision of calculations
- [ ] **C)** To enable automated string processing
- [ ] **D)** To move the data from device memory to host memory

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Downcasting reduces memory usage, which is critical for keeping large datasets within GPU VRAM and avoiding OOM errors.
 
 
</details>


---

### **Data Manipulation and Preparation**

### 5. What is the primary advantage of using cuDF's optimized readers for CSV and Parquet files compared to CPU-based data loading?

- [ ] **A)** They parallelize parsing with GPU kernels, reducing ingestion time.
- [ ] **B)** They always consume less GPU memory than CPU loading.
- [ ] **C)** They automatically convert all columns to pandas object types.
- [ ] **D)** They skip dtype verification entirely.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> cuDF readers use GPU kernels to parse files in parallel, dramatically cutting the time spent in data ingestion compared to CPU-based loading.
 
 
</details>

### 6. Which of the following are DataFrame inspection methods in cuDF that help verify data structure before GPU operations?

- [ ] **A)** .head()
- [ ] **B)** .tail()
- [ ] **C)** .info()
- [ ] **D)** .merge()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> .head(), .tail(), and .info() are inspection methods; .merge() is used for relational joins, not initial DataFrame inspection.
 
 
</details>

### 7. The code block reads a CSV and prints the dtypes of the resulting DataFrame. What is the purpose of this operation?

```python
import cudf
df = cudf.read_csv('data.csv')
print(df.dtypes)
```

- [ ] **A)** The schema and column data types are correct before executing GPU operations.
- [ ] **B)** The DataFrame is sorted by the first column.
- [ ] **C)** The number of missing values in each column.
- [ ] **D)** The data has been moved from device memory to host memory.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Printing .dtypes verifies schema and dtype alignment, helping avoid OOM and compatibility issues before expensive GPU operations.
 
 
</details>

### 8. Where must data reside for cuDF operations to benefit from GPU acceleration?

- [ ] **A)** GPU device memory (VRAM)
- [ ] **B)** System RAM (Host memory)
- [ ] **C)** CPU cache
- [ ] **D)** Local disk storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> cuDF acceleration requires data to reside in GPU high-bandwidth memory; host memory or disk prevents GPU-speed execution.
 
 
</details>

### 9. Which of the following are common traps in accelerated data workflows using cuDF?

- [ ] **A)** Assuming all pandas operations are 1:1 compatible with cuDF.
- [ ] **B)** Ignoring data types and using int64 when int32 suffices.
- [ ] **C)** Confusing host memory with device memory.
- [ ] **D)** Always using categorical types for numeric columns.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The traps include pandas compatibility assumptions, ignoring data types, and confusing host/device memory. Categorical types are beneficial for repeated strings.
 
 
</details>

### 10. The code block casts an int64 column to int32 after reading a Parquet file. What is the primary benefit of this downcasting?

```python
import cudf
df = cudf.read_parquet('data.parquet')
df['col'] = df['col'].astype('int32')
```

- [ ] **A)** It reduces the memory footprint on the GPU.
- [ ] **B)** It increases numeric precision.
- [ ] **C)** It converts the column to a categorical type.
- [ ] **D)** It enables string regex operations.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Downcasting from int64 to int32 reduces GPU memory usage, helping avoid OOM errors while maintaining sufficient precision.
 
 
</details>

### 11. How does boolean indexing enable efficient row filtering in cuDF?

- [ ] **A)** It creates a vectorized mask evaluated in parallel across GPU cores.
- [ ] **B)** It iterates through rows one by one on the CPU.
- [ ] **C)** It transfers the whole DataFrame to disk first.
- [ ] **D)** It converts all columns to strings for comparison.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> cuDF evaluates boolean masks as vectorized operations across GPU cores, avoiding slow Python-level row-wise conditional loops.
 
 
</details>


---

### **Data Science Pipelines and Workflow Automation**

### 12. Which method should be used to check the data types of each column in a cuDF DataFrame?

- [ ] **A)** .head()
- [ ] **B)** .dtypes
- [ ] **C)** .describe()
- [ ] **D)** .info()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The .dtypes method returns the data type of every column in a cuDF DataFrame, making it the direct way to verify schema and dtype alignment. .head() shows rows, .describe() gives statistics, and .info() provides a broader summary rather than a dedicated dtype series.
 
 
</details>

### 13. Which of the following are common traps when managing data types and memory in GPU-accelerated DataFrames? (Choose all that apply.)

- [ ] **A)** Using int64 for every integer column even when int32 would be sufficient
- [ ] **B)** Converting high-precision float64 columns to float32 to save memory
- [ ] **C)** Assuming data exists in GPU memory when it actually remains in system RAM
- [ ] **D)** Using category dtype for repeated string values

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Using unnecessarily wide integer types can cause OOM errors in VRAM, and confusing host memory with device memory prevents acceleration because data must reside on the GPU. Downcasting float64 to float32 and using category dtype are both effective optimization strategies, not traps.
 
 
</details>

### 14. After executing the provided code, where is the 'transactions' dataset stored so that cuDF operations can accelerate it?

```python
import cudf

df = cudf.read_parquet('transactions.parquet')
print(df.info())
```

- [ ] **A)** In GPU high-bandwidth memory (VRAM)
- [ ] **B)** In CPU system RAM (host memory)
- [ ] **C)** On the disk in the original Parquet file
- [ ] **D)** In CPU cache

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> cuDF loads data directly into GPU memory by leveraging fast device-side readers. The DataFrame resides in GPU high-bandwidth memory, enabling subsequent operations to run without moving data back to the CPU.
 
 
</details>


---

### **Descriptive Analysis and Visualization**

### 15. What is the primary advantage of using cuDF's optimized readers for CSV and Parquet files?

- [ ] **A)** They use GPU kernels to parallelize parsing, significantly reducing ingestion time.
- [ ] **B)** They compress data before storing it in CPU memory.
- [ ] **C)** They automatically convert all columns to string types.
- [ ] **D)** They load data directly into System RAM without GPU involvement.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> cuDF readers leverage GPU kernels to parse formats like CSV and Parquet in parallel, minimizing the initial data ingestion phase compared with CPU-based loading.
 
 
</details>

### 16. Which of the following methods are recommended for inspecting a cuDF DataFrame's structure before executing expensive GPU operations?

- [ ] **A)** .head()
- [ ] **B)** .info()
- [ ] **C)** .tail()
- [ ] **D)** .to_pandas()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Inspection methods such as .head(), .tail(), and .info() let data scientists quickly verify data structure and dtype alignment before running costly GPU operations.
 
 
</details>

### 17. What is the type of the object returned by this cuDF groupby operation?

```python
import cudf

df = cudf.DataFrame({'group': ['A', 'A', 'B'], 'value': [1, 2, 3]})
result = df.groupby('group')['value'].transform('mean')
print(type(result))
```

- [ ] **A)** A cudf.Series with the same length as the original DataFrame
- [ ] **B)** A cudf.DataFrame with one row per group
- [ ] **C)** A cudf.Index containing the group labels
- [ ] **D)** A Python float representing the overall mean

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> groupby().transform() returns a Series of the same length as the original, unlike aggregate(), which reduces the dimensionality.
 
 
</details>


---

### **Foundations of Accelerated Data Science**

### 18. Which NVIDIA library provides GPU-accelerated DataFrame readers that ingest CSV and Parquet files directly into GPU memory?

- [ ] **A)** cuDF
- [ ] **B)** pandas
- [ ] **C)** NumPy
- [ ] **D)** Matplotlib

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> cuDF is RAPIDS' GPU DataFrame library. Its optimized readers use GPU kernels to parse CSV and Parquet files directly into GPU memory, significantly reducing ingestion time compared to CPU-based pandas loading.
 
 
</details>

### 19. Which of the following are common traps when working with cuDF in accelerated data science? Select all that apply.

- [ ] **A)** Assuming all pandas operations are 1:1 compatible with cuDF
- [ ] **B)** Confusing host memory with device memory
- [ ] **C)** Using int32 instead of int64 when memory is limited
- [ ] **D)** Always dropping missing values to speed up preprocessing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Common cuDF traps include assuming pandas compatibility, confusing host and device memory, and dropping missing values without analysis. Downcasting to int32 is a recommended memory-saving practice, not a trap.
 
 
</details>

### 20. Review the code block. What dtype is assigned to the `scores` column when `df.dtypes` is printed?

```python
import cudf

df = cudf.DataFrame({'ids': [10, 20], 'scores': [9.5, 8.5]})
print(df.dtypes)
```

- [ ] **A)** float64
- [ ] **B)** float32
- [ ] **C)** int64
- [ ] **D)** object

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When a cuDF DataFrame is created from Python float values, cuDF infers a float64 dtype for the column. Therefore, `scores` is displayed as float64.
 
 
</details>


---

### **Introductory MLOps Practices**

### 21. What is the primary reason cuDF readers accelerate the initial ingestion of large datasets compared to CPU-based loading?

- [ ] **A)** GPU kernels parallelize parsing
- [ ] **B)** Data is compressed automatically
- [ ] **C)** Data stays in host memory
- [ ] **D)** Files are converted to CSV first

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> cuDF uses GPU kernels to parse formats like Parquet and CSV in parallel, moving data directly into VRAM unlike CPU-based loading.
 
 
</details>

### 22. Which actions help prevent Out-of-Memory errors when using cuDF on the GPU?

- [ ] **A)** Convert string columns to categorical types
- [ ] **B)** Downcast numeric columns to smaller types
- [ ] **C)** Use float64 for all numeric columns
- [ ] **D)** Keep data in system RAM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Categorical encoding and downcasting reduce memory footprint. High-precision types and host memory placement increase memory pressure or prevent acceleration, causing OOM.
 
 
</details>

### 23. What does the output of `.dtypes` in this snippet confirm before further GPU processing?

```python
import cudf

df = cudf.read_parquet('data.parquet')
print(df.dtypes)
print(df.head())
```

- [ ] **A)** Column types and schema alignment
- [ ] **B)** Descriptive statistics
- [ ] **C)** Number of null values
- [ ] **D)** Join compatibility

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> .dtypes shows the data type of each column, allowing schema verification before expensive GPU operations.
 
 
</details>


---

### **Machine Learning With NVIDIA RAPIDS**

### 24. What is the primary benefit of using cuDF’s optimized readers, such as read_parquet, for data ingestion?

- [ ] **A)** It parallelizes file parsing across GPU cores, reducing ingestion time.
- [ ] **B)** It automatically sorts all data after reading.
- [ ] **C)** It converts all columns to float64 by default.
- [ ] **D)** It moves data from GPU to host memory automatically.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> cuDF uses GPU kernels to parse file formats such as Parquet and CSV in parallel, loading data directly into GPU memory and significantly reducing ingestion time. It does not sort the data automatically, does not default to float64, and does not move data to host memory.
 
 
</details>

### 25. Which two statements about data types and memory in accelerated RAPIDS workflows are correct?

- [ ] **A)** Choosing int64 when int32 is sufficient can cause OOM errors on the GPU.
- [ ] **B)** Using 64-bit types always improves GPU processing performance.
- [ ] **C)** Downcasting columns reduces the memory footprint in GPU VRAM.
- [ ] **D)** String-heavy columns require no extra memory management.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Selecting unnecessarily large dtypes such as int64 can waste GPU memory and lead to OOM errors. Downcasting, such as converting int64 to int32 or float64 to float32, reduces VRAM usage. 64-bit types are not always better, and string-heavy columns require careful memory management.
 
 
</details>

### 26. What is the purpose of the operation shown in the code block?

```python
import cudf

df = cudf.read_parquet("/data/sales.parquet")
print(df.dtypes)
```

- [ ] **A)** Inspect the schema and dtype of each column.
- [ ] **B)** Sort the DataFrame by index.
- [ ] **C)** Compute descriptive statistics for numeric columns.
- [ ] **D)** Filter rows where values are null.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Using .dtypes on a cuDF DataFrame displays each column’s data type. This is a schema and dtype verification step, allowing the user to confirm whether column types are appropriate before performing expensive GPU operations.
 
 
</details>

### 27. What is a key purpose of sorting data in a GPU-accelerated data pipeline?

- [ ] **A)** It enables more efficient joins and window functions.
- [ ] **B)** It reduces the memory footprint of categorical columns.
- [ ] **C)** It eliminates the need to check for missing values.
- [ ] **D)** It automatically encodes string columns as integers.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Sorting is a prerequisite for efficient joins and window functions in GPU-accelerated workflows. It does not reduce categorical memory usage, remove missing values, or automatically encode strings.
 
 
</details>

### 28. Which two statements about the category dtype in cuDF are true?

- [ ] **A)** It represents repeated strings as integers.
- [ ] **B)** It reduces memory footprint compared to raw string columns.
- [ ] **C)** It slows down groupby and join operations.
- [ ] **D)** It can only be used after dropping all null values.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Categorical data uses integer codes to represent repeated strings, reducing memory usage and accelerating grouping and joining operations. It is not slower, and it does not require dropping all null values before use.
 
 
</details>


---

### **Software and Environment Management**

### 29. What is the primary reason cuDF's optimized readers can load large-scale datasets faster than CPU-based loading?

- [ ] **A)** They use GPU kernels to parallelize parsing of file formats like Parquet and CSV.
- [ ] **B)** They bypass VRAM and read data directly into system RAM.
- [ ] **C)** They rely on pandas for parsing and add a caching layer.
- [ ] **D)** They load only a sample of the data instead of the full file.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> cuDF's optimized readers leverage GPU kernels to parse files in parallel, which significantly reduces the time spent in the data ingestion phase compared to CPU-based loading.
 
 
</details>

### 30. Which of the following are common traps when working with cuDF in accelerated workflows? Select all that apply.

- [ ] **A)** Assuming every pandas operation is 1:1 compatible with cuDF.
- [ ] **B)** Using int64 when int32 would be sufficient, potentially causing out-of-memory errors.
- [ ] **C)** Failing to distinguish between GPU memory and system RAM.
- [ ] **D)** Converting string-heavy columns to categorical types to reduce memory.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Common traps include assuming pandas compatibility for every operation, ignoring data types, and confusing host memory with device memory. Converting string-heavy columns to categorical types is a recommended practice, not a pitfall.
 
 
</details>

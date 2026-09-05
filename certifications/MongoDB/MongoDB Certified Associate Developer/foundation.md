<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/MongoDB/MongoDB%20Associate%20Developer" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>MongoDB Certified Associate Developer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Aggregations](#aggregations) (6 questions)
- [CRUD Operations](#crud-operations) (6 questions)
- [Data Access (Driver usage)](#data-access-driver-usage) (4 questions)
- [Data Modeling](#data-modeling) (4 questions)
- [Indexes](#indexes) (5 questions)
- [Performance](#performance) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:29.052Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Aggregations | 6 |
| CRUD Operations | 6 |
| Data Access (Driver usage) | 4 |
| Data Modeling | 4 |
| Indexes | 5 |
| Performance | 5 |

---

### **Aggregations**

### 1. What data structure does MongoDB use for single field indexes?

- [ ] **A)** B-Tree
- [ ] **B)** Hash table
- [ ] **C)** Linked list
- [ ] **D)** Binary heap

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MongoDB uses a B-Tree for single field indexes, enabling efficient logarithmic searches and sorted operations.
 
 
</details>

### 2. Which statements about single field index direction are correct? Select all that apply.

- [ ] **A)** Direction is irrelevant for equality matches.
- [ ] **B)** Direction is important when the index supports a sort.
- [ ] **C)** A single field index can only be traversed in one direction.
- [ ] **D)** Descending indexes cannot support equality queries.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> For equality matches index direction does not matter, but for sort operations direction determines whether MongoDB can traverse the index in the required order.
 
 
</details>

### 3. Given the code snippet that creates an index on a field containing an array, what type of index will be created?

```javascript
db.collection.createIndex({ tags: 1 })
```

- [ ] **A)** Multikey index
- [ ] **B)** Sparse index
- [ ] **C)** Compound index
- [ ] **D)** Wildcard index

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Indexing an array field causes MongoDB to create a multikey index with an entry for every array element.
 
 
</details>

### 4. What is true about a sparse index?

- [ ] **A)** Documents that have the indexed field
- [ ] **B)** All documents in the collection
- [ ] **C)** Only documents with array fields
- [ ] **D)** Only documents created recently

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Sparse indexes contain entries only for documents that possess the indexed field, reducing index size and memory use.
 
 
</details>

### 5. Which operations are slowed down by adding too many indexes to a collection? Select all that apply.

- [ ] **A)** Insert operations
- [ ] **B)** Update operations
- [ ] **C)** Delete operations
- [ ] **D)** Read operations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Every index must be updated on insert, update, and delete; write-heavy workloads suffer most from excessive indexing.
 
 
</details>

### 6. The code snippet creates a compound index on three fields. Which query can use this index based on the prefix rule?

```javascript
db.collection.createIndex({ a: 1, b: 1, c: 1 })
```

- [ ] **A)** A query filtering only on the first field
- [ ] **B)** A query filtering only on the second field
- [ ] **C)** A query filtering only on the third field
- [ ] **D)** A query filtering only on the second and third fields

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A compound index supports queries on prefixes of its fields, such as the first field alone, but not non-prefix combinations.
 
 
</details>


---

### **CRUD Operations**

### 7. In MongoDB, what data structure is used to implement single-field indexes for efficient lookups and sorting?

- [ ] **A)** B-Tree
- [ ] **B)** Hash table
- [ ] **C)** Linked list
- [ ] **D)** Binary heap

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MongoDB uses a B-Tree, which enables logarithmic time complexity for lookups, range queries, and sorting.
 
 
</details>

### 8. When evaluating a single-field index in MongoDB, which two statements accurately describe the role of ascending and descending direction?

- [ ] **A)** Irrelevant for equality matches
- [ ] **B)** Critical for supported sort operations
- [ ] **C)** Determines number of index entries
- [ ] **D)** Descending indexes cannot help sorting

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> For equality matches, a single-field index can be traversed both ways. For sorts, direction must match the requested order.
 
 
</details>

### 9. Review the query in the code block. According to the ESR rule, which compound index field order is optimal?

```javascript
db.orders.find({ status: 'active', total: { $gt: 100 } }).sort({ created_at: -1 });
```

- [ ] **A)** status, created_at, total
- [ ] **B)** created_at, status, total
- [ ] **C)** total, status, created_at
- [ ] **D)** status, total, created_at

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ESR says equality fields first, then sort fields, then range fields. Thus status, created_at, and total is optimal.
 
 
</details>

### 10. Why is an index on a high-selectivity field such as user_id more efficient than one on a low-cardinality field such as gender?

- [ ] **A)** Discards more non-matching documents
- [ ] **B)** Reduces need for multikey indexes
- [ ] **C)** Prevents all write overhead
- [ ] **D)** Guarantees sort without indexes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> High selectivity means many unique values, so the index can discard more non-matching documents and narrow the result set quickly.
 
 
</details>

### 11. Select the two correct statements about how MongoDB handles an index on a field that contains an array.

- [ ] **A)** Automatically created for array fields
- [ ] **B)** One entry per array element
- [ ] **C)** Compresses array entries into one
- [ ] **D)** Cannot contain array fields

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> When the indexed field is an array, MongoDB automatically creates a multikey index with one entry for each array element.
 
 
</details>

### 12. Given the index creation in the code block, what type of index will MongoDB build if the tags field contains arrays?

```javascript
db.posts.createIndex({ tags: 1 });
```

- [ ] **A)** Multikey index
- [ ] **B)** Sparse index
- [ ] **C)** Partial index
- [ ] **D)** Compound index

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Indexing an array creates a multikey index, with entries per array element for efficient element lookups.
 
 
</details>


---

### **Data Access (Driver usage)**

### 13. Which underlying data structure powers single field indexes in MongoDB?

- [ ] **A)** B-Tree
- [ ] **B)** Hash table
- [ ] **C)** Linked list
- [ ] **D)** Binary heap

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MongoDB uses a B-Tree structure for single field indexes, enabling logarithmic traversal and efficient searches, range queries, and sorting.
 
 
</details>

### 14. What statements about multikey indexes are true? Select all that apply.

- [ ] **A)** A compound index cannot include more than one array field.
- [ ] **B)** MongoDB creates a multikey index when the indexed field is an array.
- [ ] **C)** Each element in an indexed array receives an index entry.
- [ ] **D)** A multikey index can include multiple array fields to improve performance.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A single compound multikey index cannot contain more than one array field, and MongoDB indexes each array element separately, improving array query selectivity but increasing index size.
 
 
</details>

### 15. Based on the index created in the code, which query cannot be efficiently supported?

```javascript
db.users.createIndex({ last_name: 1, first_name: 1 })
```

- [ ] **A)** Filter on first_name only
- [ ] **B)** Filter on last_name only
- [ ] **C)** Filter on both last_name and first_name
- [ ] **D)** Filter on last_name and sort by first_name

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Index prefixes are last_name and last_name+first_name. A filter on first_name alone cannot use this index because first_name is not a leading prefix.
 
 
</details>

### 16. According to the ESR rule, what is the recommended field order for a compound index?

- [ ] **A)** Equality, Sort, Range
- [ ] **B)** Range, Sort, Equality
- [ ] **C)** Sort, Equality, Range
- [ ] **D)** Equality, Range, Sort

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ESR stands for Equality, Sort, Range. Ordering fields this way narrows matches first, supports sorting, and applies range filters last.
 
 
</details>


---

### **Data Modeling**

### 17. What data structure does MongoDB use to implement single field indexes?

- [ ] **A)** B-Tree
- [ ] **B)** Hash table
- [ ] **C)** Linked list
- [ ] **D)** Unordered heap

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MongoDB implements single field indexes using a B-Tree, giving logarithmic time complexity for lookups, range queries, and sorting operations.
 
 
</details>

### 18. Which statements about single field indexes in MongoDB are correct? Select all that apply.

- [ ] **A)** The ascending/descending direction is largely irrelevant for equality matches.
- [ ] **B)** Index direction is crucial when the index is used to support a sort operation.
- [ ] **C)** A sparse index contains entries for documents that are missing the indexed field.
- [ ] **D)** An index on a low-cardinality field such as gender is always more efficient than an index on user_id.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> For equality matches, index direction does not matter, but for sort operations it does. Sparse indexes omit documents missing the field, and high-cardinality fields provide better selectivity.
 
 
</details>

### 19. You execute the MongoDB command shown in the code block on a collection where the indexed field contains arrays. What type of index is created?

```javascript
db.users.createIndex({ tags: 1 })
```

- [ ] **A)** Multikey index
- [ ] **B)** Sparse index
- [ ] **C)** Compound index
- [ ] **D)** Wildcard index

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When a single indexed field contains an array, MongoDB automatically creates a multikey index with an entry for each array element.
 
 
</details>

### 20. An index is defined as { status: 1, created_at: 1 }. According to the index prefix rule, which query can use this index?

- [ ] **A)** A filter on status only
- [ ] **B)** A filter on created_at only
- [ ] **C)** A filter on neither field
- [ ] **D)** A sort on created_at only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Index prefixing allows a compound index to support queries on a prefix of its fields. { status: 1, created_at: 1 } can support status-only filters but not created_at-only filters.
 
 
</details>


---

### **Indexes**

### 21. Which data structure does MongoDB use when creating a single field index?

- [ ] **A)** B-Tree
- [ ] **B)** Hash Table
- [ ] **C)** Linked List
- [ ] **D)** LSM Tree

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> MongoDB uses a B-Tree structure for single field indexes, enabling logarithmic lookups and efficient traversal for searches, ranges, and sorts.
 
 
</details>

### 22. Select all the true statements about single field indexes in MongoDB.

- [ ] **A)** Index direction is irrelevant for equality matches.
- [ ] **B)** Index direction is crucial for supporting sort operations.
- [ ] **C)** Indexing a low-cardinality field always outperforms a collection scan.
- [ ] **D)** Every stored index adds overhead to write operations.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> A single field index can be traversed in both directions, so direction matters mainly for sorts. Indexes always add write overhead, and low-cardinality fields are not guaranteed to outperform collection scans.
 
 
</details>

### 23. Look at the index creation command in the code block. If the indexed field contains arrays in some documents, which type of index will be created by MongoDB?

```javascript
db.collection.createIndex({ tags: 1 })
```

- [ ] **A)** Multikey index
- [ ] **B)** Sparse index
- [ ] **C)** Text index
- [ ] **D)** Compound index

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When a single indexed field contains an array, MongoDB creates a multikey index, with one index entry per array element.
 
 
</details>

### 24. According to the ESR rule, what is the recommended order of fields in a compound index?

- [ ] **A)** Equality, then Sort, then Range
- [ ] **B)** Range, then Sort, then Equality
- [ ] **C)** Sort, then Equality, then Range
- [ ] **D)** Equality, then Range, then Sort

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ESR stands for Equality, Sort, Range. Equality fields first narrow the search space, sort fields provide ordering, and range filters are applied last.
 
 
</details>

### 25. Select all true statements about compound indexes and the index prefix rule.

- [ ] **A)** 
- [ ] **B)** 
- [ ] **C)** The order of fields in a compound index is significant because of the prefix rule.
- [ ] **D)** 

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The prefix rule means the leading field must be part of the query. An index on { a: 1, b: 1 } supports a alone or a and b together, but not b alone.
 
 
</details>


---

### **Performance**

### 26. Which data structure does MongoDB use to implement single field indexes?

- [ ] **A)** Hash table
- [ ] **B)** B-Tree
- [ ] **C)** Linked list
- [ ] **D)** LSM tree

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> MongoDB uses a B-Tree structure for single field indexes, enabling logarithmic lookup, range queries, and sorting efficiency.
 
 
</details>

### 27. Which statements are true regarding single field indexes? Select all that apply.

- [ ] **A)** A single field index can be traversed in both directions.
- [ ] **B)** An index on a low-cardinality field is always more efficient than one on a high-cardinality field.
- [ ] **C)** Every index adds overhead to insert, update, and delete operations.
- [ ] **D)** A single field index on an array is known as a wildcard index.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Single field indexes are bidirectional and impose write overhead. High-cardinality fields are more selective, and array indexes are multikey, not wildcard.
 
 
</details>

### 28. Review the index creation command in the code block. What type of index does it create?

```javascript
db.collection.createIndex({ status: 1 })
```

- [ ] **A)** Ascending single field index
- [ ] **B)** Descending single field index
- [ ] **C)** Compound index
- [ ] **D)** Multikey index

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code creates an ascending index on the status field. It is a single field index because only one field is specified.
 
 
</details>

### 29. Why is an index on a high-cardinality field such as user_id more efficient than one on a low-cardinality field such as gender?

- [ ] **A)** It allows the engine to discard non-matching documents more quickly.
- [ ] **B)** It eliminates the need for any index on other fields.
- [ ] **C)** It guarantees that all queries will use the index.
- [ ] **D)** It reduces the overhead of every write operation.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> High-selectivity indexes narrow the search space quickly by discarding many non-matching documents, making queries more efficient.
 
 
</details>

### 30. Which statements about multikey indexes are correct? Select all that apply.

- [ ] **A)** An entry is created for every element in the indexed array.
- [ ] **B)** A multikey index is automatically created when the indexed field contains an array.
- [ ] **C)** A compound index can include two different array fields.
- [ ] **D)** Multikey indexes are the same as wildcard indexes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Multikey indexes are automatic for array fields and create one entry per element. MongoDB prohibits compound multikey indexes with multiple array fields.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/MongoDB/MongoDB%20Associate%20Database%20Administrator" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>MongoDB Certified Associate Database Administrator</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [CRUD Operations](#crud-operations) (8 questions)
- [Indexes](#indexes) (5 questions)
- [Monitoring and Performance Tuning](#monitoring-and-performance-tuning) (3 questions)
- [Philosophy and Features](#philosophy-and-features) (2 questions)
- [Replication](#replication) (4 questions)
- [Security](#security) (5 questions)
- [Server Administration](#server-administration) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:26.499Z |
| Domains | 7 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| CRUD Operations | 8 |
| Indexes | 5 |
| Monitoring and Performance Tuning | 3 |
| Philosophy and Features | 2 |
| Replication | 4 |
| Security | 5 |
| Server Administration | 3 |

---

### **CRUD Operations**

### 1. Which statement best describes a single-field index in MongoDB?

- [ ] **A)** An index created on a single field of a document.
- [ ] **B)** An index that combines two or more fields.
- [ ] **C)** An index that stores the entire document.
- [ ] **D)** An index that requires a unique constraint.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A single-field index is built on one field and speeds up equality and range queries on that key. It is the fundamental building block for query performance.
 
 
</details>

### 2. What statements accurately describe compound indexes?

- [ ] **A)** They reference multiple fields in a single B-tree structure.
- [ ] **B)** The order of fields in the index is important.
- [ ] **C)** Field order has no effect on query support.
- [ ] **D)** They cannot support queries on leading fields.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Compound indexes hold references to several fields in one B-tree. Field order is critical and queries can use the leading prefix of the index.
 
 
</details>

### 3. The code block creates a compound index. Based on the Prefix Rule, which query can be efficiently supported?

```javascript
db.orders.createIndex({ a: 1, b: 1 })
```

- [ ] **A)** db.orders.find({ a: 5 })
- [ ] **B)** db.orders.find({ b: 5 })
- [ ] **C)** db.orders.find({}).sort({ b: 1 })
- [ ] **D)** db.orders.find({ c: 5 })

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Prefix Rule lets an index support queries that include its leftmost fields. Since the index is on {a:1,b:1}, querying only on a uses the prefix; b alone cannot.
 
 
</details>

### 4. What does the Prefix Rule state about compound indexes?

- [ ] **A)** Only the rightmost field of an index can be used.
- [ ] **B)** A compound index supports queries on its leading leftmost fields.
- [ ] **C)** Any field in a compound index can be used independently.
- [ ] **D)** The prefix rule only applies to TTL indexes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Prefix Rule states that a compound index supports queries on the leading fields, but cannot efficiently support queries on later fields alone.
 
 
</details>

### 5. Which problems can result from over-indexing a MongoDB collection?

- [ ] **A)** High write latency.
- [ ] **B)** Memory pressure in the WiredTiger cache.
- [ ] **C)** Faster deletes with no overhead.
- [ ] **D)** Reduced storage usage.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Each index adds write overhead and consumes cache memory. Over-indexing increases write latency and can exhaust the WiredTiger cache.
 
 
</details>

### 6. Examine the TTL index in the code block. Which statements about its expiration behavior are true?

```javascript
db.sessions.createIndex({ lastModified: 1 }, { expireAfterSeconds: 3600 })
```

- [ ] **A)** Documents expire 3600 seconds after the lastModified date.
- [ ] **B)** The background thread runs at most once every 60 seconds.
- [ ] **C)** Deletion happens instantly when the TTL value is reached.
- [ ] **D)** The index works with integer timestamp fields.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> TTL indexes delete documents after expireAfterSeconds from the date field. A background thread runs about every 60 seconds and the field must be a BSON date type.
 
 
</details>

### 7. On what field type can a TTL index be created?

- [ ] **A)** BSON date type or array of BSON dates.
- [ ] **B)** Integer timestamp only.
- [ ] **C)** String date only.
- [ ] **D)** Any numeric value.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TTL indexes can only be created on single fields containing BSON dates or arrays of BSON dates. Integer timestamps will not trigger expiration.
 
 
</details>

### 8. Which field values are valid for a TTL index?

- [ ] **A)** A BSON date.
- [ ] **B)** An array of BSON dates.
- [ ] **C)** A Unix epoch integer.
- [ ] **D)** A string formatted as a date.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The TTL index only expires documents when the field holds a BSON date or an array of BSON dates. Other types are not supported.
 
 
</details>


---

### **Indexes**

### 9. What is a single-field index in MongoDB?

- [ ] **A)** An index on multiple fields in a B-tree structure
- [ ] **B)** An index on a single field used to speed up queries on that key
- [ ] **C)** An index that automatically expires documents
- [ ] **D)** An index created only on array fields

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A single-field index is built on one field and is the fundamental tool for accelerating equality and range queries on that specific key.
 
 
</details>

### 10. Which statements accurately describe compound indexes?

- [ ] **A)** They store references to multiple fields in one B-tree structure
- [ ] **B)** Field order has no effect on which queries the index can support
- [ ] **C)** They follow a prefix rule, meaning leftmost fields can support queries by themselves
- [ ] **D)** Compound indexes are sensitive to sort direction, whereas single-field indexes can be traversed in either direction

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Compound indexes store multiple fields in one B-tree, respect the prefix rule, and require sort direction to match their field order.
 
 
</details>

### 11. Examine the compound index definition and query in the code block. Which statement about index usage is correct?

```javascript
db.people.createIndex({ status: 1, age: -1 })
db.people.find({ status: "active" }).sort({ age: -1 })
```

- [ ] **A)** The query uses the index because status is the leading field and the sort order matches
- [ ] **B)** The index cannot support sorting by age descending because status is ascending
- [ ] **C)** The query requires a separate index only on age
- [ ] **D)** The index will be ignored because it includes a sort field

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The index prefix on status matches the query filter, and the age direction matches the sort, so the compound index is used efficiently.
 
 
</details>

### 12. Compared with using index intersection, what is a primary advantage of a well-designed compound index?

- [ ] **A)** It eliminates the need for all write operations
- [ ] **B)** It is generally more efficient for satisfying queries on multiple fields
- [ ] **C)** It automatically covers every possible query
- [ ] **D)** It does not consume any storage space

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Index intersection can satisfy some queries, but a single compound index is usually more efficient and is the preferred design.
 
 
</details>

### 13. Which statements about TTL indexes are true?

- [ ] **A)** They can only be created on a single field containing BSON date values
- [ ] **B)** They support compound indexes if one field is a date
- [ ] **C)** A background thread removes expired documents approximately every 60 seconds
- [ ] **D)** TTL indexes require integer timestamps and delete documents immediately

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> TTL indexes require a single BSON date field and are processed by a background thread at most every 60 seconds.
 
 
</details>


---

### **Monitoring and Performance Tuning**

### 14. What type of index is the fundamental building block used to speed up equality and range queries on a specific key?

- [ ] **A)** Single-field index
- [ ] **B)** Compound index
- [ ] **C)** Multikey index
- [ ] **D)** TTL index

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A single-field index is created on one document field and is the fundamental tool for optimizing equality and range queries on a specific key.
 
 
</details>

### 15. Which two statements accurately describe how TTL indexes handle the automatic expiration and eventual deletion of stored documents?

- [ ] **A)** Requires a single field containing a BSON date
- [ ] **B)** Background thread runs at most once every 60 seconds
- [ ] **C)** Works with integer Unix timestamps
- [ ] **D)** Deletion occurs immediately when time expires

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> TTL indexes require BSON date fields, are processed by a background thread at most every 60 seconds, and deletions are eventually consistent rather than immediate.
 
 
</details>

### 16. The code block contains explain() output for a query. Which stage in the winning plan proves that the query used an index?

```json
{"queryPlanner":{"winningPlan":{"stage":"FETCH","inputStage":{"stage":"IXSCAN","indexName":"status_1_createdAt_1"}}}}
```

- [ ] **A)** IXSCAN
- [ ] **B)** COLLSCAN
- [ ] **C)** SORT
- [ ] **D)** FETCH

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IXSCAN is the execution stage that indicates an index was used, while COLLSCAN indicates a collection scan. The other stages are not evidence of index usage.
 
 
</details>


---

### **Philosophy and Features**

### 17. What does the Prefix Rule state about compound indexes in MongoDB?

- [ ] **A)** An index can support queries that include the leading fields of the index.
- [ ] **B)** An index can support queries on any field, regardless of position.
- [ ] **C)** An index can only support equality filters, never range filters.
- [ ] **D)** An index is valid only if all fields are used in the query.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The prefix rule means a compound index can serve queries that filter on its leftmost fields. A query on the leading fields can use the index, while a query on a later field alone cannot.
 
 
</details>

### 18. Which two statements about TTL indexes are correct in MongoDB?

- [ ] **A)** TTL indexes require a single field that contains a BSON date or an array of BSON dates.
- [ ] **B)** TTL indexes can be created on compound indexes.
- [ ] **C)** TTL indexes accept integer Unix timestamps for expiration.
- [ ] **D)** TTL expiration is processed by a background thread that runs at most once every 60 seconds.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> TTL indexes are single-field indexes on BSON date values. A background thread deletes expired documents at most every 60 seconds. Compound indexes and integer timestamps are not supported.
 
 
</details>


---

### **Replication**

### 19. What does a single-field index do in MongoDB?

- [ ] **A)** Speeds up equality and range queries on a key
- [ ] **B)** Creates a unique constraint on a date field
- [ ] **C)** Builds compound indexes without field order
- [ ] **D)** Automatically deletes documents after sixty seconds

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A single-field index is the fundamental building block for performance, speeding up equality and range queries on the indexed key.
 
 
</details>

### 20. Which two statements about compound indexes are true? Select all that apply.

- [ ] **A)** Field order in a compound index is paramount
- [ ] **B)** Compound indexes follow increasing selectivity
- [ ] **C)** A compound index can be used starting from any field, regardless of order
- [ ] **D)** Sort direction is irrelevant in compound indexes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Field order determines utility, and compound indexes are built with increasing selectivity. The prefix rule prevents use from rightmost fields alone, and direction matters in compound sorts.
 
 
</details>

### 21. The code block shows a compound index. According to the Prefix Rule, which query can be efficiently supported by this index?

```javascript
db.collection.createIndex({ a: 1, b: 1 })
```

- [ ] **A)** Query filtering only on field a
- [ ] **B)** Query filtering only on field b
- [ ] **C)** Query filtering only on field c
- [ ] **D)** Query filtering on neither a nor b

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Prefix Rule says a compound index can support queries that include the leading leftmost fields. Filtering only on field b ignores the leading field a, so it cannot use the index.
 
 
</details>

### 22. Which field type is required by a TTL index to expire documents?

- [ ] **A)** BSON date or array of BSON dates
- [ ] **B)** Integer Unix timestamp
- [ ] **C)** String containing a readable date
- [ ] **D)** Any numeric field

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TTL indexes require a single field containing a BSON date type or an array of BSON dates; integer timestamps do not trigger expiration.
 
 
</details>


---

### **Security**

### 23. What data type must a TTL index field contain to trigger automatic expiration?

- [ ] **A)** BSON Date
- [ ] **B)** Integer timestamp
- [ ] **C)** String
- [ ] **D)** ObjectId

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TTL indexes require a single field containing a BSON date type or an array of BSON date types; integer timestamps do not trigger expiration.
 
 
</details>

### 24. Which statements about TTL index behavior are correct? Select all that apply.

- [ ] **A)** TTL indexes can only be created on a single field.
- [ ] **B)** The background expiration thread runs at most once every 60 seconds.
- [ ] **C)** Documents are removed immediately once expireAfterSeconds has passed.
- [ ] **D)** TTL indexes can be created on integer timestamp fields.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> TTL indexes support only single fields; a background thread runs up to every 60 seconds, so deletion is not immediate; integer timestamps are not valid.
 
 
</details>

### 25. Examine the explain() output in the code block. Which execution stage is shown?

```json
{
  "queryPlanner": {
    "winningPlan": {
      "stage": "COLLSCAN"
    }
  }
}
```

- [ ] **A)** Collection Scan
- [ ] **B)** Index Scan
- [ ] **C)** Sort Merge Join
- [ ] **D)** Covered Query

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> COLLSCAN indicates a collection scan, usually meaning no suitable index was used.
 
 
</details>

### 26. According to the Prefix Rule, what queries can a compound index on {a: 1, b: 1} support?

- [ ] **A)** Queries filtering on b only
- [ ] **B)** Queries filtering on a only or a and b together
- [ ] **C)** Queries filtering on neither a nor b
- [ ] **D)** Any query containing b if sorted by a

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A compound index supports queries on leading leftmost fields; {a:1,b:1} cannot efficiently serve b-only queries.
 
 
</details>

### 27. Which of the following are common mistakes when working with MongoDB indexes? Select all that apply.

- [ ] **A)** Ignoring the index prefix rule when querying a compound index
- [ ] **B)** Assuming single-field indexes are direction-agnostic for sort operations
- [ ] **C)** Creating indexes on every field to cover all queries
- [ ] **D)** Using a TTL index on a BSON date field

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> A common trap is ignoring the prefix rule; over-indexing every field causes write latency and memory pressure. Single-field indexes are direction-agnostic, and TTL on BSON date is valid.
 
 
</details>


---

### **Server Administration**

### 28. What is the main purpose of a single-field index in MongoDB when a query filters on that field?

- [ ] **A)** Speeds up simple lookups on that field
- [ ] **B)** Speeds up queries with multiple filter fields
- [ ] **C)** Automatically created on the _id field
- [ ] **D)** Designed only for sorting results

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A single-field index speeds up equality and range queries on one key. It is the foundational performance tool but does not directly optimize queries that filter on multiple fields.
 
 
</details>

### 29. Which conditions are required for a TTL index to automatically remove documents after they expire? Select all that apply.

- [ ] **A)** Requires a single BSON date or date-array field
- [ ] **B)** Works with integer Unix timestamps
- [ ] **C)** Runs a background thread every 60 seconds
- [ ] **D)** Can be part of a compound index

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> TTL indexes require a single date or date-array field. A background thread runs every 60 seconds to delete expired documents, so integer timestamps and compound TTL indexes are not supported.
 
 
</details>

### 30. Review the compound index definition in the code block. According to the Prefix Rule, which query can benefit from this index?

```javascript
db.collection.createIndex(
  { a: 1, b: 1 }
)
```

- [ ] **A)** Filters only on the leading field
- [ ] **B)** Filters only on the second field
- [ ] **C)** Filters only on an unrelated field
- [ ] **D)** Requires no filter fields

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Prefix Rule states that a compound index supports queries on its leftmost leading fields. A filter on the second field alone cannot use the index efficiently.
 
 
</details>

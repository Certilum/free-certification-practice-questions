<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Amazon%20Web%20Services%20Training%20and%20Certification/AWS%20Certified%20Developer%20%E2%80%93%20Associate

" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>AWS Certified Developer – Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Deployment](#deployment) (7 questions)
- [Development with AWS Services](#development-with-aws-services) (10 questions)
- [Security](#security) (8 questions)
- [Troubleshooting and Optimization](#troubleshooting-and-optimization) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:03.294Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Deployment | 7 |
| Development with AWS Services | 10 |
| Security | 8 |
| Troubleshooting and Optimization | 5 |

---

### **Deployment**

### 1. In DynamoDB, what is the main role of the partition key when the service stores an item?

- [ ] **A)** Uses a hash to locate partition
- [ ] **B)** Sorts items within a partition
- [ ] **C)** Replicates data across regions
- [ ] **D)** Sets read and write capacity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The partition key is hashed to identify the physical partition that stores the item. This enables data distribution.
 
 
</details>

### 2. Which statements correctly describe the main differences between provisioned and on-demand capacity modes in DynamoDB?

- [ ] **A)** Provisioned requires specifying RCU/WCU
- [ ] **B)** On-demand scales automatically for spikes
- [ ] **C)** On-demand is always cheapest
- [ ] **D)** Provisioned suits unpredictable workloads

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Provisioned mode requires defined capacity; on-demand mode scales automatically. On-demand is not always cheaper, and provisioned mode suits predictable workloads.
 
 
</details>

### 3. Study the Python snippet and determine which DynamoDB feature is being implemented by the update operation.

```python
table.update_item(
    Key={'id': '123'},
    UpdateExpression='SET #v = #v + :inc',
    ConditionExpression='attribute_not_exists(#v) OR #v = :expected',
    ExpressionAttributeNames={'#v': 'version'},
    ExpressionAttributeValues={':inc': 1, ':expected': 2}
)
```

- [ ] **A)** Optimistic locking with condition expressions
- [ ] **B)** Eventually consistent read request
- [ ] **C)** Global secondary index query
- [ ] **D)** DynamoDB Streams processing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The version check in the condition expression prevents concurrent writes from overwriting each other, a pattern known as optimistic locking.
 
 
</details>

### 4. What does the sort key in DynamoDB allow you to do with items that share the same partition key?

- [ ] **A)** Ordered grouping and range queries
- [ ] **B)** Cross-region data replication
- [ ] **C)** Automatic item expiration
- [ ] **D)** Capacity scaling across partitions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A sort key organizes items under the same partition key, enabling ordered grouping and range queries such as begins_with and between.
 
 
</details>

### 5. Which statements correctly compare Global Secondary Indexes with Local Secondary Indexes in DynamoDB tables? Select all that apply.

- [ ] **A)** GSIs can be added later
- [ ] **B)** LSIs share the table partition key
- [ ] **C)** LSIs can use a different partition key
- [ ] **D)** GSIs must be created with the table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> GSIs can be created anytime and may use a different partition key; LSIs must be created with the table and share its partition key.
 
 
</details>

### 6. Consider the Python snippet and state what purpose the generated URL serves for a private Amazon S3 object.

```python
import boto3
s3 = boto3.client('s3')
url = s3.generate_presigned_url('get_object',
                                Params={'Bucket': 'my-bucket', 'Key': 'report.pdf'},
                                ExpiresIn=300)
```

- [ ] **A)** Grants temporary access without credentials
- [ ] **B)** Permanently makes object public
- [ ] **C)** Applies lifecycle management rule
- [ ] **D)** Replicates object to another bucket

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A pre-signed URL grants temporary access to a private object without requiring the user to possess AWS credentials.
 
 
</details>

### 7. What consistency model does Amazon S3 provide for both new object puts and object overwrites?

- [ ] **A)** Strong read-after-write consistency
- [ ] **B)** Eventual consistency only
- [ ] **C)** No consistency guarantee
- [ ] **D)** Consistent only for new objects

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> S3 delivers strong read-after-write consistency for all applications, including overwrites and new puts, so no polling logic is needed.
 
 
</details>


---

### **Development with AWS Services**

### 8. What is the primary responsibility of a Partition Key (PK) in a DynamoDB table?

- [ ] **A)** It generates secondary indexes
- [ ] **B)** It uses a hash function to determine the physical partition where data is stored
- [ ] **C)** It uniquely identifies each item in a multi-Region replica
- [ ] **D)** It automatically orders items by their timestamp

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The partition key is hashed to determine which physical partition stores the item. It does not create indexes or order items on its own.
 
 
</details>

### 9. Which statements about DynamoDB Global Secondary Indexes (GSIs) are true? (Select two.)

- [ ] **A)** GSIs can be created after the table has been created
- [ ] **B)** GSIs must share the same partition key as the base table
- [ ] **C)** GSIs allow queries on attributes that are not part of the primary key
- [ ] **D)** GSIs can only be created during initial table creation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Unlike LSIs, GSIs can be created at any time and may use a different partition key; they project data for querying non-primary-key attributes.
 
 
</details>

### 10. Review the DynamoDB code snippet. What is the consequence of setting ConsistentRead to True?

```python
response = table.get_item(
    Key={'id': '123'},
    ConsistentRead=True
)
```

- [ ] **A)** It reduces the read cost of the operation
- [ ] **B)** It ensures the returned item reflects the most recent write
- [ ] **C)** It allows reading attributes that are not part of the primary key
- [ ] **D)** It enables auto-scaling for the table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Strongly consistent reads return the latest committed data, but they cost more and may have higher latency than eventually consistent reads.
 
 
</details>

### 11. In DynamoDB On-Demand mode, how is read/write capacity handled?

- [ ] **A)** You must provision RCU and WCU manually
- [ ] **B)** It automatically scales to accommodate sudden traffic spikes
- [ ] **C)** It supports a maximum of 300 transactions per second
- [ ] **D)** It requires a DynamoDB Streams trigger

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> On-Demand mode automatically adjusts capacity for unpredictable workloads, removing the need to manage RCU/WCU manually.
 
 
</details>

### 12. Which statements about DynamoDB Streams are correct? (Select two.)

- [ ] **A)** They capture a time-ordered sequence of item-level changes
- [ ] **B)** They can trigger Lambda functions for event-driven processing
- [ ] **C)** They automatically create Global Secondary Indexes
- [ ] **D)** They are only available on tables using provisioned capacity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Streams capture item-level changes in time order and can invoke Lambda for event-driven architectures. They do not create indexes or depend on capacity mode.
 
 
</details>

### 13. Given this DynamoDB update with a version condition, what happens if another process has already changed the version?

```python
table.update_item(
    Key={'id': '123'},
    UpdateExpression='SET status = :new',
    ConditionExpression='version = :expected',
    ExpressionAttributeValues={
        ':new': 'shipped',
        ':expected': 5
    }
)
```

- [ ] **A)** The write succeeds because conditions are optional
- [ ] **B)** The write fails, preserving data integrity
- [ ] **C)** The item is overwritten with the new version
- [ ] **D)** DynamoDB automatically increments the version

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The condition expression acts as optimistic locking; if the version attribute does not match the expected value, the update is rejected.
 
 
</details>

### 14. According to AWS best practices, which statement about S3 Glacier retrieval is correct?

- [ ] **A)** All Glacier storage classes provide instant retrieval
- [ ] **B)** Instant Retrieval and Flexible/Deep Archive have the same retrieval latency
- [ ] **C)** Only some Glacier classes are designed for instant retrieval; others take minutes to hours
- [ ] **D)** Glacier retrieval is always measured in milliseconds

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Glacier storage classes vary: Instant Retrieval is for rapid access, while Flexible and Deep Archive involve longer retrieval times. Do not assume uniform latency.
 
 
</details>

### 15. Which S3 features help protect data against accidental deletes and optimize storage costs? (Select two.)

- [ ] **A)** Object Versioning to keep multiple variants of objects
- [ ] **B)** Pre-signed URLs to allow anonymous public writes
- [ ] **C)** S3 Lifecycle Management to transition objects to lower-cost storage classes
- [ ] **D)** Bucket deletion policies to remove unused buckets automatically

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Versioning preserves object variants and allows recovery from accidental deletes or overwrites; lifecycle rules automate transitions or expirations to reduce costs.
 
 
</details>

### 16. Review the code for generating a URL. What does this function allow an end user to do?

```python
url = s3.generate_presigned_url(
    ClientMethod='get_object',
    Params={'Bucket': 'my-bucket', 'Key': 'report.pdf'},
    ExpiresIn=300
)
```

- [ ] **A)** It makes the object permanently public
- [ ] **B)** It grants temporary access to download the object for 300 seconds
- [ ] **C)** It allows the user to delete the object
- [ ] **D)** It creates a new S3 bucket

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A pre-signed URL grants time-limited access to a private object; here, a GET URL is valid for 300 seconds.
 
 
</details>

### 17. Which statement describes S3's consistency model?

- [ ] **A)** S3 provides strong read-after-write consistency for all applications
- [ ] **B)** S3 is eventually consistent for all reads
- [ ] **C)** S3 reads require a pre-signed URL to be consistent
- [ ] **D)** Consistency is only guaranteed if versioning is enabled

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> S3 now provides strong read-after-write consistency for both new PUTs and overwrites, so developers should not add unnecessary polling or propagation handling.
 
 
</details>


---

### **Security**

### 18. In DynamoDB, what is the primary purpose of the Sort Key within a composite primary key?

- [ ] **A)** Ordered grouping and range queries
- [ ] **B)** Hashing data across partitions
- [ ] **C)** Encrypting items at rest
- [ ] **D)** Replacing the partition key for all queries

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Sort Key enables ordered grouping of items under the same Partition Key and supports range queries using operators like begins_with or between.
 
 
</details>

### 19. Which statements accurately describe DynamoDB read consistency models?

- [ ] **A)** Eventually Consistent reads are the default and lower cost
- [ ] **B)** Strongly Consistent reads return the latest data
- [ ] **C)** Strongly Consistent reads have higher cost
- [ ] **D)** Strongly Consistent reads are always the best choice

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Eventually Consistent reads are the default and less expensive; Strongly Consistent reads return the most recent data but cost more.
 
 
</details>

### 20. A developer uses the following DynamoDB call. What behavior does the ConditionExpression enforce?

```python
dynamodb.put_item(
    TableName='Products',
    Item={'id': {'S': 'p100'}, 'stock': {'N': '10'}},
    ConditionExpression='attribute_not_exists(id)'
)
```

- [ ] **A)** Write only succeeds if the item key does not already exist
- [ ] **B)** Write always succeeds and overwrites the existing item
- [ ] **C)** Write succeeds only if the item has never been read
- [ ] **D)** Write fails if the partition key has a sort key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> attribute_not_exists(id) makes the write atomic: the PutItem succeeds only when no item with that key exists, preventing unintended overwrites.
 
 
</details>

### 21. What is the intended purpose of an S3 pre-signed URL?

- [ ] **A)** Grant time-limited access to private objects
- [ ] **B)** Make objects permanently public
- [ ] **C)** Transition objects to Glacier
- [ ] **D)** Replicate objects across regions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Pre-signed URLs grant temporary access to private S3 objects without requiring the end user to have AWS credentials.
 
 
</details>

### 22. Which actions can S3 Lifecycle Management automate for developers?

- [ ] **A)** Transition objects between storage classes
- [ ] **B)** Expire objects after a retention period
- [ ] **C)** Trigger Lambda on object upload
- [ ] **D)** Provide strong read-after-write consistency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> S3 Lifecycle Management automates storage class transitions and object expiration to optimize cost and retention.
 
 
</details>

### 23. Given this S3 Select query, what is the primary benefit over downloading the entire object?

```sql
SELECT name
FROM s3object s
WHERE s.age >= 21
```

- [ ] **A)** Filter data at the storage layer to reduce latency and bandwidth
- [ ] **B)** Create a new S3 bucket automatically
- [ ] **C)** Transition the object to a colder storage class
- [ ] **D)** Enable versioning on the S3 bucket

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> S3 Select filters data at the storage layer before sending it to the application, reducing latency and network bandwidth.
 
 
</details>

### 24. What does a DynamoDB Stream capture?

- [ ] **A)** Time-ordered sequence of item-level changes
- [ ] **B)** Read request logs for a table
- [ ] **C)** A list of all IAM users
- [ ] **D)** A static backup stored in S3

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> DynamoDB Streams captures a time-ordered sequence of item-level changes, enabling event-driven architectures.
 
 
</details>

### 25. Which statements correctly compare Step Functions Standard and Express workflows?

- [ ] **A)** Standard workflows are for long-running, auditable, exactly-once
- [ ] **B)** Express workflows are for high-volume, short-duration, at-least-once
- [ ] **C)** Express workflows are ideal for long-running audits
- [ ] **D)** Standard workflows always have lower latency than Express

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Standard workflows provide exactly-once execution for long-running processes; Express workflows handle high-volume, short-duration tasks with at-least-once execution.
 
 
</details>


---

### **Troubleshooting and Optimization**

### 26. In Amazon DynamoDB, what is the primary role of the Partition Key in data distribution?

- [ ] **A)** It hashes the key to select a partition.
- [ ] **B)** It groups items in sorted order.
- [ ] **C)** It replicates items across Availability Zones.
- [ ] **D)** It chooses the read consistency model.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Partition Key is hashed by DynamoDB to determine the physical partition where the item is stored. Sort keys provide ordered grouping.
 
 
</details>

### 27. Which statements about Global Secondary Indexes (GSIs) and Local Secondary Indexes (LSIs) are correct?

- [ ] **A)** GSIs can be created after table creation.
- [ ] **B)** LSIs must be defined at table creation.
- [ ] **C)** LSIs can use a different partition key.
- [ ] **D)** GSIs must share the base table partition key.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> GSIs can be created anytime and use any partition key. LSIs are fixed at creation and share the base table partition key.
 
 
</details>

### 28. Given the DynamoDB code snippet, what does the ConditionExpression ensure?

```python
try:
    table.update_item(
        Key={'id': '123'},
        UpdateExpression='SET price = :new_price',
        ConditionExpression='attribute_not_exists(price)',
        ExpressionAttributeValues={':new_price': 100}
    )
except dynamodb.meta.client.exceptions.ConditionalCheckFailedException:
    print('Item already has a price set')
```

- [ ] **A)** Updates only when the price attribute is absent.
- [ ] **B)** It prevents updates after item creation.
- [ ] **C)** It requires a positive price value.
- [ ] **D)** It deletes items with a price present.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The condition attribute_not_exists(price) makes the update succeed only when the price attribute is missing. This prevents overwrites atomically, avoiding a separate read-then-write step.
 
 
</details>

### 29. Which DynamoDB read option is most cost-effective when slightly stale data is acceptable?

- [ ] **A)** Eventually Consistent Reads
- [ ] **B)** Strongly Consistent Reads
- [ ] **C)** Transactional Reads
- [ ] **D)** Batch Reads

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Eventually consistent reads are the default and use fewer resources, reducing cost and latency. Strongly consistent reads cost more and always return the latest data.
 
 
</details>

### 30. Which use cases are well suited to DynamoDB Streams?

- [ ] **A)** Reacting to item changes with a Lambda function
- [ ] **B)** Capturing a time-ordered sequence of item-level changes
- [ ] **C)** Replacing a Global Secondary Index for queries
- [ ] **D)** Providing strongly consistent reads for all access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DynamoDB Streams capture ordered item-level changes and can trigger Lambda for event-driven workflows. They do not replace GSIs or provide read consistency.
 
 
</details>

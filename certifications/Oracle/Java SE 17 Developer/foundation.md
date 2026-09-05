<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Java%20SE%2017%20Developer.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Java SE 17 Developer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Arrays and Collections](#arrays-and-collections) (3 questions)
- [Concurrency](#concurrency) (4 questions)
- [Controlling Program Flow](#controlling-program-flow) (1 questions)
- [Handling Date, Time, Text, Numeric and Boolean Values](#handling-date-time-text-numeric-and-boolean-values) (2 questions)
- [Handling Exceptions](#handling-exceptions) (2 questions)
- [I/O and NIO.2](#i-o-and-nio-2) (2 questions)
- [JDBC](#jdbc) (2 questions)
- [Localization](#localization) (1 questions)
- [Modules and Deployment](#modules-and-deployment) (2 questions)
- [Object-Oriented Concepts](#object-oriented-concepts) (6 questions)
- [Streams and Lambda Expressions](#streams-and-lambda-expressions) (4 questions)
- [Supplementary Topics](#supplementary-topics) (1 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:47.523Z |
| Domains | 12 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Arrays and Collections | 3 |
| Concurrency | 4 |
| Controlling Program Flow | 1 |
| Handling Date, Time, Text, Numeric and Boolean Values | 2 |
| Handling Exceptions | 2 |
| I/O and NIO.2 | 2 |
| JDBC | 2 |
| Localization | 1 |
| Modules and Deployment | 2 |
| Object-Oriented Concepts | 6 |
| Streams and Lambda Expressions | 4 |
| Supplementary Topics | 1 |

---

### **Arrays and Collections**

### 1. Why is it critical to close JDBC resources such as Connection, Statement, and ResultSet in a finally block or with try-with-resources?

- [ ] **A)** To release database resources and prevent leaks
- [ ] **B)** To make the SQL statement execute faster
- [ ] **C)** To automatically commit the transaction
- [ ] **D)** To increase the number of returned rows

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Unclosed JDBC resources hold database connections and network resources. Closing them in a finally block or using try-with-resources prevents exhausting the connection pool.
 
 
</details>

### 2. Which of the following situations are described in the JDBC playbook as common traps? (Choose all that apply.)

- [ ] **A)** Assuming JDBC URLs follow normal URI syntax
- [ ] **B)** Forgetting to register OUT parameters in a CallableStatement
- [ ] **C)** Reading a ResultSet after re-executing the Statement
- [ ] **D)** Closing JDBC resources with try-with-resources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The URL syntax trap, unregistered OUT parameters, and ResultSet scope are listed as traps. Closing resources properly is a recommended practice, not a mistake.
 
 
</details>

### 3. In the code shown, a boolean value is assigned after an SQL query is executed. What does that boolean represent?

```java
String sql = "SELECT id, name FROM employee";
Statement stmt = connection.createStatement();
boolean hasResultSet = stmt.execute(sql);
if (hasResultSet) {
    ResultSet rs = stmt.getResultSet();
}
```

- [ ] **A)** It indicates a ResultSet was produced
- [ ] **B)** It indicates the affected row count
- [ ] **C)** It indicates the connection is open
- [ ] **D)** It indicates the SQL was formatted correctly

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In JDBC, execute() returns a boolean. A true value means the first result is a ResultSet, while false means there was no result set or it was an update count.
 
 
</details>


---

### **Concurrency**

### 4. Which group of JDBC objects must be explicitly closed after use to prevent a database resource leak?

- [ ] **A)** Connection, Statement, ResultSet
- [ ] **B)** Connection, DriverManager, DatabaseMetaData
- [ ] **C)** Statement, ResultSet, Driver
- [ ] **D)** Connection, PrintWriter, Statement

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Closing Connection, Statement, and ResultSet releases database resources; DriverManager, Driver, and PrintWriter do not represent JDBC resources to close.
 
 
</details>

### 5. Which statements about JDBC URLs are correct with respect to the connection string syntax supported by database drivers?

- [ ] **A)** Every JDBC URL begins with the prefix `jdbc:` followed by a driver-specific subprotocol.
- [ ] **B)** All JDBC drivers require the exact same subname format after the subprotocol.
- [ ] **C)** JDBC URL syntax is defined by the driver vendor and is not required to follow standard URI rules.
- [ ] **D)** `jdbc:mysql://localhost:3306/books` is an accepted form of JDBC URL for MySQL.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> JDBC URLs begin with jdbc: and a driver-specific subprotocol; the remainder is driver-defined and may not comply with standard URI syntax.
 
 
</details>

### 6. Given the driver-loading code, which statement best describes the use of Class.forName when the driver on the classpath is JDBC 4.0+ compliant?

```java
try {
    Class.forName("com.mysql.cj.jdbc.Driver");
} catch (ClassNotFoundException e) {
    e.printStackTrace();
}
String url = "jdbc:mysql://localhost:3306/books";
Connection conn = DriverManager.getConnection(url, "user", "pass");
```

- [ ] **A)** It is optional because DriverManager can discover JDBC 4.0+ drivers automatically from the classpath.
- [ ] **B)** It is mandatory even for JDBC 4.0+ drivers.
- [ ] **C)** It must be executed after a connection is opened.
- [ ] **D)** It is required to release the driver at the end of the program.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> JDBC 4.0+ drivers on the classpath are registered automatically, so a manual Class.forName call is not required.
 
 
</details>

### 7. When Statement.executeUpdate() is called for an UPDATE, DELETE, or INSERT statement, what type of value is returned to the caller?

- [ ] **A)** boolean
- [ ] **B)** int representing the affected row count
- [ ] **C)** ResultSet with generated keys
- [ ] **D)** void

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> executeUpdate() returns an int. For UPDATE, DELETE, and INSERT statements, the int is the number of affected rows.
 
 
</details>


---

### **Controlling Program Flow**

### 8. In JDBC, what is the accurate difference between the return type of execute() and the return type of executeUpdate()?

- [ ] **A)** execute() returns boolean; executeUpdate() returns int.
- [ ] **B)** execute() returns int; executeUpdate() returns boolean.
- [ ] **C)** execute() returns ResultSet; executeUpdate() returns boolean.
- [ ] **D)** execute() returns long; executeUpdate() returns boolean.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> execute() returns a boolean that indicates whether the first result is a ResultSet. executeUpdate() returns an int indicating the number of affected rows. Mixing up these return types is a common JDBC trap.
 
 
</details>


---

### **Handling Date, Time, Text, Numeric and Boolean Values**

### 9. Which JDBC Statement method returns a boolean value to show whether the SQL produced a ResultSet?

- [ ] **A)** Statement.execute()
- [ ] **B)** Statement.executeQuery()
- [ ] **C)** Statement.executeUpdate()
- [ ] **D)** Connection.prepareStatement()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Statement.execute() returns true when SQL produces a ResultSet and false otherwise. executeQuery() returns ResultSet; executeUpdate() returns int.
 
 
</details>

### 10. Which JDBC objects should be closed after your database work is complete to prevent resource leaks? Select all that apply.

- [ ] **A)** Connection
- [ ] **B)** Statement
- [ ] **C)** ResultSet
- [ ] **D)** DriverManager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Connection, Statement, and ResultSet all hold database resources and should be closed, ideally in a try-with-resources block. DriverManager is a manager class and should not be closed.
 
 
</details>


---

### **Handling Exceptions**

### 11. Which practice prevents resource leaks when a JDBC `Connection`, `Statement`, or `ResultSet` is used and an exception occurs during processing?

- [ ] **A)** Use `try-with-resources` to close all JDBC resources.
- [ ] **B)** Close only the `ResultSet` after executing the query.
- [ ] **C)** Set each JDBC resource to `null` after use.
- [ ] **D)** Rely on the garbage collector to free JDBC resources.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> `try-with-resources` closes all declared JDBC resources when the `try` block exits normally or by exception. Manually closing only the ResultSet or relying on garbage collection can cause resource leaks.
 
 
</details>

### 12. Which statements correctly describe the JDBC driver-loading trap and the exception that can occur when a driver class is not found?

- [ ] **A)** `Class.forName` was required in older JDBC.
- [ ] **B)** `Class.forName` throws `ClassNotFoundException` if the class is absent.
- [ ] **C)** Modern JDBC auto-registers drivers from the classpath.
- [ ] **D)** `Class.forName` is mandatory after JDBC 4.0.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Older JDBC required `Class.forName` for driver loading. Modern JDBC auto-registers drivers from the classpath. A missing driver class makes `Class.forName` throw `ClassNotFoundException`; manual loading is unnecessary after JDBC 4.0.
 
 
</details>


---

### **I/O and NIO.2**

### 13. Which statement accurately describes how JDBC drivers are loaded in JDBC 4.0 and later versions?

- [ ] **A)** The driver is automatically discovered and loaded using the service provider mechanism.
- [ ] **B)** The driver must always be loaded with Class.forName before it can be used.
- [ ] **C)** The driver must be manually instantiated and passed to the DriverManager.
- [ ] **D)** The driver is loaded automatically only when the URL begins with http.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In JDBC 4.0, drivers are loaded from the classpath by the service provider mechanism, making explicit driver loading optional.
 
 
</details>

### 14. Which three JDBC objects must be closed after use to avoid database resource leaks? Select all that apply.

- [ ] **A)** Connection
- [ ] **B)** Statement
- [ ] **C)** ResultSet
- [ ] **D)** DriverManager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Connection, Statement, and ResultSet must be closed to free database resources. DriverManager does not implement AutoCloseable and is not closed directly.
 
 
</details>


---

### **JDBC**

### 15. Which return type is correct for the execute() method of a Statement?

- [ ] **A)** boolean
- [ ] **B)** int
- [ ] **C)** ResultSet
- [ ] **D)** long

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The execute() method returns a boolean, indicating whether the SQL produced a ResultSet. In contrast, executeUpdate() returns an int affected row count.
 
 
</details>

### 16. Which two steps are required to retrieve an OUT parameter from a stored procedure with CallableStatement?

- [ ] **A)** Call registerOutParameter() before execution
- [ ] **B)** Retrieve value with the appropriate getter after execution
- [ ] **C)** Call registerOutParameter() after execution
- [ ] **D)** Use ResultSet.next() to retrieve the value

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OUT parameters must be registered with registerOutParameter() before the procedure is executed. After execution, the value is retrieved using an appropriate getter method.
 
 
</details>


---

### **Localization**

### 17. In JDBC, what does the executeUpdate() method return when it successfully performs an INSERT, UPDATE, or DELETE statement?

- [ ] **A)** A boolean true or false
- [ ] **B)** A ResultSet object
- [ ] **C)** An int containing the row count
- [ ] **D)** A Connection object

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> executeUpdate() returns an int indicating the number of rows affected. execute() returns a boolean, while executeQuery() returns a ResultSet.
 
 
</details>


---

### **Modules and Deployment**

### 18. Which practice is most likely to cause a JDBC resource leak according to the documented common traps?

- [ ] **A)** Leaving JDBC resources unclosed
- [ ] **B)** Closing resources in a finally block
- [ ] **C)** Using try-with-resources
- [ ] **D)** Registering output parameters before calls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A resource leak occurs when JDBC objects such as Connection or Statement are not closed. Developers often focus on SQL logic and overlook these resources.
 
 
</details>

### 19. Based on the common JDBC traps described in the source, which two of the following actions are recognized as pitfalls?

- [ ] **A)** Using a ResultSet outside its valid scope
- [ ] **B)** Closing resources with try-with-resources
- [ ] **C)** Assuming JDBC URLs follow standard URI syntax only
- [ ] **D)** Registering OUT parameters before calling the procedure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The source identifies the ResultSet scope and JDBC URL syntax as common traps. Registering OUT parameters and using try-with-resources are proper, recommended practices.
 
 
</details>


---

### **Object-Oriented Concepts**

### 20. Why must JDBC objects such as Connection, Statement, and ResultSet be closed after use in a database application?

- [ ] **A)** To prevent database resource leaks
- [ ] **B)** To make SQL compile faster
- [ ] **C)** To ensure the driver is loaded
- [ ] **D)** To validate the JDBC URL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> These objects hold underlying database resources; failure to close them can exhaust database connections and degrade application performance.
 
 
</details>

### 21. Resource management is important in JDBC programs. Which two statements correctly describe JDBC resource management?

- [ ] **A)** try-with-resources automatically closes declared JDBC resources.
- [ ] **B)** Resource leaks can consume available database connections.
- [ ] **C)** JDBC resources should never be closed manually.
- [ ] **D)** Closing a single Statement also closes the Connection automatically.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> JDBC resources should be explicitly closed, ideally with try-with-resources, because each open resource consumes a limited database connection.
 
 
</details>

### 22. Look at the connection string in the code block. Which segment is the JDBC subprotocol?

```java
String url = "jdbc:mysql://localhost:3306/school";
```

- [ ] **A)** mysql
- [ ] **B)** jdbc
- [ ] **C)** localhost:3306/school
- [ ] **D)** school

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In a JDBC URL of the form jdbc:subprotocol:subname, the subprotocol appears immediately after the jdbc: prefix.
 
 
</details>

### 23. In modern JDBC drivers, how is the appropriate driver normally discovered when a database connection is requested?

- [ ] **A)** Detected automatically through ServiceLoader
- [ ] **B)** It must be loaded using an explicit driver class
- [ ] **C)** The developer manually creates the driver instance
- [ ] **D)** It is registered by executing a special command

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> JDBC 4+ uses ServiceLoader to find driver implementations on the classpath automatically, so Class.forName is not required in most cases.
 
 
</details>

### 24. In JDBC, which two statements correctly describe the return types of execute and executeUpdate when used to run SQL?

- [ ] **A)** execute() returns a boolean value.
- [ ] **B)** executeUpdate() returns an int row count.
- [ ] **C)** execute() returns the number of affected rows.
- [ ] **D)** executeUpdate() returns a ResultSet.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> execute indicates whether the first result is a ResultSet, while executeUpdate returns an int for insert, update, delete, or DDL.
 
 
</details>

### 25. Consider the code block. What does the boolean value from the first execution imply?

```java
Connection conn = DriverManager.getConnection(url, user, password);
Statement stmt = conn.createStatement();
boolean hasResultSet = stmt.execute("SELECT * FROM students");
if (hasResultSet) {
    ResultSet rs = stmt.getResultSet();
}
int affectedRows = stmt.executeUpdate("DELETE FROM students WHERE id = 1");
```

- [ ] **A)** The first SQL result is a ResultSet.
- [ ] **B)** The first SQL was a DELETE that affected rows.
- [ ] **C)** The database connection is invalid.
- [ ] **D)** The driver cannot handle the SQL type.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> execute returns true only when the first result is a ResultSet; false means an update count or no result.
 
 
</details>


---

### **Streams and Lambda Expressions**

### 26. Which Java construct automatically closes JDBC resources such as Connection, Statement, and ResultSet when the code block finishes?

- [ ] **A)** Use try-with-resources and declare the resources in its parentheses.
- [ ] **B)** Create each resource inside a private constructor and await finalization.
- [ ] **C)** Use a finally block without calling close in it.
- [ ] **D)** Rely on the ResultSet to close the Connection automatically.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> try-with-resources closes each resource automatically when the try block exits, preventing the resource leak that happens when close calls are forgotten.
 
 
</details>

### 27. When you are building a database connection string in JDBC, which two statements correctly describe the parts that make up the URL?

- [ ] **A)** A JDBC URL starts with the prefix `jdbc:`.
- [ ] **B)** After `jdbc:` come a subprotocol and a subname.
- [ ] **C)** The subprotocol always matches the driver vendor's website.
- [ ] **D)** JDBC URLs must start with `https://` to be accepted.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A JDBC URL has the form `jdbc:<subprotocol>:<subname>`. The subprotocol identifies the driver mechanism, and the subname carries database-specific information; `https://` is not a JDBC connection form.
 
 
</details>

### 28. In the provided code, what is true about the line that loads the driver class for this JDBC 4.0-compliant driver?

```java
public class JdbcConnection {
    public static void main(String[] args) throws Exception {
        Class.forName("com.mysql.cj.jdbc.Driver");
        try (var con = DriverManager.getConnection(
                "jdbc:mysql://localhost:3306/shop", "root", "pass")) {
            System.out.println("Connected");
        }
    }
}
```

- [ ] **A)** It is still mandatory for every JDBC driver in Java 17.
- [ ] **B)** It is optional because DriverManager can discover JDBC 4.0 drivers from the classpath.
- [ ] **C)** It allows the program to connect without producing a Connection object.
- [ ] **D)** It removes the need to provide host information in the JDBC URL.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Because the driver jar is on the classpath and implements JDBC 4.0, DriverManager loads it automatically through the service-provider mechanism; manual class loading is optional.
 
 
</details>

### 29. Which JDBC method should be used to obtain the number of rows affected by an UPDATE statement?

- [ ] **A)** `executeUpdate()` returns an int with the number of affected rows.
- [ ] **B)** `execute()` returns an int with the number of affected rows.
- [ ] **C)** `executeQuery()` returns an int with the number of affected rows.
- [ ] **D)** `registerOutParameter()` returns an int with the number of affected rows.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> executeUpdate() returns the row count for INSERT, UPDATE, DELETE, and DDL statements. execute() returns a boolean, executeQuery() returns a ResultSet, and registerOutParameter() is used with CallableStatement.
 
 
</details>


---

### **Supplementary Topics**

### 30. According to common JDBC traps, which method of a Statement returns a boolean value?

- [ ] **A)** execute()
- [ ] **B)** executeUpdate()
- [ ] **C)** executeQuery()
- [ ] **D)** executeBatch()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In JDBC, execute() returns a boolean indicating whether the first result is a ResultSet. executeUpdate() returns an int, and executeQuery() returns a ResultSet.
 
 
</details>

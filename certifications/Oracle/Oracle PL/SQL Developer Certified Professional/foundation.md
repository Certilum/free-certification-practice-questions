<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Oracle%20PL%3ASQL%20Developer%20Certified%20Professional.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Oracle PL/SQL Developer Certified Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Code Management](#code-management) (3 questions)
- [Dynamic SQL and Advanced Topics](#dynamic-sql-and-advanced-topics) (5 questions)
- [Exception Handling](#exception-handling) (3 questions)
- [PL/SQL Fundamentals](#pl-sql-fundamentals) (5 questions)
- [SQL in PL/SQL](#sql-in-pl-sql) (3 questions)
- [Subprograms and Packages](#subprograms-and-packages) (6 questions)
- [Working with Data](#working-with-data) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:46:36.320Z |
| Domains | 7 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Code Management | 3 |
| Dynamic SQL and Advanced Topics | 5 |
| Exception Handling | 3 |
| PL/SQL Fundamentals | 5 |
| SQL in PL/SQL | 3 |
| Subprograms and Packages | 6 |
| Working with Data | 5 |

---

### **Code Management**

### 1. Which SQL construct is used in a PL/SQL block to put the result of a single-row query into local variables?

- [ ] **A)** SELECT INTO statement
- [ ] **B)** OPEN-FOR statement
- [ ] **C)** EXECUTE IMMEDIATE statement
- [ ] **D)** NULLIF function

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A single-row query is embedded in PL/SQL with SELECT INTO. The INTO clause names the variables that receive the selected column values.
 
 
</details>

### 2. Which statements are true about static SQL embedded directly in a PL/SQL block?

- [ ] **A)** It is parsed at compile time.
- [ ] **B)** It can execute DML statements.
- [ ] **C)** Its SQL text is determined at run time.
- [ ] **D)** It must always use EXECUTE IMMEDIATE.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Static SQL is parsed at compile time and supports DML statements directly. The SQL text is fixed at compile time and does not require dynamic SQL.
 
 
</details>

### 3. Review the supplied PL/SQL block. Which missing keyword should replace the blank so the selected values are assigned to the declared variables?

```sql
DECLARE
   v_name   employees.last_name%TYPE;
   v_salary employees.salary%TYPE;
BEGIN
   SELECT last_name, salary
      ___ v_name, v_salary
     FROM employees
    WHERE employee_id = 100;
END;
```

- [ ] **A)** INTO
- [ ] **B)** WHERE
- [ ] **C)** SET
- [ ] **D)** FROM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The INTO clause is required in a SELECT embedded in PL/SQL when values must be assigned to local variables.
 
 
</details>


---

### **Dynamic SQL and Advanced Topics**

### 4. Which PL/SQL feature permits SQL statements to be constructed and executed at the time the program is running?

- [ ] **A)** Static SQL
- [ ] **B)** Dynamic SQL
- [ ] **C)** Embedded SQL
- [ ] **D)** Cursor expression

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Dynamic SQL lets a PL/SQL program build and process SQL statements at run time. Static SQL is compiled when the PL/SQL unit is compiled, so it cannot change at run time.
 
 
</details>

### 5. Which two statements are true about the EXECUTE IMMEDIATE statement in PL/SQL native dynamic SQL? (Choose two.)

- [ ] **A)** It is the main statement used for native dynamic SQL.
- [ ] **B)** It can be used to execute DDL statements such as CREATE TABLE.
- [ ] **C)** It is required for every static SELECT in PL/SQL.
- [ ] **D)** It displays the row results of a SELECT in the console.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> EXECUTE IMMEDIATE is the native dynamic SQL statement in PL/SQL. It can execute DDL statements and supports bind variables through its USING clause.
 
 
</details>

### 6. Examine the code block. What type of element is used as the placeholder for the value supplied by the USING clause?

```sql
DECLARE
  v_sql VARCHAR2(200);
BEGIN
  v_sql := 'DELETE FROM employees WHERE department_id = :dept_id';
  EXECUTE IMMEDIATE v_sql USING 50;
END;
```

- [ ] **A)** Bind variable placeholder
- [ ] **B)** Cursor attribute
- [ ] **C)** Index value
- [ ] **D)** Schema object name

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A bind variable is written with a leading colon and acts as a placeholder. The USING clause supplies a value at runtime, and this technique also helps prevent SQL injection.
 
 
</details>

### 7. Which Oracle-supplied PL/SQL package provides advanced dynamic SQL functionality beyond the basic EXECUTE IMMEDIATE statement?

- [ ] **A)** DBMS_SQL
- [ ] **B)** DBMS_SCHEDULER
- [ ] **C)** DBMS_JOB
- [ ] **D)** DBMS_PIPE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> DBMS_SQL is the Oracle-supplied package for advanced dynamic SQL. It is used when dynamic SQL support beyond EXECUTE IMMEDIATE is needed, such as an unknown number of selected columns.
 
 
</details>

### 8. Which two kinds of SQL statements usually require dynamic SQL in PL/SQL because they cannot be written as static SQL? (Choose two.)

- [ ] **A)** DDL statements such as CREATE INDEX
- [ ] **B)** Session-control statements such as ALTER SESSION
- [ ] **C)** Fixed SELECT statements whose table and column names are already known
- [ ] **D)** Simple UPDATE statements with a known WHERE clause

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DDL and session-control statements cannot be included in static SQL in PL/SQL. DML and well-formed SELECT statements can usually be static when all object names are known.
 
 
</details>


---

### **Exception Handling**

### 9. Which predefined exception is raised when a SELECT INTO statement does not return any rows?

- [ ] **A)** NO_DATA_FOUND
- [ ] **B)** TOO_MANY_ROWS
- [ ] **C)** VALUE_ERROR
- [ ] **D)** ZERO_DIVIDE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A SELECT INTO that returns no rows raises NO_DATA_FOUND. TOO_MANY_ROWS occurs when the statement returns more than one row.
 
 
</details>

### 10. Which two of the following listed options are predefined PL/SQL exception names in Oracle Database?

- [ ] **A)** NO_DATA_FOUND
- [ ] **B)** TOO_MANY_ROWS
- [ ] **C)** CUSTOM_EXCEPTION
- [ ] **D)** TABLE_NOT_FOUND

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> NO_DATA_FOUND and TOO_MANY_ROWS are predefined built-in exceptions. CUSTOM_EXCEPTION and TABLE_NOT_FOUND are not predefined in Oracle PL/SQL.
 
 
</details>

### 11. Assuming server output is enabled, what message is displayed when the code in the code block is run?

```sql
DECLARE
   v_fname employees.first_name%TYPE;
BEGIN
   SELECT first_name
      INTO v_fname
      FROM employees
     WHERE department_id = 9999;

   DBMS_OUTPUT.PUT_LINE('Found one');
EXCEPTION
   WHEN NO_DATA_FOUND THEN
      DBMS_OUTPUT.PUT_LINE('No rows');
END;
/
```

- [ ] **A)** No rows
- [ ] **B)** Found one
- [ ] **C)** ORA-01403: no data found
- [ ] **D)** The block produces no output

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When SELECT INTO finds no matching row, it raises NO_DATA_FOUND, and the exception handler prints 'No rows'. The 'Found one' message is not executed.
 
 
</details>


---

### **PL/SQL Fundamentals**

### 12. Which statement is correct about using a SQL SELECT query inside a PL/SQL block?

- [ ] **A)** It needs an INTO clause to assign values.
- [ ] **B)** It returns rows directly to the screen.
- [ ] **C)** It is not allowed in a PL/SQL block.
- [ ] **D)** It must be executed with an open cursor.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A SELECT used directly in PL/SQL must include an INTO clause when its result is assigned to variables; static SQL does not return rows to the host environment.
 
 
</details>

### 13. Which two SQL statements can be embedded directly in a PL/SQL block as static SQL?

- [ ] **A)** INSERT
- [ ] **B)** CREATE TABLE
- [ ] **C)** DELETE
- [ ] **D)** TRUNCATE TABLE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> INSERT and DELETE are DML statements and can be written directly in PL/SQL as static SQL. CREATE TABLE and TRUNCATE TABLE are DDL and require native dynamic SQL.
 
 
</details>

### 14. In the displayed PL/SQL block, what is the final output?

```plsql
DECLARE
  v_job employees.job_id%TYPE;
BEGIN
  SELECT job_id
    INTO v_job
    FROM employees
   WHERE employee_id = 0;

  DBMS_OUTPUT.PUT_LINE('Found');
EXCEPTION
  WHEN NO_DATA_FOUND THEN
    DBMS_OUTPUT.PUT_LINE('No such employee');
END;
```

- [ ] **A)** No such employee
- [ ] **B)** Found
- [ ] **C)** A syntax error is reported
- [ ] **D)** Nothing is printed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The SELECT INTO returns no row because employee_id 0 is not found, so PL/SQL raises NO_DATA_FOUND and the handler prints the specified message.
 
 
</details>

### 15. Which PL/SQL variable declaration is best for storing the result of a row count query?

- [ ] **A)** v_count NUMBER;
- [ ] **B)** v_count DATE;
- [ ] **C)** v_count BOOLEAN;
- [ ] **D)** v_count employees%ROWTYPE;

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> COUNT and other aggregate functions return numeric values. NUMBER is the best choice among the listed types for storing such a result in PL/SQL.
 
 
</details>

### 16. Which two attributes are valid for an implicit SQL cursor in PL/SQL?

- [ ] **A)** SQL%FOUND
- [ ] **B)** SQL%LASTINSERTID
- [ ] **C)** SQL%ERRORSTATE
- [ ] **D)** SQL%ROWCOUNT

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> SQL%FOUND and SQL%ROWCOUNT are valid implicit cursor attributes in PL/SQL. SQL%LASTINSERTID and SQL%ERRORSTATE are not recognized Oracle PL/SQL attributes.
 
 
</details>


---

### **SQL in PL/SQL**

### 17. In PL/SQL, which class of SQL statements can be embedded directly in a procedural block without dynamic SQL?

- [ ] **A)** Data Definition Language (DDL) statements
- [ ] **B)** Data Control Language (DCL) statements
- [ ] **C)** Data Manipulation Language (DML) statements
- [ ] **D)** Every SQL statement type

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> PL/SQL supplies native support for DML statements and SELECT queries. DDL and DCL are not executed directly; they must be run through dynamic SQL.
 
 
</details>

### 18. Which two of the following are SQL DML operations that can be used directly inside a PL/SQL block?

- [ ] **A)** CREATE INDEX
- [ ] **B)** DELETE
- [ ] **C)** INSERT
- [ ] **D)** GRANT

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> DELETE and INSERT are DML operations that PL/SQL supports natively. CREATE INDEX is DDL, and GRANT is DCL; both require dynamic SQL if used in PL/SQL.
 
 
</details>

### 19. What value is assigned to the variable when this PL/SQL block is run?

```plsql
DECLARE
  v_answer NUMBER;
BEGIN
  SELECT 20 - 4 INTO v_answer FROM dual;
END;
/
```

- [ ] **A)** 20
- [ ] **B)** 24
- [ ] **C)** 16
- [ ] **D)** 4

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The SELECT INTO statement reads from DUAL and evaluates 20 - 4 once. The expression result, 16, is therefore placed into the declared variable.
 
 
</details>


---

### **Subprograms and Packages**

### 20. Which PL/SQL construct retrieves exactly one row from a database table into local variables?

- [ ] **A)** SELECT INTO
- [ ] **B)** FETCH cursor
- [ ] **C)** OPEN FOR cursor
- [ ] **D)** EXECUTE IMMEDIATE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SELECT INTO is the native static SQL statement in PL/SQL for retrieving a single row into scalar variables or a record.
 
 
</details>

### 21. Which SQL statements can be written directly as static SQL inside a PL/SQL subprogram? (Choose all that apply.)

- [ ] **A)** INSERT
- [ ] **B)** UPDATE
- [ ] **C)** SELECT INTO
- [ ] **D)** CREATE TABLE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Static SQL in PL/SQL supports DML and single-row SELECT INTO. DDL such as CREATE TABLE requires dynamic SQL.
 
 
</details>

### 22. Examine the code. If no employee has employee_id 9000, what is displayed?

```plsql
DECLARE
  v_last_name employees.last_name%TYPE;
BEGIN
  SELECT last_name
    INTO v_last_name
    FROM employees
   WHERE employee_id = 9000;
EXCEPTION
  WHEN NO_DATA_FOUND THEN
    DBMS_OUTPUT.PUT_LINE('No row');
END;
```

- [ ] **A)** No row
- [ ] **B)** NULL
- [ ] **C)** ORA-01403
- [ ] **D)** ORA-01422

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A SELECT INTO that returns no rows raises NO_DATA_FOUND; the exception handler catches it and prints 'No row'.
 
 
</details>

### 23. After a successful single-row SELECT INTO in PL/SQL, which implicit cursor attribute evaluates to TRUE?

- [ ] **A)** SQL%FOUND
- [ ] **B)** SQL%NOTFOUND
- [ ] **C)** SQL%ROWCOUNT
- [ ] **D)** SQL%ISOPEN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SQL%FOUND returns TRUE when the most recent implicit SQL statement found at least one row.
 
 
</details>

### 24. Which statements about SQL%ROWCOUNT are true? (Choose all that apply.)

- [ ] **A)** Returns rows processed by most recent implicit SQL
- [ ] **B)** Valid after DML statements such as UPDATE
- [ ] **C)** Raises NO_DATA_FOUND when zero rows are processed
- [ ] **D)** Rolls back transaction when value is zero

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SQL%ROWCOUNT is a numeric attribute updated after an implicit SQL statement. It does not raise exceptions or control transactions.
 
 
</details>

### 25. Examine this procedure. When update_salary(100, 100) is executed and employee 100 exists, what is printed?

```plsql
CREATE OR REPLACE PROCEDURE update_salary (
  p_emp_id   employees.employee_id%TYPE,
  p_increase NUMBER
) IS
BEGIN
  UPDATE employees
     SET salary = salary + p_increase
   WHERE employee_id = p_emp_id;

  IF SQL%NOTFOUND THEN
    DBMS_OUTPUT.PUT_LINE('Not found');
  ELSE
    DBMS_OUTPUT.PUT_LINE('Updated rows: ' || SQL%ROWCOUNT);
  END IF;
END;
```

- [ ] **A)** Updated rows: 1
- [ ] **B)** Updated rows: 0
- [ ] **C)** Not found
- [ ] **D)** No output

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When one row qualifies, SQL%NOTFOUND is FALSE and SQL%ROWCOUNT is 1, so the ELSE branch prints 'Updated rows: 1'.
 
 
</details>


---

### **Working with Data**

### 26. Which SQL statement must a PL/SQL program use to retrieve a single row from a database table into local variables?

- [ ] **A)** SELECT INTO
- [ ] **B)** FETCH
- [ ] **C)** OPEN
- [ ] **D)** EXECUTE IMMEDIATE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PL/SQL uses SELECT INTO to transfer a single row's column values into variables. OPEN and FETCH belong to explicit cursor processing, and EXECUTE IMMEDIATE is used for dynamic SQL.
 
 
</details>

### 27. Which attributes can be applied to the SQL implicit cursor to evaluate the outcome of a DML statement in PL/SQL?

- [ ] **A)** %FOUND
- [ ] **B)** %NOTFOUND
- [ ] **C)** %ROWCOUNT
- [ ] **D)** %TYPE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> %FOUND, %NOTFOUND, and %ROWCOUNT are valid SQL cursor attributes used after DML in PL/SQL. %TYPE declares a variable with the same data type as a column.
 
 
</details>

### 28. What happens when the embedded query in the block returns more than one row?

```sql
DECLARE
   v_employee_id  employees.employee_id%TYPE;
BEGIN
   SELECT employee_id
     INTO v_employee_id
     FROM employees;
END;
/
```

- [ ] **A)** TOO_MANY_ROWS is raised
- [ ] **B)** NO_DATA_FOUND is raised
- [ ] **C)** Only the first generated row is assigned
- [ ] **D)** All matching rows are assigned to the variables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The SELECT INTO statement requires the query to return exactly one row. If multiple rows are returned, PL/SQL raises the predefined TOO_MANY_ROWS exception.
 
 
</details>

### 29. What does SQL%ROWCOUNT return after an UPDATE statement has executed in a PL/SQL block?

- [ ] **A)** Number of rows updated by the statement
- [ ] **B)** Number of rows present in the updated table
- [ ] **C)** Total number of rows updated by all sessions
- [ ] **D)** Number of columns modified by the statement

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SQL%ROWCOUNT contains the number of rows affected by the most recently executed DML statement, such as the number of rows updated by an UPDATE.
 
 
</details>

### 30. Which of the following data manipulation statements can be executed directly as static SQL in a PL/SQL block?

- [ ] **A)** INSERT
- [ ] **B)** UPDATE
- [ ] **C)** DELETE
- [ ] **D)** CREATE TABLE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> INSERT, UPDATE, and DELETE are static DML statements supported directly in PL/SQL. CREATE TABLE is DDL and normally requires dynamic SQL.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Astronomer/Astronomer%20Certification%20DAG%20Authoring%20for%20Apache%20Airflow%203" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Apache Airflow DAG Authoring</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Advanced DAG Authoring](#advanced-dag-authoring) (8 questions)
- [DAG Development Fundamentals](#dag-development-fundamentals) (8 questions)
- [Deployment and Security](#deployment-and-security) (3 questions)
- [Operators and Hooks](#operators-and-hooks) (8 questions)
- [Testing and Quality Assurance](#testing-and-quality-assurance) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:06.418Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Advanced DAG Authoring | 8 |
| DAG Development Fundamentals | 8 |
| Deployment and Security | 3 |
| Operators and Hooks | 8 |
| Testing and Quality Assurance | 3 |

---

### **Advanced DAG Authoring**

### 1. What is the purpose of Jinja templating in Apache Airflow?

- [ ] **A)** To define DAG structure at parse time
- [ ] **B)** To evaluate expressions at runtime within templated fields
- [ ] **C)** To replace Python in operator arguments
- [ ] **D)** To generate dynamic DAG IDs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Jinja templating allows dynamic values to be computed at task execution time, not during DAG parsing. Only certain operator fields support templating.
 
 
</details>

### 2. Which of the following are valid ways to parameterize a DAG? (Select all that apply)

- [ ] **A)** Using f-strings in DAG definition
- [ ] **B)** Using Jinja templates in default_args
- [ ] **C)** Using dag_run.conf in templated fields
- [ ] **D)** Using environment variables at parse time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> f-strings work at parse time, dag_run.conf runtime, environment variables parse time. default_args does not support templating.
 
 
</details>

### 3. What type of DAG authoring pattern is demonstrated in the code?

```python
def create_dag(table_name):
    with DAG(dag_id=f"process_{table_name}", start_date=datetime(2023,1,1)) as dag:
        # tasks
        pass
table_names = ["sales", "inventory"]
for t in table_names:
    create_dag(t)
```

- [ ] **A)** Static DAG
- [ ] **B)** Dynamic DAG factory
- [ ] **C)** Dynamic task mapping
- [ ] **D)** Triggered DAG

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code uses a function to create DAG objects based on a list, which is the DAG factory pattern.
 
 
</details>

### 4. What happens when a BranchPythonOperator returns the task_id of a task that does not exist?

- [ ] **A)** The DAG fails immediately
- [ ] **B)** The task is skipped
- [ ] **C)** Airflow raises a ValueError
- [ ] **D)** The branching operator defaults to all downstream tasks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The BranchPythonOperator requires that the returned task id matches an existing downstream task; otherwise it raises an error.
 
 
</details>

### 5. Which of the following trigger rules allow a task to run even if upstream tasks are skipped? (Select all that apply)

- [ ] **A)** all_success
- [ ] **B)** all_done
- [ ] **C)** none_failed
- [ ] **D)** one_success

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C, D**
 
> 💡  **Explanation** 
> 
> all_done runs regardless of state, none_failed allows skipped, one_success allows at least one success.
 
 
</details>

### 6. What should the return type of a branch function be for a single downstream task?

```python
@task.branch
def branch_func():
    if condition:
        return "task_a"
    else:
        return "task_b"
```

- [ ] **A)** A string
- [ ] **B)** A list of strings
- [ ] **C)** A boolean
- [ ] **D)** None

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The branch function should return the task_id of the downstream task to execute, which is a string.
 
 
</details>

### 7. In the TaskFlow API, how does Airflow automatically infer task dependencies?

- [ ] **A)** By reading function decorators
- [ ] **B)** By matching parameter names to upstream task names
- [ ] **C)** By analyzing docstrings
- [ ] **D)** By scanning import statements

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> When a task function has a parameter with the same name as an upstream task's function name, Airflow creates a dependency and passes the return value via XCom.
 
 
</details>

### 8. Which of the following are benefits of using the @task decorator over traditional PythonOperator? (Select all that apply)

- [ ] **A)** Automatic XCom passing
- [ ] **B)** Support for manual context provision
- [ ] **C)** Cleaner code with less boilerplate
- [ ] **D)** Ability to use any operator type

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> @task automatically passes XComs and reduces boilerplate. It does not support all operator types.
 
 
</details>


---

### **DAG Development Fundamentals**

### 9. What is the recommended pattern for defining a DAG in Airflow 2.x?

- [ ] **A)** Using the `with DAG(...)` context manager
- [ ] **B)** Using the `@dag` decorator
- [ ] **C)** Using the `dag = DAG(...)` constructor without context
- [ ] **D)** Using a YAML configuration file

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The `@dag` decorator is the recommended pattern in Airflow 2.x for its conciseness and alignment with Python function-based design.
 
 
</details>

### 10. Which of the following are valid ways to attach a task to a DAG? (Select two)

- [ ] **A)** Instantiate the operator inside a `with DAG(...)` block
- [ ] **B)** Pass the `dag` parameter to the operator constructor
- [ ] **C)** Define the operator after the `with` block has ended
- [ ] **D)** Use the `dag_id` parameter instead of the `dag` object

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Operators inside a `with DAG(...)` block are automatically attached. Alternatively, passing `dag` explicitly also works.
 
 
</details>

### 11. Examine the DAG code in the code block. What is the critical mistake that will cause an import error?

```python
from airflow.decorators import dag
from airflow.operators.dummy import DummyOperator
from datetime import datetime

@dag(schedule='@daily', start_date=datetime(2024,1,1), catchup=False)
def my_dag():
    start = DummyOperator(task_id='start')
    end = DummyOperator(task_id='end')
    start >> end
```

- [ ] **A)** The function does not return the DAG object
- [ ] **B)** The `@dag` decorator is missing parentheses
- [ ] **C)** The `schedule` parameter should be `schedule_interval`
- [ ] **D)** The `start_date` uses `datetime` without timezone

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The `@dag` decorator expects the decorated function to return the DAG object. Omitting `return dag` causes an import error.
 
 
</details>

### 12. What does the `default_args` dictionary provide in an Airflow DAG?

- [ ] **A)** It defines the schedule and start date of the DAG
- [ ] **B)** It sets default parameter values for all tasks in the DAG
- [ ] **C)** It stores the default dag_id for the DAG
- [ ] **D)** It enables automatic XCom passing between tasks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> `default_args` sets default values for operator-level arguments like `owner`, `retries`, and `depends_on_past` for all tasks.
 
 
</details>

### 13. Which of the following are DAG-level parameters? (Select two)

- [ ] **A)** catchup
- [ ] **B)** retries
- [ ] **C)** schedule_interval
- [ ] **D)** email_on_failure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> `catchup` and `schedule_interval` are DAG-level parameters. Task-level parameters like `retries` belong in `default_args`.
 
 
</details>

### 14. Review the DAG snippet in the code block. Why might the DAG not create any runs after the start_date?

```python
from airflow import DAG
from datetime import datetime

with DAG(dag_id='test_dag', start_date=datetime(2024,1,1), schedule=None) as dag:
    pass
```

- [ ] **A)** The `catchup` parameter is set to False
- [ ] **B)** The `start_date` is after the `schedule_interval` offset
- [ ] **C)** The `schedule` parameter is set to `None`
- [ ] **D)** The `default_args` do not include `owner`

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Setting `schedule=None` means the DAG is not automatically scheduled and will only run when triggered manually.
 
 
</details>

### 15. What is the primary role of the Airflow Scheduler?

- [ ] **A)** It executes tasks by allocating resources on workers
- [ ] **B)** It decides which tasks to run and when, then enqueues them
- [ ] **C)** It stores task outputs and manages DAG file storage
- [ ] **D)** It handles load balancing across multiple Airflow instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Scheduler determines task eligibility based on dependencies and schedule, then queues tasks for the Executor.
 
 
</details>

### 16. Which of the following are valid executors in Apache Airflow? (Select two)

- [ ] **A)** SequentialExecutor
- [ ] **B)** CeleryExecutor
- [ ] **C)** KubernetesExecutor
- [ ] **D)** PythonExecutor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> CeleryExecutor and KubernetesExecutor support distributed execution. SequentialExecutor is for debugging only.
 
 
</details>


---

### **Deployment and Security**

### 17. When Airflow looks for a connection, which backend is checked first by default?

- [ ] **A)** Environment variables
- [ ] **B)** MetastoreDB
- [ ] **C)** HashiCorp Vault
- [ ] **D)** AWS Secrets Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The environment variable backend (AIRFLOW_CONN_* prefix) is checked first by default in Airflow's secrets resolution order.
 
 
</details>

### 18. Which default Airflow roles have permission to trigger a DAG by default? (Select two)

- [ ] **A)** Admin
- [ ] **B)** Op
- [ ] **C)** User
- [ ] **D)** Viewer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Admin and Op roles have the can_create permission on DAGs by default, allowing them to trigger runs.
 
 
</details>

### 19. Complete the code to fetch a connection URI securely inside a DAG instead of using os.environ.

```python
from airflow.hooks.base import BaseHook
conn = ___________('my_conn_id')
```

- [ ] **A)** BaseHook.get_connection
- [ ] **B)** Variable.get
- [ ] **C)** os.environ.get
- [ ] **D)** Connection.get_uri

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> BaseHook.get_connection is the secure way to fetch connections, respecting secrets backend order.
 
 
</details>


---

### **Operators and Hooks**

### 20. Which operator is designed to execute an arbitrary Python function within Airflow?

- [ ] **A)** PythonOperator
- [ ] **B)** BashOperator
- [ ] **C)** PostgresOperator
- [ ] **D)** DummyOperator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The PythonOperator is specifically designed to execute a Python callable. The BashOperator runs shell commands, PostgresOperator executes SQL, and DummyOperator does nothing.
 
 
</details>

### 21. Select the operators that are built-in to Apache Airflow (as per the documentation).

- [ ] **A)** PythonOperator
- [ ] **B)** BashOperator
- [ ] **C)** PostgresOperator
- [ ] **D)** FileOperator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The three built-in operators discussed are PythonOperator, BashOperator, and PostgresOperator. FileOperator is not a standard Airflow operator.
 
 
</details>

### 22. Examine the code snippet in the code block. Which import statement correctly imports the PythonOperator?

```python
# airflow/operators/python.py (part of standard installation)
```

- [ ] **A)** from airflow.operators.python import PythonOperator
- [ ] **B)** from airflow.operators.bash import PythonOperator
- [ ] **C)** from airflow.operators.dummy import PythonOperator
- [ ] **D)** from airflow.operators.postgres import PythonOperator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PythonOperator resides in the airflow.operators.python module. The other options are incorrect because they reference different operator modules.
 
 
</details>

### 23. What is the default poke_interval for a sensor in Apache Airflow?

- [ ] **A)** 30 seconds
- [ ] **B)** 60 seconds
- [ ] **C)** 90 seconds
- [ ] **D)** 120 seconds

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The default poke_interval is 60 seconds. This is a key fact about sensor configuration.
 
 
</details>

### 24. Which parameters can be set on a sensor to control its maximum waiting time?

- [ ] **A)** timeout
- [ ] **B)** execution_timeout
- [ ] **C)** poke_interval
- [ ] **D)** retries

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Both timeout (sensor-specific) and execution_timeout (task-level) can limit sensor duration. poke_interval controls frequency, not total time; retries control number of attempts after failure.
 
 
</details>

### 25. Below is a BashOperator task definition. What command will be executed?

```python
BashOperator(
    task_id='print_date',
    bash_command='echo "{{ ds }}"',
    dag=dag
)
```

- [ ] **A)** echo "2025-04-01"
- [ ] **B)** echo "{{ ds }}"
- [ ] **C)** echo 2025-04-01
- [ ] **D)** echo {{ ds }}

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The template {{ ds }} is rendered as the date string (e.g., 2025-04-01) before execution, so the final command is echo \"2025-04-01\" (with quotes preserved). Option B is the raw template before rendering.
 
 
</details>

### 26. Which operator would you use to perform a SQL query on a PostgreSQL database?

- [ ] **A)** PostgresOperator
- [ ] **B)** PythonOperator
- [ ] **C)** BashOperator
- [ ] **D)** SqlOperator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PostgresOperator is the built-in operator specifically for executing SQL on PostgreSQL. SqlOperator is generic and not part of core Airflow.
 
 
</details>

### 27. Which of the following are valid parameters for the PythonOperator?

- [ ] **A)** python_callable
- [ ] **B)** op_args
- [ ] **C)** op_kwargs
- [ ] **D)** bash_command

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> PythonOperator accepts python_callable, op_args, and op_kwargs. bash_command is a parameter for BashOperator, not PythonOperator.
 
 
</details>


---

### **Testing and Quality Assurance**

### 28. Which method is used for lightweight unit testing of a DAG without requiring a database or scheduler?

- [ ] **A)** dag.run()
- [ ] **B)** dag.test()
- [ ] **C)** airflow dags test
- [ ] **D)** airflow tasks test

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> dag.test() runs the DAG inline without requiring a database or scheduler, making it ideal for unit tests.
 
 
</details>

### 29. Which of the following are features of dag.test()?

- [ ] **A)** Uses LocalExecutor by default
- [ ] **B)** Uses a SQLite database that persists after test
- [ ] **C)** Cleans up temporary database after execution
- [ ] **D)** Runs tasks sequentially in a single process

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> dag.test() uses LocalExecutor, runs tasks sequentially, and cleans up the temp database by default.
 
 
</details>

### 30. Refer to the code block. Which pytest-airflow fixture is used to access the DagBag for testing?

```python
import pytest

def test_dag_import_errors(dag_bag):
    assert len(dag_bag.import_errors) == 0
```

- [ ] **A)** dag_bag
- [ ] **B)** dag
- [ ] **C)** dag_bag_list
- [ ] **D)** dag_file

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The dag_bag fixture from pytest-airflow loads all DAGs into a DagBag for validation.
 
 
</details>

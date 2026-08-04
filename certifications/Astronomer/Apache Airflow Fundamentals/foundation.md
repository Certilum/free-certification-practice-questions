<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Astronomer/Astronomer%20Certification%20for%20Apache%20Airflow%203%20Fundamentals" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Apache Airflow Fundamentals</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Airflow Core Concepts](#airflow-core-concepts) (7 questions)
- [DAG Authoring and Scheduling](#dag-authoring-and-scheduling) (8 questions)
- [Execution and Production Deployment](#execution-and-production-deployment) (6 questions)
- [Operators, Hooks, and Connections](#operators-hooks-and-connections) (6 questions)
- [Security, Governance, and Best Practices](#security-governance-and-best-practices) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:09.039Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Airflow Core Concepts | 7 |
| DAG Authoring and Scheduling | 8 |
| Execution and Production Deployment | 6 |
| Operators, Hooks, and Connections | 6 |
| Security, Governance, and Best Practices | 3 |

---

### **Airflow Core Concepts**

### 1. Which component of Apache Airflow is responsible for interpreting DAG definitions and managing task dependencies?

- [ ] **A)** Scheduler
- [ ] **B)** Executor
- [ ] **C)** Web Server
- [ ] **D)** Worker

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Scheduler interprets DAG definitions, manages dependencies, and decides when tasks should run based on schedules and triggers. Executors only delegate tasks; Web Server provides UI; Workers execute task code.
 
 
</details>

### 2. Which two components in Airflow's architecture are required for task execution to occur?

- [ ] **A)** Executor
- [ ] **B)** Worker
- [ ] **C)** Scheduler
- [ ] **D)** Web Server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> The Scheduler prepares and queues tasks; the Worker actually runs the task code. The Executor is only a bridge; the Web Server is optional for execution.
 
 
</details>

### 3. Analyze this configuration snippet and identify the executor type that will be used.

```plaintext
AIRFLOW__CORE__EXECUTOR=LocalExecutor
AIRFLOW__CORE__PARALLELISM=16
```

- [ ] **A)** SequentialExecutor
- [ ] **B)** LocalExecutor
- [ ] **C)** CeleryExecutor
- [ ] **D)** KubernetesExecutor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The configuration sets core.executor to 'LocalExecutor' (shown in the code block). No broker URL is provided, so Celery/K8s are not possible. Sequential is not set.
 
 
</details>

### 4. What does the bitshift operator >> in a DAG definition indicate?

- [ ] **A)** task2 runs before task1
- [ ] **B)** task1 depends on task2
- [ ] **C)** task2 depends on task1
- [ ] **D)** No dependency, it's a syntax error

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The bitshift operator >> sets the downstream task to depend on the upstream. So task1 >> task2 means task2 depends on task1.
 
 
</details>

### 5. Which two statements are true about a DAG Run in Airflow?

- [ ] **A)** A DAG Run is created for every data interval that ends after start_date if catchup=True
- [ ] **B)** A DAG Run always appears immediately after the DAG file is parsed
- [ ] **C)** Each DAG Run has its own execution_date which is the start of the data interval
- [ ] **D)** A DAG Run state is the same as the state of its first task instance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> DAG Runs are created when the schedule interval passes (or manually). The execution_date is the beginning of the data interval. Runs are not created immediately after parsing. The DAG Run state is a summary of all tasks, not just the first.
 
 
</details>

### 6. Given this DAG snippet, what will be the trigger rule for task3 if we want it to run as soon as any one of task1 or task2 succeeds?

```python
with DAG(...):
    task1 = DummyOperator(task_id='t1')
    task2 = DummyOperator(task_id='t2')
    task3 = DummyOperator(task_id='t3', trigger_rule='one_success')
    [task1, task2] >> task3
```

- [ ] **A)** all_success
- [ ] **B)** one_success
- [ ] **C)** all_done
- [ ] **D)** one_failed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The trigger_rule='one_success' makes the downstream task run as soon as any upstream task succeeds. all_success requires all to succeed; all_done runs regardless of outcome; one_failed runs if any fails.
 
 
</details>

### 7. What is the main difference between a DAG and a DAG Run?

- [ ] **A)** A DAG Run is the blueprint; a DAG is an execution
- [ ] **B)** A DAG is static; a DAG Run is a runtime instance
- [ ] **C)** A DAG Run contains tasks; a DAG contains operators
- [ ] **D)** They are synonyms

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A DAG is the static workflow definition written in Python; a DAG Run is a specific execution of that DAG for a particular data interval.
 
 
</details>


---

### **DAG Authoring and Scheduling**

### 8. What is the purpose of the `with DAG(...) as dag:` statement in Airflow?

- [ ] **A)** It creates a DAG object and automatically assigns tasks defined inside the block to that DAG.
- [ ] **B)** It defines the schedule interval for the DAG.
- [ ] **C)** It sets default_args for all tasks in the DAG.
- [ ] **D)** It adds tags to the DAG for UI filtering.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The context manager ensures tasks within the block are associated with the DAG without needing explicit dag=dag parameter.
 
 
</details>

### 9. Which statements about `default_args` in Airflow are correct? (Select all that apply)

- [ ] **A)** It is a dictionary passed to the DAG constructor.
- [ ] **B)** It sets default parameters for all tasks within that DAG.
- [ ] **C)** Task-level arguments always override the corresponding default_args.
- [ ] **D)** It must contain the 'start_date' parameter.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> default_args is an optional dict; start_date is required but can be set elsewhere. Task parameters have higher precedence.
 
 
</details>

### 10. In the provided code, which parameter is used to add searchable metadata labels to the DAG in the Airflow UI?

```python
with DAG(
    dag_id='example_dag',
    default_args={'owner': 'airflow'},
    tags=['production', 'ETL'],
    schedule='@daily',
    start_date=datetime(2023,1,1)
) as dag:
```

- [ ] **A)** tags
- [ ] **B)** default_args
- [ ] **C)** dag_id
- [ ] **D)** schedule_interval

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Tags are a list of strings that appear as filterable labels in the Airflow UI; they do not affect execution.
 
 
</details>

### 11. What type of task dependency is created by `task1 >> [task2, task3]`?

- [ ] **A)** Fan-out (parallel downstream tasks)
- [ ] **B)** Fan-in (synchronization point)
- [ ] **C)** Linear (sequential chain)
- [ ] **D)** Conditional branching

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Fan-out means one upstream task triggers multiple downstream tasks that can run in parallel.
 
 
</details>

### 12. Which statements about cron-based scheduling in Airflow are true? (Select all that apply)

- [ ] **A)** The schedule parameter accepts standard cron strings like '0 5 * * 1'.
- [ ] **B)** @daily is equivalent to '0 0 * * *'.
- [ ] **C)** Cron scheduling aligns to calendar boundaries.
- [ ] **D)** Cron expressions can specify seconds.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Cron has 5-6 fields; seconds are not standard. @daily maps to midnight. Cron aligns to wall-clock time.
 
 
</details>

### 13. Given the TaskFlow code below, what is automatically created when `return_value` is passed to another task?

```python
@task
def extract():
    return {'data': 42}

@task
def transform(data):
    return data['data'] * 2

with DAG(...):
    result = extract()
    transformed = transform(result)
```

- [ ] **A)** An XCom that establishes an implicit dependency
- [ ] **B)** A bitwise shift operator dependency
- [ ] **C)** A manual set_downstream() call
- [ ] **D)** A separate DummyOperator dependency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TaskFlow automatically pushes return values to XCom and creates dependencies when passed as arguments to other decorated functions.
 
 
</details>

### 14. What is the default value of the `retries` parameter in an Airflow task?

- [ ] **A)** 0
- [ ] **B)** 1
- [ ] **C)** 3
- [ ] **D)** Infinite

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The default retries parameter is 0; tasks fail permanently unless retries is explicitly set to a positive integer.
 
 
</details>

### 15. Which of the following are valid schedule types in Airflow? (Select all that apply)

- [ ] **A)** Cron expression string
- [ ] **B)** datetime.timedelta object
- [ ] **C)** List of Dataset objects
- [ ] **D)** SQLAlchemy query

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Airflow supports cron, timedelta, and dataset-driven scheduling. SQLAlchemy query is not a schedule type.
 
 
</details>


---

### **Execution and Production Deployment**

### 16. Which executor runs tasks as subprocesses on the scheduler host?

- [ ] **A)** LocalExecutor
- [ ] **B)** CeleryExecutor
- [ ] **C)** KubernetesExecutor
- [ ] **D)** SequentialExecutor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> LocalExecutor runs tasks as subprocesses on the scheduler host, leveraging multiprocessing.
 
 
</details>

### 17. Which two executors require a metadata database that supports multiple concurrent connections?

- [ ] **A)** LocalExecutor
- [ ] **B)** CeleryExecutor
- [ ] **C)** KubernetesExecutor
- [ ] **D)** SequentialExecutor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> LocalExecutor and CeleryExecutor require a database like PostgreSQL or MySQL that supports multiple concurrent connections.
 
 
</details>

### 18. Given the following Dockerfile snippet, which Airflow configuration is being set?

```dockerfile
ENV AIRFLOW__CORE__PARALLELISM=32
```

- [ ] **A)** core.parallelism
- [ ] **B)** core.dag_concurrency
- [ ] **C)** core.max_active_runs
- [ ] **D)** core.worker_concurrency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The environment variable AIRFLOW__CORE__PARALLELISM sets the global parallelism limit for the scheduler.
 
 
</details>

### 19. What is the default executor when using SQLite as the metadata database?

- [ ] **A)** SequentialExecutor
- [ ] **B)** LocalExecutor
- [ ] **C)** CeleryExecutor
- [ ] **D)** KubernetesExecutor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The SequentialExecutor is the default executor when SQLite is used as the metadata database.
 
 
</details>

### 20. Which of the following are valid ways to set environment variables in an Astronomer deployment?

- [ ] **A)** Using the Astro CLI command astro deployment variable set
- [ ] **B)** Directly editing the Dockerfile ENV directive
- [ ] **C)** By modifying the running container's environment file
- [ ] **D)** Through the Astronomer UI under Deployment > Variables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Environment variables can be set via the Astro CLI, the Dockerfile ENV command, or the Astronomer UI.
 
 
</details>

### 21. What does the following Airflow metric indicate? pool.starving > 0

```text
# Metric from Prometheus exporter: pool.starving
```

- [ ] **A)** Tasks are waiting for pool slots
- [ ] **B)** The scheduler is overloaded
- [ ] **C)** Workers are idle
- [ ] **D)** Database connections are exhausted

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A positive value for pool.starving indicates that tasks are queued because no pool slots are available.
 
 
</details>


---

### **Operators, Hooks, and Connections**

### 22. Which built-in operator is designed to execute a Python callable?

- [ ] **A)** PythonOperator
- [ ] **B)** BashOperator
- [ ] **C)** PostgresOperator
- [ ] **D)** KubernetesPodOperator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The PythonOperator executes a Python callable via the python_callable parameter.
 
 
</details>

### 23. Which of the following operators support Jinja templating in their command or SQL parameters?

- [ ] **A)** BashOperator
- [ ] **B)** PostgresOperator
- [ ] **C)** PythonOperator
- [ ] **D)** KubernetesPodOperator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> BashOperator and PostgresOperator have templatable fields (bash_command, sql). PythonOperator does not template its callable; KubernetesPodOperator does not support templating.
 
 
</details>

### 24. In the provided code snippet, what type of object does get_records return?

```python
hook = PostgresHook(postgres_conn_id='prod_postgres')
results = hook.get_records('SELECT * FROM sales')

```

- [ ] **A)** A list of tuples
- [ ] **B)** A list of dictionaries
- [ ] **C)** A pandas DataFrame
- [ ] **D)** A single string

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> get_records returns a list of tuples, each tuple representing a row.
 
 
</details>

### 25. Which method of storing connections has the highest precedence in Airflow?

- [ ] **A)** Secret Backend
- [ ] **B)** Environment Variables
- [ ] **C)** Connections UI
- [ ] **D)** All have equal precedence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Secret Backends are checked first, overriding environment variables and UI connections.
 
 
</details>

### 26. Which of the following are common built-in Hooks in Airflow?

- [ ] **A)** PostgresHook
- [ ] **B)** S3Hook
- [ ] **C)** GCSHook
- [ ] **D)** KubernetesHook

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> PostgresHook, S3Hook, and GCSHook are listed as common built-in Hooks. KubernetesHook is not mentioned in the document.
 
 
</details>

### 27. What is the purpose of the template_fields attribute in the custom operator?

```python
class MyOperator(BaseOperator):
    template_fields = ('sql_query',)
    def __init__(self, sql_query, **kwargs):
        super().__init__(**kwargs)
        self.sql_query = sql_query
    def execute(self, context):
        pass

```

- [ ] **A)** Enables Jinja templating for the parameter
- [ ] **B)** Makes the parameter mandatory
- [ ] **C)** Automatically pushes the parameter to XCom
- [ ] **D)** Defines a default value for the parameter

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> template_fields tells Airflow which parameters should be processed through Jinja templating.
 
 
</details>


---

### **Security, Governance, and Best Practices**

### 28. What is the default authentication method for Apache Airflow?

- [ ] **A)** Password-based (local database)
- [ ] **B)** LDAP
- [ ] **C)** OAuth
- [ ] **D)** SAML

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The default Airflow authentication is password-based using a local database with hashed passwords.
 
 
</details>

### 29. Which Airflow roles can manage connections and variables through the UI?

- [ ] **A)** Admin
- [ ] **B)** Op
- [ ] **C)** User
- [ ] **D)** Viewer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Only the Admin role has full access to manage connections, variables, and other configurations in the UI.
 
 
</details>

### 30. Examine the configuration snippet and determine the missing authentication backend.

```ini
[webserver]
auth_backend = ???
```

- [ ] **A)** airflow.api.auth.backend.session
- [ ] **B)** airflow.api.auth.backend.default
- [ ] **C)** airflow.api.auth.backend.ldap
- [ ] **D)** airflow.api.auth.backend.oauth

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> For production, the auth_backend must be set to 'airflow.api.auth.backend.session' to enforce RBAC authentication.
 
 
</details>

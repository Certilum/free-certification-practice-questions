<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Oracle%20Cloud%20Infrastructure%202026%20Data%20Science%20Professional.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Oracle Cloud Infrastructure 2026 Data Science Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Apply MLOps Practices](#apply-mlops-practices) (6 questions)
- [Design and Set up Data Science Workspace](#design-and-set-up-data-science-workspace) (5 questions)
- [Implement end-to-end Machine Learning Lifecycle](#implement-end-to-end-machine-learning-lifecycle) (13 questions)
- [OCI Data Science - Introduction and Configuration](#oci-data-science-introduction-and-configuration) (3 questions)
- [Use related OCI Services](#use-related-oci-services) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:46:05.431Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Apply MLOps Practices | 6 |
| Design and Set up Data Science Workspace | 5 |
| Implement end-to-end Machine Learning Lifecycle | 13 |
| OCI Data Science - Introduction and Configuration | 3 |
| Use related OCI Services | 3 |

---

### **Apply MLOps Practices**

### 1. Which OCI Data Science resource is used to logically group the artifacts of an ML project, such as notebook sessions, jobs, pipelines, and model deployments?

- [ ] **A)** Model catalog
- [ ] **B)** Project
- [ ] **C)** Job
- [ ] **D)** Model deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A project is the logical container in OCI Data Science for organizing related ML resources such as notebook sessions, jobs, pipelines, and model deployments.
 
 
</details>

### 2. Which statements correctly describe characteristics of the OCI Data Science model catalog? Select all that apply.

- [ ] **A)** It stores model artifacts and associated metadata
- [ ] **B)** It supports registering and versioning models for reuse and management
- [ ] **C)** It directly executes training jobs on dedicated infrastructure
- [ ] **D)** It provides registered models to model deployments for online serving

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> The model catalog stores, registers, and versions model artifacts. Model deployments use models from the catalog. Training is performed by jobs or pipelines, not by the model catalog.
 
 
</details>

### 3. A data scientist runs the command presented in the code block. Which OCI Data Science resource is created by this command?

```bash
oci data-science job create --compartment-id ocid1.compartment.oc1..example --project-id ocid1.datascienceproject.oc1..example --display-name model-training-job
```

- [ ] **A)** Notebook session
- [ ] **B)** Job
- [ ] **C)** Model deployment
- [ ] **D)** Pipeline

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The oci data-science job create command creates a job definition for running ML workloads on OCI Data Science.
 
 
</details>

### 4. Which OCI mechanism is recommended for a Data Science job or notebook session to access OCI services without requiring long-lived user API keys in the code?

- [ ] **A)** Resource principal
- [ ] **B)** Customer-managed key
- [ ] **C)** Static API signing key
- [ ] **D)** Object Storage namespace

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Resource principals allow OCI Data Science resources to call OCI services based on policies, avoiding the need to embed long-lived user credentials in code.
 
 
</details>

### 5. Which practices are core to applying MLOps on OCI Data Science? Select all that apply.

- [ ] **A)** Automating experiment training through Data Science Jobs or Pipelines
- [ ] **B)** Storing versioned model artifacts in the model catalog
- [ ] **C)** Manually copying model files to instances after every retraining run
- [ ] **D)** Monitoring deployed models to detect drift and performance degradation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> MLOps emphasizes automation, versioning, reproducibility, and monitoring. Manually copying model files is not a scalable or auditable MLOps practice.
 
 
</details>

### 6. The code block uses the OCI Python SDK from a notebook session. What does this code create in OCI Data Science?

```python
import oci

client = oci.data_science.DataScienceClient(config)

model_details = oci.data_science.models.CreateModelDetails(
    display_name='demand-forecast',
    project_id='ocid1.datascienceproject.oc1..example',
    compartment_id='ocid1.compartment.oc1..example'
)
client.create_model(model_details)
```

- [ ] **A)** Model catalog entry
- [ ] **B)** Pipeline run
- [ ] **C)** Job run
- [ ] **D)** Model deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Python SDK passes CreateModelDetails to create_model, which creates a model entry in the OCI Data Science model catalog.
 
 
</details>


---

### **Design and Set up Data Science Workspace**

### 7. What is the primary resource in OCI Data Science used to logically organize notebook sessions, jobs, and models?

- [ ] **A)** Project
- [ ] **B)** Notebook Session
- [ ] **C)** Model Deployment
- [ ] **D)** Data Flow Application

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A project is the main logical container in OCI Data Science. It organizes related models, notebook sessions, and jobs so they can be managed and collaborated on together.
 
 
</details>

### 8. What must be configured or created before a data scientist can launch a notebook session in OCI Data Science?

- [ ] **A)** Create an OCI project
- [ ] **B)** Configure a virtual cloud network and subnet for the notebook session
- [ ] **C)** Grant IAM policies so the Data Science service can use network resources
- [ ] **D)** Set up an on-premises database for all training data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Before launching a notebook session, you must have a project, a virtual cloud network or subnet for the session, and IAM policies that allow the Data Science service to use resources in OCI.
 
 
</details>

### 9. Review the OCI CLI command in the code block. Which OCI Data Science resource is created by executing this command?

```bash
oci data-science project create --compartment-id ocid1.compartment.oc1..aaaa --display-name Customer_Churn_Project

```

- [ ] **A)** A project
- [ ] **B)** A notebook session
- [ ] **C)** A model catalog entry
- [ ] **D)** A data pipeline

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command uses the OCI Data Science CLI service to create a project with the display name Customer_Churn_Project in the specified compartment.
 
 
</details>

### 10. Which statement accurately describes a notebook session in OCI Data Science after the workspace and project have been set up?

- [ ] **A)** A managed JupyterLab environment running on a compute resource
- [ ] **B)** A static dashboard used only for viewing model metrics
- [ ] **C)** A desktop application installed on the data scientist's laptop
- [ ] **D)** A SQL query engine used exclusively for data preparation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A notebook session in OCI Data Science is a fully managed JupyterLab environment that runs on a compute resource and provides an interactive space for developing machine learning models.
 
 
</details>

### 11. Which of the following are core OCI Data Science resource types that a data scientist can work with in a project?

- [ ] **A)** Projects
- [ ] **B)** Notebook sessions
- [ ] **C)** The model catalog
- [ ] **D)** Big Data Service clusters

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Projects, notebook sessions, and the model catalog are all part of OCI Data Science. Big Data Service is a separate OCI service and is not a Data Science workspace resource.
 
 
</details>


---

### **Implement end-to-end Machine Learning Lifecycle**

### 12. Which OCI Data Science artifact acts as the container for resources created for one machine-learning business use case?

- [ ] **A)** Project
- [ ] **B)** Compartment
- [ ] **C)** Object Storage bucket
- [ ] **D)** Notebook session

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Project is the logical container in OCI Data Science that groups notebook sessions, jobs, models and deployments. Compartments are used to organize OCI resources at a broader tenancy level.
 
 
</details>

### 13. Which of the following are core components used when implementing an end to end ML workload on OCI Data Science?

- [ ] **A)** Notebook session
- [ ] **B)** Model catalog
- [ ] **C)** Model deployment
- [ ] **D)** Data Flow application

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Notebook sessions support interactive development, the model catalog stores model artifacts, and model deployments serve predictions. Data Flow applications are not an OCI Data Science component.
 
 
</details>

### 14. Look at the Python code block. What type of resource is created by the client call?

```python
import oci
from oci.data_science import DataScienceClient
from oci.data_science.models import CreateProjectDetails

config = oci.config.from_file()
client = DataScienceClient(config)
project_details = CreateProjectDetails(
    compartment_id='ocid1.compartment.oc1..example',
    display_name='customer-churn-project'
)
response = client.create_project(project_details)

```

- [ ] **A)** Project
- [ ] **B)** Model catalog
- [ ] **C)** Notebook session
- [ ] **D)** Data Science job

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The request object in the code describes a project and invokes client.create_project. Therefore the returned response contains a Project resource in OCI Data Science.
 
 
</details>

### 15. Which statement best describes a notebook session in OCI Data Science?

- [ ] **A)** Managed JupyterLab environment with attached compute
- [ ] **B)** SQL editor for Autonomous Database
- [ ] **C)** Data integration pipeline designer
- [ ] **D)** Container orchestration platform

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An OCI Data Science notebook session is a managed JupyterLab environment with a selected compute shape and block storage. It is used for interactive exploration and model development.
 
 
</details>

### 16. Which items do you explicitly configure when you create a notebook session in OCI Data Science?

- [ ] **A)** Compute shape
- [ ] **B)** Block storage size
- [ ] **C)** Subnet
- [ ] **D)** Model algorithm

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> When creating a notebook session, the user selects a compute shape, block storage size, and subnet. Model accuracy is a training evaluation metric, not a notebook session configuration value.
 
 
</details>

### 17. The code block registers an ML artifact. What kind of OCI Data Science resource is created?

```python
import oci
from oci.data_science import DataScienceClient
from oci.data_science.models import CreateModelDetails

config = oci.config.from_file()
client = DataScienceClient(config)
model_details = CreateModelDetails(
    compartment_id='ocid1.compartment.oc1..example',
    project_id='ocid1.datascienceproject.oc1..example',
    display_name='churn-classifier'
)
response = client.create_model(model_details)

```

- [ ] **A)** Model
- [ ] **B)** Project
- [ ] **C)** Notebook session
- [ ] **D)** Data Flow application

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CreateModelDetails and client.create_model add a model to the OCI Data Science model catalog. The resource created by the API call is therefore a Model.
 
 
</details>

### 18. Which OCI Data Science feature persists trained model artifacts and metadata for later reuse?

- [ ] **A)** Model catalog
- [ ] **B)** Project
- [ ] **C)** Job
- [ ] **D)** Container registry

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The model catalog stores model artifacts and associated metadata so models can be reused, evaluated, and deployed later. Projects organize resources, while jobs execute code.
 
 
</details>

### 19. Which model-related tasks are supported by OCI Data Science in the end-to-end ML lifecycle?

- [ ] **A)** Train in notebook session
- [ ] **B)** Run as a repeatable job
- [ ] **C)** Deploy as a REST endpoint
- [ ] **D)** Purchase database licenses

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> In OCI Data Science a model can be trained in a notebook, run in a job, and served through a deployment. Buying database licenses is unrelated to the model lifecycle.
 
 
</details>

### 20. Look at the code block. What type of resources are returned by the API request?

```python
import oci
from oci.data_science import DataScienceClient

config = oci.config.from_file()
client = DataScienceClient(config)
response = client.list_model_deployments(compartment_id='ocid1.compartment.oc1..example')

```

- [ ] **A)** Model deployment
- [ ] **B)** Project
- [ ] **C)** Job
- [ ] **D)** Conda environment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code calls list_model_deployments, so the returned collection contains model deployments. This method does not list projects, jobs, or conda environments.
 
 
</details>

### 21. Which statement best describes a data science job in OCI Data Science?

- [ ] **A)** Managed and repeatable execution of code
- [ ] **B)** Real-time model prediction endpoint
- [ ] **C)** Persistent storage for training data
- [ ] **D)** Visual ETL flow canvas

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Data Science jobs provide managed, repeatable execution of ML code without an interactive notebook. They are commonly used for scheduled and production workloads.
 
 
</details>

### 22. Which of the following can be created inside an OCI Data Science project?

- [ ] **A)** Notebook sessions
- [ ] **B)** Data Science jobs
- [ ] **C)** Model deployments
- [ ] **D)** Oracle Analytics Cloud workbook

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Projects group all OCI Data Science resources created for one use case, including notebook sessions, jobs, pipelines, models, and deployments. Oracle Analytics Cloud is a separate analytics service.
 
 
</details>

### 23. The code block configures a client without embedding user credentials. Which principal is being used?

```python
import oci
from oci.data_science import DataScienceClient

signer = oci.auth.signers.get_resource_principals_signer()
client = DataScienceClient(config={}, signer=signer)

```

- [ ] **A)** Resource principal
- [ ] **B)** User API key
- [ ] **C)** Federation user
- [ ] **D)** Database user

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code uses get_resource_principals_signer, which returns the OCI resource principal signer. Resource principals allow a Data Science job to make API calls without user API keys.
 
 
</details>

### 24. Which OCI service should a deployed model use to keep database credentials secure?

- [ ] **A)** OCI Vault
- [ ] **B)** In the model artifact
- [ ] **C)** In a public Git repository
- [ ] **D)** In plain text logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Secrets should be managed in OCI Vault and referenced by OCID. Storing credentials in artifacts, repositories, or logs creates a security risk.
 
 
</details>


---

### **OCI Data Science - Introduction and Configuration**

### 25. Which statement correctly describes the Oracle Cloud Infrastructure Data Science service for a data science team?

- [ ] **A)** A fully managed machine learning platform
- [ ] **B)** A relational database administration service
- [ ] **C)** A serverless web hosting service
- [ ] **D)** A traditional data warehouse

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI Data Science is a fully managed machine learning platform for the complete ML lifecycle, from experimentation to deployment.
 
 
</details>

### 26. Which two statements about how projects support an OCI Data Science workflow are true? (Choose two.)

- [ ] **A)** Projects organize notebook sessions and jobs
- [ ] **B)** Projects are created to hold only one experiment
- [ ] **C)** A project is created before its associated resources
- [ ] **D)** Projects can contain only model artifacts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Projects are core containers in OCI Data Science. They are created first and organize notebook sessions, jobs, and related artifacts throughout the ML workflow.
 
 
</details>

### 27. Review the shell command in the code block. What is the main result when this command is executed successfully?

```shell
oci data-science project create --compartment-id ocid1.compartment.oc1..example --display-name customer-churn-project
```

- [ ] **A)** A project is created
- [ ] **B)** A notebook session is started
- [ ] **C)** A model is registered
- [ ] **D)** A deployment is provisioned

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command creates a Data Science project, which is the parent container needed before adding resources such as notebook sessions and jobs.
 
 
</details>


---

### **Use related OCI Services**

### 28. In the context of machine learning operations, what is the main purpose of using the OCI Data Science managed platform in Oracle Cloud?

- [ ] **A)** Building, training, and deploying machine learning models
- [ ] **B)** Hosting corporate web applications at scale
- [ ] **C)** Replacing traditional data warehouses
- [ ] **D)** Synchronizing on-premise files with cloud storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI Data Science is Oracle's managed service for end-to-end machine learning, including building, training, and deploying models. The other options describe storage, hosting, and file synchronization services.
 
 
</details>

### 29. Which of the following are typical component choices that must be configured when setting up an OCI Data Science solution for a machine learning project?

- [ ] **A)** Projects
- [ ] **B)** Notebook sessions
- [ ] **C)** Model deployments
- [ ] **D)** Cloud Shell

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> An OCI Data Science configuration typically includes projects, notebook sessions, and model deployments. Cloud Shell is a browser-based shell environment, not a component of the Data Science service.
 
 
</details>

### 30. A data scientist runs the displayed code segment in an OCI notebook session during environment configuration. Which OCI service is the code attempting to access?

```python
import oci

config = oci.config.from_file("~/.oci/config")
identity = oci.identity.IdentityClient(config)
user = identity.get_user(config["user"]).data
print(user.name)
```

- [ ] **A)** Identity and Access Management
- [ ] **B)** Object Storage
- [ ] **C)** Data Science
- [ ] **D)** Functions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code imports the OCI SDK and creates an IdentityClient using a config file. Calling get_user requests user information from OCI Identity and Access Management.
 
 
</details>

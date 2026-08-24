<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Azure%20DevOps%20Engineer%20Expert.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Azure DevOps Engineer Expert</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Design and implement a source control strategy](#design-and-implement-a-source-control-strategy) (3 questions)
- [Design and implement build and release pipelines](#design-and-implement-build-and-release-pipelines) (17 questions)
- [Design and implement processes and communications](#design-and-implement-processes-and-communications) (4 questions)
- [Develop a security and compliance plan](#develop-a-security-and-compliance-plan) (4 questions)
- [Implement an instrumentation strategy](#implement-an-instrumentation-strategy) (2 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:52:39.222Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Design and implement a source control strategy | 3 |
| Design and implement build and release pipelines | 17 |
| Design and implement processes and communications | 4 |
| Develop a security and compliance plan | 4 |
| Implement an instrumentation strategy | 2 |

---

### **Design and implement a source control strategy**

### 1. Which version control system does Azure DevOps recommend for all new repositories?

- [ ] **A)** Git
- [ ] **B)** Team Foundation Version Control (TFVC)
- [ ] **C)** Subversion
- [ ] **D)** Mercurial

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Git is the default and recommended version control system in Azure DevOps because it supports distributed workflows and modern branching strategies.
 
 
</details>

### 2. Which of the following are benefits of using Git in Azure Repos?

- [ ] **A)** Local commits and branching without network access
- [ ] **B)** Every developer has a full copy of the repository history
- [ ] **C)** Branching and merging are fast and inexpensive
- [ ] **D)** Files can be locked to block concurrent edits

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Git is distributed, so developers can commit, branch, and merge locally. Central file locking is a TFVC characteristic, not a Git benefit.
 
 
</details>

### 3. What action does the command shown in the code block perform?

```bash
git checkout -b feature/azure-001
```

- [ ] **A)** Creates and switches to a new feature branch
- [ ] **B)** Merges a feature branch into the main branch
- [ ] **C)** Deletes the specified branch from the local repository
- [ ] **D)** Pushes the current branch to the remote repository

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command checkout -b creates a new branch and immediately switches to it.
 
 
</details>


---

### **Design and implement build and release pipelines**

### 4. Which file is the default YAML definition for an Azure Pipelines build pipeline?

- [ ] **A)** azure-pipelines.yml
- [ ] **B)** build.yml
- [ ] **C)** pipeline.json
- [ ] **D)** Jenkinsfile

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Pipelines uses azure-pipelines.yml as the default convention for defining a YAML pipeline.
 
 
</details>

### 5. Which two options are repository triggers used to start a pipeline automatically?

- [ ] **A)** Continuous integration (CI) trigger
- [ ] **B)** Pull request (PR) trigger
- [ ] **C)** Scheduled trigger
- [ ] **D)** Manual review trigger

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CI and PR triggers are repository-based automatic triggers in Azure Pipelines. Scheduled triggers are time-based and not repository triggers.
 
 
</details>

### 6. In the YAML snippet, which event starts the pipeline automatically?

```yaml
trigger:
- main
pool:
  vmImage: ubuntu-latest
steps:
- script: echo Hello
```

- [ ] **A)** A commit to the main branch
- [ ] **B)** A pull request to any branch
- [ ] **C)** A push to any branch except main
- [ ] **D)** Manual execution only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The trigger includes main, so the pipeline starts automatically when a commit is pushed to the main branch.
 
 
</details>

### 7. Which YAML element defines where a pipeline job runs?

- [ ] **A)** pool
- [ ] **B)** steps
- [ ] **C)** trigger
- [ ] **D)** variables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The pool keyword selects an agent pool, such as a Microsoft-hosted or self-hosted pool, for the job.
 
 
</details>

### 8. Which two approval types can be configured in a classic release pipeline?

- [ ] **A)** Pre-deployment approval
- [ ] **B)** Post-deployment approval
- [ ] **C)** Build signature approval
- [ ] **D)** Merge approval

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Classic release pipelines can use pre-deployment and post-deployment approvals to control each release stage.
 
 
</details>

### 9. How many jobs are defined in the YAML snippet?

```yaml
jobs:
- job: Build
  steps:
  - script: npm install
```

- [ ] **A)** One
- [ ] **B)** Two
- [ ] **C)** Three
- [ ] **D)** Zero

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet contains a single job named Build under the jobs collection.
 
 
</details>

### 10. What is the purpose of a pipeline variable in Azure DevOps?

- [ ] **A)** Store a value that can be used during pipeline execution
- [ ] **B)** Store compiled binaries
- [ ] **C)** Define a branch policy
- [ ] **D)** Create a new agent pool

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Variables store values such as configuration settings or secrets that can be referenced throughout pipeline execution.
 
 
</details>

### 11. Which two features help you reuse steps in Azure Pipelines?

- [ ] **A)** Task groups
- [ ] **B)** Templates
- [ ] **C)** Release gates
- [ ] **D)** Secure files

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Task groups and templates are used to reuse steps or YAML content across multiple pipelines and jobs.
 
 
</details>

### 12. What value will the script in the YAML snippet output?

```yaml
variables:
  environment: production
steps:
- script: echo $(environment)
```

- [ ] **A)** production
- [ ] **B)** $(environment)
- [ ] **C)** environment
- [ ] **D)** null

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The variable environment is defined as production, so the expression $(environment) evaluates to production.
 
 
</details>

### 13. Which Azure Pipelines concept provides a logical boundary for approvals and deployment conditions?

- [ ] **A)** Environment
- [ ] **B)** Artifact
- [ ] **C)** Task
- [ ] **D)** Build

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An environment represents a deployment target and can be configured with approvals, checks, and deployment history.
 
 
</details>

### 14. Which two are built-in deployment strategies in Azure Pipelines?

- [ ] **A)** Rolling
- [ ] **B)** Canary
- [ ] **C)** Blue-green
- [ ] **D)** Red-black

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure Pipelines deployment jobs support runOnce, rolling, and canary as built-in deployment strategies.
 
 
</details>

### 15. In the YAML snippet, which pipeline layer directly contains the Compile job?

```yaml
stages:
- stage: Build
  jobs:
  - job: Compile
    steps:
    - script: dotnet build
```

- [ ] **A)** Stage
- [ ] **B)** Task
- [ ] **C)** Step
- [ ] **D)** Release

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Compile job is defined under the jobs collection of the Build stage, so the stage directly contains the job.
 
 
</details>

### 16. What is the purpose of a service connection in Azure DevOps?

- [ ] **A)** Connect to external services securely
- [ ] **B)** Store test results
- [ ] **C)** Schedule releases
- [ ] **D)** Manage code reviews

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Service connections store credentials and other connection information needed to securely access external services.
 
 
</details>

### 17. Which two artifact types can be published by a build pipeline in Azure DevOps?

- [ ] **A)** Pipeline artifacts
- [ ] **B)** Build artifacts
- [ ] **C)** SQL database backups
- [ ] **D)** PDF reports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure Pipelines supports publishing and consuming pipeline artifacts and build artifacts from build and release stages.
 
 
</details>

### 18. If three commits are pushed to main at the same time, how many builds will the trigger start?

```yaml
trigger:
  batch: true
  branches:
    include:
    - main
```

- [ ] **A)** One build
- [ ] **B)** Three builds
- [ ] **C)** No builds
- [ ] **D)** Six builds

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The batch setting causes the pipeline to wait and run a single build for the latest commit when multiple commits arrive together.
 
 
</details>

### 19. What is the purpose of pipeline caching in Azure Pipelines?

- [ ] **A)** Reuse dependencies and speed up later runs
- [ ] **B)** Encrypt pipeline secrets
- [ ] **C)** Monitor deployment status
- [ ] **D)** Replace unit testing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Pipeline caching stores dependencies or folders from one run and restores them later to reduce build time.
 
 
</details>

### 20. Which two agent types are available for running Azure Pipelines jobs?

- [ ] **A)** Microsoft-hosted agents
- [ ] **B)** Self-hosted agents
- [ ] **C)** Remote browsers
- [ ] **D)** Database servers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure Pipelines supports Microsoft-hosted agents and self-hosted agents installed on infrastructure you manage.
 
 
</details>


---

### **Design and implement processes and communications**

### 21. What is the main purpose of a release gate in Azure Pipelines?

- [ ] **A)** To evaluate specified conditions before or after a deployment and pause if unmet
- [ ] **B)** To compile application source code and generate build artifacts
- [ ] **C)** To automatically assign work items to team members after a release
- [ ] **D)** To store release documentation and approval history

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Release gates evaluate external conditions, such as quality metrics or incident status, and can pause or reject a deployment. They are not used for compilation, work item assignment, or documentation storage.
 
 
</details>

### 22. Which Azure DevOps capabilities directly support communication and traceability when implementing process changes? (Choose all that apply.)

- [ ] **A)** Work item discussions and mentions
- [ ] **B)** Service hooks and notifications
- [ ] **C)** Pipeline variable groups
- [ ] **D)** Build artifact feeds

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Work item discussions and mentions provide context-specific collaboration, while service hooks and notifications keep teams informed. Variable groups and artifact feeds are configuration and package stores, not communication or traceability features.
 
 
</details>

### 23. Examine the YAML pipeline snippet. What happens when a commit is pushed to 'main'?

```yaml
trigger:
- main

pool:
  vmImage: 'ubuntu-latest'

steps:
- script: echo "Build"

```

- [ ] **A)** It runs only when changes are pushed to the 'main' branch
- [ ] **B)** It runs when any branch in the repository changes
- [ ] **C)** It runs only for pull request validations
- [ ] **D)** It runs on a scheduled nightly basis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The trigger section lists only 'main', so the pipeline starts only on commits to that branch. No PR trigger or schedule is defined; the pool value only selects the hosted runner image.
 
 
</details>

### 24. What is the purpose of a branch policy in Azure Repos?

- [ ] **A)** Require pull request reviews and successful builds before changes are merged
- [ ] **B)** Delete remote branches automatically after each release
- [ ] **C)** Encrypt repository files at rest
- [ ] **D)** Prevent developers from cloning the repository

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Branch policies protect important branches by requiring pull request reviews, successful builds, and other checks before merging. They do not manage branch deletion, encryption, or clone permissions.
 
 
</details>


---

### **Develop a security and compliance plan**

### 25. Which Azure DevOps element is used to grant or restrict permissions for users and groups across an organization?

- [ ] **A)** Security groups
- [ ] **B)** Service connections
- [ ] **C)** Build agents
- [ ] **D)** Artifact feeds

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Security groups are the core permission containers in Azure DevOps, allowing administrators to grant consistent access to projects, repositories, and pipelines.
 
 
</details>

### 26. Which practices should be included when developing a security and compliance plan for Azure DevOps? (Choose all that apply.)

- [ ] **A)** Enforce multi-factor authentication
- [ ] **B)** Rotate personal access tokens and limit their scope
- [ ] **C)** Store passwords in pipeline variables
- [ ] **D)** Disable auditing to reduce log volume

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> MFA and careful PAT lifecycle management reduce unauthorized access. Storing passwords in pipelines and disabling audit logs violate security and compliance best practices.
 
 
</details>

### 27. The JSON below represents a security policy applied to a repository. What type of Azure DevOps feature is configured by this policy?

```json
{
  "enforceAdmins": true,
  "requiredReviewers": 1,
  "autoReset": true,
  "policyType": "MinimumNumberOfReviewers",
  "blocking": true
}
```

- [ ] **A)** Branch policies
- [ ] **B)** Service hooks
- [ ] **C)** Release gates
- [ ] **D)** Library variable groups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The configuration enforces a minimum number of reviewers before a pull request can be merged, which is a branch policy in Azure DevOps.
 
 
</details>

### 28. What is the primary purpose of Azure DevOps audit logs in a compliance plan?

- [ ] **A)** Detect and investigate changes and access events
- [ ] **B)** Automatically block all malicious users
- [ ] **C)** Replace the need for authentication policies
- [ ] **D)** Store source code backups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Audit logs provide a record of activities, including permission changes and sign-ins, enabling organizations to meet compliance requirements and investigate suspicious actions.
 
 
</details>


---

### **Implement an instrumentation strategy**

### 29. Which Azure Monitor component is used to collect telemetry from an application for diagnostics and usage analysis?

- [ ] **A)** Application Insights
- [ ] **B)** Azure Boards
- [ ] **C)** Azure Repos
- [ ] **D)** Azure Pipelines

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Application Insights is an Azure Monitor feature that provides application performance monitoring and telemetry collection, while Azure Boards, Azure Repos, and Azure Pipelines are Azure DevOps services.
 
 
</details>

### 30. Which telemetry data types can be collected by Azure Application Insights? Choose all that apply.

- [ ] **A)** Metrics
- [ ] **B)** Dependencies
- [ ] **C)** Exceptions
- [ ] **D)** User Stories

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Application Insights accepts telemetry such as requests, dependencies, exceptions, traces, and metrics. User stories are work items in Azure Boards, not telemetry types.
 
 
</details>

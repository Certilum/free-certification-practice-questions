<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Salesforce/Salesforce%20Certified%20Platform%20Development%20Lifecycle%20and%20Deployment%20Architect.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Salesforce Certified Development Lifecycle and Deployment Designer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Deployment Management](#deployment-management) (9 questions)
- [Development Lifecycle Management](#development-lifecycle-management) (9 questions)
- [Governance and Risk Management](#governance-and-risk-management) (6 questions)
- [Testing and Validation](#testing-and-validation) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:47:17.168Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Deployment Management | 9 |
| Development Lifecycle Management | 9 |
| Governance and Risk Management | 6 |
| Testing and Validation | 6 |

---

### **Deployment Management**

### 1. What is a Change Set in Salesforce deployment management?

- [ ] **A)** A declarative point-to-point process that uploads selected metadata components to a target org
- [ ] **B)** A Git-integrated visual tool that automates sandbox synchronization
- [ ] **C)** An API designed for high-volume package deployments
- [ ] **D)** A tool for migrating data between environments

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Change Sets are manual, declarative point-to-point transfers requiring a direct org connection; they do not integrate with Git or manage data migration.
 
 
</details>

### 2. Which limitations are correctly associated with Change Sets?

- [ ] **A)** They require a direct connection between orgs
- [ ] **B)** They cannot support branching or parallel development streams
- [ ] **C)** They lack detailed historical change tracking
- [ ] **D)** They support Git merge and pull request workflows

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Change Sets are linear and single-path, require org connections, and do not offer granular historical tracking or Git workflows.
 
 
</details>

### 3. Examine the XML snippet and identify the API that primarily relies on this manifest style for package-level operations.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<Package xmlns="http://soap.sforce.com/2006/04/metadata">
    <types>
        <members>Account</members>
        <name>CustomObject</name>
    </types>
    <version>58.0</version>
</Package>
```

- [ ] **A)** Metadata API
- [ ] **B)** Tooling API
- [ ] **C)** DevOps Center Work Items
- [ ] **D)** Data Migration API

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Metadata API uses package manifests to deploy or retrieve large metadata bundles; Change Sets and CLI depend on it.
 
 
</details>

### 4. What does DevOps Center require to function effectively?

- [ ] **A)** An external Git repository
- [ ] **B)** A direct org-to-org connection
- [ ] **C)** A Metadata API package
- [ ] **D)** A sandbox-only architecture

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> DevOps Center relies on an external Git provider to version, branch, merge, and synchronize metadata changes.
 
 
</details>

### 5. Which advantages does DevOps Center provide over Change Sets?

- [ ] **A)** Work Items group related metadata changes
- [ ] **B)** Conflicts are identified through Git integration
- [ ] **C)** Sandbox and Git repository synchronization is automated
- [ ] **D)** Metadata components are uploaded without any connection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> DevOps Center visualizes work, automates sandbox-Git sync, and detects conflicts via Git, unlike disconnected Change Sets.
 
 
</details>

### 6. The CLI command in the code block is run to check deployment readiness. Which deployment pattern does it support?

```bash
sf project deploy start --dry-run --source-dir force-app --target-org production
```

- [ ] **A)** Validate First
- [ ] **B)** Push-to-Pull
- [ ] **C)** Direct-to-Production
- [ ] **D)** Data Migration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The validation-only or dry-run pattern verifies errors, dependencies, and test coverage before actual deployment.
 
 
</details>

### 7. Which API is designed for high-volume operations and complete package deployments?

- [ ] **A)** Metadata API
- [ ] **B)** Tooling API
- [ ] **C)** DevOps Center
- [ ] **D)** Change Sets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Metadata API handles complex dependencies and large, package-level deployments across environments.
 
 
</details>

### 8. Which statements about Metadata API and Tooling API are true?

- [ ] **A)** Metadata API operates at package level
- [ ] **B)** Tooling API allows surgical updates to selected components
- [ ] **C)** Tooling API is optimized for developer velocity
- [ ] **D)** Metadata API is intended only for data migration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Metadata API handles package deployments; Tooling API is lightweight, granular, and built for developer-centric tasks.
 
 
</details>

### 9. The snippet below retrieves only metadata about an Apex class without performing a full deployment. Which API is represented?

```text
/services/data/v57.0/tooling/sobjects/ApexClass/01p5A000001x3aXQAQ
```

- [ ] **A)** Tooling API
- [ ] **B)** Metadata API
- [ ] **C)** Bulk API
- [ ] **D)** REST API for Change Sets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A URL path containing /tooling/ identifies the Tooling API, optimized for granular developer workflow calls.
 
 
</details>


---

### **Development Lifecycle Management**

### 10. Which answer best describes the role of a Change Set in Salesforce metadata movement between connected orgs?

- [ ] **A)** Manual point-to-point metadata transfer between orgs
- [ ] **B)** Git-based branch management for parallel work
- [ ] **C)** API for real-time code analysis in IDEs
- [ ] **D)** Tool for migrating records between orgs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Change Set is a manual, declarative process that packages selected metadata and uploads it to a target org through a direct connection.
 
 
</details>

### 11. Which two statements are true about the features and requirements of Salesforce DevOps Center?

- [ ] **A)** Salesforce-native and Git-integrated
- [ ] **B)** Groups related changes into Work Items
- [ ] **C)** Eliminates the need for Git
- [ ] **D)** Only supports linear deployments

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DevOps Center is Salesforce-native and uses Git integration. It groups related changes into Work Items, but it requires Git and does not replace branching.
 
 
</details>

### 12. Based on the command shown in the code block, what action is being performed on the target production org?

```bash
sf project deploy start --dry-run --source-dir force-app --target-org production
```

- [ ] **A)** Validates without saving changes
- [ ] **B)** Deploys metadata to production
- [ ] **C)** Retrieves metadata from Git
- [ ] **D)** Creates a Scratch Org

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The --dry-run flag runs a validation-only deployment, checking components and tests without making changes to the target org.
 
 
</details>

### 13. In the Salesforce development lifecycle, what is the Tooling API primarily designed to optimize?

- [ ] **A)** Granular developer metadata interactions
- [ ] **B)** Bulk package deploys
- [ ] **C)** Data migration between orgs
- [ ] **D)** Automatic Change Set creation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Tooling API is lightweight and optimized for developer workflows such as IDE integrations, code analysis, and surgical metadata updates.
 
 
</details>

### 14. Which two statements correctly compare the Metadata API with the Tooling API for deployment and development tasks?

- [ ] **A)** Metadata API handles large package deployments
- [ ] **B)** Tooling API supports granular developer updates
- [ ] **C)** Tooling API replaces Metadata API entirely
- [ ] **D)** Metadata API can only retrieve metadata

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Metadata API is for high-volume package deployments and retrievals; Tooling API enables surgical, real-time developer interactions. Neither replaces the other.
 
 
</details>

### 15. What is the outcome of running the conversion command shown in the code block for metadata format management?

```bash
sf project convert mdapi --root-dir mdapi --output-dir force-app
```

- [ ] **A)** Metadata API format to source format
- [ ] **B)** Source format to Metadata API format
- [ ] **C)** Deploys metadata to production
- [ ] **D)** Creates a Scratch Org

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The convert mdapi command transforms Metadata API format into source format so metadata can be managed in a Git-based workflow.
 
 
</details>

### 16. What is a Work Item in Salesforce DevOps Center and how does it improve release visibility?

- [ ] **A)** Related metadata changes grouped with visibility
- [ ] **B)** Single point-to-point Change Set upload
- [ ] **C)** A Git branch for hotfixes only
- [ ] **D)** An XML metadata definition file

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Work Items group related metadata changes under one logical unit, improving visibility and traceability in the pipeline.
 
 
</details>

### 17. Which two statements correctly describe the differences between Change Sets and DevOps Center in a deployment lifecycle?

- [ ] **A)** Change Sets do not support branching
- [ ] **B)** DevOps Center requires a Git repository
- [ ] **C)** Change Sets support complex branching
- [ ] **D)** DevOps Center does not need Git

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Change Sets are linear and require a direct org connection. DevOps Center depends on Git and supports branching, merging, and pull requests.
 
 
</details>

### 18. In source-driven development, what does the command in the code block indicate about the location of the authoritative source?

```bash
sf project deploy start --source-dir force-app --target-org sandbox
```

- [ ] **A)** The Git repository
- [ ] **B)** The target org
- [ ] **C)** The Change Set
- [ ] **D)** The production environment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In source-driven development, local source managed in Git is the source of truth; deployments synchronize that source to target orgs.
 
 
</details>


---

### **Governance and Risk Management**

### 19. What is a defining characteristic of Change Sets?

- [ ] **A)** They automatically create branches for parallel development.
- [ ] **B)** They manually package selected metadata and require a direct org-to-org connection.
- [ ] **C)** They rely on an external GitHub repository to store metadata versions.
- [ ] **D)** They record every historical change at the component level.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Change Sets are manual point-to-point tools that package selected metadata and require a direct connection. They do not support branching or granular historical tracking.
 
 
</details>

### 20. Which statements about DevOps Center are correct? Select all that apply.

- [ ] **A)** It is a Salesforce-native application with a visual management interface.
- [ ] **B)** It automates synchronization between a sandbox and a Git repository.
- [ ] **C)** It can operate without an external Git repository when used for simple deployments.
- [ ] **D)** It groups related metadata changes into Work Items for better pipeline visibility.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> DevOps Center is Salesforce-native, Git-integrated, and uses Work Items. It requires an external Git provider and is not designed to function without one.
 
 
</details>

### 21. What is the purpose of the command shown in the code block?

```bash
sf project deploy start --target-org myDevSandbox
```

- [ ] **A)** It deploys local source to the specified Salesforce org.
- [ ] **B)** It retrieves metadata from a sandbox to local files.
- [ ] **C)** It creates a scratch org for isolated development.
- [ ] **D)** It converts source-format files into Metadata API format.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The sf project deploy start command pushes local source code into the target org, making it the primary CLI deployment command.
 
 
</details>

### 22. What is the primary purpose of the Metadata API's retrieve call?

- [ ] **A)** To deploy Apex classes to production
- [ ] **B)** To retrieve metadata components from an org so they can be versioned or deployed
- [ ] **C)** To query individual record data stored in custom objects
- [ ] **D)** To run automated Apex tests before deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Metadata API retrieve call extracts metadata from an org for version control or later deployment. It does not migrate data or run Apex tests.
 
 
</details>

### 23. Which characteristics are true of the Tooling API? Select all that apply.

- [ ] **A)** It is optimized for developer-centric, granular interactions.
- [ ] **B)** It is commonly used for IDE integrations and real-time code analysis.
- [ ] **C)** It is the standard choice for high-volume, full package deployments.
- [ ] **D)** It can perform surgical updates to specific metadata elements.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> The Tooling API is lightweight and designed for developer workflows. The Metadata API, not the Tooling API, is best for high-volume package deployments.
 
 
</details>

### 24. What does this command do in the deployment process?

```bash
sf project deploy start --dry-run --target-org production
```

- [ ] **A)** It applies all changes to production immediately.
- [ ] **B)** It validates deployment, dependencies, and tests without changing the org.
- [ ] **C)** It creates a rollback plan for the previous deployment.
- [ ] **D)** It generates a package from the org's current metadata.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The --dry-run flag uses the validate-first pattern, checking components, dependencies, and Apex test readiness before an actual deployment.
 
 
</details>


---

### **Testing and Validation**

### 25. Which deployment pattern does the Salesforce CLI enable by using dry-run or validation-only flags before any changes are committed to production?

- [ ] **A)** Validate First
- [ ] **B)** Retroactive Deployment
- [ ] **C)** Hot Swap
- [ ] **D)** Schema Compare

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Salesforce CLI supports the Validate First deployment pattern through dry-run or validation-only flags, allowing teams to check deployment errors and test coverage before committing changes.
 
 
</details>

### 26. Which statements correctly describe DevOps Center? Select all that apply.

- [ ] **A)** It requires an external Git repository to operate effectively.
- [ ] **B)** It provides a visual interface and automates synchronization between sandboxes and Git.
- [ ] **C)** It groups related metadata changes into Work Items for better deployment visibility.
- [ ] **D)** It eliminates the need for Git by operating entirely inside Salesforce.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> DevOps Center is a Salesforce-native, Git-integrated tool. It requires an external Git provider, provides a visual interface, automates sandbox-Git synchronization, and uses Work Items to group metadata changes. It does not remove the need for Git.
 
 
</details>

### 27. A developer executes the following Salesforce CLI command. What is the primary purpose of this command?

```bash
sf project deploy start --target-org production --dry-run --test-level RunLocalTests
```

- [ ] **A)** Deploy all local metadata to production and run local tests.
- [ ] **B)** Validate the deployment and run tests without committing changes.
- [ ] **C)** Retrieve metadata from production into the local source directory.
- [ ] **D)** Delete the production org's metadata and recreate it.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The --dry-run flag triggers a validation-only deployment, confirming whether the metadata would deploy and whether tests pass, without actually changing the target org.
 
 
</details>

### 28. Which API is designed for high-volume operations, complete package deployments, and serves as the backbone of Change Sets and CLI-driven deployments?

- [ ] **A)** Metadata API
- [ ] **B)** Tooling API
- [ ] **C)** Analytics API
- [ ] **D)** Connect REST API

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Metadata API handles high-volume operations, complete package deployments, and complex metadata dependencies. It is the backbone of Change Sets and CLI-driven deployments.
 
 
</details>

### 29. Which statements correctly describe the Tooling API? Select all that apply.

- [ ] **A)** It is a lightweight version of the Metadata API optimized for developer-centric tasks.
- [ ] **B)** It is the primary engine for deploying complete packages and complex dependency bundles.
- [ ] **C)** It allows faster, more granular interactions with specific metadata components.
- [ ] **D)** It is essential for IDE integrations, real-time code analysis, and surgical updates.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> The Tooling API is a lightweight, developer-focused API for granular interactions and speeds up IDE integrations and code analysis. It does not handle large package deployments like the Metadata API.
 
 
</details>

### 30. A CI/CD pipeline runs the Salesforce CLI command below. Which outcome should the pipeline expect?

```bash
sf project deploy start --target-org ci-sandbox --dry-run --test-level RunAllTestsInOrg
```

- [ ] **A)** The target sandbox receives all changes and runs all tests.
- [ ] **B)** The command validates the deployment and executes all tests, but makes no permanent changes.
- [ ] **C)** The command synchronizes local source with the sandbox and then deletes the sandbox.
- [ ] **D)** The command only retrieves Apex test results from the target sandbox.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> This command is a validation-only deployment with --dry-run. It checks whether the package can be deployed and whether tests pass, without permanently changing the target org.
 
 
</details>

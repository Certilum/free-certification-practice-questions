<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/HashiCorp/HashiCorp%20Certified%3A%20Terraform%20Associate%20(004)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>HashiCorp Certified: Terraform Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [HCP Terraform Workspaces and Projects](#hcp-terraform-workspaces-and-projects) (2 questions)
- [Infrastructure as Code (IaC) with Terraform](#infrastructure-as-code-iac-with-terraform) (4 questions)
- [Lifecycle and Advanced Configuration Rules](#lifecycle-and-advanced-configuration-rules) (1 questions)
- [Terraform CLI and Providers](#terraform-cli-and-providers) (4 questions)
- [Terraform Cloud and Enterprise Capabilities](#terraform-cloud-and-enterprise-capabilities) (3 questions)
- [Terraform Configuration Language](#terraform-configuration-language) (6 questions)
- [Terraform Lifecycle and Workflows](#terraform-lifecycle-and-workflows) (4 questions)
- [Terraform Modules](#terraform-modules) (3 questions)
- [Terraform State Management](#terraform-state-management) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:53.122Z |
| Domains | 9 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| HCP Terraform Workspaces and Projects | 2 |
| Infrastructure as Code (IaC) with Terraform | 4 |
| Lifecycle and Advanced Configuration Rules | 1 |
| Terraform CLI and Providers | 4 |
| Terraform Cloud and Enterprise Capabilities | 3 |
| Terraform Configuration Language | 6 |
| Terraform Lifecycle and Workflows | 4 |
| Terraform Modules | 3 |
| Terraform State Management | 3 |

---

### **HCP Terraform Workspaces and Projects**

### 1. Which statement accurately describes the relationship between HCP Terraform projects and workspaces?

- [ ] **A)** Project groups workspaces; each has own state.
- [ ] **B)** Workspace groups projects; project shares state.
- [ ] **C)** Projects store workspace state files.
- [ ] **D)** Workspaces require project membership to store state.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Projects are administrative containers that group workspaces for governance. Each workspace holds its own unique state file and execution environment, while projects do not hold state.
 
 
</details>

### 2. Which two statements about HCP Terraform variable sets are correct?

- [ ] **A)** Can be applied to multiple workspaces or projects.
- [ ] **B)** Updates propagate to all associated workspaces.
- [ ] **C)** They replace locally defined workspace variables.
- [ ] **D)** They store state files for shared workspaces.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Variable sets centralize shared configuration and can be assigned to multiple workspaces or projects. A single update propagates to all associated workspaces, reducing overhead and preventing drift.
 
 
</details>


---

### **Infrastructure as Code (IaC) with Terraform**

### 3. Which statement best defines Infrastructure as Code (IaC) as a practice for managing IT environments?

- [ ] **A)** Managing infrastructure through machine-readable configuration files
- [ ] **B)** Using manual runbooks to configure cloud resources
- [ ] **C)** Writing shell scripts to call cloud APIs
- [ ] **D)** Deploying application code to running servers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IaC encodes the desired infrastructure state in configuration files, enabling version control, automated review, and consistent provisioning.
 
 
</details>

### 4. Which benefits does Infrastructure as Code provide when it is used to manage cloud environments? Select all that apply.

- [ ] **A)** Version control integration
- [ ] **B)** Idempotent provisioning
- [ ] **C)** Reproducible environments
- [ ] **D)** Real-time performance monitoring

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> IaC provides version control, idempotent applies, and repeatable environments. It does not replace performance monitoring or remove the need for credentials.
 
 
</details>

### 5. What type of infrastructure component is declared by each top-level block in the configuration? Choose the best answer.

```hcl
resource "aws_instance" "web" {
  ami           = "ami-0c55b159cbfafe1f0"
  instance_type = "t3.micro"
}

```

- [ ] **A)** Resource
- [ ] **B)** Provider
- [ ] **C)** Variable
- [ ] **D)** Output

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Terraform configuration declares resources, such as aws_instance, that the provider creates and manages.
 
 
</details>

### 6. What is the meaning of idempotency when Terraform apply is executed multiple times against an unchanged configuration?

- [ ] **A)** No changes after desired state is reached
- [ ] **B)** Repeated commands produce identical output
- [ ] **C)** Performance is monitored continuously
- [ ] **D)** Resource deletion is permanently prevented

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An idempotent apply makes no changes when actual state already matches the defined desired state.
 
 
</details>


---

### **Lifecycle and Advanced Configuration Rules**

### 7. Which lifecycle meta-argument prevents Terraform from destroying a resource during a plan or apply?

- [ ] **A)** prevent_destroy
- [ ] **B)** create_before_destroy
- [ ] **C)** ignore_changes
- [ ] **D)** ensure_destroy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> prevent_destroy is a lifecycle meta-argument that protects a resource from being destroyed by Terraform. If a plan would destroy the resource, Terraform halts with an error, which is useful for high-value assets such as production databases.
 
 
</details>


---

### **Terraform CLI and Providers**

### 8. What is the primary distinction between Terraform CLI installation and Terraform initialization?

- [ ] **A)** Installing the CLI places the binary on the system, while initialization prepares the working directory by downloading providers and setting up the backend.
- [ ] **B)** Installing the CLI downloads provider plugins, while initialization simply verifies the HCL syntax.
- [ ] **C)** Installing the CLI creates the .terraform.lock.hcl file, while initialization makes the terraform command available globally.
- [ ] **D)** There is no difference; both terms describe the same action.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CLI installation makes the terraform binary executable from the system PATH. Initialization is project-specific and prepares the working directory by downloading providers and configuring the backend.
 
 
</details>

### 9. Which two artifacts are generated or managed when you run terraform init?

- [ ] **A)** The local .terraform directory containing provider plugins
- [ ] **B)** The .terraform.lock.hcl dependency lock file
- [ ] **C)** The main.tf configuration file
- [ ] **D)** The state file in the remote backend

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> During initialization, Terraform downloads provider plugins into the .terraform directory and creates or updates .terraform.lock.hcl. It does not create configuration files or the state file.
 
 
</details>

### 10. After cloning a repository that contains the configuration shown, what command must be run before terraform plan can succeed?

```hcl
terraform {
  required_providers {
    aws = {
      source  = "hashicorp/aws"
      version = "~> 4.0"
    }
  }
}

resource "aws_s3_bucket" "example" {
  bucket = "my-example-bucket"
}

```

- [ ] **A)** terraform init
- [ ] **B)** terraform install
- [ ] **C)** terraform download
- [ ] **D)** terraform validate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> terraform init is required to download provider plugins, initialize the backend, and create the dependency lock file before planning or applying.
 
 
</details>

### 11. What does the version constraint ~> 1.2 indicate in a provider block?

- [ ] **A)** Any version from 1.2 up to, but not including, 2.0
- [ ] **B)** Exactly version 1.2
- [ ] **C)** Any version from 1.2 up to, but not including, 1.3
- [ ] **D)** Any version greater than or equal to 2.0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The pessimistic constraint ~> 1.2 allows versions greater than or equal to 1.2 and less than 2.0, preventing major breaking upgrades.
 
 
</details>


---

### **Terraform Cloud and Enterprise Capabilities**

### 12. Which Terraform Cloud feature automatically prevents non-compliant infrastructure from being deployed in a managed organization?

- [ ] **A)** Policy as Code with Sentinel or OPA
- [ ] **B)** Local state files
- [ ] **C)** Public Terraform Registry
- [ ] **D)** Manual code reviews

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Policy as Code uses Sentinel or OPA to evaluate plans and block non-compliant infrastructure before deployment, providing automated governance.
 
 
</details>

### 13. Which of the following are benefits of Terraform Cloud or HCP Terraform compared to local CLI workflows? Select all that apply.

- [ ] **A)** Centralized remote state management
- [ ] **B)** Automated policy enforcement
- [ ] **C)** VCS-driven workflow automation
- [ ] **D)** Local execution on developer machines

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Terraform Cloud provides centralized state, automated governance, and VCS-driven workflows. Local execution on developer machines is opposite to its remote execution model.
 
 
</details>

### 14. Refer to the configuration code block below. Which Terraform Cloud capability is being demonstrated by this resource?

```hcl
data "terraform_remote_state" "network" {
  backend = "remote"
  config = {
    organization = "example-corp"
    workspaces = {
      name = "network"
    }
  }
}
```

- [ ] **A)** Remote state sharing between workspaces
- [ ] **B)** Private module registry
- [ ] **C)** Sentinel policy enforcement
- [ ] **D)** Local CLI execution

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The terraform_remote_state data source reads output values from another workspace's remote state, demonstrating centralized remote state sharing in Terraform Cloud.
 
 
</details>


---

### **Terraform Configuration Language**

### 15. Which HCL element is the primary structural unit that acts as a container for arguments and nested blocks?

- [ ] **A)** Block
- [ ] **B)** Argument
- [ ] **C)** Expression
- [ ] **D)** Attribute

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A block is the primary structural unit in HCL, acting as a container for arguments and nested blocks.
 
 
</details>

### 16. Which statements about Terraform parameterization mechanisms are correct? (Select all that apply.)

- [ ] **A)** Input variables are the primary interface for external customization.
- [ ] **B)** Local values can be set by users through .tfvars files.
- [ ] **C)** Output values are consumer-facing return values from a module.
- [ ] **D)** Output values are commonly used to set resource arguments inside the same module.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Input variables allow external customization, and output values expose module data. Local values are internal, and outputs do not flow back into resource arguments.
 
 
</details>

### 17. In the displayed HCL code, how should the value assigned to the 'Name' tag be classified?

```hcl
resource "aws_instance" "web" {
  ami           = "ami-12345"
  instance_type = "t2.micro"
  tags = {
    Name = "web-server-${var.environment}"
  }
}
```

- [ ] **A)** A literal string
- [ ] **B)** An interpolation expression
- [ ] **C)** An argument name
- [ ] **D)** A block label

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Name tag value contains ${...}, so it is an interpolation expression that embeds a dynamic value inside a string.
 
 
</details>

### 18. What is the main purpose of input variables in Terraform?

- [ ] **A)** To enable customization of deployments from outside the configuration
- [ ] **B)** To store internal calculated values used in multiple locations
- [ ] **C)** To expose resource attributes to module consumers
- [ ] **D)** To replace the remote state backend

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Input variables are the primary interface for external configuration, allowing users to customize parameters without modifying the core logic.
 
 
</details>

### 19. Which statements about resource dependencies are correct? (Select all that apply.)

- [ ] **A)** An implicit dependency is created when one resource references another resource's attribute.
- [ ] **B)** depends_on should be used for every resource relationship.
- [ ] **C)** depends_on is appropriate when no attribute reference exists between resources.
- [ ] **D)** The DAG permits circular dependencies so resources can wait on each other.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Implicit dependencies come from attribute references, while depends_on should be used only when no attribute link exists. Circular dependencies are not allowed in a DAG.
 
 
</details>

### 20. In the resource configuration shown, what type of dependency exists between the instance and the subnet?

```hcl
resource "aws_instance" "web" {
  ami           = "ami-12345"
  instance_type = "t2.micro"
  subnet_id     = aws_subnet.main.id
}

resource "aws_subnet" "main" {
  vpc_id     = "vpc-12345"
  cidr_block = "10.0.1.0/24"
}
```

- [ ] **A)** Implicit dependency
- [ ] **B)** Explicit dependency
- [ ] **C)** Circular dependency
- [ ] **D)** No dependency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The instance references aws_subnet.main.id, so Terraform automatically detects an implicit dependency.
 
 
</details>


---

### **Terraform Lifecycle and Workflows**

### 21. Which Terraform command previews the changes that will be made to infrastructure without modifying real-world resources?

- [ ] **A)** terraform plan
- [ ] **B)** terraform apply
- [ ] **C)** terraform validate
- [ ] **D)** terraform init

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> terraform plan is the speculative phase of the workflow. It reads the current state and provider information to produce an execution plan, but it does not change infrastructure or persist updates to the state file.
 
 
</details>

### 22. Which statements correctly describe the core Terraform workflow phases? Select all that apply.

- [ ] **A)** The write phase uses HCL to define the desired state of infrastructure.
- [ ] **B)** The plan phase is a dry-run that does not alter real infrastructure.
- [ ] **C)** The apply phase updates the state file to match the real-world resources.
- [ ] **D)** The plan phase writes changes to the state file on disk.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The write phase codifies the desired state in HCL. The plan phase is speculative and only reads state and provider data, so it has no side effects. The apply phase executes API calls and updates the state file. Terraform plan never persists changes to the state file.
 
 
</details>

### 23. Review the command output in the code block. Which Terraform command produces this execution summary before changing infrastructure?

```plaintext
Plan: 1 to add, 0 to change, 0 to destroy.
```

- [ ] **A)** terraform plan
- [ ] **B)** terraform apply
- [ ] **C)** terraform init
- [ ] **D)** terraform validate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The output \"Plan: 1 to add, 0 to change, 0 to destroy\" is an execution plan summary produced by terraform plan. It describes proposed actions without applying them to real infrastructure.
 
 
</details>

### 24. Which Terraform command performs a lightweight, local check of configuration syntax and internal consistency without needing provider credentials or state access?

- [ ] **A)** terraform validate
- [ ] **B)** terraform plan
- [ ] **C)** terraform apply
- [ ] **D)** terraform init

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> terraform validate performs static analysis on the configuration to check syntax and internal consistency. It does not interact with the state file or cloud provider APIs, making it a fast and local safety check.
 
 
</details>


---

### **Terraform Modules**

### 25. Which type of path is required to call a local Terraform module?

- [ ] **A)** Relative or absolute filesystem path (e.g., './modules/vpc')
- [ ] **B)** Registry namespace/name/provider (e.g., 'hashicorp/vpc/aws')
- [ ] **C)** Git URL with a version tag
- [ ] **D)** Remote S3 object URL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A local module is called by setting source to a filesystem path such as './modules/vpc'. Registry modules use the namespace/name/provider format, not file paths.
 
 
</details>

### 26. Which two statements about module inputs and outputs are correct? (Select two.)

- [ ] **A)** Input variables define the module's inbound interface
- [ ] **B)** Output values expose resource attributes to the calling module
- [ ] **C)** Variables inside a module are automatically assigned from root variables
- [ ] **D)** Resource attributes in a module are directly accessible to the root

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Variables are the module's inbound API, and outputs expose results to the caller. Terraform requires explicit passing and does not allow direct access to encapsulated resources.
 
 
</details>

### 27. After the module block in this configuration is added, which command must be run before terraform plan?

```hcl
module "vpc" {
  source = "./modules/vpc"
}
```

- [ ] **A)** terraform init
- [ ] **B)** terraform plan
- [ ] **C)** terraform apply
- [ ] **D)** terraform validate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> After adding a new module, terraform init must be run because it indexes the path and populates .terraform/modules. The other commands do not perform this step.
 
 
</details>


---

### **Terraform State Management**

### 28. What is the primary role of the Terraform state file?

- [ ] **A)** It maps logical resource names to real-world resource IDs.
- [ ] **B)** It stores the HCL configuration source code.
- [ ] **C)** It records all user commands and API calls.
- [ ] **D)** It caches provider plugins for faster execution.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The state file is Terraform's source of truth for mapping configured resource names to provider-generated IDs. This mapping enables updates, dependency tracking, and drift detection.
 
 
</details>

### 29. Which two statements about Terraform state are correct? Select all that apply.

- [ ] **A)** State stores sensitive values such as passwords in plain text.
- [ ] **B)** State records the relationship between configuration and live resources.
- [ ] **C)** State files are written in HCL format like configuration files.
- [ ] **D)** State files should be committed to Git for version control.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> State contains sensitive values in plain text and links configuration to real infrastructure. It is JSON, not HCL, and should never be committed to version control.
 
 
</details>

### 30. A resource block was renamed as shown in the code. Which command updates the state so Terraform does not plan to replace the resource?

```hcl
# Original configuration
resource "aws_instance" "web_server" {
  ami           = "ami-123456"
  instance_type = "t3.micro"
}

# Renamed configuration
resource "aws_instance" "application_server" {
  ami           = "ami-123456"
  instance_type = "t3.micro"
}
```

- [ ] **A)** terraform state mv aws_instance.web_server aws_instance.application_server
- [ ] **B)** terraform state rm aws_instance.web_server
- [ ] **C)** terraform state list
- [ ] **D)** terraform destroy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> terraform state mv updates the state address without touching the cloud resource. Without it, Terraform would plan to destroy the old instance and create a new one.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Oracle%20Cloud%20Infrastructure%202026%20DevOps%20Professional.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Oracle Cloud Infrastructure 2026 DevOps Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [CI/CD Practices](#ci-cd-practices) (9 questions)
- [Container Orchestration (OKE)](#container-orchestration-oke) (9 questions)
- [DevOps Principles and Containerization](#devops-principles-and-containerization) (5 questions)
- [DevSecOps](#devsecops) (3 questions)
- [Infrastructure as Code](#infrastructure-as-code) (3 questions)
- [Monitoring and Observability](#monitoring-and-observability) (1 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:46:07.981Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| CI/CD Practices | 9 |
| Container Orchestration (OKE) | 9 |
| DevOps Principles and Containerization | 5 |
| DevSecOps | 3 |
| Infrastructure as Code | 3 |
| Monitoring and Observability | 1 |

---

### **CI/CD Practices**

### 1. Which statement best defines continuous integration in a DevOps context?

- [ ] **A)** Frequently merging code changes and running automated builds and tests
- [ ] **B)** Deploying every merge directly to production only
- [ ] **C)** Substituting automated tests with manual release tests
- [ ] **D)** Keeping code changes isolated for several weeks before review

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Continuous integration means frequently integrating code changes into a shared repository and validating each change with automated builds and tests, which helps detect issues early.
 
 
</details>

### 2. Which of the following are core DevOps principles? Select all that apply.

- [ ] **A)** Automation
- [ ] **B)** Feedback loops
- [ ] **C)** Manual handoffs
- [ ] **D)** Siloed teams

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DevOps principles emphasize automation, collaboration, measurement, and feedback. Manual handoffs and siloed teams slow delivery and reduce shared responsibility.
 
 
</details>

### 3. In the pipeline snippet, what is the purpose of the stage named test?

```yaml
stages:
  - build
  - test
  - deploy
job:
  stage: test
  script:
    - echo "Running tests"
    - mvn test
```

- [ ] **A)** Compile source code into deployable artifacts
- [ ] **B)** Run automated tests against the application
- [ ] **C)** Publish container images to a registry
- [ ] **D)** Provision production infrastructure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In a CI/CD pipeline, the test stage runs automated tests to validate application behavior before the deployment or packaging stages.
 
 
</details>

### 4. Which statement describes a core benefit of containerization?

- [ ] **A)** Applications and their dependencies can be packaged together and run consistently across environments
- [ ] **B)** All security vulnerabilities are automatically removed from the application source code
- [ ] **C)** Containers remove the need for operating-system-level isolation
- [ ] **D)** Applications no longer require any runtime environment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Containerization packages application code and its dependencies into a lightweight image, making application behavior consistent across development, testing, and production.
 
 
</details>

### 5. Which of the following are essential parts of a containerized CI/CD pipeline? Select all that apply.

- [ ] **A)** Container image
- [ ] **B)** Container registry
- [ ] **C)** Dockerfile-like image definition
- [ ] **D)** Physical server lease agreement

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A container image is built from an image definition file, stored and distributed through a container registry, and then pulled by runtime platforms for deployment.
 
 
</details>

### 6. Given the provided container image definition, which instruction sets the base runtime image?

```dockerfile
FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
CMD ["npm", "start"]
```

- [ ] **A)** FROM node:18-alpine
- [ ] **B)** WORKDIR /app
- [ ] **C)** RUN npm install
- [ ] **D)** COPY . /app

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The FROM instruction initializes a new image and defines the base runtime environment by referencing an existing image such as node:18-alpine.
 
 
</details>

### 7. What is meant by continuous delivery in a software delivery context?

- [ ] **A)** Every change that passes automated tests can be released to production at any time
- [ ] **B)** Every change is released to production automatically without running any tests
- [ ] **C)** Releases can only happen once per year after a complete manual review
- [ ] **D)** Software testing is completed after the production deployment is finished

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Continuous delivery keeps software in a releasable state at all times by automating builds and tests, allowing releases to be executed whenever needed.
 
 
</details>

### 8. Which practices support a mature CI/CD environment? Select all that apply.

- [ ] **A)** Version control and configuration management
- [ ] **B)** Automated testing at multiple stages
- [ ] **C)** Consistent and reproducible environments
- [ ] **D)** Unreproducible manual server changes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A mature CI/CD environment relies on version control, automated testing, and reproducible environments. Manual server changes make delivery unpredictable and risky.
 
 
</details>

### 9. According to the pipeline snippet, what does the quality stage execute?

```yaml
stages:
  - build
  - quality
  - package
quality:
  stage: quality
  script:
    - sonar-scanner
```

- [ ] **A)** Run static code analysis
- [ ] **B)** Build application binaries from source code
- [ ] **C)** Create encrypted database backups
- [ ] **D)** Destroy temporary cloud resources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The quality stage runs the sonar-scanner command, which is a common static code analysis tool used to inspect code quality and identify defects.
 
 
</details>


---

### **Container Orchestration (OKE)**

### 10. In Oracle Cloud Infrastructure, what does the acronym OKE represent?

- [ ] **A)** Oracle Kubernetes Engine
- [ ] **B)** Oracle Key Management Engine
- [ ] **C)** Oracle Kernel Enclave
- [ ] **D)** Open Kubernetes Environment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OKE is Oracle's managed Kubernetes service, which handles Kubernetes control plane operations and simplifies deploying containerized workloads.
 
 
</details>

### 11. Which two statements reflect core DevOps principles that support container orchestration in a modern cloud environment?

- [ ] **A)** Automating the application delivery pipeline
- [ ] **B)** Collaborating across development and operations teams
- [ ] **C)** Separating application monitoring from operations responsibilities
- [ ] **D)** Requiring manual approval for every infrastructure change

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DevOps combines automated delivery, collaboration, monitoring, and infrastructure as code. Manual approvals and isolated teams conflict with DevOps.
 
 
</details>

### 12. Look at the command in the code block. Which OKE resource is inspected by that command?

```bash
kubectl get nodes
```

- [ ] **A)** Nodes
- [ ] **B)** Pods
- [ ] **C)** Deployments
- [ ] **D)** Services

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The kubectl get nodes command lists worker nodes in the Kubernetes cluster. This helps inspect OKE node status and availability.
 
 
</details>

### 13. What is the role of a node pool in an OKE cluster?

- [ ] **A)** It defines a set of worker nodes with identical configuration.
- [ ] **B)** It stores container images used by deployments.
- [ ] **C)** It manages DNS records for published services.
- [ ] **D)** It provides persistent block storage to application containers.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A node pool is a group of worker nodes that share compute shape, image, network, and other settings, making management and upgrades predictable.
 
 
</details>

### 14. Which methods can be used to connect to and manage an OKE cluster? Select all that apply.

- [ ] **A)** Using kubectl commands
- [ ] **B)** Using the OCI Console
- [ ] **C)** Using the standard Kubernetes API
- [ ] **D)** Using MySQL Shell

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> OKE exposes the standard Kubernetes API, so kubectl, SDKs, the OCI Console, and REST calls can manage cluster resources. MySQL Shell is unrelated.
 
 
</details>

### 15. The code block contains a Kubernetes manifest. Which object kind is defined by the manifest?

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: storefront
spec:
  replicas: 3
```

- [ ] **A)** Deployment
- [ ] **B)** Service
- [ ] **C)** Pod
- [ ] **D)** ReplicaSet

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The manifest uses kind: Deployment to declare a storefront Deployment with three replicas, which manages pods in OKE.
 
 
</details>

### 16. Which container characteristic helps a container run consistently across different OKE environments?

- [ ] **A)** It packages application code together with its dependencies and runtime.
- [ ] **B)** It includes a separate guest operating system for each workload.
- [ ] **C)** It depends on the exact kernel configuration of the source host.
- [ ] **D)** It must be recompiled for every target environment.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Containers bundle an application and dependencies, but share the host OS kernel. This packaging provides consistency and portability.
 
 
</details>

### 17. Which two statements are true about worker nodes in OKE?

- [ ] **A)** Worker nodes run pods and containers.
- [ ] **B)** Worker nodes are grouped into node pools.
- [ ] **C)** Worker nodes are created by applying a Helm chart.
- [ ] **D)** Worker nodes are the same as a Kubernetes namespace.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Worker nodes provide the compute capacity that runs pods. OKE organizes worker nodes into node pools for easier lifecycle management and scaling.
 
 
</details>

### 18. The code block shows a kubectl command. What happens when this command is executed against the storefront deployment?

```bash
kubectl scale deployment storefront --replicas=5
```

- [ ] **A)** It sets the storefront deployment to five replicas.
- [ ] **B)** It deletes the storefront deployment.
- [ ] **C)** It creates a namespace called storefront.
- [ ] **D)** It restarts all storefront pods and keeps three replicas.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> kubectl scale changes the number of desired replicas for a Deployment to five, instructing the controller to add or remove pods as needed.
 
 
</details>


---

### **DevOps Principles and Containerization**

### 19. In a DevOps context, what is the main purpose of using containers to deliver applications?

- [ ] **A)** Package an application with its dependencies
- [ ] **B)** Replace continuous integration tools
- [ ] **C)** Eliminate the need for application testing
- [ ] **D)** Provide graphical user interfaces for servers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Containerization packages an application with its runtime dependencies, making it portable. It does not replace CI tools, testing, or server GUIs.
 
 
</details>

### 20. In a DevOps transformation, which of the following practices and philosophies are usually considered core principles?

- [ ] **A)** Continuous collaboration between development and operations
- [ ] **B)** Automating build, test, and deployment processes
- [ ] **C)** Measuring results and sharing feedback
- [ ] **D)** Requiring manual approvals for every delivery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> DevOps emphasizes collaboration, automated pipelines, and measurement/feedback. Manual approval for every delivery conflicts with continuous delivery practices.
 
 
</details>

### 21. In the Dockerfile shown in the code block, what effect does the WORKDIR instruction have on the build process?

```dockerfile
FROM python:3.11-slim
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY app.py .
CMD ["python", "app.py"]
```

- [ ] **A)** Changes the active directory for subsequent instructions
- [ ] **B)** Exposes a port to the host machine
- [ ] **C)** Adds an environment variable to the container
- [ ] **D)** Selects the base image to use

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> WORKDIR sets the working directory for instructions that follow, such as COPY, RUN, and CMD, inside the container image.
 
 
</details>

### 22. In modern DevOps pipelines, the acronym CI/CD refers to which pair of software delivery practices?

- [ ] **A)** Continuous Integration and Continuous Delivery/Deployment
- [ ] **B)** Centralized Infrastructure and Centralized Deployment
- [ ] **C)** Code Integration and Code Deployment
- [ ] **D)** Container Isolation and Container Deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CI/CD combines Continuous Integration with Continuous Delivery or Continuous Deployment, enabling code to move from commit to production through automated pipelines.
 
 
</details>

### 23. When considering how container engines execute applications, which of the following statements about containers are correct?

- [ ] **A)** Containers share the host operating system kernel
- [ ] **B)** Container images are composed of reusable read-only layers
- [ ] **C)** Containers provide isolated user-space processes and filesystems
- [ ] **D)** Recreate the full virtual hardware stack

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Containers share the host kernel, use layered images, and isolate processes. Unlike VMs, they do not emulate full virtual hardware.
 
 
</details>


---

### **DevSecOps**

### 24. Which of the following statements best explains why DevOps teams consider containerization valuable for software delivery?

- [ ] **A)** Creates consistent runtime environments
- [ ] **B)** Replaces version control
- [ ] **C)** Distributes binaries to users
- [ ] **D)** Enables insecure cluster access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Containerization packages an application with its runtime and dependencies, reducing environment drift and making delivery pipelines more predictable.
 
 
</details>

### 25. Which two practices are widely considered to be foundational principles of a DevOps culture and toolchain?

- [ ] **A)** Automating build, test, and deployment
- [ ] **B)** Encouraging shared ownership and feedback
- [ ] **C)** Controlling all decisions centrally
- [ ] **D)** Isolating development from operations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> DevOps values automation and collaboration or feedback to shorten delivery cycles. Centralized control and strict isolation slow feedback and work against continuous improvement.
 
 
</details>

### 26. Review the two command-line operations shown in the code block. What is the purpose of the first operation?

```bash
docker build -t devops-app:latest .
docker run --rm -p 8080:80 devops-app:latest
```

- [ ] **A)** Builds a container image
- [ ] **B)** Starts a new container
- [ ] **C)** Pushes image to registry
- [ ] **D)** Removes stopped containers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The first instruction is a build operation that creates an image. The second operation only runs a container from that previously built image.
 
 
</details>


---

### **Infrastructure as Code**

### 27. What is the primary purpose of using Infrastructure as Code to manage cloud environments in a DevOps workflow?

- [ ] **A)** Managing infrastructure through version-controlled definition files
- [ ] **B)** Configuring resources manually in the cloud console
- [ ] **C)** Deploying application code without defining underlying infrastructure
- [ ] **D)** Using unmanaged environments for cloud resources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IaC stores the desired infrastructure state in code, enabling consistent, repeatable, and automated provisioning instead of manual console changes.
 
 
</details>

### 28. Which of the following are core DevOps principles? Select all that apply.

- [ ] **A)** Automation of repetitive tasks
- [ ] **B)** Development and operations collaboration
- [ ] **C)** Manual handoffs between siloed teams
- [ ] **D)** Monitoring and continuous feedback

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> DevOps favors automation, collaboration, and continuous feedback. Manual handoffs and siloed teams contradict the shared ownership and delivery model.
 
 
</details>

### 29. Review the code block in the response. Which type of infrastructure tool is represented?

```hcl
resource "oci_core_instance" "web" {
  availability_domain = "Uocm:PHX-AD-1"
  compartment_id      = var.compartment_ocid
  shape               = "VM.Standard2.1"
  source_details {
    source_type = "image"
    source_id   = var.instance_image_ocid
  }
}
```

- [ ] **A)** Declarative provisioning tool
- [ ] **B)** Configuration management tool
- [ ] **C)** Container orchestrator
- [ ] **D)** Source code compiler

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block declares the desired cloud resource and its properties using HCL, which is characteristic of a declarative provisioning tool.
 
 
</details>


---

### **Monitoring and Observability**

### 30. In a DevOps environment that runs containerized workloads, what is the core benefit provided by observability?

- [ ] **A)** Early detection of system issues and faster troubleshooting
- [ ] **B)** Compilation of applications from source code
- [ ] **C)** Removal of all security vulnerabilities
- [ ] **D)** Automatic creation of container registries

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Observability uses metrics, logs, and traces to detect anomalies early, enabling teams to reduce downtime and troubleshoot containerized services more effectively.
 
 
</details>

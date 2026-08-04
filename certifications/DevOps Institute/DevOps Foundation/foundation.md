<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/DevOps%20Institute/DEVOPS-DevOps-Foundation.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>DevOps Foundation</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Benefits of DevOps](#benefits-of-devops) (3 questions)
- [Continuous Integration and Continuous Delivery](#continuous-integration-and-continuous-delivery) (4 questions)
- [DevOps Best Practices](#devops-best-practices) (7 questions)
- [DevOps Culture](#devops-culture) (5 questions)
- [DevOps Tools](#devops-tools) (3 questions)
- [DevSecOps](#devsecops) (3 questions)
- [Infrastructure as Code](#infrastructure-as-code) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:28:32.128Z |
| Domains | 7 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Benefits of DevOps | 3 |
| Continuous Integration and Continuous Delivery | 4 |
| DevOps Best Practices | 7 |
| DevOps Culture | 5 |
| DevOps Tools | 3 |
| DevSecOps | 3 |
| Infrastructure as Code | 5 |

---

### **Benefits of DevOps**

### 1. What is the primary business outcome of adopting DevOps as described in the DevOps Foundation curriculum?

- [ ] **A)** Achieving a sustainable competitive advantage through high-quality, rapid, and reliable software delivery
- [ ] **B)** Reducing the number of employees in the IT department to cut costs
- [ ] **C)** Eliminating the need for any manual testing or quality assurance processes
- [ ] **D)** Migrating all applications to the cloud immediately

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The primary business outcome is to achieve a sustainable competitive advantage by delivering software faster, more reliably, and with higher quality. This is a core concept from the Business Value section.
 
 
</details>

### 2. Which two of the following are key practices that directly contribute to improved agility and speed to market in a DevOps environment?

- [ ] **A)** Implementing continuous delivery (CD) pipelines to automate the release process
- [ ] **B)** Requiring all changes to go through a weekly change advisory board (CAB) meeting
- [ ] **C)** Establishing short feedback loops through automated testing and monitoring
- [ ] **D)** Increasing the size of each release to reduce the number of deployments

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Continuous delivery pipelines and short feedback loops are key enablers of agility and speed. Large, infrequent releases and manual governance boards slow down delivery and contradict DevOps principles.
 
 
</details>

### 3. The following code snippet is part of a deployment script used by a DevOps team. What DevOps practice does this code primarily support?

```terraform
resource "aws_instance" "web" {
  ami           = "ami-0c55b159cbfafe1f0"
  instance_type = "t2.micro"

  tags = {
    Name = "WebServer"
  }
}
```

- [ ] **A)** Immutable infrastructure where servers are replaced rather than patched
- [ ] **B)** Configuration drift detection and correction
- [ ] **C)** Infrastructure as Code (IaC) for consistent environment provisioning
- [ ] **D)** Manual environment setup to ensure accuracy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The code uses Terraform to define and provision cloud resources in a declarative manner. This is a quintessential example of Infrastructure as Code (IaC), which ensures environments are reproducible, reduces drift, and supports automation.
 
 
</details>


---

### **Continuous Integration and Continuous Delivery**

### 4. What is a core principle of Continuous Integration regarding commit frequency?

- [ ] **A)** Commit at least once per day
- [ ] **B)** Commit only at the end of a sprint
- [ ] **C)** Commit only when a feature is complete
- [ ] **D)** Commit weekly to reduce merge conflicts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CI requires frequent commits (daily or more) to detect integration errors early. Long-lived branches violate CI principles.
 
 
</details>

### 5. Which of the following are benefits of automated testing in a CI pipeline? (Select all that apply.)

- [ ] **A)** Immediate feedback on code changes
- [ ] **B)** Eliminates the need for any manual testing
- [ ] **C)** Reduces the cost of fixing defects by catching them early
- [ ] **D)** Guarantees 100% code coverage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Automated testing provides fast feedback and reduces defect cost by shift-left. It does not replace all manual testing nor guarantee full coverage.
 
 
</details>

### 6. Review the following CI pipeline stage snippet. What does this stage primarily represent?

```groovy
pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh 'mvn test'
        junit '**/target/surefire-reports/*.xml'
      }
    }
  }
}
```

- [ ] **A)** Static code analysis
- [ ] **B)** Unit test execution
- [ ] **C)** Integration testing
- [ ] **D)** Artifact packaging

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The snippet runs unit tests using JUnit and fails the pipeline if any test fails – a core CI feedback mechanism.
 
 
</details>

### 7. Which deployment pattern provides instant rollback with zero downtime?

- [ ] **A)** Blue-Green deployment
- [ ] **B)** Canary release
- [ ] **C)** Rolling update
- [ ] **D)** Feature toggle

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Blue-Green uses two identical environments; switching traffic back is instant. Canary and rolling do not offer instant full rollback.
 
 
</details>


---

### **DevOps Best Practices**

### 8. Which CAMS pillar emphasizes a blameless environment and learning from failures?

- [ ] **A)** Culture
- [ ] **B)** Automation
- [ ] **C)** Measurement
- [ ] **D)** Sharing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Culture is the foundation of CAMS, promoting collaboration, trust, and blamelessness to enable experimentation and learning from failure.
 
 
</details>

### 9. Which of the following are pillars of the CAMS model? (Select all that apply)

- [ ] **A)** Culture
- [ ] **B)** Automation
- [ ] **C)** Lean
- [ ] **D)** Measurement

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> CAMS includes Culture, Automation, Measurement, and Sharing. Lean is part of CALMS, not CAMS.
 
 
</details>

### 10. Based on the CI/CD pipeline definition, which CAMS pillar is being implemented?

```yaml
stages:
  - build
  - test
  - deploy

build:
  stage: build
  script:
    - echo "Building..."
test:
  stage: test
  script:
    - echo "Testing..."
deploy:
  stage: deploy
  script:
    - echo "Deploying..."
```

- [ ] **A)** Automation
- [ ] **B)** Culture
- [ ] **C)** Measurement
- [ ] **D)** Sharing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Automation is the pillar focused on reducing manual tasks using CI/CD, infrastructure as code, and automated testing.
 
 
</details>

### 11. In the CALMS framework, the letter 'L' stands for what?

- [ ] **A)** Lean
- [ ] **B)** Learning
- [ ] **C)** Leadership
- [ ] **D)** Logistics

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CALMS stands for Culture, Automation, Lean, Measurement, Sharing, where Lean focuses on waste elimination and flow.
 
 
</details>

### 12. Which two of the following are DORA metrics? (Select two)

- [ ] **A)** Server Uptime
- [ ] **B)** Lines of Code
- [ ] **C)** Deployment Frequency
- [ ] **D)** Mean Time to Recovery

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C, D**
 
> 💡  **Explanation** 
> 
> DORA's four key metrics are Deployment Frequency, Lead Time for Changes, Mean Time to Recovery, and Change Failure Rate. Server uptime and lines of code are not DORA metrics.
 
 
</details>

### 13. The script automatically rolls back on high error rate. What crucial feedback loop step is absent?

```python
if error_rate > 5%:
  send_alert("Error rate high")
  rollback_deployment()
else:
  continue()
```

- [ ] **A)** A blameless post-mortem
- [ ] **B)** More automation
- [ ] **C)** A code review
- [ ] **D)** Faster deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Closing the feedback loop requires a blameless post-mortem to learn and prevent recurrence, not just automated action.
 
 
</details>

### 14. What does the term 'Kaizen' mean in a DevOps context?

- [ ] **A)** Breakthrough innovation
- [ ] **B)** Incremental improvements
- [ ] **C)** Tool standardization
- [ ] **D)** Organizational restructuring

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Kaizen is a Japanese philosophy of continuous, incremental improvement through small daily changes.
 
 
</details>


---

### **DevOps Culture**

### 15. What is the core emphasis of the DevOps movement as defined by the DevOps Institute's Foundation certification?

- [ ] **A)** Cultural movement
- [ ] **B)** Toolset for automation
- [ ] **C)** Job title
- [ ] **D)** Agile methodology

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> DevOps is a cultural and professional movement that emphasizes integration and collaboration, not tools, roles, or specific methodologies.
 
 
</details>

### 16. Which of the following are the five pillars of the CALMS framework used to assess DevOps maturity? (Select all that apply)

- [ ] **A)** Culture
- [ ] **B)** Automation
- [ ] **C)** Lean
- [ ] **D)** Collaboration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> CALMS stands for Culture, Automation, Lean, Measurement, and Sharing. Collaboration is not one of the five pillars.
 
 
</details>

### 17. Based on the manual deployment script shown in the code block, which of the following DevOps practices is most clearly missing?

```bash
# Manual deployment steps
# 1. SSH to server
# 2. Copy files
# 3. Restart service
```

- [ ] **A)** Automation
- [ ] **B)** Collaboration
- [ ] **C)** Testing
- [ ] **D)** Monitoring

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> DevOps emphasizes automation to reduce manual errors and increase speed. This entirely manual process lacks automation.
 
 
</details>

### 18. What is the primary barrier to efficient software delivery in traditional IT organizations according to the DevOps Foundation?

- [ ] **A)** Organizational silos
- [ ] **B)** Insufficient tools
- [ ] **C)** Limited budget
- [ ] **D)** Too many meetings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Silos between development and operations are the main inhibitors of flow, causing delays and misaligned goals.
 
 
</details>

### 19. Which of the following are part of the Three Ways principles of DevOps defined by Gene Kim? (Select all that apply)

- [ ] **A)** Systems Thinking
- [ ] **B)** Amplify Feedback Loops
- [ ] **C)** Culture of Experimentation
- [ ] **D)** Centralized Control

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The Three Ways are Systems Thinking, Amplify Feedback Loops, and Culture of Continual Experimentation and Learning.
 
 
</details>


---

### **DevOps Tools**

### 20. Which tool category serves as the single source of truth for all artifacts in DevOps?

- [ ] **A)** Source Code Management (SCM)
- [ ] **B)** Continuous Integration (CI)
- [ ] **C)** Continuous Delivery (CD)
- [ ] **D)** Monitoring and Observability

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SCM tracks changes and is the single source of truth; CI builds and tests, CD deploys, monitoring observes system health.
 
 
</details>

### 21. Which two statements correctly describe DevOps CI/CD practices?

- [ ] **A)** CI builds and tests code automatically on commit
- [ ] **B)** Continuous Delivery requires manual approval before production
- [ ] **C)** Continuous Deployment requires manual approval before production
- [ ] **D)** CI automatically deploys code to production

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CI automates build/test; Continuous Delivery has manual gates; Continuous Deployment is fully automatic; CI does not deploy.
 
 
</details>

### 22. What principle ensures that running this Ansible playbook multiple times produces the same system state?

```yaml
- name: Ensure nginx is installed
  hosts: all
  tasks:
    - name: Install nginx
      apt:
        name: nginx
        state: present
```

- [ ] **A)** Idempotency
- [ ] **B)** Declarative configuration
- [ ] **C)** Procedural execution
- [ ] **D)** Masterless architecture

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Idempotency ensures repeated runs yield the same result—a core principle of configuration management tools.
 
 
</details>


---

### **DevSecOps**

### 23. In DevSecOps, what is the main objective of including security checks in the CI/CD pipeline?

- [ ] **A)** Replace the need for a security team
- [ ] **B)** Detect vulnerabilities as early as possible
- [ ] **C)** Perform a final security audit before release
- [ ] **D)** Automate all security decisions without human input

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Detecting vulnerabilities early reduces cost and risk, aligning with the shift-left principle in DevSecOps.
 
 
</details>

### 24. Which of the following are considered shift-left security practices?

- [ ] **A)** Threat modeling during the design phase
- [ ] **B)** Static application security testing (SAST) during coding
- [ ] **C)** Dynamic application security testing (DAST) after deployment
- [ ] **D)** Policy as code enforcement in the CI/CD pipeline

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Shift-left includes threat modeling, SAST, and policy as code; DAST is a later-stage test, not shift-left.
 
 
</details>

### 25. Review the following Java code snippet. What security vulnerability does it contain?

```java
String query = "SELECT * FROM users WHERE id = " + request.getParameter("id");
Statement stmt = connection.createStatement();
ResultSet rs = stmt.executeQuery(query);
```

- [ ] **A)** Cross-site scripting (XSS)
- [ ] **B)** SQL injection
- [ ] **C)** Buffer overflow
- [ ] **D)** Insecure direct object reference

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code concatenates user input directly into a SQL query, leading to SQL injection vulnerability.
 
 
</details>


---

### **Infrastructure as Code**

### 26. What is the primary purpose of configuration management in DevOps?

- [ ] **A)** To automate the deployment of code changes
- [ ] **B)** To ensure system integrity over time by systematically handling changes
- [ ] **C)** To manage user credentials and access controls
- [ ] **D)** To monitor system performance and generate alerts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Configuration management systematically handles changes to maintain integrity over time, preventing drift and manual errors.
 
 
</details>

### 27. Which two benefits does provisioning and orchestration provide in IaC?

- [ ] **A)** Eliminates configuration drift
- [ ] **B)** Increases the amount of manual configuration
- [ ] **C)** Reduces deployment lead time
- [ ] **D)** Prevents any changes from being made to infrastructure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Provisioning and orchestration eliminate drift and reduce lead time by automating consistent, repeatable deployments.
 
 
</details>

### 28. In the provided code block, which concept of immutable infrastructure is directly illustrated?

```dockerfile
FROM ubuntu:latest
RUN apt-get update && apt-get install -y nginx
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
```

- [ ] **A)** Idempotency
- [ ] **B)** Golden image creation
- [ ] **C)** Configuration drift detection
- [ ] **D)** Blue-green deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Dockerfile builds a golden image (a pre-configured template) that is used to create identical containers, a core practice of immutable infrastructure.
 
 
</details>

### 29. What does a declarative approach specify in Infrastructure as Code?

- [ ] **A)** The step-by-step instructions to execute
- [ ] **B)** The desired end state of the infrastructure
- [ ] **C)** The programming language used for automation
- [ ] **D)** The vendor-specific tool commands

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Declarative approaches define the desired outcome; the tool determines how to achieve it, ensuring consistency and idempotency.
 
 
</details>

### 30. Which two are benefits of using version control for infrastructure code?

- [ ] **A)** Enables rollback to previous configurations
- [ ] **B)** Eliminates the need for testing infrastructure changes
- [ ] **C)** Provides an audit trail of all modifications
- [ ] **D)** Makes infrastructure automatically immutable

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Version control provides history for rollback and audit trails, but does not replace testing or enforce immutability by itself.
 
 
</details>

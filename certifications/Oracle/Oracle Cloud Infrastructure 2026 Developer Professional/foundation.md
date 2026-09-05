<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Oracle%20Cloud%20Infrastructure%202026%20Developer%20Professional.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Oracle Cloud Infrastructure 2026 Developer Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Cloud Native Applications and Containerization](#cloud-native-applications-and-containerization) (10 questions)
- [Cloud Native Fundamentals](#cloud-native-fundamentals) (3 questions)
- [Leveraging Serverless Technologies](#leveraging-serverless-technologies) (10 questions)
- [Monitoring and Troubleshooting](#monitoring-and-troubleshooting) (3 questions)
- [Testing and Securing Cloud Native Applications](#testing-and-securing-cloud-native-applications) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:46:10.632Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Cloud Native Applications and Containerization | 10 |
| Cloud Native Fundamentals | 3 |
| Leveraging Serverless Technologies | 10 |
| Monitoring and Troubleshooting | 3 |
| Testing and Securing Cloud Native Applications | 4 |

---

### **Cloud Native Applications and Containerization**

### 1. Which one of the following statements best describes the architectural style that is most commonly used by cloud native applications?

- [ ] **A)** Applications are built as one very large deployment unit that cannot be changed without full redeployment.
- [ ] **B)** Applications are decomposed into smaller services that can be developed and deployed independently.
- [ ] **C)** Applications are permanently attached to manually provisioned physical servers to reduce latency.
- [ ] **D)** Applications always run inside a full guest operating system under a hypervisor.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Cloud native applications are composed of small independently deployable services rather than one coupled monolithic unit. This supports scaling, resilience, and frequent delivery.
 
 
</details>

### 2. Which two of the following principles are considered fundamental when designing applications for cloud native platforms? Select two.

- [ ] **A)** Every application must share a single server-side database for consistency.
- [ ] **B)** Application components are packaged as containers to isolate their dependencies and execution context.
- [ ] **C)** Every code change must wait for a quarterly release in order to maintain stability.
- [ ] **D)** Infrastructure is provisioned programmatically from declarative definitions and automated pipelines.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Cloud native design emphasizes container packaging and programmatic infrastructure provisioning. Legacy practices such as shared monolithic databases, quarterly releases, and manual server management are not cloud native.
 
 
</details>

### 3. In the Compose service definition shown, what effect does the ports setting have on traffic sent to the host?

```yaml
version: '3.8'
services:
  app:
    image: nginx:latest
    ports:
      - "8080:80"
```

- [ ] **A)** Host port 8080 is published and traffic is forwarded to container port 80.
- [ ] **B)** Container port 8080 is published and traffic is forwarded to host port 80.
- [ ] **C)** Container port 8080 is made available only inside the Compose network.
- [ ] **D)** Traffic on host port 80 is sent to the container published on port 8080.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Compose port mapping of \"8080:80\" publishes host port 8080 and sends incoming traffic to container port 80. The order follows host:container.
 
 
</details>

### 4. Which one of the following descriptions accurately defines a container image in containerization platforms?

- [ ] **A)** A read-only package containing application code, libraries, configuration, and runtime dependencies.
- [ ] **B)** A running process that consumes CPU and memory while executing the application.
- [ ] **C)** A virtual network adapter used to expose services to external clients.
- [ ] **D)** A host operating system profile used to tune kernel parameters.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A container image is an immutable artifact containing application code and runtime dependencies. Running processes, virtual network adapters, and kernel profiles do not define an image.
 
 
</details>

### 5. Which two benefits do containerized workloads typically deliver when compared with virtual machines? Select two.

- [ ] **A)** Containers isolate application processes from one another on the same operating system.
- [ ] **B)** Each container includes its own complete kernel and device drivers.
- [ ] **C)** Containers can start quickly and use fewer resources because they share the host kernel.
- [ ] **D)** Containers can run only when a dedicated hardware hypervisor is provisioned for them.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Containers rely on the host kernel and isolate application processes, making startup fast and resource use lower than virtual machines. Containers do not include a full guest OS or require a hypervisor.
 
 
</details>

### 6. According to the provided Kubernetes Deployment manifest, what number of pod replicas does the desired state declare?

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: payments
spec:
  replicas: 3
  selector:
    matchLabels:
      app: payments
  template:
    metadata:
      labels:
        app: payments
    spec:
      containers:
      - name: payments
        image: iad.ocir.io/example/payments:1.0
```

- [ ] **A)** 1
- [ ] **B)** 2
- [ ] **C)** 3
- [ ] **D)** 4

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The Deployment manifest declares replicas: 3, so the Kubernetes controller continuously works to keep three Pods running.
 
 
</details>

### 7. Which Oracle Cloud Infrastructure service is designed to store, tag, and share container images in a managed registry?

- [ ] **A)** OCI Registry
- [ ] **B)** OCI Object Storage
- [ ] **C)** OCI Compute
- [ ] **D)** OCI File Storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI Registry is a managed Docker v2-compatible registry for storing and distributing container images. The other services do not act as container image registries.
 
 
</details>

### 8. Which two Oracle Cloud Infrastructure services are classified as container runtime environments for cloud native workloads? Select two.

- [ ] **A)** Container Engine for Kubernetes (OKE)
- [ ] **B)** Container Instances
- [ ] **C)** Object Storage
- [ ] **D)** Virtual Cloud Network

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Container Engine for Kubernetes and Container Instances are compute services that run container workloads. Object Storage and Virtual Cloud Network do not execute containers.
 
 
</details>

### 9. Consider the docker run command shown in the snippet. Which outcome is produced when this command is executed?

```bash
docker run -d -p 8080:80 --name web nginx:alpine
```

- [ ] **A)** The container starts in detached mode, and host port 8080 is mapped to container port 80.
- [ ] **B)** The container starts in the foreground, and host port 80 is mapped to container port 8080.
- [ ] **C)** The image named nginx is built locally and then pushed to the default container registry.
- [ ] **D)** The container runs briefly and is automatically deleted when the command exits.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The -d flag runs the container detached, and -p 8080:80 publishes host port 8080 and forwards to container port 80. No --rm flag means the container is not automatically removed.
 
 
</details>

### 10. Which statement is a core characteristic of a microservice architecture used by cloud native applications?

- [ ] **A)** Business capabilities are implemented as small services that can be decoupled and deployed independently.
- [ ] **B)** The entire application is packaged into one binary and deployed as a single unit.
- [ ] **C)** Changing one microservice requires all other microservices to stop in a coordinated release.
- [ ] **D)** The same codebase must always be shared to avoid version drift between capabilities.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Microservices split application features into small services that can change and deploy without coupling. Monolithic, synchronized, or shared-repo release models do not describe microservices.
 
 
</details>


---

### **Cloud Native Fundamentals**

### 11. In modern application architecture, what does the term cloud native fundamentally represent in the software delivery model?

- [ ] **A)** Running applications with automation and cloud scalability
- [ ] **B)** Installing applications directly on physical servers
- [ ] **C)** Keeping all workloads in a legacy mainframe
- [ ] **D)** Serving applications only from static media players

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud native is an approach for building and running applications that exploits automation, dynamic scaling, and resilient cloud services rather than fixed physical infrastructure.
 
 
</details>

### 12. When adopting cloud native patterns, which two practices are normally associated with application architecture and packaging?

- [ ] **A)** One large monolith deployed annually
- [ ] **B)** Microservices exposed through well-defined APIs
- [ ] **C)** Portable containers used as the deployment unit
- [ ] **D)** Manual setup repeated on each server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Cloud native systems commonly use microservices and containerized deployment units to improve composability, resilience, and operational automation.
 
 
</details>

### 13. Inspect the supplied application descriptor. Which cloud native practice does this artifact primarily automate or enable?

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: payments-api
spec:
  replicas: 3
  selector:
    matchLabels:
      app: payments-api
  template:
    metadata:
      labels:
        app: payments-api
    spec:
      containers:
      - name: controller
        image: payments-api:2026.06
        ports:
        - containerPort: 8080
```

- [ ] **A)** Declarative container orchestration
- [ ] **B)** Synchronous mainframe scheduling
- [ ] **C)** Local printer queue management
- [ ] **D)** Manual patch installation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A manifest is a declarative infrastructure description; using it allows container orchestrators to reconcile live workloads automatically.
 
 
</details>


---

### **Leveraging Serverless Technologies**

### 14. What term describes an application built as a collection of loosely coupled services running on managed cloud infrastructure?

- [ ] **A)** Cloud-native
- [ ] **B)** Traditional monolith
- [ ] **C)** On-premise legacy system
- [ ] **D)** Mainframe architecture

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud-native applications are built and run by exploiting managed cloud infrastructure, often as microservices, and do not require on-premise or mainframe deployment.
 
 
</details>

### 15. Which of the following are core characteristics of serverless computing?

- [ ] **A)** Automatic scaling
- [ ] **B)** Event-driven execution
- [ ] **C)** Billing based on execution time
- [ ] **D)** Permanent dedicated servers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Serverless computing executes code only when events occur, scales automatically, and charges for actual execution. It does not require permanently assigned servers.
 
 
</details>

### 16. The code block reacts to which type of event?

```python
import json

def handler(ctx, data: bytes = b""):
    event = json.loads(data)
    if event["eventType"] == "com.oraclecloud.objectstorage.createobject":
        return f"New object: {event['data']['resourceName']}"

```

- [ ] **A)** Object creation in Object Storage
- [ ] **B)** Object deletion from Object Storage
- [ ] **C)** Compute instance launch
- [ ] **D)** Function deployment completion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The handler checks for the createobject event and returns a message containing the new object name, indicating an object creation event.
 
 
</details>

### 17. Which metric determines cost in an event-driven serverless compute service?

- [ ] **A)** Number of invocations and execution time
- [ ] **B)** Number of always-on virtual machines
- [ ] **C)** Total storage provisioned for the account
- [ ] **D)** Time spent waiting for new events

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Serverless billing is based on actual use, typically measured by how often the function is called and how long the function runs.
 
 
</details>

### 18. Which benefits are provided by using a serverless platform?

- [ ] **A)** Frees developers from managing hardware and operating systems
- [ ] **B)** Provides automatic high availability through scaling
- [ ] **C)** Lets applications react immediately to events
- [ ] **D)** Requires long-term committed capacity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A serverless platform removes infrastructure management, auto scales, and reacts to events. It does not require long-term capacity commitments.
 
 
</details>

### 19. What action is represented by the JSON event in the code block?

```json
{
  "eventType": "com.oraclecloud.objectstorage.deleteobject",
  "data": {
    "bucketName": "uploads",
    "resourceName": "archive.zip"
  }
}
```

- [ ] **A)** Object deletion from Object Storage
- [ ] **B)** Object upload to Object Storage
- [ ] **C)** Compute instance stop
- [ ] **D)** Database export launch

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The eventType contains com.oraclecloud.objectstorage.deleteobject, which clearly indicates that an object was deleted from Object Storage.
 
 
</details>

### 20. What best describes Function-as-a-Service execution?

- [ ] **A)** Code packages executed in response to events on a managed platform
- [ ] **B)** A suite of long-running virtual machines
- [ ] **C)** An application server that must be patched by the user
- [ ] **D)** A database-as-a-service offering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> FaaS runs code only when triggered by an event and removes the need for users to provision or operate servers.
 
 
</details>

### 21. Which practices are appropriate when developing serverless functions?

- [ ] **A)** Keep functions stateless
- [ ] **B)** Store persistent data outside the function
- [ ] **C)** Use environment variables or configuration services
- [ ] **D)** Rely on the local disk for durable state

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Serverless functions should be stateless, store durable data in managed services, and read configuration from external sources instead of depending on local storage.
 
 
</details>

### 22. Which runtime is selected by the function deployment configuration in the code block?

```yaml
schema_version: 1.0.0
name: invoice-check
version: 1.0.0
runtime: go
entrypoint: /go/func.go
```

- [ ] **A)** Go
- [ ] **B)** Python
- [ ] **C)** Java
- [ ] **D)** Node.js

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The deployment metadata contains runtime: go, so the function is configured to execute in a Go environment.
 
 
</details>

### 23. What happens when a serverless platform performs automatic scaling?

- [ ] **A)** More function instances are created as demand increases
- [ ] **B)** Developers must manually add compute capacity
- [ ] **C)** Function instances remain stopped during traffic spikes
- [ ] **D)** The application must be redeployed to handle more users

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Automatic scaling creates additional function instances when demand rises and removes them when demand falls, without developer intervention.
 
 
</details>


---

### **Monitoring and Troubleshooting**

### 24. Which OCI service is designed to track numeric data points and raise alarms based on thresholds?

- [ ] **A)** Monitoring
- [ ] **B)** Logging
- [ ] **C)** Notifications
- [ ] **D)** Functions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCI Monitoring captures performance data and evaluates alarms when metric values match thresholds.
 
 
</details>

### 25. For a cloud native application, which three observability signals are essential for diagnosing performance and reliability issues?

- [ ] **A)** Metrics
- [ ] **B)** Logs
- [ ] **C)** Traces
- [ ] **D)** Alarms

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Metrics, logs, and traces are the three pillars of observability; alarms are rule-based actions, not raw telemetry data.
 
 
</details>

### 26. The command shown in the code block is executed by a developer. Which OCI service is handling this request?

```bash
oci monitoring metric list \
  --compartment-id ocid1.compartment.oc1..example \
  --namespace oci_computeagent
```

- [ ] **A)** Monitoring
- [ ] **B)** Logging
- [ ] **C)** Notifications
- [ ] **D)** Functions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'oci monitoring metric list' command lists metric names and namespaces from the OCI Monitoring service.
 
 
</details>


---

### **Testing and Securing Cloud Native Applications**

### 27. Why is security testing an essential step in the cloud-native delivery pipeline?

- [ ] **A)** It detects vulnerabilities before production
- [ ] **B)** It removes the need for runtime monitoring
- [ ] **C)** It makes APIs publicly accessible
- [ ] **D)** It guarantees releases are bug-free

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Security testing in a cloud-native pipeline detects vulnerabilities before release. Runtime monitoring and other controls remain essential after deployment.
 
 
</details>

### 28. Which two practices are essential when securing cloud-native applications?

- [ ] **A)** Scan container images for vulnerabilities
- [ ] **B)** Use a central secrets management service
- [ ] **C)** Embed credentials directly in source code
- [ ] **D)** Keep every network port open

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Scanning images and centralizing secret management prevent common cloud-native vulnerabilities. Hard-coded credentials and open ports expose applications to unnecessary risk.
 
 
</details>

### 29. Inspect the pipeline definition in the code block. What kind of automated validation runs before the final phase?

```yaml
stages:
  - name: Build
    steps:
      - type: Build
  - name: AutomatedTests
    steps:
      - type: StaticAnalysis
      - type: UnitTest
      - type: SecretScan
  - name: Deploy
    steps:
      - type: Deploy

```

- [ ] **A)** Automated source, unit, and secret checks
- [ ] **B)** Manual confirmation by a manager
- [ ] **C)** Penetration test on the live environment
- [ ] **D)** Database migration validation after release

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block includes an automated stage with static analysis, unit tests, and secret scanning before deployment, reducing common application and credential risks.
 
 
</details>

### 30. What does immutable infrastructure mean in cloud-native application management?

- [ ] **A)** Deploy new instances and delete old ones
- [ ] **B)** Patch instances while they are running
- [ ] **C)** Edit configuration files on live instances
- [ ] **D)** Restart existing instances with the same image

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Immutable infrastructure replaces running instances instead of modifying them, preventing configuration drift and enabling consistent rollbacks.
 
 
</details>

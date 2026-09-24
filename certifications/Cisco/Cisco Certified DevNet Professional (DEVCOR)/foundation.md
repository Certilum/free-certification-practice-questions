<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cisco/Cisco%20Certified%20DevNet%20Professional%20(DEVCOR).png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Cisco Certified DevNet Professional (DEVCOR)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Application Deployment and Security](#application-deployment-and-security) (6 questions)
- [Cisco Platforms and Development](#cisco-platforms-and-development) (6 questions)
- [Infrastructure and Automation](#infrastructure-and-automation) (6 questions)
- [Software Development and Design](#software-development-and-design) (6 questions)
- [Understanding and Using APIs](#understanding-and-using-apis) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:51:20.895Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Application Deployment and Security | 6 |
| Cisco Platforms and Development | 6 |
| Infrastructure and Automation | 6 |
| Software Development and Design | 6 |
| Understanding and Using APIs | 6 |

---

### **Application Deployment and Security**

### 1. In Python development, which tool is used to create an isolated environment for managing project-specific dependencies?

- [ ] **A)** venv
- [ ] **B)** pip
- [ ] **C)** setuptools
- [ ] **D)** easy_install

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The venv module creates isolated Python environments, preventing global package pollution and version conflicts across automation projects.
 
 
</details>

### 2. Which of the following files are commonly used in Python projects to manage dependencies, lock versions, and define packaging metadata?

- [ ] **A)** Dockerfile
- [ ] **B)** requirements.txt
- [ ] **C)** pyproject.toml
- [ ] **D)** poetry.lock

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C, D**
 
> 💡  **Explanation** 
> 
> These files track dependencies, metadata, and locked versions. A Dockerfile packages containers, not Python dependencies.
 
 
</details>

### 3. What is the immediate outcome of executing the Python command shown in the provided code block?

```bash
python -m venv devnet-env
```

- [ ] **A)** Creates a virtual environment named devnet-env
- [ ] **B)** Installs all project dependencies
- [ ] **C)** Freezes packages into a requirements file
- [ ] **D)** Activates an existing virtual environment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The python -m venv command creates a new virtual environment directory, isolating dependencies for a project. This is the first step in managing dependencies safely.
 
 
</details>

### 4. According to PEP 518 and PEP 621, which file standardizes build system requirements and project metadata in modern Python projects?

- [ ] **A)** pyproject.toml
- [ ] **B)** setup.py
- [ ] **C)** requirements.txt
- [ ] **D)** Pipfile

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> pyproject.toml is the modern standard for build systems and metadata, replacing legacy setup.py in modern Python projects.
 
 
</details>

### 5. Which of the following are common secrets management traps that application developers should avoid in production environments?

- [ ] **A)** Assuming Base64 encoding is encryption
- [ ] **B)** Hardcoding fallback credentials in source code
- [ ] **C)** Rotating secrets dynamically
- [ ] **D)** Using AppRole authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Base64 is not encryption, and fallback credentials create backdoors. Dynamic rotation and AppRole authentication are secure practices.
 
 
</details>

### 6. What is the effect of the flag used in the pip install command displayed in the code block?

```bash
pip install -e .
```

- [ ] **A)** Installs the package in editable mode
- [ ] **B)** Upgrades the package to the latest version
- [ ] **C)** Exports dependencies to a file
- [ ] **D)** Installs the package globally

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The -e flag installs the package in editable mode, so source changes are immediately reflected without reinstalling.
 
 
</details>


---

### **Cisco Platforms and Development**

### 7. What DevNet resource is the central hub for accessing learning labs, code exchanges, sandboxes, and platform-specific developer centers?

- [ ] **A)** DevNet Developer Portal
- [ ] **B)** Cisco DNA Center GUI
- [ ] **C)** Meraki Dashboard
- [ ] **D)** vManage /developers page

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The DevNet Developer Portal is the central hub that provides access to learning labs, code exchanges, sandboxes, and platform-specific developer centers.
 
 
</details>

### 8. Which statements correctly describe Always-On sandboxes? Select all that apply.

- [ ] **A)** Available instantly and 24/7
- [ ] **B)** Shared state that resets frequently
- [ ] **C)** Dedicated isolated topology with full administrative control
- [ ] **D)** Read-only or restricted read-write access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Always-On sandboxes are shared public resources with instant access, frequent resets, and restricted access. Full administrative control applies to Reserved Sandboxes.
 
 
</details>

### 9. Refer to the code snippet. Which authentication mechanism is required by the Meraki Dashboard API call?

```python
import requests
url = "https://api.meraki.com/api/v1/organizations"
headers = {
    "X-Cisco-Meraki-API-Key": "YOUR_API_KEY"
}
response = requests.get(url, headers=headers)
print(response.status_code)
```

- [ ] **A)** API key in the X-Cisco-Meraki-API-Key header
- [ ] **B)** HTTP Basic Authentication
- [ ] **C)** OAuth 2.0 bearer token in Authorization header
- [ ] **D)** API key as a query parameter

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Meraki Dashboard API requires an API key sent in the X-Cisco-Meraki-API-Key header, not as Basic Auth or a query parameter.
 
 
</details>

### 10. Which HTTP method should be used to create a new resource through the Meraki Dashboard API?

- [ ] **A)** GET
- [ ] **B)** POST
- [ ] **C)** PUT
- [ ] **D)** DELETE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Creating new Meraki resources uses POST. GET retrieves data, PUT updates, and DELETE removes resources.
 
 
</details>

### 11. Which statements about Meraki Dashboard API rate limiting are correct? Select all that apply.

- [ ] **A)** Limits are typically 5 requests per second per organization
- [ ] **B)** A 429 response should be retried immediately
- [ ] **C)** Rotating API keys removes all rate limits
- [ ] **D)** Automation should implement exponential backoff

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Meraki enforces around 5 requests per second per organization. Clients should handle 429 responses with exponential backoff rather than immediate retries.
 
 
</details>

### 12. Refer to the code snippet. What operation is being performed with the Webex API?

```python
from webexpythonsdk import WebexAPI
api = WebexAPI()
room = api.rooms.create("Incident Response")
print(room.id)
```

- [ ] **A)** Creates a Webex room
- [ ] **B)** Deletes a Webex room
- [ ] **C)** Adds a membership
- [ ] **D)** Sends a message

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code uses rooms.create to create a new Webex room and prints the room ID.
 
 
</details>


---

### **Infrastructure and Automation**

### 13. In Cisco model-driven programmability, which statement correctly describes the role of YANG?

- [ ] **A)** A data modeling language that defines configuration and operational data structure.
- [ ] **B)** A transport protocol that streams telemetry over HTTP/2.
- [ ] **C)** A scripting language for automating Cisco IOS CLI commands.
- [ ] **D)** A network management protocol that replaces SNMP.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> YANG is the schema language used to model configuration and operational data for NETCONF and RESTCONF. It does not transport, script, or replace management protocols.
 
 
</details>

### 14. Which two statements correctly describe NETCONF characteristics?

- [ ] **A)** It runs over SSH on TCP port 830.
- [ ] **B)** It requires XML as its data encoding.
- [ ] **C)** It natively supports JSON payloads.
- [ ] **D)** It is a stateless, resource-oriented protocol.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> NETCONF is a stateful, session-based protocol over SSH port 830 and mandates XML encoding. JSON is not native to NETCONF; RESTCONF supports JSON.
 
 
</details>

### 15. Based on the provided command snippet, which protocol is being invoked to query the device?

```bash
curl -X GET https://192.0.2.1/restconf/data/Cisco-IOS-XE-native:native/interface/GigabitEthernet1 -H "Accept: application/yang-data+json"
```

- [ ] **A)** RESTCONF
- [ ] **B)** NETCONF
- [ ] **C)** SNMP
- [ ] **D)** gRPC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The URL path contains /restconf and uses HTTPS plus a YANG data format, so the command invokes RESTCONF.
 
 
</details>

### 16. On which standard transport and port does RESTCONF typically communicate with Cisco devices?

- [ ] **A)** HTTP/HTTPS over TCP port 443
- [ ] **B)** SSH over TCP port 830
- [ ] **C)** gRPC over HTTP/2
- [ ] **D)** UDP over port 161

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RESTCONF uses HTTP or HTTPS, typically TCP port 443, and supports both JSON and XML payloads.
 
 
</details>

### 17. Which two statements about NETCONF datastores are correct?

- [ ] **A)** The candidate datastore allows configuration changes to be staged before commit.
- [ ] **B)** The startup datastore holds the configuration that will be applied when the device boots.
- [ ] **C)** The operational datastore is directly writable through NETCONF.
- [ ] **D)** The running datastore cannot be changed after initial startup.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> NETCONF explicitly supports running, candidate, and startup datastores. Candidate staging and startup boot-time configuration are key features, while operational state is not writable.
 
 
</details>

### 18. What is the purpose of the connection: network_cli directive in the provided Ansible playbook snippet?

```yaml
- name: Configure interfaces
  hosts: switches
  gather_facts: false
  connection: network_cli
  tasks:
    - name: Set interface description
      cisco.ios.ios_interfaces:
        config:
          - name: GigabitEthernet0/1
            description: Uplink to core
        state: merged
```

- [ ] **A)** It selects the network connection plugin used to reach managed switches.
- [ ] **B)** It installs an agent on the target Cisco device.
- [ ] **C)** It encrypts sensitive variables inside the playbook.
- [ ] **D)** It sets the Python interpreter path on the control node.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> network_cli is an Ansible connection plugin for network devices. It allows Ansible to communicate over SSH without requiring an agent on the device.
 
 
</details>


---

### **Software Development and Design**

### 19. What best describes a monolithic application architecture?

- [ ] **A)** All business logic, data access, and user interface layers are combined into a single deployable unit.
- [ ] **B)** The application is broken into independently deployable, loosely coupled services.
- [ ] **C)** Each service owns its own private database and communicates through message brokers.
- [ ] **D)** The application is made up of multiple containers orchestrated by Kubernetes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A monolithic architecture couples all business logic, data access, and user interface layers into one unified codebase and deployable artifact.
 
 
</details>

### 20. Which two statements are characteristics of microservices architectures?

- [ ] **A)** Services are independently deployable and loosely coupled.
- [ ] **B)** A failure in one microservice usually brings down the entire application.
- [ ] **C)** Services communicate over lightweight protocols such as HTTP/REST or asynchronous messaging brokers.
- [ ] **D)** All microservices must share one centralized database to keep data consistent.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Microservices are independently deployable, loosely coupled services that communicate over lightweight protocols. Sharing a single database recreates monolithic coupling and is an anti-pattern.
 
 
</details>

### 21. The structure shown in the code block is written in which data serialization format?

```yaml
employees:
  - name: Ana
    role: engineer
  - name: Ben
    role: manager

```

- [ ] **A)** JSON
- [ ] **B)** YAML
- [ ] **C)** XML
- [ ] **D)** gRPC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> YAML uses indentation-based structure to define hierarchical data, as shown by the indented list of employees.
 
 
</details>

### 22. What is idempotency in API design?

- [ ] **A)** Making multiple identical requests produces the same result as a single request.
- [ ] **B)** Each request can produce a different state depending on network conditions.
- [ ] **C)** The API returns cached responses without processing the request.
- [ ] **D)** The server stores session state to guarantee consistency.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Idempotency ensures repeated identical requests produce the same result as a single request, preventing duplicate resources or conflicting state changes.
 
 
</details>

### 23. Which two patterns are explicitly associated with preventing cascading failures or overload when integrating with downstream APIs?

- [ ] **A)** Circuit Breakers
- [ ] **B)** Exponential Backoff with jitter
- [ ] **C)** Synchronous polling
- [ ] **D)** Shared database anti-pattern

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Circuit breakers isolate failing services, and exponential backoff with jitter prevents retry storms against downstream APIs.
 
 
</details>

### 24. The code block illustrates the central behavior of which distributed design pattern?

```python
if failures >= threshold:
    open_circuit()
    return fallback()

```

- [ ] **A)** Circuit Breaker
- [ ] **B)** Load Balancer
- [ ] **C)** Database sharding
- [ ] **D)** REST API gateway

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code detects repeated failures, opens a circuit, and returns a fallback response, which is the core behavior of a circuit breaker.
 
 
</details>


---

### **Understanding and Using APIs**

### 25. Which HTTP method is classified as non-idempotent in RESTful API design?

- [ ] **A)** GET
- [ ] **B)** POST
- [ ] **C)** PUT
- [ ] **D)** DELETE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> POST is non-idempotent because repeated identical requests can create multiple resources. GET, PUT, and DELETE remain idempotent.
 
 
</details>

### 26. Which statements about HTTP status code classes are correct? (Choose two)

- [ ] **A)** 2xx codes indicate successful request handling.
- [ ] **B)** 3xx codes indicate internal server failures.
- [ ] **C)** 4xx codes generally indicate client-side errors.
- [ ] **D)** 5xx codes require the client to change the payload before retrying.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> 2xx indicates success, 4xx indicates client errors, 5xx indicates server errors. 3xx is redirection, not a server failure.
 
 
</details>

### 27. Analyze the following Python script that calls a Cisco API. What is the most likely cause of the failure?

```python
import requests

url = "https://catalyst.example.com/dna/intent/api/v1/device"
payload = {"name": "SW1", "siteId": "site1"}
headers = {"Authorization": "Bearer token", "Content-Type": "application/json"}
response = requests.post(url, params=payload, headers=headers)
print(response.status_code)
```

- [ ] **A)** The payload is incorrectly sent as query parameters; use json=payload.
- [ ] **B)** The Authorization header should be omitted.
- [ ] **C)** POST cannot be used with headers.
- [ ] **D)** The device name should be in the URL path.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Using params= sends the payload in the query string. The API expects a JSON body, so the request should use json=payload.
 
 
</details>

### 28. Which authentication mechanism uses a Base64-encoded username and password in the Authorization header?

- [ ] **A)** OAuth 2.0 Bearer Token
- [ ] **B)** HTTP Basic Authentication
- [ ] **C)** API Key
- [ ] **D)** Mutual TLS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> HTTP Basic Authentication encodes username and password with Base64 and places the result in the Authorization header using the Basic scheme.
 
 
</details>

### 29. Which HTTP methods are considered idempotent? (Choose three)

- [ ] **A)** GET
- [ ] **B)** POST
- [ ] **C)** PUT
- [ ] **D)** DELETE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> GET, PUT, and DELETE are idempotent. POST is non-idempotent because repeated calls can create multiple resources.
 
 
</details>

### 30. Given the following JSON response object, which Python expression extracts the task ID?

```python
response = {
    "response": {
        "taskId": "task123",
        "url": "/api/v1/task/task123"
    },
    "version": "1.0"
}
```

- [ ] **A)** response['response']['taskId']
- [ ] **B)** response['taskId']
- [ ] **C)** response['response']['id']
- [ ] **D)** response.taskId

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The JSON hierarchy nests taskId under response. The expression response['response']['taskId'] reaches the correct value.
 
 
</details>

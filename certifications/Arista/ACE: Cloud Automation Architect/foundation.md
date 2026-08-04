<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Arista/ACE:%20L7%20(Arista%20Cloud%20Engineer:%20Level%207)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>ACE: Cloud Automation Architect</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Automation with Ansible](#automation-with-ansible) (7 questions)
- [Automation with Terraform](#automation-with-terraform) (6 questions)
- [CloudVision and Automation Foundation](#cloudvision-and-automation-foundation) (6 questions)
- [Design and Troubleshoot Automated Deployments](#design-and-troubleshoot-automated-deployments) (5 questions)
- [Python and REST APIs for Automation](#python-and-rest-apis-for-automation) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:42.464Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Automation with Ansible | 7 |
| Automation with Terraform | 6 |
| CloudVision and Automation Foundation | 6 |
| Design and Troubleshoot Automated Deployments | 5 |
| Python and REST APIs for Automation | 6 |

---

### **Automation with Ansible**

### 1. What is the architecture of Ansible?

- [ ] **A)** Agent-based, pull model
- [ ] **B)** Push-based, agentless model
- [ ] **C)** Agent-based, push model
- [ ] **D)** Pull-based, agentless model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Ansible operates with a push-based, agentless architecture. It connects via SSH or eAPI to managed nodes without requiring installed agents.
 
 
</details>

### 2. Which file formats can be used for static Ansible inventory? (Choose two)

- [ ] **A)** INI
- [ ] **B)** YAML
- [ ] **C)** XML
- [ ] **D)** JSON

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Ansible static inventories can be written in INI or YAML format. JSON and XML are not native inventory formats.
 
 
</details>

### 3. Examine the inventory snippet. What is the ansible_host value for the host 'leaf1'?

```ini
[leafs]
leaf1 ansible_host=10.1.1.1
leaf2 ansible_host=10.1.1.2

[spines]
spine1 ansible_host=10.1.1.10
```

- [ ] **A)** 10.1.1.1
- [ ] **B)** 10.1.1.2
- [ ] **C)** 10.1.1.10
- [ ] **D)** Undefined

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The inventory line 'leaf1 ansible_host=10.1.1.1' sets the ansible_host variable to 10.1.1.1.
 
 
</details>

### 4. Which module is used to push configuration commands to Arista EOS devices?

- [ ] **A)** eos_command
- [ ] **B)** eos_config
- [ ] **C)** eos_facts
- [ ] **D)** eos_eapi

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> eos_config is the module designed for declarative and idempotent configuration changes on Arista EOS devices.
 
 
</details>

### 5. Which of the following are valid connection methods for Ansible to manage Arista EOS devices? (Choose two)

- [ ] **A)** network_cli
- [ ] **B)** httpapi
- [ ] **C)** netconf
- [ ] **D)** local

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Arista supports network_cli (SSH CLI) and httpapi (eAPI over HTTPS). netconf is not supported; local is deprecated.
 
 
</details>

### 6. Analyze the playbook task. Will this task be idempotent?

```yaml
- name: Create VLAN 100
  arista.eos.eos_command:
    commands: "vlan 100"
```

- [ ] **A)** Yes, because eos_config uses match: line
- [ ] **B)** Yes, because it uses the parents parameter
- [ ] **C)** No, because it uses eos_command
- [ ] **D)** No, because the command is not stateful

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The task uses eos_command, which executes the command each time and does not check current state. It is not idempotent.
 
 
</details>

### 7. What is the highest precedence variable source in Ansible?

- [ ] **A)** Play vars
- [ ] **B)** Host vars
- [ ] **C)** Extra vars
- [ ] **D)** Role vars

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Extra vars (passed via -e) have the highest precedence in Ansible's variable hierarchy.
 
 
</details>


---

### **Automation with Terraform**

### 8. What is the primary function of the Terraform provider for Arista CloudVision?

- [ ] **A)** It manages device configuration via direct CLI commands to each switch.
- [ ] **B)** It bridges Infrastructure as Code practices with the Arista CloudVision platform.
- [ ] **C)** It replaces the CloudVision GUI with a text-based interface.
- [ ] **D)** It provides a real-time dashboard for network traffic monitoring.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The provider abstracts Arista's RESTful APIs into declarative resources for Terraform, enabling IaC for CloudVision.
 
 
</details>

### 9. Which of the following are resources provided by the Arista CloudVision Terraform provider? (Select two.)

- [ ] **A)** cloudvision_device
- [ ] **B)** cloudvision_container
- [ ] **C)** cloudvision_vlan
- [ ] **D)** cloudvision_bgp

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The provider includes resources for devices and containers; VLAN and BGP are for direct EOS management, not CloudVision.
 
 
</details>

### 10. In the provided Terraform configuration block, what is the correct value for the 'endpoint' attribute when using CloudVision as a Service (CVaaS)?

```hcl
provider "arista" {
  endpoint   = ???
  token      = var.cvp_token
}
```

- [ ] **A)** https://www.arista.io
- [ ] **B)** https://192.168.1.100
- [ ] **C)** https://cvp.corporate.com
- [ ] **D)** https://localhost:8443

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> For CVaaS, the endpoint is the CVaaS API gateway at www.arista.io.
 
 
</details>

### 11. What is the main purpose of the 'cloudvision_configlet' resource in the Terraform provider for Arista CloudVision?

- [ ] **A)** To store device credentials securely.
- [ ] **B)** To define a named set of CLI commands for configuration.
- [ ] **C)** To create a backup of the CloudVision database.
- [ ] **D)** To monitor network traffic in real time.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Configlets are the fundamental unit of configuration; the resource defines the CLI commands to be applied.
 
 
</details>

### 12. Which two methods are valid for authentication when configuring the Arista CloudVision Terraform provider? (Select two.)

- [ ] **A)** Token
- [ ] **B)** Username and password
- [ ] **C)** API key from a third-party service
- [ ] **D)** Certificate installed on the Terraform host

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The provider supports token-based or username/password authentication; other methods are not documented.
 
 
</details>

### 13. The following Terraform resource is missing a required attribute. What is missing?

```hcl
resource "cloudvision_device" "leaf1" {
  hostname = "leaf1-dc1"
  container_id = data.cloudvision_container.spine.id
}
```

- [ ] **A)** serial_number
- [ ] **B)** fqdn
- [ ] **C)** parent_container_id
- [ ] **D)** configlet_id

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The cloudvision_device resource requires a serial number to onboard the device.
 
 
</details>


---

### **CloudVision and Automation Foundation**

### 14. Which CloudVision component stores the intended state (desired configuration) for managed devices?

- [ ] **A)** CloudVision Portal (CVP)
- [ ] **B)** CloudVision eXchange (CVX)
- [ ] **C)** TerminAttr agent
- [ ] **D)** NetDB stream

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CVP stores intended state in configlets and provisioning containers. CVX maintains observed operational state.
 
 
</details>

### 15. Which two statements correctly describe the role of CloudVision eXchange (CVX)? (Choose two.)

- [ ] **A)** It maintains a real-time unified state database from streaming telemetry.
- [ ] **B)** It proxies configuration pushes from CVP to switches.
- [ ] **C)** It aggregates telemetry streams like NetDB and BGP routes.
- [ ] **D)** It serves as the primary user interface for network operators.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> CVX aggregates telemetry and maintains a real-time state database. It does not proxy configuration pushes; CVP handles that directly.
 
 
</details>

### 16. Examine the following configlet content. What is the primary purpose of this configuration block?

```eos
ntp server 192.168.1.100
clock timezone America/New_York
```

- [ ] **A)** It defines a static route for management traffic.
- [ ] **B)** It enables BGP unnumbered on an interface.
- [ ] **C)** It configures NTP client settings on the device.
- [ ] **D)** It sets up a VXLAN tunnel endpoint.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The configlet sets NTP server and timezone, which is a common base configuration for all devices.
 
 
</details>

### 17. In CloudVision provisioning, what does a provisioning container represent?

- [ ] **A)** A logical grouping of devices that inherit common configlets.
- [ ] **B)** A network segment isolated by VLAN.
- [ ] **C)** A physical location of switches in a rack.
- [ ] **D)** A security zone with independent RBAC.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Containers are logical groupings for automation; they do not enforce network topology or physical location.
 
 
</details>

### 18. Which two features are part of CloudVision's day-2 operations capabilities? (Choose two.)

- [ ] **A)** Configuration drift detection via streaming telemetry
- [ ] **B)** Zero-touch provisioning of new devices
- [ ] **C)** Software image management and staged upgrades
- [ ] **D)** Initial device bootstrapping via DHCP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Day-2 includes drift detection and image management. ZTP and DHCP bootstrapping are Day-0 activities.
 
 
</details>

### 19. Consider the following JSON payload used in a CloudVision API call. Which action does this request perform?

```json
{
  "configletId": "c1",
  "netElementIds": ["device123"]
}
```

- [ ] **A)** It creates a new configlet named 'lldp-config'.
- [ ] **B)** It updates an existing configlet with LLDP commands.
- [ ] **C)** It attaches the 'lldp-config' configlet to a device.
- [ ] **D)** It deletes the 'lldp-config' configlet from CloudVision.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The JSON includes 'netElementIds' and 'configletId', which is the pattern for attaching a configlet to devices via the applyConfig endpoint.
 
 
</details>


---

### **Design and Troubleshoot Automated Deployments**

### 20. What is the primary benefit of idempotency in scalable automation workflows?

- [ ] **A)** Repeated execution produces the same final state
- [ ] **B)** It ensures the fastest possible execution
- [ ] **C)** It allows manual intervention during runs
- [ ] **D)** It requires no error handling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Idempotency ensures that running a workflow multiple times results in the same desired state, preventing configuration drift and enabling safe retries.
 
 
</details>

### 21. Which of the following are key concepts for designing scalable automation workflows? (Select all that apply.)

- [ ] **A)** Idempotency and state management
- [ ] **B)** Parallel execution and throttling
- [ ] **C)** Modularity and reusability
- [ ] **D)** Manual rollback procedures

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Manual rollback is not a key concept; scalable workflows emphasize automated rollback, error handling, and orchestration.
 
 
</details>

### 22. An architect is designing a workflow that must push configlets to 500 switches without overwhelming CloudVision. Which approach should be used?

```yaml
workflow:
  steps:
    - apply_configlet:
        batch_size: 20
        max_concurrency: 5
```

- [ ] **A)** Configure a throttling mechanism that limits parallel tasks
- [ ] **B)** Execute all tasks simultaneously for speed
- [ ] **C)** Use a single sequential playbook for all devices
- [ ] **D)** Disable error checking to increase throughput

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Throttling (e.g., using batch sizes or semaphores) prevents overwhelming the management plane and ensures reliable execution.
 
 
</details>

### 23. What is the primary role of Git in network automation?

- [ ] **A)** To version control configuration templates and track changes
- [ ] **B)** To replace the need for backup configurations
- [ ] **C)** To directly push commands to switches
- [ ] **D)** To monitor network performance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Git serves as the single source of truth for declarative configurations, enabling change tracking, rollback, and collaboration.
 
 
</details>

### 24. Which branching strategies are appropriate for network automation CI/CD? (Select all that apply.)

- [ ] **A)** Trunk-based development with short-lived feature branches
- [ ] **B)** GitFlow with long-lived release branches
- [ ] **C)** One permanent branch per environment without merging
- [ ] **D)** No branching; push directly to main

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Both trunk-based and GitFlow can be used; however, trunk-based is often preferred for continuous delivery. Direct pushes to main are not allowed.
 
 
</details>


---

### **Python and REST APIs for Automation**

### 25. What protocol does Arista eAPI use for communication?

- [ ] **A)** JSON-RPC
- [ ] **B)** SOAP
- [ ] **C)** REST
- [ ] **D)** gRPC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Arista eAPI uses JSON-RPC, which is a remote procedure call protocol encoded in JSON. It is not RESTful; it always uses POST to /command-api.
 
 
</details>

### 26. Which HTTP methods are commonly used in RESTful APIs for CRUD operations?

- [ ] **A)** GET
- [ ] **B)** POST
- [ ] **C)** PUT
- [ ] **D)** PATCH

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> RESTful CRUD operations: GET (read), POST (create), PUT (update/replace), DELETE (delete). PATCH is for partial updates but not considered a primary CRUD method.
 
 
</details>

### 27. The following Python code snippet attempts to authenticate to CloudVision API. What critical step is missing?

```python
import requests
resp = requests.post('https://cvp.example.com/login', json={'user': 'admin', 'pass': 'secret'})
token = resp.json()['sessionId']
# missing step
response = requests.get('https://cvp.example.com/api/v2/inventory')
print(response.json())
```

- [ ] **A)** Setting the Authorization header
- [ ] **B)** Using HTTPS instead of HTTP
- [ ] **C)** Adding a request body
- [ ] **D)** Setting a timeout

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CloudVision API requires a bearer token set in the Authorization header. The code below does not include that header; it only makes a POST to login but then doesn't use the token.
 
 
</details>

### 28. What is the default output format of Arista eAPI commands?

- [ ] **A)** JSON
- [ ] **B)** XML
- [ ] **C)** CSV
- [ ] **D)** Text

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> eAPI returns JSON by default. The 'format' parameter can be set to 'text' to get raw CLI output, but JSON is the default and most commonly used for automation.
 
 
</details>

### 29. Which Python libraries are used for parsing YAML data safely?

- [ ] **A)** PyYAML
- [ ] **B)** yaml
- [ ] **C)** json
- [ ] **D)** xml.etree

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> PyYAML provides the 'yaml' module. The safe function is yaml.safe_load(). json and xml.etree are for other formats.
 
 
</details>

### 30. Consider the Python code below. Which function would correctly parse a JSON string from an API response?

```python
import requests
response = requests.get('https://api.example.com/data')
json_string = response.text
parsed_data = # what goes here?
```

- [ ] **A)** json.loads()
- [ ] **B)** json.load()
- [ ] **C)** json.dumps()
- [ ] **D)** str()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> json.loads() parses a JSON string into a Python object. json.load() reads from a file stream. dumps serializes Python to JSON string.
 
 
</details>

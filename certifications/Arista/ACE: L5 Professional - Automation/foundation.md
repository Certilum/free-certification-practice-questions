<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Arista/AristaP.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>ACE: L5 Professional - Automation</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Arista EOS Automation](#arista-eos-automation) (7 questions)
- [Automation Fundamentals and Tools](#automation-fundamentals-and-tools) (6 questions)
- [Automation Workflows and CI/CD](#automation-workflows-and-ci-cd) (6 questions)
- [Network Programmability](#network-programmability) (6 questions)
- [Troubleshooting and Optimization](#troubleshooting-and-optimization) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:55.869Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Arista EOS Automation | 7 |
| Automation Fundamentals and Tools | 6 |
| Automation Workflows and CI/CD | 6 |
| Network Programmability | 6 |
| Troubleshooting and Optimization | 5 |

---

### **Arista EOS Automation**

### 1. What is the method name used in JSON-RPC requests to execute multiple EOS commands via eAPI?

- [ ] **A)** runCmds
- [ ] **B)** executeCommands
- [ ] **C)** batchRun
- [ ] **D)** cliExec

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The correct JSON-RPC method is runCmds. Other names are not used in eAPI.
 
 
</details>

### 2. Which authentication methods are supported by eAPI? (Select two.)

- [ ] **A)** HTTP Basic
- [ ] **B)** HTTP Digest
- [ ] **C)** SNMPv3
- [ ] **D)** Token-based OAuth

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> eAPI supports HTTP Basic, HTTP Digest, and session-based. SNMP and OAuth are not supported.
 
 
</details>

### 3. In the provided JSON-RPC request, what is missing from the parameters to make it valid for eAPI?

```json
{
  "jsonrpc": "2.0",
  "method": "runCmds",
  "params": {
    "version": 1,
    "format": "json"
  },
  "id": 1
}
```

- [ ] **A)** cmds array
- [ ] **B)** method field
- [ ] **C)** jsonrpc version
- [ ] **D)** id number

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The params must contain a 'cmds' array listing the commands to execute.
 
 
</details>

### 4. What is the default format for eAPI command output?

- [ ] **A)** JSON
- [ ] **B)** XML
- [ ] **C)** text
- [ ] **D)** YAML

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> eAPI uses JSON as the default encoding for structured output.
 
 
</details>

### 5. Which two fields are mandatory in every eAPI JSON-RPC request? (Select two.)

- [ ] **A)** jsonrpc
- [ ] **B)** method
- [ ] **C)** params
- [ ] **D)** result

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Every JSON-RPC request must contain 'jsonrpc' and 'method'. 'params' is often required but not mandatory per JSON-RPC spec; however, eAPI requires it.
 
 
</details>

### 6. The JSON-RPC response below contains an error. What is the error code?

```json
{
  "jsonrpc": "2.0",
  "id": 1,
  "error": {
    "code": 1000,
    "message": "Command invalid",
    "data": {}
  }
}
```

- [ ] **A)** -32601
- [ ] **B)** -32700
- [ ] **C)** 1000
- [ ] **D)** 1001

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Error code 1000 is a custom eAPI code for 'command invalid'.
 
 
</details>

### 7. Which command must be included in the cmds array to escalate privileges to enable mode?

- [ ] **A)** enable
- [ ] **B)** privilege 15
- [ ] **C)** login
- [ ] **D)** super

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'enable' command must be explicitly sent to escalate to privileged EXEC mode.
 
 
</details>


---

### **Automation Fundamentals and Tools**

### 8. Which Python library is native to Arista for automating EOS devices?

- [ ] **A)** pyeapi
- [ ] **B)** paramiko
- [ ] **C)** netmiko
- [ ] **D)** requests

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> pyeapi is Arista's native Python library that abstracts eAPI calls.
 
 
</details>

### 9. Identify the libraries that are essential for network automation with Arista. (choose two)

- [ ] **A)** requests
- [ ] **B)** json
- [ ] **C)** flask
- [ ] **D)** django

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The playbook mentions requests for RESTful APIs and json for structured data handling.
 
 
</details>

### 10. What transport protocol is used in this pyeapi connection?

```python
import pyeapi
conn = pyeapi.connect(host='192.0.2.1', username='admin', password='secret', transport='https')
```

- [ ] **A)** HTTPS
- [ ] **B)** SSH
- [ ] **C)** Telnet
- [ ] **D)** HTTP (without SSL)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The transport parameter is set to 'https', indicating HTTPS.
 
 
</details>

### 11. Identify the Ansible module for idempotent configuration management on Arista EOS.

- [ ] **A)** arista.eos.eos_config
- [ ] **B)** arista.eos.eos_command
- [ ] **C)** arista.eos.eos_facts
- [ ] **D)** arista.eos.eos_vlan

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> eos_config is used for idempotent configuration pushes.
 
 
</details>

### 12. Select the two Ansible connection plugins suitable for Arista EOS.

- [ ] **A)** httpapi
- [ ] **B)** network_cli
- [ ] **C)** ssh
- [ ] **D)** paramiko

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The playbook mentions httpapi (preferred) and network_cli as fallback.
 
 
</details>

### 13. Which Ansible module is executed in this task to run a show command?

```yaml
- name: Show version
  arista.eos.eos_command:
    commands: show version
```

- [ ] **A)** arista.eos.eos_command
- [ ] **B)** arista.eos.eos_config
- [ ] **C)** arista.eos.eos_facts
- [ ] **D)** arista.eos.eos_vlan

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> eos_command is used for running show commands.
 
 
</details>


---

### **Automation Workflows and CI/CD**

### 14. What is the primary role of Jenkins in a CI/CD pipeline for Arista network automation?

- [ ] **A)** Orchestration engine
- [ ] **B)** Source of truth for configurations
- [ ] **C)** Secret management system
- [ ] **D)** Testing framework

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Jenkins acts as the orchestration engine that pulls sources from GitLab and triggers builds in a CI/CD pipeline.
 
 
</details>

### 15. Which two stages are essential in a CI/CD pipeline for Arista EOS configuration changes?

- [ ] **A)** Linting
- [ ] **B)** Production deployment without testing
- [ ] **C)** Testing in a sandbox
- [ ] **D)** Manual backup of all devices

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Linting and sandbox testing are essential; production deployment requires testing and approval, not bypass.
 
 
</details>

### 16. Refer to the code. What does this Jenkins pipeline stage do?

```groovy
stage('Lint') {
    steps {
        sh 'ansible-lint playbooks/'
    }
}
```

- [ ] **A)** Deploy to production
- [ ] **B)** Run ansible-lint for syntax checks
- [ ] **C)** Back up current configurations
- [ ] **D)** Create a change control in CloudVision

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The stage executes `ansible-lint` to validate syntax and best practices before further deployment.
 
 
</details>

### 17. What does GitLab primarily provide in a CI/CD pipeline for Arista?

- [ ] **A)** Source of truth for infrastructure-as-code
- [ ] **B)** Configuration orchestration engine
- [ ] **C)** Network device testing platform
- [ ] **D)** Secrets vault

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> GitLab serves as the source of truth for infrastructure-as-code, storing configurations and enabling merge request approvals.
 
 
</details>

### 18. Which two tools are commonly used for automated testing of Arista network configurations?

- [ ] **A)** pytest
- [ ] **B)** Ansible
- [ ] **C)** pyATS
- [ ] **D)** Terraform

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> pytest and pyATS are testing frameworks; Ansible and Terraform are IaC tools, not test frameworks.
 
 
</details>

### 19. Given the pytest fixture, what does it set up for network tests?

```python
@pytest.fixture
def device():
    from arista import eapi
    return eapi.connect(host='10.0.0.1', username='admin', password='secret')
```

- [ ] **A)** A connection to an Arista device via eAPI
- [ ] **B)** A temporary VLAN on the device
- [ ] **C)** A local configuration backup file
- [ ] **D)** A virtual environment for test execution

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The fixture establishes an eAPI connection (via `device.eapi()`) to interact with the Arista device.
 
 
</details>


---

### **Network Programmability**

### 20. What is the primary purpose of OpenConfig YANG models?

- [ ] **A)** To provide vendor-neutral data models for network management
- [ ] **B)** To create Arista-specific configuration syntax
- [ ] **C)** To replace SNMP with CLI commands
- [ ] **D)** To define hardware specifications

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OpenConfig models are vendor-neutral YANG models for consistent network management across heterogeneous devices.
 
 
</details>

### 21. Which two subtrees are present in the OpenConfig interfaces model?

- [ ] **A)** config
- [ ] **B)** state
- [ ] **C)** statistics
- [ ] **D)** operational

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OpenConfig interface model has config (read-write) and state (read-only) subtrees.
 
 
</details>

### 22. What is missing in the path '/interfaces/interface/state' for OpenConfig?

```yang
/interfaces/interface/state
```

- [ ] **A)** Module prefix
- [ ] **B)** List key
- [ ] **C)** Container name
- [ ] **D)** Leaf value

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OpenConfig paths require the module prefix (e.g., openconfig-interfaces:) to avoid ambiguity.
 
 
</details>

### 23. Which network management protocol uses SSH as its transport?

- [ ] **A)** NETCONF
- [ ] **B)** gNMI
- [ ] **C)** eAPI
- [ ] **D)** SNMP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NETCONF uses SSH (TCP 22) as its transport layer as per RFC 6241.
 
 
</details>

### 24. Which two RPCs are part of the gNMI service?

- [ ] **A)** Capabilities
- [ ] **B)** Set
- [ ] **C)** Commit
- [ ] **D)** Lock

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> gNMI defines Capabilities, Get, Set, and Subscribe RPCs. Commit and Lock are NETCONF.
 
 
</details>

### 25. Which gNMI Set operation removes all existing data at a path before writing new data?

```protobuf
SET: {
  path: /interfaces/interface[name=eth1]/config
  val: { ... }
}
```

- [ ] **A)** replace
- [ ] **B)** update
- [ ] **C)** delete
- [ ] **D)** merge

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The replace operation deletes the entire subtree at the path then writes the new value.
 
 
</details>


---

### **Troubleshooting and Optimization**

### 26. Which is the most effective debugging method for an Ansible playbook that intermittently fails in production?

- [ ] **A)** Set ANSIBLE_DEBUG=1
- [ ] **B)** Use --check mode
- [ ] **C)** Use -vvv verbosity
- [ ] **D)** Run --syntax-check

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> -vvv shows the exact commands sent and received, enabling identification of intermittent issues without excessive overhead.
 
 
</details>

### 27. Which of the following operations are idempotent? (Select all that apply)

- [ ] **A)** Setting an interface description with eos_config
- [ ] **B)** Copying a file without checksum verification
- [ ] **C)** Reloading a switch
- [ ] **D)** Creating a VLAN with eos_config

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Idempotent operations produce the same state regardless of repetition. eos_config tasks are idempotent; file copy without checksum and reload are not.
 
 
</details>

### 28. Analyze the following Arista EOS role configuration. What access level does it provide?

```eos
role automation_role
   permit read all
   permit write using configure terminal interface vlan
   deny write all
```

- [ ] **A)** Least privilege
- [ ] **B)** Full admin
- [ ] **C)** Read-only
- [ ] **D)** Custom but unrestricted

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The role permits only show commands and specific configure commands, denying all others, which is the essence of least privilege.
 
 
</details>

### 29. What is the primary purpose of querying the CMDB before an automated network change?

- [ ] **A)** To verify device reachability
- [ ] **B)** To obtain the intended IP subnet and role
- [ ] **C)** To validate API credentials
- [ ] **D)** To check the software version

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The CMDB serves as the source of truth for device attributes such as subnet assignment and role, which must be known before applying changes.
 
 
</details>

### 30. Which monitoring methods are supported for automation jobs in Arista CloudVision? (Select all that apply)

- [ ] **A)** Syslog
- [ ] **B)** SNMP traps
- [ ] **C)** DHCP logs
- [ ] **D)** Prometheus exporter

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> CloudVision supports Syslog, SNMP traps, and Prometheus integration. DHCP logs are unrelated to job monitoring.
 
 
</details>

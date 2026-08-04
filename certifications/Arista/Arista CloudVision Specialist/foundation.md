<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Arista/Arista%20CloudVision%20Specialist" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Arista CloudVision Specialist</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Automation and Integration](#automation-and-integration) (6 questions)
- [CloudVision Architecture and Deployment](#cloudvision-architecture-and-deployment) (7 questions)
- [Provisioning and Change Management](#provisioning-and-change-management) (9 questions)
- [Telemetry and Analytics](#telemetry-and-analytics) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:01.175Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Automation and Integration | 6 |
| CloudVision Architecture and Deployment | 7 |
| Provisioning and Change Management | 9 |
| Telemetry and Analytics | 8 |

---

### **Automation and Integration**

### 1. What is the primary data serialization format used by CloudVision REST API?

- [ ] **A)** JSON
- [ ] **B)** Protocol Buffers
- [ ] **C)** XML
- [ ] **D)** YAML

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CloudVision REST API uses JSON for data serialization, as stated in the document. Protocol Buffers are used by gRPC.
 
 
</details>

### 2. Which two statements are true about CloudVision's gRPC API?

- [ ] **A)** It uses HTTP/2 as transport protocol
- [ ] **B)** It uses token-based authentication
- [ ] **C)** It supports server streaming
- [ ] **D)** It uses JSON for payload serialization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> gRPC uses HTTP/2 and supports server streaming. It uses certificate-based mTLS, not tokens, and Protocol Buffers, not JSON.
 
 
</details>

### 3. Examine the code block. What header is required to authenticate this REST API request?

```python
import requests
url = 'https://cvp.company.com/api/v2/device'
headers = {}
response = requests.get(url, headers=headers)
```

- [ ] **A)** Authorization: Bearer <token>
- [ ] **B)** X-API-Key: <key>
- [ ] **C)** Content-Type: application/json
- [ ] **D)** User-Agent: CloudVision

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CloudVision REST API uses token-based authentication. The token must be included in the Authorization header as a Bearer token.
 
 
</details>

### 4. Which API type is designed for high-performance bidirectional streaming of telemetry data?

- [ ] **A)** REST API
- [ ] **B)** gRPC API
- [ ] **C)** SNMP API
- [ ] **D)** NETCONF API

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> gRPC supports bidirectional streaming and is optimized for high-frequency telemetry. REST is pull-based and not designed for streaming.
 
 
</details>

### 5. Which two methods are used for pagination with CloudVision REST API?

- [ ] **A)** Using limit and offset parameters
- [ ] **B)** Using page tokens
- [ ] **C)** Using gRPC streaming
- [ ] **D)** Automatic pagination without parameters

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The document states that REST API uses '?limit=' and '?offset=' or page tokens. gRPC streaming is not used for pagination.
 
 
</details>

### 6. Look at the HTTP request. What is the HTTP method being used?

```http
GET /api/v2/configlet HTTP/1.1
Host: cvp.company.com
Authorization: Bearer <token>
```

- [ ] **A)** GET
- [ ] **B)** POST
- [ ] **C)** PUT
- [ ] **D)** DELETE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The request line starts with 'GET', indicating a retrieval operation.
 
 
</details>


---

### **CloudVision Architecture and Deployment**

### 7. Which CloudVision component provides the primary web-based management interface and REST API gateway?

- [ ] **A)** CloudVision Portal (CVP)
- [ ] **B)** CloudVision eXchange (CVX)
- [ ] **C)** CloudVision Network Controller (CVNC)
- [ ] **D)** Telemetry Database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CVP is the central management interface and API gateway, while CVX handles state relay and CVNC enforces policies.
 
 
</details>

### 8. Select two core functions of the CloudVision eXchange (CVX) component.

- [ ] **A)** Secure state relay between switches and CVP
- [ ] **B)** Storage of historical telemetry data
- [ ] **C)** Proxy for NetDB and BGP-LS information
- [ ] **D)** Enforcement of network policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> CVX relays state and proxies protocols like NetDB; it does not store data or enforce policies—those are done by the Telemetry DB and CVNC respectively.
 
 
</details>

### 9. Examine the script snippet below. What is its primary purpose?

```bash
#!/bin/bash
hostname leaf-01
cvp reg --server https://cvp.company.com --token abc123
```

- [ ] **A)** Configure BGP peering
- [ ] **B)** Perform zero-touch provisioning onboarding
- [ ] **C)** Enable streaming telemetry
- [ ] **D)** Shut down the switch

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The script sets a hostname and registers the switch with CloudVision, which is part of ZTP Day-0 provisioning.
 
 
</details>

### 10. What is the minimum number of CloudVision nodes required to form a highly available cluster?

- [ ] **A)** 2
- [ ] **B)** 3
- [ ] **C)** 4
- [ ] **D)** 5

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A 3-node cluster provides quorum; 2 nodes lack a tiebreaker and cannot maintain writes if one fails.
 
 
</details>

### 11. Which two requirements are necessary for a switch to successfully onboard using Zero-Touch Provisioning (ZTP)?

- [ ] **A)** DHCP server offering Option 67 with a config URL
- [ ] **B)** Static IP configuration on the switch
- [ ] **C)** IP reachability to the CloudVision cluster
- [ ] **D)** Physical console access to approve the device

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> ZTP relies on DHCP to provide a script URL and on network connectivity to reach CVP. Static IP or console access is not required.
 
 
</details>

### 12. Given the firewall rule below, which port is being opened for CloudVision telemetry?

```plaintext
permit tcp any host 192.168.10.10 eq 8080
```

- [ ] **A)** 443
- [ ] **B)** 22
- [ ] **C)** 8080
- [ ] **D)** 514

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> CloudVision Collector listens on TCP port 8080 for streaming telemetry from switches. Port 443 is for GUI/API, 22 for SSH, 514 for syslog.
 
 
</details>

### 13. Which CloudVision component is responsible for enforcing network policies?

- [ ] **A)** CloudVision Portal (CVP)
- [ ] **B)** CloudVision eXchange (CVX)
- [ ] **C)** CloudVision Network Controller (CVNC)
- [ ] **D)** Telemetry Database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> CVNC is the orchestration engine that enforces policies; CVP manages, CVX relays, and Telemetry DB stores data.
 
 
</details>


---

### **Provisioning and Change Management**

### 14. Which DHCP option is typically used to point a bare-metal Arista switch to the CloudVision bootstrap files during Zero-Touch Provisioning?

- [ ] **A)** Option 67
- [ ] **B)** Option 125
- [ ] **C)** Option 151
- [ ] **D)** Option 66

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> CloudVision ZTP uses DHCP option 125 for Arista-specific bootstrapping, as stated in the playbook.
 
 
</details>

### 15. Which of the following are correct statements about CloudVision configlets? (Select two.)

- [ ] **A)** A configlet is a complete device startup configuration.
- [ ] **B)** Configlets are applied to devices via containers or tags.
- [ ] **C)** Configlets can contain variables for dynamic substitution.
- [ ] **D)** Configlets are automatically pushed to devices immediately upon creation.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Configlets are configuration fragments assigned via containers/tags and support variable substitution, but they are not full startup configs and require explicit application.
 
 
</details>

### 16. Study the following YAML data file used for template-based configuration deployment. Which issue will prevent CloudVision from rendering the template correctly?

```yaml
leaf-101:
  hostname: leaf-101
  mgmt_ip: 10.1.1.1
  vlans:
	- 10
	- 20
```

- [ ] **A)** The template expects a variable 'vlan_list' but the data provides 'vlans'.
- [ ] **B)** The indentation is inconsistent (tab used instead of spaces).
- [ ] **C)** The data file is missing a required 'device_id' field.
- [ ] **D)** The YAML file uses a .json extension but contains YAML content.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> YAML strictly requires spaces for indentation; tabs cause parsing errors. CloudVision will reject the template rendering.
 
 
</details>

### 17. What is the primary purpose of a Compliance Engine in CloudVision?

- [ ] **A)** It pushes configuration changes to devices.
- [ ] **B)** It continuously monitors device configurations against desired state.
- [ ] **C)** It generates audit logs for user actions.
- [ ] **D)** It manages firmware image uploads.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Compliance Engine continuously verifies that actual device configurations match the intended state defined by configlets and rules.
 
 
</details>

### 18. Which of the following are required to perform a rollback of a failed change control in CloudVision? (Select two.)

- [ ] **A)** A pre-change snapshot must have been taken.
- [ ] **B)** The change control must have been approved by two people.
- [ ] **C)** The rollback option must be enabled in the change control template.
- [ ] **D)** The device must be in maintenance mode.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Pre-change snapshots capture the baseline for rollback, and the rollback action must be explicitly configured in the change control template.
 
 
</details>

### 19. Look at the following Jinja2 template snippet. What will be the output for a device with data 'hostname: leaf-01'?

```jinja2
hostname {{ hostname }}
```

- [ ] **A)** hostname leaf-01
- [ ] **B)** hostname {{ hostname }}
- [ ] **C)** leaf-01
- [ ] **D)** hostname leaf01

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Jinja2 variable substitution replaces {{ hostname }} with the actual value 'leaf-01', producing 'hostname leaf-01'.
 
 
</details>

### 20. In CloudVision, where are EOS image files stored for firmware upgrades?

- [ ] **A)** In the Configlet database
- [ ] **B)** In the Analytics database
- [ ] **C)** In the Image Repository under /cvpi/images/
- [ ] **D)** In the device flash memory

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> CVP stores uploaded image files in the Image Repository, specifically under /cvpi/images/ directory.
 
 
</details>

### 21. Which of the following are valid steps in a CloudVision change control workflow for a configlet update? (Select two.)

- [ ] **A)** Create workspace and stage changes
- [ ] **B)** Build workspace to preview configuration diff
- [ ] **C)** Approve the change by a designated approver
- [ ] **D)** Automatically push config without approval

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> A typical change control includes building the workspace for preview and an approval step. Workspace creation is a prerequisite, not a step within the change control itself.
 
 
</details>

### 22. The following command is entered directly on an Arista switch's CLI. After this manual change, CloudVision will detect a drift. What is the correct remediation according to best practices?

```eos
switch# configure terminal
switch(config)# interface Ethernet1
switch(config-if-Et1)# description Manual Change
```

- [ ] **A)** Ignore the drift because the change was intentional.
- [ ] **B)** Apply the corresponding configlet via a change control.
- [ ] **C)** Reboot the device to re-apply the last known good config.
- [ ] **D)** Delete the device from CloudVision and re-add it via ZTP.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The correct practice is to re-apply the intended configlet through a change control, not to ignore or use disruptive methods.
 
 
</details>


---

### **Telemetry and Analytics**

### 23. What is the core component that enables streaming telemetry on Arista EOS?

- [ ] **A)** TerminAttr Agent
- [ ] **B)** SNMP Poller
- [ ] **C)** CloudVision API
- [ ] **D)** EOS Logging Agent

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TerminAttr is the daemon that acts as a gRPC client to stream operational data to CloudVision.
 
 
</details>

### 24. Which two of the following are valid TerminAttr parameters?

- [ ] **A)** ingestgrpcurl
- [ ] **B)** ingestauth
- [ ] **C)** grpc-port
- [ ] **D)** telemetry-profile

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> TerminAttr uses ingestgrpcurl for collector URL and ingestauth for authentication token; others are not direct parameters.
 
 
</details>

### 25. What information does the command 'show daemon TerminAttr' provide?

```bash
show daemon TerminAttr
```

- [ ] **A)** Agent status and connectivity to CloudVision
- [ ] **B)** Interface error counters
- [ ] **C)** BGP neighbor states
- [ ] **D)** CPU utilization over time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This command shows the TerminAttr agent status, including connection state and uptime.
 
 
</details>

### 26. Which CloudVision widget type is best for displaying current CPU load as a single value?

- [ ] **A)** Gauge
- [ ] **B)** Time Series Graph
- [ ] **C)** Top-N Table
- [ ] **D)** Pie Chart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Gauge widget displays a single metric value, ideal for current load monitoring.
 
 
</details>

### 27. Which two of the following are valid notification channels in CloudVision?

- [ ] **A)** Email
- [ ] **B)** Webhook
- [ ] **C)** SNMP Polling
- [ ] **D)** SSH

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CloudVision supports email and webhook notifications; SNMP polling is not a notification channel.
 
 
</details>

### 28. What does the following telemetry profile path configure? (Select two)\npath /interfaces/interface[name=Ethernet1]/state/counters sample-interval 30

```bash
path /interfaces/interface[name=Ethernet1]/state/counters sample-interval 30
```

- [ ] **A)** Sample interval
- [ ] **B)** Interface name
- [ ] **C)** BGP peer state
- [ ] **D)** CPU temperature

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The path specifies interface counters for Ethernet1 with a 30-second sample interval.
 
 
</details>

### 29. What is the range of the CloudVision device health score?

- [ ] **A)** 0 to 100
- [ ] **B)** 0 to 10
- [ ] **C)** 1 to 5
- [ ] **D)** 0 to 1000

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Health score is a composite value from 0 (worst) to 100 (best), summarizing device health.
 
 
</details>

### 30. Which two of the following are advantages of streaming telemetry over SNMP polling?

- [ ] **A)** Push-based data delivery
- [ ] **B)** Sub-second granularity
- [ ] **C)** Higher CPU overhead on switch
- [ ] **D)** Requires polling intervals

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Streaming telemetry pushes data with fine granularity, unlike SNMP polling which is pull-based and coarse.
 
 
</details>

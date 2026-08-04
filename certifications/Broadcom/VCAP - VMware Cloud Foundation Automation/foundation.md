<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Broadcom/Cloud%20Foundation%20Automation.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>VCAP - VMware Cloud Foundation Automation</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Automation Security and Compliance](#automation-security-and-compliance) (4 questions)
- [Automation Troubleshooting and Monitoring](#automation-troubleshooting-and-monitoring) (6 questions)
- [Integration with External Systems and Scripting](#integration-with-external-systems-and-scripting) (6 questions)
- [VMware Cloud Foundation Automation Architecture](#vmware-cloud-foundation-automation-architecture) (6 questions)
- [Workload Domain Lifecycle Automation](#workload-domain-lifecycle-automation) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:52.767Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Automation Security and Compliance | 4 |
| Automation Troubleshooting and Monitoring | 6 |
| Integration with External Systems and Scripting | 6 |
| VMware Cloud Foundation Automation Architecture | 6 |
| Workload Domain Lifecycle Automation | 8 |

---

### **Automation Security and Compliance**

### 1. Which role type in VCF Automation cannot be modified but provides predefined permissions?

- [ ] **A)** Custom role
- [ ] **B)** Built-in role
- [ ] **C)** Organization Owner
- [ ] **D)** Project Administrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Built-in roles have predefined permissions that cannot be modified; custom roles allow granular permission sets.
 
 
</details>

### 2. Which statements about RBAC roles in VCF Automation are true? (Select two)

- [ ] **A)** Organization Owner has full access across all projects
- [ ] **B)** Service Administrator can manage only one specific service across all projects
- [ ] **C)** Project Administrator can add vCenter endpoints
- [ ] **D)** Custom roles can be edited but built-in roles can also be modified

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Organization Owner has full access; Service Administrator manages a specific service across all projects. Project administrators cannot add endpoints; built-in roles cannot be modified.
 
 
</details>

### 3. Review the code block and select the correct outcome for the user.

```python
# Assume: User John has Organization Viewer role (Org-wide)
# John is assigned Project Administrator role in Project A
# In VCF Automation, project-level roles override org-level roles unless explicitly denied.
# Effective permission in Project A: Project Administrator

```

- [ ] **A)** User has Project Administrator rights in Project A
- [ ] **B)** User is restricted to Organization Viewer in Project A
- [ ] **C)** User has no access to Project A
- [ ] **D)** User has Service Administrator rights in Project A

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Project roles override organization roles; therefore, the user has full Project Administrator rights in Project A.
 
 
</details>

### 4. Which authentication method is recommended for long-running service accounts in VCF Automation?

- [ ] **A)** OAuth 2.0 tokens with refresh
- [ ] **B)** Client certificate-based authentication
- [ ] **C)** Session cookies
- [ ] **D)** Username and password directly in API calls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Certificate-based authentication avoids token expiration and reduces secret rotation overhead for long-running service accounts.
 
 
</details>


---

### **Automation Troubleshooting and Monitoring**

### 5. Which component is used to identify the exact step where an automation task failed in VCF?

- [ ] **A)** Audit Log Viewer
- [ ] **B)** Task Details pane
- [ ] **C)** vRealize Log Insight
- [ ] **D)** vCenter alarms

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Task Details pane in SDDC Manager shows the failed subtask name and error message, enabling precise identification of the failure point.
 
 
</details>

### 6. Which two are common root causes of automation failures in VCF?

- [ ] **A)** Network misconfigurations
- [ ] **B)** Certificate expiration
- [ ] **C)** Hardware incompatibility
- [ ] **D)** DNS resolution failures

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The playbook document lists network misconfigurations and certificate expiration as root causes of automation failures.
 
 
</details>

### 7. Examine the log snippet. What error pattern does it indicate?

```plaintext
com.vmware.vcac.platform.provisioning.deployment.FailedReservationException: Provisioning failed due to reservation error
```

- [ ] **A)** Provisioning error
- [ ] **B)** Authentication failure
- [ ] **C)** Resource exhaustion
- [ ] **D)** Network timeout

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The log shows a 'FailedReservationException', which is a provisioning error related to reservation failures.
 
 
</details>

### 8. What HTTP status code signifies an authentication failure in VCF API calls?

- [ ] **A)** 200
- [ ] **B)** 401
- [ ] **C)** 403
- [ ] **D)** 500

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A 401 Unauthorized status indicates authentication failure, such as an expired or invalid token.
 
 
</details>

### 9. Which two factors can cause a 403 Forbidden error in VCF Automation API?

- [ ] **A)** Insufficient role scope
- [ ] **B)** Token scope mismatch
- [ ] **C)** IdP unreachable
- [ ] **D)** Certificate chain untrusted

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A 403 error occurs when the token is valid but lacks sufficient permissions due to role scope or token scope mismatch.
 
 
</details>

### 10. Given the job status snippet, what is the overall job status?

```json
{
  "status": "FAILED",
  "errorCode": "VCF_RESOURCE_LOCKED",
  "tasks": [
    {
      "status": "SUCCESS"
    }
  ]
}
```

- [ ] **A)** SUCCESS
- [ ] **B)** FAILED
- [ ] **C)** RUNNING
- [ ] **D)** CANCELLED

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The overall job status is 'FAILED' despite individual task successes, as indicated by the status field in the JSON.
 
 
</details>


---

### **Integration with External Systems and Scripting**

### 11. What is the primary purpose of VMware PowerCLI in VCF automation?

- [ ] **A)** To provide a web-based management interface
- [ ] **B)** To offer cmdlet-driven access to vSphere and related products
- [ ] **C)** To replace REST API calls for all VCF operations
- [ ] **D)** To manage only NSX-T components

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> PowerCLI provides deep, cmdlet-driven access to vSphere and related VMware products for rapid scripting within Windows environments.
 
 
</details>

### 12. Which of the following are common methods to authenticate against VMware SSO in VCF automation? (Choose two.)

- [ ] **A)** PowerCLI Connect-VIServer with a password
- [ ] **B)** Python direct POST to /sdk/login with Basic auth
- [ ] **C)** Using local OS account credentials
- [ ] **D)** FTP file transfer with embedded token

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> PowerCLI uses Connect-VIServer with credentials; Python can perform a POST to the vCenter SSO endpoint with Basic auth.
 
 
</details>

### 13. Examine the code block. What is the purpose of the loop in this REST API automation?

```python
task_id = response.json()['taskId']
while True:
    task = requests.get(f'https://vcf-manager/v1/tasks/{task_id}', headers=auth_header).json()
    if task['status'] in ['SUCCESSFUL', 'FAILED']:
        break
    time.sleep(5)
```

- [ ] **A)** To retry authentication
- [ ] **B)** To wait for an asynchronous task to complete
- [ ] **C)** To send multiple API requests in parallel
- [ ] **D)** To handle rate limiting

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> After a 202 Accepted response, the loop polls the task endpoint until status becomes SUCCESSFUL or FAILED.
 
 
</details>

### 14. What is the default token lifetime for VCF API bearer tokens?

- [ ] **A)** 1 hour
- [ ] **B)** 12 hours
- [ ] **C)** 24 hours
- [ ] **D)** 48 hours

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The VCF API bearer token has a configurable expiration, defaulting to 24 hours, as stated in the PLAYBOOK_DOCUMENT.
 
 
</details>

### 15. Which of the following are best practices for error handling in VCF automation scripts? (Choose two.)

- [ ] **A)** Using try-catch blocks
- [ ] **B)** Ignoring all errors with SilentlyContinue
- [ ] **C)** Implementing retry logic with exponential backoff
- [ ] **D)** Hardcoding error messages in logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Try-catch and retry with exponential backoff are key error handling patterns; ignoring errors is not recommended.
 
 
</details>

### 16. Analyze the PowerCLI snippet. What is the main idempotency pattern used?

```powershell
$hostName = 'esxi-51.lab.com'
$existing = Get-VMHost -Name $hostName -ErrorAction SilentlyContinue
if (-not $existing) {
    Add-VMHost -Name $hostName -Location Datacenter01 -Credential $cred
}
```

- [ ] **A)** Retry on failure
- [ ] **B)** State checking before modification
- [ ] **C)** Using -Force parameter
- [ ] **D)** Error swallowing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The script checks if the host exists using Get-VMHost before calling Add-VMHost, ensuring idempotency.
 
 
</details>


---

### **VMware Cloud Foundation Automation Architecture**

### 17. Which component is responsible for tenant workload provisioning in VMware Cloud Foundation?

- [ ] **A)** SDDC Manager
- [ ] **B)** vRealize Automation (Aria Automation)
- [ ] **C)** SaltStack Config
- [ ] **D)** vRealize Orchestrator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> vRealize Automation handles self-service provisioning of workloads. SDDC Manager manages infrastructure lifecycle, not tenant VMs.
 
 
</details>

### 18. Which two of the following are core components of the VCF automation architecture?

- [ ] **A)** SDDC Manager
- [ ] **B)** Ansible
- [ ] **C)** vRealize Automation
- [ ] **D)** Terraform

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> SDDC Manager and vRealize Automation are core VCF components. Ansible and Terraform are external integrations.
 
 
</details>

### 19. Refer to the code block. What authentication method is being used for the API call?

```bash
curl -X GET https://sddc-manager.vcf.local/v1/domains \
  -H "Authorization: Bearer eyJhbGciOiJSUzI1NiIs..."
```

- [ ] **A)** Basic Authentication
- [ ] **B)** Token-based (Bearer) Authentication
- [ ] **C)** Session-based Authentication
- [ ] **D)** Certificate-based Authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 'Authorization: Bearer <token>' header indicates token-based authentication.
 
 
</details>

### 20. What is the primary role of SDDC Manager in VCF automation?

- [ ] **A)** Tenant workload provisioning
- [ ] **B)** Infrastructure lifecycle orchestration
- [ ] **C)** Configuration management of guest OS
- [ ] **D)** Network security policy enforcement

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SDDC Manager orchestrates Day-0/1 infrastructure lifecycle, not tenant workloads or guest OS.
 
 
</details>

### 21. Which two are automation constructs provided by vRealize Automation?

- [ ] **A)** Cloud Templates
- [ ] **B)** Host Profiles
- [ ] **C)** Projects
- [ ] **D)** NSX Transport Zones

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Cloud Templates (blueprints) and Projects are vRA constructs. Host profiles and NSX transport zones are infrastructure-level.
 
 
</details>

### 22. Based on the API call below, what does the '202 Accepted' response indicate?

```http
POST /v1/domains HTTP/1.1
Host: sddc-manager.vcf.local
Authorization: Bearer <token>
Content-Type: application/json

Response: HTTP/1.1 202 Accepted
Location: /v1/tasks/abc123
```

- [ ] **A)** The operation completed successfully
- [ ] **B)** The request is in progress, poll the task endpoint
- [ ] **C)** Authentication failed
- [ ] **D)** Invalid request format

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A 202 Accepted means the request is accepted for processing; the caller must poll /tasks for completion.
 
 
</details>


---

### **Workload Domain Lifecycle Automation**

### 23. What is the base URL for all SDDC Manager REST API calls?

- [ ] **A)** https://<sddc-manager-fqdn>/v1/
- [ ] **B)** https://<sddc-manager-fqdn>/api/v1/
- [ ] **C)** https://<sddc-manager-fqdn>/sddc/v1/
- [ ] **D)** https://<sddc-manager-fqdn>/rest/v1/

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The SDDC Manager API uses base URL https://<sddc-manager-fqdn>/v1/ for all endpoints.
 
 
</details>

### 24. Which two HTTP methods does SDDC Manager API use for creating and updating resources?

- [ ] **A)** POST
- [ ] **B)** PUT
- [ ] **C)** PATCH
- [ ] **D)** DELETE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> SDDC Manager uses POST for creation and PATCH for partial updates. PUT is not supported for domain modification.
 
 
</details>

### 25. Based on the API response, what should the automation script do next?

```json
{
  "status": "202 Accepted",
  "Location": "/v1/tasks/12345"
}
```

- [ ] **A)** Retry the same POST request
- [ ] **B)** Poll the task URL from the Location header
- [ ] **C)** Check the response body for domain ID
- [ ] **D)** Wait for 60 seconds and then call GET on the domain

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 202 response includes a Location header with the task URL. The script must poll that endpoint to monitor progress.
 
 
</details>

### 26. What HTTP status code indicates a malformed payload during domain creation?

- [ ] **A)** 200
- [ ] **B)** 202
- [ ] **C)** 400
- [ ] **D)** 500

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> A 400 Bad Request is returned when payload validation fails before any async task is created.
 
 
</details>

### 27. Which two fields are mandatory in a workload domain creation payload?

- [ ] **A)** name
- [ ] **B)** description
- [ ] **C)** type
- [ ] **D)** backupConfig

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The payload requires name and type fields. Description and backupConfig are optional.
 
 
</details>

### 28. Why does the automation script refresh the bearer token during long-running operations?

```python
if time.time() > token_expiry:
    token = authenticate()
    token_expiry = time.time() + 1800
```

- [ ] **A)** To avoid 401 errors due to token expiration
- [ ] **B)** To increase API call speed
- [ ] **C)** To comply with security policies
- [ ] **D)** To reduce network latency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SDDC Manager tokens expire after a default 30 minutes. Long-running domain creation tasks may exceed this, so refreshing prevents 401 Unauthorized.
 
 
</details>

### 29. Which endpoint is used to retrieve the status of an asynchronous task?

- [ ] **A)** GET /v1/tasks/{taskId}
- [ ] **B)** GET /v1/workflows/{workflowId}
- [ ] **C)** GET /v1/domains/{domainId}
- [ ] **D)** GET /v1/clusters/{clusterId}

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The task status is obtained by sending a GET request to /v1/tasks/{taskId} with the task ID from the Location header.
 
 
</details>

### 30. Which two workload domain types are commonly created using SDDC Manager?

- [ ] **A)** VI
- [ ] **B)** MANAGEMENT
- [ ] **C)** EDGE
- [ ] **D)** STORAGE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The common domain types are 'VI' for virtual infrastructure and 'MANAGEMENT' for management domain. Edge and storage are not domain types.
 
 
</details>

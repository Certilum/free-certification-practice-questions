<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Avaya/AXP%20Public%20Cloud%20Developer" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>AXP Public Cloud Developer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [API Integration and Development](#api-integration-and-development) (9 questions)
- [Architecture and Core Concepts](#architecture-and-core-concepts) (6 questions)
- [Automation and Workflow Design](#automation-and-workflow-design) (7 questions)
- [Deployment and Lifecycle Management](#deployment-and-lifecycle-management) (5 questions)
- [Troubleshooting and Optimization](#troubleshooting-and-optimization) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:26:14.259Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| API Integration and Development | 9 |
| Architecture and Core Concepts | 6 |
| Automation and Workflow Design | 7 |
| Deployment and Lifecycle Management | 5 |
| Troubleshooting and Optimization | 3 |

---

### **API Integration and Development**

### 1. What OAuth 2.0 flow is recommended for server-to-server communication in Avaya AXP?

- [ ] **A)** Client Credentials Grant
- [ ] **B)** Authorization Code Grant with PKCE
- [ ] **C)** Implicit Grant
- [ ] **D)** Resource Owner Password Credentials Grant

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Client Credentials Grant is designed for server-to-server communication without user interaction.
 
 
</details>

### 2. Which two properties are true regarding API keys in Avaya AXP?

- [ ] **A)** They are static alphanumeric strings.
- [ ] **B)** They provide user-level granularity.
- [ ] **C)** They can be sent in custom headers or query parameters.
- [ ] **D)** They are ideal for client-side applications like mobile apps.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> API keys are static strings sent in headers or query params; they lack user granularity and should not be used client-side.
 
 
</details>

### 3. Analyze the code snippet to determine which OAuth 2.0 flow is being used.

```http
POST /oauth/token HTTP/1.1
Content-Type: application/x-www-form-urlencoded
grant_type=client_credentials&client_id=abc&client_secret=secret123
```

- [ ] **A)** Client Credentials Grant
- [ ] **B)** Authorization Code Grant with PKCE
- [ ] **C)** Implicit Grant
- [ ] **D)** Resource Owner Password Credentials

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code exchanges client_id and client_secret for a token without user context, indicating Client Credentials Grant.
 
 
</details>

### 4. What HTTP method is used to create a new contact record via AXP Contact API?

- [ ] **A)** POST
- [ ] **B)** GET
- [ ] **C)** PUT
- [ ] **D)** DELETE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> POST is used to create new resources; the Contact API uses POST /api/v2/contacts.
 
 
</details>

### 5. Which two features are characteristic of the AXP Reporting API?

- [ ] **A)** Uses cursor-based pagination.
- [ ] **B)** Returns synchronous results immediately.
- [ ] **C)** Supports cursor-based pagination with 'page[after]' parameter.
- [ ] **D)** Requires WebSocket for real-time data.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Reporting API uses cursor pagination; it may return large datasets asynchronously, not always immediate.
 
 
</details>

### 6. Review the API response snippet to determine the correct action for pagination.

```json
{
  "data": [ ... ],
  "next": "eyJpZCI6Ijc4RkZDQ0ExIn0="
}
```

- [ ] **A)** Use the 'next' cursor value for the next request.
- [ ] **B)** Increment a 'page' parameter by 1.
- [ ] **C)** Increase the 'limit' parameter to 1000.
- [ ] **D)** Re-send the same request without changes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AXP uses cursor-based pagination; the 'next' field contains the token for the next page.
 
 
</details>

### 7. What is the primary protocol used for real-time event streaming in Avaya AXP?

- [ ] **A)** WebSocket
- [ ] **B)** HTTP long polling
- [ ] **C)** Server-Sent Events
- [ ] **D)** RESTful APIs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> WebSocket provides persistent low-latency bidirectional communication suitable for real-time events.
 
 
</details>

### 8. Which two are required steps when setting up a webhook subscription in AXP?

- [ ] **A)** Provide a target URL for event delivery.
- [ ] **B)** Include an OAuth 2.0 token in the subscription request.
- [ ] **C)** Respond to a verification challenge from AXP.
- [ ] **D)** Set up a WebSocket connection first.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Webhook registration requires a target URL and successful verification of the endpoint by responding to a challenge.
 
 
</details>

### 9. Given the code snippet, identify the purpose of the 'X-Avaya-Signature' header.

```javascript
// Server-side webhook handler
const signature = request.headers['X-Avaya-Signature'];
const computed = crypto.createHmac('sha256', secret).update(body).digest('hex');
if (signature !== computed) throw new Error('Invalid signature');
```

- [ ] **A)** To verify the webhook payload authenticity.
- [ ] **B)** To authenticate the client application.
- [ ] **C)** To indicate the event type.
- [ ] **D)** To specify the retry count.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The X-Avaya-Signature header contains an HMAC-SHA256 signature used to verify the payload came from AXP.
 
 
</details>


---

### **Architecture and Core Concepts**

### 10. What is the primary communication method between AXP microservices for state changes?

- [ ] **A)** Synchronous REST calls
- [ ] **B)** Asynchronous events via Kafka or AMQP
- [ ] **C)** Direct database sharing
- [ ] **D)** Remote Procedure Calls over gRPC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The document states that services communicate asynchronously via Kafka or AMQP for state changes, while synchronous REST is used for queries. Direct database sharing is not used in microservices; gRPC can be used for synchronous invocation but not for state change events.
 
 
</details>

### 11. Which two components are part of AXP's observability stack?

- [ ] **A)** ELK stack (Elasticsearch, Logstash, Kibana)
- [ ] **B)** Prometheus
- [ ] **C)** Istio
- [ ] **D)** Resilience4j

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The document lists structured logs (ELK), metrics (Prometheus), and traces (OpenTelemetry) as the observability triad. Istio is a service mesh, Resilience4j is a circuit breaker library—neither are observability tools.
 
 
</details>

### 12. Refer to the code block. What does the YAML snippet represent in AXP's deployment model?

```yaml
apiVersion: v1
kind: ResourceQuota
metadata:
  name: tenant-a-quota
spec:
  hard:
    requests.cpu: "4"
    requests.memory: 8Gi
    limits.cpu: "8"
    limits.memory: 16Gi
```

- [ ] **A)** Kubernetes namespace isolation for multi-tenancy
- [ ] **B)** Service mesh traffic splitting
- [ ] **C)** API gateway rate limiting rule
- [ ] **D)** Prometheus alerting rule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The YAML defines a Kubernetes ResourceQuota limiting compute resources per namespace, which is a standard way AXP enforces tenant isolation in its multi-tenant environment.
 
 
</details>

### 13. What is the primary function of the API Gateway in AXP?

- [ ] **A)** Handle East-West microservice communication
- [ ] **B)** Act as a single entry point for external clients, handling authentication and routing
- [ ] **C)** Orchestrate container lifecycle on Kubernetes
- [ ] **D)** Store tenant-specific data in schemas

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The document describes the API Gateway as a unified entry point that handles authentication, rate limiting, and routing. East-West traffic is managed by the service mesh; Kubernetes orchestrates containers; data storage is separate.
 
 
</details>

### 14. Which two statements correctly describe AXP's multi-tenant dedicated model?

- [ ] **A)** Tenants share the same compute resources with logical isolation
- [ ] **B)** Each tenant gets its own isolated set of cloud resources
- [ ] **C)** It reduces the risk of noisy neighbor problems
- [ ] **D)** It is the default and most cost-effective option

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> The dedicated model provides dedicated resources per tenant, reducing noisy neighbor risk. The shared model uses logical isolation on shared resources and is more cost-effective; dedicated is not default.
 
 
</details>

### 15. The code block shows a fragment of an AXP orchestration flow. What action does the flow likely perform after this node?

```json
{
  "type": "Transfer",
  "target": "skill",
  "params": {
    "skillName": "Claims_Intake",
    "context": "policyNumber"
  }
}
```

- [ ] **A)** Invoke an AI service to classify user utterance
- [ ] **B)** Transfer the interaction to an Engagement Center skill
- [ ] **C)** Play a prompt and collect DTMF input
- [ ] **D)** Log a session variable to the ELK stack

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The JSON shows a 'Transfer' node with a 'skill' parameter, which is how orchestration directs an interaction to an Engagement Center skill for agent assignment. AI invocation would use an 'InvokeAI' node; prompts/collect are different nodes.
 
 
</details>


---

### **Automation and Workflow Design**

### 16. In AXP Composer, which flow type is designed for synchronous, real-time telephony interactions?

- [ ] **A)** Digital Flow
- [ ] **B)** Voice Flow
- [ ] **C)** Hybrid Flow
- [ ] **D)** Chat Flow

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Voice flows handle synchronous telephony interactions such as IVR menus, while digital flows handle asynchronous events like chat.
 
 
</details>

### 17. Which of the following are valid components in AXP Composer? (Select two)

- [ ] **A)** Play Audio
- [ ] **B)** Send Message
- [ ] **C)** Play Video
- [ ] **D)** Get DTMF

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> AXP Composer includes Play Audio (voice), Send Message (digital), and Get DTMF (voice) nodes. Play Video is not a standard node.
 
 
</details>

### 18. Given the following flow configuration, what is the purpose of the 'error' path in the REST node?

```plaintext
REST Profile: GET /api/account, Success -> Set Variable, Error -> Log Error and End
```

- [ ] **A)** Redirect to another REST call
- [ ] **B)** Handle failures gracefully
- [ ] **C)** Skip the step if error occurs
- [ ] **D)** Repeat the call automatically

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The error path allows the flow to execute fallback actions when the REST call fails, preventing abrupt termination.
 
 
</details>

### 19. In a Switch node, what is the recommended practice to handle input values that do not match any defined case?

- [ ] **A)** Omit a default branch
- [ ] **B)** Add a default branch
- [ ] **C)** Use multiple Switch nodes
- [ ] **D)** Ignore the input

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A default branch ensures unhandled inputs are caught gracefully, preventing flow termination.
 
 
</details>

### 20. Which of the following are valid data mapping techniques in AXP workflows? (Select two)

- [ ] **A)** One-to-one field copy
- [ ] **B)** Transform using JavaScript
- [ ] **C)** Hard-code values in each node
- [ ] **D)** Use XSLT for XML transformation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Data mapping can be done via direct mapping, JavaScript transformers, or XSLT for XML. Hard-coding is not a dynamic technique.
 
 
</details>

### 21. What type of node is represented by this code snippet in AXP Composer?

```javascript
if (language == 'es') { branch_to_spanish; } else { branch_to_english; }
```

- [ ] **A)** Switch node
- [ ] **B)** Set Variable
- [ ] **C)** REST Profile
- [ ] **D)** Log node

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Conditional branching logic like if-else is implemented using the Switch node in AXP.
 
 
</details>

### 22. Which authentication method is recommended for integrating AXP with external AI services like Dialogflow?

- [ ] **A)** Basic Auth
- [ ] **B)** API Key with OAuth2
- [ ] **C)** No authentication
- [ ] **D)** SAML

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> OAuth2 client credentials flow is the standard secure method for API access. Basic auth is insecure and deprecated.
 
 
</details>


---

### **Deployment and Lifecycle Management**

### 23. Which deployment slots are available in AXP?

- [ ] **A)** Staging and production
- [ ] **B)** Dev, staging, and production
- [ ] **C)** Test and production
- [ ] **D)** Staging only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AXP provides staging for validation and production for live traffic. No 'dev' slot exists.
 
 
</details>

### 24. Which of the following are valid AXP CLI commands? (Select two)

- [ ] **A)** axp deploy --slot staging
- [ ] **B)** axp app version create
- [ ] **C)** axp app start --app-id
- [ ] **D)** axp config set --api-token

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Valid commands: axp deploy and axp app version create. 'start' is not a command; config set is for setup but not a deployment command.
 
 
</details>

### 25. What is the effect of the command in the code block?

```bash
axp deploy --slot staging --version 1.0.0 --app-id APP123
```

- [ ] **A)** Deploys version 1.0.0 to staging
- [ ] **B)** Promotes version 1.0.0 to production
- [ ] **C)** Rolls back to previous version
- [ ] **D)** Creates a new application version

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command deploys the specified version to the staging slot as indicated by the --slot staging flag.
 
 
</details>

### 26. What is true about deployed AXP versions?

- [ ] **A)** They cannot be modified after deployment
- [ ] **B)** They can be edited using the CLI
- [ ] **C)** They are automatically deleted after 30 days
- [ ] **D)** They support hot-patching of code

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AXP versions are immutable once deployed; any update requires creating a new version.
 
 
</details>

### 27. Which are secure credential storage practices? (Select two)

- [ ] **A)** Use cloud secrets manager
- [ ] **B)** Hardcode in configuration files
- [ ] **C)** Use IAM roles for compute resources
- [ ] **D)** Store in environment variables

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Cloud secrets manager and IAM roles provide secure, auditable credential management. Hardcoding and env vars are insecure.
 
 
</details>


---

### **Troubleshooting and Optimization**

### 28. What HTTP status code indicates that an OAuth 2.0 access token has expired?

- [ ] **A)** 401 Unauthorized
- [ ] **B)** 403 Forbidden
- [ ] **C)** 429 Too Many Requests
- [ ] **D)** 502 Bad Gateway

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A 401 status code indicates missing or invalid authentication, such as an expired token.
 
 
</details>

### 29. Which of the following are features of the AXP debug CLI utility? (Select all that apply)

- [ ] **A)** Connect to running containers
- [ ] **B)** Dump thread states
- [ ] **C)** Analyze heap memory
- [ ] **D)** Deploy code patches

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> axp-debug allows attaching a debugger, dumping threads, and analyzing heap, but not deploying patches.
 
 
</details>

### 30. Examine the cURL command for refreshing an OAuth token. Which value should replace 'REFRESH'?

```bash
curl -X POST https://auth.avaya.com/oauth/token -d "grant_type=REFRESH&refresh_token=abc&client_id=xyz" -H "Content-Type: application/x-www-form-urlencoded"
```

- [ ] **A)** grant_type=refresh_token
- [ ] **B)** grant_type=authorization_code
- [ ] **C)** grant_type=client_credentials
- [ ] **D)** grant_type=password

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The OAuth 2.0 refresh token grant requires grant_type=refresh_token.
 
 
</details>

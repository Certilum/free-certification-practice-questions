<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Salesforce/Salesforce%20Certified%20System%20Architect.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Salesforce Certified System Architect</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Data Modeling and Management](#data-modeling-and-management) (7 questions)
- [Identity and Access Management](#identity-and-access-management) (7 questions)
- [Integration Architecture](#integration-architecture) (8 questions)
- [Platform Development Lifecycle and Deployment](#platform-development-lifecycle-and-deployment) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:47:35.084Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Data Modeling and Management | 7 |
| Identity and Access Management | 7 |
| Integration Architecture | 8 |
| Platform Development Lifecycle and Deployment | 8 |

---

### **Data Modeling and Management**

### 1. In a Salesforce integration architecture, which API protocol is optimized for high-volume, asynchronous data processing to avoid synchronous timeout constraints?

- [ ] **A)** Bulk API
- [ ] **B)** REST API
- [ ] **C)** SOAP API
- [ ] **D)** Metadata API

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Bulk API is designed for large data volumes and asynchronous processing, avoiding synchronous timeout constraints that commonly affect REST or SOAP callouts.
 
 
</details>

### 2. Which two characteristics are associated with SOAP API when compared to REST for Salesforce web service integrations? (Choose two.)

- [ ] **A)** Strictly typed XML payloads
- [ ] **B)** Lightweight JSON by default
- [ ] **C)** Transactional integrity
- [ ] **D)** Stateless and cacheable

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> SOAP is strictly typed and XML-based, and supports transactional integrity. REST is lightweight and stateless, so those are not SOAP characteristics.
 
 
</details>

### 3. Review the Apex code block in the interactive panel. Which type of HTTP integration behavior is being executed by this Salesforce code?

```apex
HttpRequest req = new HttpRequest();
req.setEndpoint('https://api.example.com/verify');
req.setMethod('POST');
Http http = new Http();
HttpResponse res = http.send(req);
```

- [ ] **A)** Synchronous callout
- [ ] **B)** Queueable asynchronous job
- [ ] **C)** Platform Event publish
- [ ] **D)** Batch Apex chunk

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code uses HttpRequest and Http.send, which blocks until a response returns; therefore it represents a synchronous callout.
 
 
</details>

### 4. Which OAuth 2.0 flow should an architect select for a server-to-server Salesforce integration that must run without any end-user interaction?

- [ ] **A)** JWT Bearer flow
- [ ] **B)** User-Agent flow
- [ ] **C)** Authorization Code flow
- [ ] **D)** Password Grant

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> JWT Bearer flow uses a digital certificate and private key for machine-to-machine authentication with no user interaction.
 
 
</details>

### 5. Which two benefits does asynchronous processing provide in a Salesforce integration architecture compared with synchronous transactions? (Choose two.)

- [ ] **A)** Higher governor limits
- [ ] **B)** Immediate user-visible error messages
- [ ] **C)** Improved overall throughput
- [ ] **D)** Lower latency for a single transaction

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Asynchronous processing offers higher governor limits and improves overall throughput, while synchronous processing provides lower latency and immediate errors.
 
 
</details>

### 6. Examine the Apex code block shown in the panel. What type of Salesforce event is being published by the EventBus.publish call?

```apex
EventBus.publish(new Order_Event__c(Status__c = 'Shipped'));
```

- [ ] **A)** Platform Event
- [ ] **B)** Change Data Capture event
- [ ] **C)** Custom Object
- [ ] **D)** Task

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> EventBus.publish indicates a Platform Event being published. Change Data Capture fires automatically on record changes, not through this statement.
 
 
</details>

### 7. In Salesforce API governance, what mechanism should an integration design use to handle '429 Too Many Requests' errors gracefully?

- [ ] **A)** Retry logic and circuit breakers
- [ ] **B)** Increasing synchronous timeout
- [ ] **C)** Removing OAuth scopes
- [ ] **D)** Converting to synchronous calls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Retry logic with circuit breakers handles 429 responses gracefully by backing off and avoiding retry storms that worsen API limits.
 
 
</details>


---

### **Identity and Access Management**

### 8. Which API type is designed for high-volume, asynchronous data processing to avoid synchronous timeout limits?

- [ ] **A)** REST API
- [ ] **B)** SOAP API
- [ ] **C)** Bulk API
- [ ] **D)** Event Bus

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Bulk API processes high volumes asynchronously. REST and SOAP are synchronous and cannot handle massive datasets without timeout constraints.
 
 
</details>

### 9. Which two governance techniques are used to handle '429 Too Many Requests' errors gracefully in API integrations?

- [ ] **A)** Designing retry logic
- [ ] **B)** Implementing circuit breakers
- [ ] **C)** Creating more SOAP endpoints
- [ ] **D)** Disabling OAuth scopes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> API governance uses retries and circuit breakers to handle rate-limit errors, preserving platform stability and preventing request overload.
 
 
</details>

### 10. Examine the Apex code snippet. Which asynchronous processing style is shown in the code block?

```apex
public class ExternalSync {
    @future(callout=true)
    public static void sendInventoryUpdate() {
        System.debug('Sending update');
    }
}
```

- [ ] **A)** Future method
- [ ] **B)** Queueable
- [ ] **C)** Batch Apex
- [ ] **D)** Scheduled Apex

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The @future(callout=true) annotation marks a future method that runs asynchronously for outbound callouts.
 
 
</details>

### 11. Which OAuth 2.0 flow uses a digital certificate to establish trust for server-to-server integration?

- [ ] **A)** JWT Bearer Flow
- [ ] **B)** User-Agent Flow
- [ ] **C)** Authorization Code Flow
- [ ] **D)** Password Grant

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> JWT Bearer flow uses a certificate-based digital signature, making it ideal for trusted server-to-server automation.
 
 
</details>

### 12. Which two communication channels are recommended to alert administrators when an asynchronous process fails after the caller has disconnected?

- [ ] **A)** Email
- [ ] **B)** Custom Log object
- [ ] **C)** Toast notification
- [ ] **D)** Synchronous Debug log

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Because users do not see errors in async flows, architects should use Email or Custom Log objects as secondary notification channels.
 
 
</details>

### 13. Analyze the HTTP request in the code block. Which OAuth 2.0 grant type is being used?

```http
POST /services/oauth2/token HTTP/1.1
Host: login.salesforce.com
Content-Type: application/x-www-form-urlencoded

client_id=3MVG9xLxYb8example&client_secret=ABC123
```

- [ ] **A)** Client Credentials
- [ ] **B)** Authorization Code
- [ ] **C)** JWT Bearer
- [ ] **D)** Password Grant

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A request presenting only client credentials, with no redirect_uri or user identity, indicates the client credentials grant.
 
 
</details>

### 14. In Salesforce, what architectural component acts as the gateway for external applications to request OAuth access?

- [ ] **A)** Connected App
- [ ] **B)** API Gateway
- [ ] **C)** Platform Event
- [ ] **D)** Event Bus

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Connected App is the OAuth configuration that lets architects set scopes, IP restrictions, and required permissions for integrations.
 
 
</details>


---

### **Integration Architecture**

### 15. Which API protocol is specifically designed to process massive data volumes asynchronously without hitting synchronous timeout limits?

- [ ] **A)** REST API
- [ ] **B)** SOAP API
- [ ] **C)** Bulk API
- [ ] **D)** Metadata API

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Bulk APIs are built for high-volume asynchronous data processing, while REST and SOAP are synchronous and can timeout on large datasets.
 
 
</details>

### 16. Which two characteristics are true of SOAP-based integration? Choose two.

- [ ] **A)** XML-based message format
- [ ] **B)** Lightweight and stateless
- [ ] **C)** Strictly typed contracts
- [ ] **D)** Built for massive asynchronous workloads

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> SOAP relies on XML, enforces strict typing, and supports transactional integrity; it is not lightweight or asynchronous bulk-oriented.
 
 
</details>

### 17. The code block shows a token request. What does the grant_type indicate about this integration?

```http
grant_type=client_credentials&client_id=3MVG9x&client_secret=XXXX
```

- [ ] **A)** A server-to-server integration with no user context
- [ ] **B)** A client-side user-agent flow
- [ ] **C)** A JWT bearer flow using a certificate
- [ ] **D)** An authorization code flow with user login

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Client credentials is a machine-to-machine flow; authorization code and user-agent involve users, while JWT uses a certificate.
 
 
</details>

### 18. Which OAuth flow is the gold standard for automated server-to-server integration when a digital certificate is required?

- [ ] **A)** JWT Bearer Flow
- [ ] **B)** User-Agent Flow
- [ ] **C)** Authorization Code Flow
- [ ] **D)** Password Grant

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> JWT Bearer Flow uses a private key/certificate for server-to-server trust and requires no user interaction.
 
 
</details>

### 19. Which two Salesforce-native tools can be used to publish events for an event-driven integration? Choose two.

- [ ] **A)** Platform Events
- [ ] **B)** Change Data Capture
- [ ] **C)** Enterprise Service Bus
- [ ] **D)** Connected App

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Platform Events are custom event objects, and Change Data Capture publishes record-change events on the Salesforce Event Bus.
 
 
</details>

### 20. The Apex class in the code block is queued for asynchronous execution. What primary advantage does this offer over running the same work synchronously in a trigger?

```apex
public class HeavyCalculation implements Queueable {
    public void execute(QueueableContext context) {
        // simulate long-running calculation
    }
}
```

- [ ] **A)** It provides higher governor limits than a synchronous transaction
- [ ] **B)** It guarantees the calculation finishes before the transaction commits
- [ ] **C)** It removes the need for any exception handling
- [ ] **D)** It automatically tells the user the result in real time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Queueable runs outside the user transaction and gets higher limits, preventing CPU and timeout failures.
 
 
</details>

### 21. Which integration architecture centralizes message routing, data transformation, and protocol conversion between systems?

- [ ] **A)** Enterprise Service Bus
- [ ] **B)** Data Lake
- [ ] **C)** Change Data Capture
- [ ] **D)** Connected App

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An ESB acts as a centralized hub that provides routing, transformation, and protocol conversion.
 
 
</details>

### 22. When choosing between synchronous and asynchronous integration, which two architectural trade-offs must be considered? Choose two.

- [ ] **A)** Throughput versus latency
- [ ] **B)** Whether the client can remain blocked waiting for a response
- [ ] **C)** The color scheme of the external UI
- [ ] **D)** The need to avoid all database indexes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Synchronous patterns favor low latency and blocking calls; asynchronous patterns favor throughput and non-blocking flows.
 
 
</details>


---

### **Platform Development Lifecycle and Deployment**

### 23. Which API protocol is designed for high-volume asynchronous data processing?

- [ ] **A)** REST API
- [ ] **B)** SOAP API
- [ ] **C)** Bulk API
- [ ] **D)** Streaming API

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Bulk API is optimized for high-volume, asynchronous data processing, avoiding synchronous timeout constraints.
 
 
</details>

### 24. Which two statements accurately describe REST and SOAP API protocols?

- [ ] **A)** REST is lightweight, stateless, and uses JSON.
- [ ] **B)** SOAP provides strict XML typing and transactional integrity.
- [ ] **C)** Bulk API is the preferred protocol for single synchronous record operations.
- [ ] **D)** REST is always the most efficient choice for massive datasets.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> REST uses stateless JSON, while SOAP relies on strict XML and transactional integrity. Bulk API is needed for massive datasets.
 
 
</details>

### 25. Review the Apex code block. Which asynchronous mechanism is being used?

```apex
public class MyAsyncJob implements Queueable {
    public void execute(QueueableContext context) {
        System.debug('Running async job');
    }
}
```

- [ ] **A)** Queueable Apex
- [ ] **B)** Batch Apex
- [ ] **C)** Scheduled Apex
- [ ] **D)** Future Method

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The class implements the Queueable interface and its execute method, so Queueable Apex is used.
 
 
</details>

### 26. Which OAuth 2.0 flow is designed for high-security server-to-server integration using a digital certificate?

- [ ] **A)** User-Agent Flow
- [ ] **B)** JWT Bearer Flow
- [ ] **C)** Authorization Code Flow
- [ ] **D)** Password Grant

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> JWT Bearer Flow is for server-to-server integration, using a private key or certificate to establish trust without user interaction.
 
 
</details>

### 27. Which two statements correctly distinguish OAuth 2.0 grant types in Salesforce integrations?

- [ ] **A)** Authorization Code is for user-delegated access.
- [ ] **B)** Client Credentials is for system-to-system access.
- [ ] **C)** Password Grant is the recommended modern integration flow.
- [ ] **D)** JWT Bearer relies only on a client secret for trust.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Authorization Code delegates on behalf of a user, while Client Credentials supports system-to-system access. Password Grant and secret-only JWT are not best practices.
 
 
</details>

### 28. Given the Apex trigger in the code block, which Salesforce event mechanism is being published?

```apex
trigger AccountAfterInsert on Account (after insert) {
    List<Account_Change__e> events = new List<Account_Change__e>();
    for (Account acc : Trigger.new) {
        events.add(new Account_Change__e(Account_Id__c = acc.Id));
    }
    EventBus.publish(events);
}
```

- [ ] **A)** Platform Event
- [ ] **B)** Change Data Capture
- [ ] **C)** Outbound Message
- [ ] **D)** Custom Notification

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The trigger creates a custom Platform Event object and publishes it via EventBus.publish.
 
 
</details>

### 29. Which asynchronous Apex mechanism is implemented by implementing the Queueable interface and calling System.enqueueJob?

- [ ] **A)** Queueable Apex
- [ ] **B)** Batch Apex
- [ ] **C)** Future Method
- [ ] **D)** Scheduled Apex

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A class implementing Queueable and submitted with System.enqueueJob uses Queueable Apex, which offloads processing and provides higher limits.
 
 
</details>

### 30. Which two statements about asynchronous processing are true in Salesforce architecture?

- [ ] **A)** Asynchronous patterns optimize for high throughput.
- [ ] **B)** Asynchronous errors can be handled immediately in the user's session.
- [ ] **C)** Asynchronous processing provides higher governor limits than synchronous processing.
- [ ] **D)** The client remains blocked until the asynchronous call completes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Async optimizes throughput and provides higher limits; errors are not visible to the user and require separate logging and retry mechanisms.
 
 
</details>

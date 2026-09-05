<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Salesforce/Salesforce%20Certified%20Integration%20Architecture%20Designer.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Salesforce Certified Integration Architecture Designer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Build Solution](#build-solution) (7 questions)
- [Design Integration Solutions](#design-integration-solutions) (8 questions)
- [Evaluate Business Needs](#evaluate-business-needs) (3 questions)
- [Identity and Access Management](#identity-and-access-management) (5 questions)
- [Translate Needs to Integration Requirements](#translate-needs-to-integration-requirements) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:47:22.289Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Build Solution | 7 |
| Design Integration Solutions | 8 |
| Evaluate Business Needs | 3 |
| Identity and Access Management | 5 |
| Translate Needs to Integration Requirements | 7 |

---

### **Build Solution**

### 1. According to integration architecture best practices, which execution pattern should be used to avoid the 10-second synchronous timeout limit?

- [ ] **A)** Asynchronous patterns
- [ ] **B)** Synchronous callouts
- [ ] **C)** REST API polling
- [ ] **D)** Manual Apex triggers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Asynchronous patterns such as @future, Queueable, or Batch Apex are preferred for long-running processes to avoid the 10-second synchronous timeout limit.
 
 
</details>

### 2. Which Apex mechanisms can be used to perform asynchronous callouts in a Salesforce integration? Select all that apply.

- [ ] **A)** @future
- [ ] **B)** Queueable
- [ ] **C)** Batch Apex
- [ ] **D)** Synchronous Apex

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> @future, Queueable, and Batch Apex are asynchronous mechanisms. Synchronous Apex executes in the immediate context and can hit timeout limits.
 
 
</details>

### 3. The Apex trigger in the code block tries to perform a callout. What integration trap is being demonstrated?

```apex
trigger AccountTrigger on Account (after insert) {
    Http http = new Http();
    HttpRequest req = new HttpRequest();
    req.setEndpoint('https://api.example.com/account');
    req.setMethod('GET');
    HttpResponse res = http.send(req);
}
```

- [ ] **A)** Callout in a trigger without asynchronous wrapper
- [ ] **B)** Heap size explosion
- [ ] **C)** Named Credential missing
- [ ] **D)** Using Platform Events for validation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A callout directly inside a trigger execution context is forbidden; it must be wrapped in @future, Queueable, or Batch Apex.
 
 
</details>

### 4. Which limit error is associated with parsing a massive JSON response in a single synchronous transaction?

- [ ] **A)** Apex heap size exceeded
- [ ] **B)** SocketTimeoutException
- [ ] **C)** System.CalloutException
- [ ] **D)** QueryException

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Parsing large JSON payloads in one synchronous transaction can cause LimitException: Apex heap size exceeded.
 
 
</details>

### 5. Which strategies should an architect use to create a resilient HTTP callout process in an integration design?

- [ ] **A)** Handling 4xx and 5xx status codes
- [ ] **B)** Implementing exponential backoff
- [ ] **C)** Using Platform Events to signal failed integration attempts
- [ ] **D)** Ignoring server errors

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Resilient callouts handle HTTP error codes, retry with exponential backoff, and can use Platform Events to trigger reprocessing of failures.
 
 
</details>

### 6. In the Apex code block, what does the named endpoint reference in the HTTP request?

```apex
HttpRequest req = new HttpRequest();
req.setEndpoint('callout:MyExternalSystem');
req.setMethod('GET');
Http http = new Http();
HttpResponse res = http.send(req);
```

- [ ] **A)** A Named Credential abstraction
- [ ] **B)** A raw external URL
- [ ] **C)** A Platform Event channel
- [ ] **D)** A Queueable job name

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Named Credential abstracts the endpoint and authentication details, allowing Apex to reference it with the callout: prefix.
 
 
</details>

### 7. Which protocol does Change Data Capture use to stream object changes from Salesforce to external subscribers?

- [ ] **A)** CometD
- [ ] **B)** SOAP
- [ ] **C)** REST
- [ ] **D)** Bulk API

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CDC uses the CometD protocol for long-polling, enabling Salesforce to act as event producer for external subscribers.
 
 
</details>


---

### **Design Integration Solutions**

### 8. What is the primary characteristic of a synchronous integration callout?

- [ ] **A)** Blocks the UI until the callout completes
- [ ] **B)** Runs in the background with @future
- [ ] **C)** Always uses Platform Events
- [ ] **D)** Cannot connect to external systems

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Synchronous callouts block the current transaction until they finish. They are limited by the 10-second timeout and should not be used for long-running operations.
 
 
</details>

### 9. Which options are supported asynchronous callout mechanisms in Apex? Select all that apply.

- [ ] **A)** @future methods
- [ ] **B)** Queueable Apex
- [ ] **C)** Batch Apex
- [ ] **D)** Synchronous REST callout

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Apex provides @future, Queueable, and Batch Apex for asynchronous callouts. Synchronous REST callouts execute in the original request context.
 
 
</details>

### 10. Review the code block. Which integration trap is illustrated?

```apex
trigger AccountTrigger on Account (after insert) {
    HttpRequest req = new HttpRequest();
    req.setEndpoint('https://api.example.com/account');
    req.setMethod('POST');
    Http http = new Http();
    HttpResponse res = http.send(req);
}
```

- [ ] **A)** Trigger Callout Error
- [ ] **B)** Timeout Oversight
- [ ] **C)** Heap Size Explosion
- [ ] **D)** Authentication Failure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A callout directly inside a trigger is not allowed. It must be wrapped in an asynchronous mechanism such as @future or Queueable Apex.
 
 
</details>

### 11. What is the synchronous callout timeout limit in Salesforce?

- [ ] **A)** 10 seconds
- [ ] **B)** 30 seconds
- [ ] **C)** 60 seconds
- [ ] **D)** 120 seconds

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Salesforce enforces a 10-second timeout for synchronous callouts. Longer-running work should use asynchronous Apex patterns.
 
 
</details>

### 12. Which two callout governance practices help avoid Salesforce limit exceptions?

- [ ] **A)** Set explicit HTTP timeouts
- [ ] **B)** Monitor heap size for response payloads
- [ ] **C)** Ignore the response body size
- [ ] **D)** Raise the callout limit per transaction

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Setting timeouts and watching heap usage keep integrations within platform constraints. Callout limits cannot be changed by the architect.
 
 
</details>

### 13. Analyze the code block. Which trap is it most likely to cause?

```apex
String payload = response.getBody();
List<Object> records = (List<Object>) JSON.deserializeUntyped(payload);
```

- [ ] **A)** Heap Size Explosion
- [ ] **B)** Trigger Callout Error
- [ ] **C)** Timeout Oversight
- [ ] **D)** Named Credential Misconfiguration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Deserializing a very large JSON response into memory can quickly exceed the Apex heap limit and throw LimitException.
 
 
</details>

### 14. What should an architect use to securely abstract callout authentication?

- [ ] **A)** Named Credentials
- [ ] **B)** Custom Labels
- [ ] **C)** Static Resources
- [ ] **D)** Remote Site Settings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Named Credentials abstract authentication and help manage OAuth flows securely. They avoid exposing credentials in Apex code.
 
 
</details>

### 15. Which two strategies improve error handling and retry logic for integrations?

- [ ] **A)** Implement exponential backoff on retries
- [ ] **B)** Use Platform Events to flag failed attempts
- [ ] **C)** Disable timeouts to avoid errors
- [ ] **D)** Log credentials for debugging

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Exponential backoff prevents retry storms, and Platform Events can signal failures for later processing. Disabling timeouts or logging credentials is unsafe.
 
 
</details>


---

### **Evaluate Business Needs**

### 16. In Salesforce integration architecture, which action represents the trap known as the Trigger Callout Error?

- [ ] **A)** Callout in @future method
- [ ] **B)** Direct callout in trigger without async wrapper
- [ ] **C)** Callout in Queueable Apex
- [ ] **D)** Callout in Batch Apex

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The playbook identifies direct callouts in a trigger with no asynchronous wrapper as the Trigger Callout Error trap. The recommended alternatives are @future, Queueable, and Batch Apex.
 
 
</details>

### 17. According to the playbook, which two benefits does event-driven decoupling provide in system integration architecture?

- [ ] **A)** Reduces latency in the primary transaction
- [ ] **B)** Prevents cascading failures if downstream system unavailable
- [ ] **C)** Guarantees immediate synchronous responses
- [ ] **D)** Removes the need for replay identifiers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The playbook states event-driven decoupling reduces latency in the primary transaction and prevents cascading failures when a downstream system is temporarily unavailable. It does not guarantee synchronous responses or remove replay requirements.
 
 
</details>

### 18. Review the provided Apex code snippet. Which Salesforce integration architecture trap does the trigger implementation demonstrate?

```apex
trigger AccountTrigger on Account (after insert) {
    for (Account acc : Trigger.new) {
        Http http = new Http();
        HttpRequest req = new HttpRequest();
        req.setEndpoint('https://external.service.example.com/api');
        req.setMethod('GET');
        HttpResponse res = http.send(req);
    }
}
```

- [ ] **A)** Trigger Callout Error
- [ ] **B)** Timeout Oversight
- [ ] **C)** Heap Size Explosion
- [ ] **D)** Publish/Subscribe Model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code makes a synchronous HTTP callout directly inside a trigger with no asynchronous wrapper. This matches the Trigger Callout Error trap described in the playbook.
 
 
</details>


---

### **Identity and Access Management**

### 19. Which Salesforce feature abstracts and manages authentication logic for outbound integration callouts?

- [ ] **A)** Named Credentials
- [ ] **B)** Platform Events
- [ ] **C)** Change Data Capture
- [ ] **D)** Flow Orchestration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Named Credentials abstract authentication by storing endpoint URLs and credentials, so Apex callouts do not manage OAuth directly.
 
 
</details>

### 20. Which practices help maintain security when making callouts? Select all that apply.

- [ ] **A)** Using Named Credentials to avoid hard-coded secrets
- [ ] **B)** Ensuring OAuth flows are handled correctly
- [ ] **C)** Preventing sensitive data leakage through secure logging
- [ ] **D)** Storing credentials in Apex classes for reuse

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Named Credentials, correct OAuth handling, and secure logging are security best practices; storing credentials in Apex is unsafe.
 
 
</details>

### 21. The Apex code below represents a known integration anti-pattern. What is the architectural trap?

```apex
trigger AccountTrigger on Account (before insert) {
    HttpRequest req = new HttpRequest();
    req.setEndpoint('https://example.com/api/account');
    req.setMethod('GET');
    Http http = new Http();
    HttpResponse res = http.send(req);
}
```

- [ ] **A)** The Trigger Callout Error
- [ ] **B)** The Timeout Oversight
- [ ] **C)** The Heap Size Explosion
- [ ] **D)** The Publish/Subscribe Misuse

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Performing a callout directly in a trigger without an asynchronous wrapper is the Trigger Callout Error trap.
 
 
</details>

### 22. Which statement best describes the synchronous callout timeout limit in Salesforce?

- [ ] **A)** 10 seconds
- [ ] **B)** 20 seconds
- [ ] **C)** 30 seconds
- [ ] **D)** 5 seconds

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Synchronous callouts must complete within the 10-second timeout limit or they fail with a timeout exception.
 
 
</details>

### 23. Which platform constraints apply to callouts? Select all that apply.

- [ ] **A)** Maximum number of callouts per transaction
- [ ] **B)** Heap size limitations for large payloads
- [ ] **C)** Strictly enforced timeout limits
- [ ] **D)** Automatic callout retries for every error

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Salesforce enforces callout count limits, heap size limits, and timeout limits, but it does not automatically retry every failed callout.
 
 
</details>


---

### **Translate Needs to Integration Requirements**

### 24. What is the primary reason to use asynchronous Apex, such as Queueable or @future, for a long-running callout?

- [ ] **A)** To block the UI until the callout completes
- [ ] **B)** To avoid hitting the 10-second synchronous timeout limit
- [ ] **C)** To automatically increase the heap size for large payloads
- [ ] **D)** To eliminate all platform governor limits

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Asynchronous Apex patterns are preferred for long-running processes because synchronous callouts are subject to a strict 10-second timeout limit. Moving the callout to an asynchronous context prevents the timeout and keeps the UI responsive.
 
 
</details>

### 25. Which two scenarios clearly require an asynchronous integration pattern instead of a synchronous callout?

- [ ] **A)** The external system response may exceed the 10-second timeout
- [ ] **B)** The process is long-running and may exhaust synchronous execution limits
- [ ] **C)** The payload is small and the external API always responds instantly
- [ ] **D)** The callout count remains below the per-transaction limit

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Asynchronous patterns are required when there is a risk of exceeding the synchronous timeout or when long-running work may exhaust execution limits. Small, fast, low-volume callouts do not necessarily require asynchronous handling.
 
 
</details>

### 26. Given the Apex trigger in the code block, which architectural trap does it demonstrate?

```apex
trigger AccountTrigger on Account (after insert) {
    HttpRequest req = new HttpRequest();
    req.setEndpoint('https://api.example.com/accounts');
    req.setMethod('POST');
    Http http = new Http();
    HttpResponse res = http.send(req);
}
```

- [ ] **A)** The Trigger Callout Error
- [ ] **B)** The Timeout Oversight
- [ ] **C)** The Heap Size Explosion
- [ ] **D)** Event-Driven Decoupling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Performing a callout directly inside a trigger execution context is a well-known trap. Callouts inside triggers require an asynchronous wrapper, such as Queueable or @future, to avoid blocking the trigger and risking platform limits.
 
 
</details>

### 27. What is the main benefit of using Named Credentials for integration callouts?

- [ ] **A)** They increase the callout timeout limit
- [ ] **B)** They abstract authentication logic and securely store credentials
- [ ] **C)** They automatically convert JSON responses into Apex objects
- [ ] **D)** They remove the need for any security protocol

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Named Credentials centralize and abstract authentication details, including OAuth flows, so developers do not expose or hard-code credentials in Apex. This is a core security best practice for callouts.
 
 
</details>

### 28. Which two factors are critical when processing a very large JSON response synchronously?

- [ ] **A)** Apex heap size limits
- [ ] **B)** CPU time limits during parsing
- [ ] **C)** The 72-hour replay window
- [ ] **D)** The number of Named Credentials available

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Heap size and CPU time are key limits when deserializing and processing large JSON payloads. Replay windows apply to event streaming, not to synchronous JSON parsing, and Named Credentials are unrelated to payload size.
 
 
</details>

### 29. Which platform limit is most likely to be exceeded when executing the code block in a synchronous transaction?

```apex
String jsonBody = '[{"name":"Account1","fields":{"industry":"Technology","billingCity":"San Francisco"}},{"name":"Account2","fields":{"industry":"Finance","billingCity":"New York"}}]';
List<Object> results = (List<Object>) JSON.deserializeUntyped(jsonBody);
System.debug(results.size());
```

- [ ] **A)** SocketTimeoutException
- [ ] **B)** LimitException: Apex heap size exceeded
- [ ] **C)** CalloutException: Unauthorized endpoint
- [ ] **D)** QueryException: Too many SOQL queries

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Deserializing a massive JSON payload in a single synchronous transaction can quickly exhaust Apex heap memory, resulting in a LimitException for heap size. This is the Heap Size Explosion trap.
 
 
</details>

### 30. What is a key characteristic of Platform Events in an event-driven architecture?

- [ ] **A)** They are only used for synchronous data validation
- [ ] **B)** The publisher broadcasts a state change without waiting for subscriber responses
- [ ] **C)** They guarantee immediate delivery before the transaction commits
- [ ] **D)** They replace Custom Objects for all persistent data storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Platform Events support event-driven decoupling by allowing the publisher to emit an event and continue without waiting. This reduces latency in the primary transaction and prevents cascading failures if downstream systems are unavailable.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CREST/CREST%20Certified%20Tester%20-%20Application%20(CCT%20APP)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Certified Tester - Application</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Application Security Fundamentals](#application-security-fundamentals) (4 questions)
- [Application Security Testing Tools and Techniques](#application-security-testing-tools-and-techniques) (9 questions)
- [Professional Practice and Ethics](#professional-practice-and-ethics) (3 questions)
- [Reporting and Communication](#reporting-and-communication) (4 questions)
- [Web Application Attacks and Exploitation](#web-application-attacks-and-exploitation) (10 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:26.610Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Application Security Fundamentals | 4 |
| Application Security Testing Tools and Techniques | 9 |
| Professional Practice and Ethics | 3 |
| Reporting and Communication | 4 |
| Web Application Attacks and Exploitation | 10 |

---

### **Application Security Fundamentals**

### 1. What is the core principle of 'shifting left' in the Secure Software Development Lifecycle?

- [ ] **A)** Performing all security testing only at the end of development
- [ ] **B)** Integrating security activities early in the development lifecycle
- [ ] **C)** Moving security responsibilities from developers to testers
- [ ] **D)** Implementing security only after a breach occurs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Shifting left means incorporating security early to reduce cost and risk, not postponing it.
 
 
</details>

### 2. Which of the following are integral components of a Secure Software Development Lifecycle (SSDLC)? (Select all that apply)

- [ ] **A)** Threat modeling during design phase
- [ ] **B)** Secure coding standards enforcement
- [ ] **C)** Final stage security review only
- [ ] **D)** Security requirements engineering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> SSDLC integrates security throughout; final-only review is insufficient.
 
 
</details>

### 3. Examine the following code snippet. Which vulnerability does it exhibit?

```java
String query = "SELECT * FROM users WHERE username = '" + userInput + "';";
```

- [ ] **A)** SQL Injection
- [ ] **B)** Cross-Site Scripting (XSS)
- [ ] **C)** Cross-Site Request Forgery (CSRF)
- [ ] **D)** Insecure Deserialization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Concatenating user input directly into a SQL query creates an injection vulnerability.
 
 
</details>

### 4. What does the OWASP Top 10 category 'Broken Authentication' primarily cover?

- [ ] **A)** Authorization and privilege escalation
- [ ] **B)** Session management and credential handling
- [ ] **C)** Input validation and output encoding
- [ ] **D)** Network security and encryption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Broken Authentication involves vulnerabilities in session management and credential handling.
 
 
</details>


---

### **Application Security Testing Tools and Techniques**

### 5. What is the primary purpose of automated vulnerability scanning tools in application security testing?

- [ ] **A)** To completely replace manual penetration testing
- [ ] **B)** To serve as a force multiplier during reconnaissance and discovery phases
- [ ] **C)** To guarantee the discovery of all business logic flaws
- [ ] **D)** To automate the entire exploitation process without human intervention

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Automated scanners are force multipliers, not replacements; they aid in reconnaissance and discovery but miss logic flaws.
 
 
</details>

### 6. Which of the following are common limitations of automated vulnerability scanners? (Select all that apply.)

- [ ] **A)** They produce a high volume of false positives
- [ ] **B)** They can detect business logic flaws effectively
- [ ] **C)** They may miss vulnerabilities without known signatures
- [ ] **D)** They guarantee zero false negatives

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Scanners often generate false positives and miss zero-day or signature-less vulnerabilities; they do not handle logic flaws.
 
 
</details>

### 7. In the context of automated scanning, what does the term 'signature-based detection' refer to?

```plaintext
Example: A scanner sends ' OR '1'='1 to login fields and flags a response containing a database error.
```

- [ ] **A)** Detection based on known vulnerability patterns
- [ ] **B)** Detection based on anomaly analysis of user behavior
- [ ] **C)** Detection based on machine learning models
- [ ] **D)** Detection based on manual code review

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Signature-based detection relies on a database of known vulnerability patterns to identify issues.
 
 
</details>

### 8. What is a false positive in the context of automated vulnerability scanning?

- [ ] **A)** A real vulnerability that the scanner correctly identifies
- [ ] **B)** A vulnerability reported by the scanner that does not actually exist
- [ ] **C)** A vulnerability missed by the scanner
- [ ] **D)** A vulnerability that requires manual intervention to confirm

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A false positive is an incorrect alert where the scanner reports a vulnerability that does not truly exist.
 
 
</details>

### 9. Which of the following are types of application security testing? (Select all that apply.)

- [ ] **A)** Dynamic Application Security Testing (DAST)
- [ ] **B)** Static Application Security Testing (SAST)
- [ ] **C)** Interactive Application Security Testing (IAST)
- [ ] **D)** Random Application Security Testing (RAST)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The standard types are DAST, SAST, and IAST; RAST is not a recognized term.
 
 
</details>

### 10. What is the difference between DAST and SAST?

```plaintext
Example: DAST tool like Burp Suite sends HTTP requests; SAST tool like Checkmarx parses code files.
```

- [ ] **A)** DAST tests running applications externally; SAST analyzes source code internally
- [ ] **B)** DAST requires source code access; SAST does not
- [ ] **C)** DAST is slower than SAST
- [ ] **D)** SAST is always more accurate than DAST

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> DAST scans running applications without source code; SAST analyzes code internally.
 
 
</details>

### 11. Which of the following best describes a limitation of DAST?

- [ ] **A)** It cannot assess code paths not exercised during testing
- [ ] **B)** It can analyze all code paths regardless of execution
- [ ] **C)** It is ideal for finding business logic flaws
- [ ] **D)** It does not require a running application

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> DAST can only test paths that are executed; it misses code not covered during scanning.
 
 
</details>

### 12. Which of the following are true about false negatives in automated scanning? (Select all that apply.)

- [ ] **A)** A false negative is when a real vulnerability is missed
- [ ] **B)** False negatives are more dangerous than false positives
- [ ] **C)** False negatives can be avoided by using multiple tools
- [ ] **D)** False negatives occur when a scanner reports a non-existent vulnerability

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> False negatives miss real vulnerabilities; they are dangerous. Multiple tools reduce but do not eliminate them.
 
 
</details>

### 13. What is the main reason automated scanners can miss business logic flaws?

```plaintext
Example: A scanner may test for SQLi but cannot understand that a user should not be able to modify another user's balance.
```

- [ ] **A)** Scanners lack understanding of the application's intended business flow
- [ ] **B)** Scanners do not have enough time to test all inputs
- [ ] **C)** Scanners are not designed for web applications
- [ ] **D)** Scanners only detect signature-based vulnerabilities

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Scanners cannot interpret business context or multi-step workflows, and are limited to known patterns.
 
 
</details>


---

### **Professional Practice and Ethics**

### 14. What is the primary purpose of the CREST Code of Conduct?

- [ ] **A)** To provide aspirational guidelines without enforcement
- [ ] **B)** To define binding, enforceable standards of professional behaviour
- [ ] **C)** To replace all legal requirements for penetration testers
- [ ] **D)** To limit the technical skills of certified testers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The CREST Code of Conduct is a binding, enforceable framework that governs the behaviour of all CREST members, not merely aspirational guidelines.
 
 
</details>

### 15. Which of the following are principles of the CREST Code of Conduct? (Select all that apply)

- [ ] **A)** Integrity
- [ ] **B)** Objectivity
- [ ] **C)** Profit maximisation
- [ ] **D)** Confidentiality

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> The CREST Code of Conduct includes Integrity, Objectivity, and Confidentiality. Profit maximisation is not a principle.
 
 
</details>

### 16. Consider the following scenario: A tester discovers an out-of-scope server during a penetration test. What should the tester do according to the code of conduct?

```plaintext
// Example: A tester sees a new IP 10.0.1.100 during scanning
// The scope document only lists 10.0.1.0/24 but excludes 10.0.1.100
// The tester must not proceed without authorisation
```

- [ ] **A)** Run a quick scan to check for vulnerabilities
- [ ] **B)** Immediately exploit any easy wins to show value
- [ ] **C)** Stop testing and request a scope change from the client
- [ ] **D)** Ignore the server and continue with in-scope testing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The code requires testers to respect scope boundaries. The correct action is to stop, notify the client, and request a formal scope change.
 
 
</details>


---

### **Reporting and Communication**

### 17. What is the primary audience of an executive summary in a vulnerability report?

- [ ] **A)** Senior management
- [ ] **B)** Developers
- [ ] **C)** IT operations
- [ ] **D)** QA testers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The executive summary targets non-technical senior management to communicate business impact and strategic priorities.
 
 
</details>

### 18. Which two items are essential components of a technical vulnerability description?

- [ ] **A)** Root cause
- [ ] **B)** Personal opinion
- [ ] **C)** Security impact
- [ ] **D)** Developer name

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Root cause and security impact are required for a factual, actionable description. Personal opinion and developer names are inappropriate.
 
 
</details>

### 19. Given the CVSS vector string, what is the Attack Vector value?

```text
CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H
```

- [ ] **A)** Network
- [ ] **B)** Adjacent
- [ ] **C)** Local
- [ ] **D)** Physical

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AV:N stands for Attack Vector: Network, meaning the vulnerability is exploitable remotely over the network.
 
 
</details>

### 20. What does the CVSS severity category 'High' correspond to in scores?

- [ ] **A)** 7.0 – 8.9
- [ ] **B)** 4.0 – 6.9
- [ ] **C)** 9.0 – 10.0
- [ ] **D)** 0.1 – 3.9

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CVSS v3.1 defines High as scores from 7.0 to 8.9 inclusive. Critical is 9.0-10.0, Medium 4.0-6.9.
 
 
</details>


---

### **Web Application Attacks and Exploitation**

### 21. What is the primary defense against SQL injection according to OWASP?

- [ ] **A)** Parameterized queries (prepared statements)
- [ ] **B)** Input blacklisting
- [ ] **C)** Client-side input validation
- [ ] **D)** Web application firewall only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Parameterized queries treat user input as data, not executable code, preventing SQL injection. OWASP recommends this as primary defense.
 
 
</details>

### 22. Which of the following are types of SQL injection? (Choose two)

- [ ] **A)** Error-based SQLi
- [ ] **B)** Blind SQLi (boolean-based)
- [ ] **C)** HTML injection
- [ ] **D)** LDAP injection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Error-based and blind (boolean/time-based) are two main SQL injection types. HTML and LDAP are separate injection categories.
 
 
</details>

### 23. Analyze the code snippet. What type of injection vulnerability exists?

```java
String query = "SELECT * FROM users WHERE id = '" + request.getParameter("id") + "'";
```

- [ ] **A)** SQL injection
- [ ] **B)** OS command injection
- [ ] **C)** LDAP injection
- [ ] **D)** NoSQL injection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The string concatenation of user input into an SQL query is a classic SQL injection vulnerability.
 
 
</details>

### 24. Which character is commonly used to test for SQL injection in a numeric parameter?

- [ ] **A)** Single quote (')
- [ ] **B)** Double quote (")
- [ ] **C)** A comment delimiter (--)
- [ ] **D)** A number or mathematical expression

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> For numeric parameters, injecting a mathematical expression (e.g., 2-1) tests if input is treated as part of a numeric SQL context.
 
 
</details>

### 25. Which of the following are common XSS variants? (Choose three)

- [ ] **A)** Reflected XSS
- [ ] **B)** Stored XSS
- [ ] **C)** DOM-based XSS
- [ ] **D)** SQLi-based XSS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Reflected, stored, and DOM-based are the three main XSS variants. SQLi-based XSS is not a valid category.
 
 
</details>

### 26. Evaluate the code below. What XSS context does the user input appear in?

```php
<input type="text" value="<?php echo $_GET['input']; ?>" />
```

- [ ] **A)** HTML body
- [ ] **B)** HTML attribute
- [ ] **C)** JavaScript variable
- [ ] **D)** CSS style

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The input is placed inside an HTML attribute (value=\"...\"), requiring breaking out of the attribute with a quote.
 
 
</details>

### 27. What does the HttpOnly flag on a cookie prevent?

- [ ] **A)** Cross-site scripting (access to cookie via JavaScript)
- [ ] **B)** Cross-site request forgery
- [ ] **C)** SQL injection
- [ ] **D)** Session fixation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> HttpOnly prevents client-side scripts from accessing the cookie, mitigating XSS-based cookie theft.
 
 
</details>

### 28. Which of the following are common CSRF mitigation techniques? (Choose two)

- [ ] **A)** Anti-CSRF tokens
- [ ] **B)** SameSite cookie attribute
- [ ] **C)** Client-side JavaScript validation
- [ ] **D)** SSL/TLS encryption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CSRF tokens and SameSite cookies are primary defenses. Client-side validation and TLS do not prevent CSRF.
 
 
</details>

### 29. Examine the CSRF PoC. Which protection is missing?

```html
<form action="https://bank.com/transfer" method="POST">
  <input name="amount" value="1000" />
  <input name="toAccount" value="attacker" />
  <input type="submit" />
</form>
```

- [ ] **A)** Anti-CSRF token
- [ ] **B)** SameSite=Lax cookie
- [ ] **C)** Secure cookie flag
- [ ] **D)** Referer header validation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The form is a standard PoC for CSRF as it submits a state-changing request without any token verification.
 
 
</details>

### 30. What is the typical goal of an SSRF attack?

- [ ] **A)** Internal network resources and cloud metadata
- [ ] **B)** Client-side session cookies
- [ ] **C)** DNS servers
- [ ] **D)** External CDN endpoints

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SSRF tricks the server into making requests to internal systems, cloud metadata endpoints, or otherwise inaccessible resources.
 
 
</details>

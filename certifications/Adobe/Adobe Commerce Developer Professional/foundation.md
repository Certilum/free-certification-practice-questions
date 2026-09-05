<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Adobe/Adobe%20Professional.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Adobe Commerce Developer Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Architecture and Design](#architecture-and-design) (6 questions)
- [Development](#development) (9 questions)
- [Integration](#integration) (3 questions)
- [Performance Optimization](#performance-optimization) (4 questions)
- [Security](#security) (3 questions)
- [Testing and Debugging](#testing-and-debugging) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:43:55.599Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Architecture and Design | 6 |
| Development | 9 |
| Integration | 3 |
| Performance Optimization | 4 |
| Security | 3 |
| Testing and Debugging | 5 |

---

### **Architecture and Design**

### 1. Which Adobe Commerce class is the core utility for preventing Cross-Site Scripting (XSS)?

- [ ] **A)** Escaper
- [ ] **B)** Validator
- [ ] **C)** Session
- [ ] **D)** Crypt

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Escaper class neutralizes output with context-specific methods such as escapeHtml and escapeJs, preventing XSS. It is the fundamental utility used to render data safely in the browser.
 
 
</details>

### 2. What two statements correctly describe input filtering and output escaping?

- [ ] **A)** Input filtering cleans data as it enters the system.
- [ ] **B)** Output escaping neutralizes data when it is rendered in the browser.
- [ ] **C)** Input filtering makes output escaping unnecessary.
- [ ] **D)** Output escaping is only needed for SQL queries.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Both techniques are required for a defense-in-depth strategy. Input filtering cleans incoming data, while output escaping protects the client at render time.
 
 
</details>

### 3. The code block shows a database query using a named placeholder. Which security practice does this illustrate?

```php
$result = $connection->fetchAll('SELECT * FROM customer_entity WHERE entity_id = :id', ['id' => $id]);
```

- [ ] **A)** Parameterized query
- [ ] **B)** String concatenation
- [ ] **C)** Blacklist filtering
- [ ] **D)** Output escaping

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A parameterized query treats user input strictly as data, preventing it from being interpreted as executable SQL.
 
 
</details>

### 4. Which Escaper method should be used to render a variable inside an HTML document?

- [ ] **A)** escapeHtml
- [ ] **B)** escapeJs
- [ ] **C)** escapeCss
- [ ] **D)** escapeAttr

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The escapeHtml method is specifically designed to neutralize values printed in HTML body content, preventing XSS.
 
 
</details>

### 5. Which three contexts are recognized for context-aware sanitization in Adobe Commerce?

- [ ] **A)** HTML body
- [ ] **B)** JavaScript variable
- [ ] **C)** URL parameter
- [ ] **D)** Database table name

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Context-aware sanitization changes based on destination: HTML body, JavaScript variables, and URL parameters each require unique encoding.
 
 
</details>

### 6. The code block processes an untrusted request parameter. Which two security techniques are being used?

```php
$id = (int) $this->getRequest()->getParam('id'); if (!in_array($id, [1, 2, 3], true)) { throw new \Magento\Framework\Exception\LocalizedException(__('Invalid id.')); }
```

- [ ] **A)** Type casting
- [ ] **B)** Whitelisting
- [ ] **C)** Blacklisting
- [ ] **D)** Output escaping

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The parameter is cast to an integer, enforcing a strict data type, and checked against a whitelist of allowed values.
 
 
</details>


---

### **Development**

### 7. In Adobe Commerce, which statement best describes the main purpose of the Escaper class in templates and blocks?

- [ ] **A)** Prevent XSS through context-specific escaping
- [ ] **B)** Prevent SQL injection in custom queries
- [ ] **C)** Manage user session tokens
- [ ] **D)** Encrypt cached product data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Escaper class neutralizes output for contexts such as HTML, JavaScript, CSS, and attributes, preventing XSS attacks.
 
 
</details>

### 8. Which statements correctly describe input filtering and output escaping for defense against XSS in Adobe Commerce?

- [ ] **A)** Input filtering cleans data when it enters the system
- [ ] **B)** Output escaping neutralizes data when it is rendered in the browser
- [ ] **C)** Both techniques are necessary for defense-in-depth against XSS
- [ ] **D)** Validating a field length is sufficient to sanitize it

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Validation only checks constraints; sanitization and escaping are required. Input filtering and output escaping together reduce XSS risks.
 
 
</details>

### 9. The code block renders a variable inside an inline script tag. Which Escaper method should be selected to prevent XSS in that context?

```php
<script>
    var customerEmail = '<?= $block->escapeHtml($block->getCustomerEmail()) ?>';
</script>
```

- [ ] **A)** escapeJs
- [ ] **B)** escapeHtml
- [ ] **C)** escapeUrl
- [ ] **D)** escapeCss

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> JavaScript contexts require escapeJs; escapeHtml does not neutralize characters that are meaningful to JavaScript and can lead to XSS.
 
 
</details>

### 10. What is the recommended way to prevent SQL injection when using the Adobe Commerce Resource Connection in custom code?

- [ ] **A)** Use parameterized queries or prepared statements
- [ ] **B)** Concatenate user input after escaping it
- [ ] **C)** Remove all quote characters from input
- [ ] **D)** Encode input with base64

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Parameterized queries and prepared statements ensure user input is treated strictly as data, preventing SQL injection.
 
 
</details>

### 11. Which statements about OAuth 2.0 and OpenID Connect in Adobe Commerce are correct?

- [ ] **A)** OAuth 2.0 provides authorization through access and refresh tokens
- [ ] **B)** OpenID Connect is an identity layer built on top of OAuth 2.0
- [ ] **C)** OIDC enables client verification of end-user identity for SSO
- [ ] **D)** OAuth 2.0 relies on SAML XML assertions for all token exchange

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> OAuth 2.0 is for authorization, while OpenID Connect adds identity verification for SSO. OAuth does not rely on SAML assertions.
 
 
</details>

### 12. The code block is taken from an Adobe Commerce module configuration. Which type of security resource does this code define?

```xml
<config xmlns:xsi='http://www.w3.org/2001/XMLSchema-instance'>
    <acl>
        <resources>
            <admin>
                <children>
                    <Vendor_Module::config>
                        <title>Custom Module Config</title>
                    </Vendor_Module::config>
                </children>
            </admin>
        </resources>
    </acl>
</config>
```

- [ ] **A)** ACL resource
- [ ] **B)** Route configuration
- [ ] **C)** Database schema
- [ ] **D)** Cron job

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> acl.xml declares resources that map custom module actions into Adobe Commerce's RBAC engine.
 
 
</details>

### 13. In Adobe Commerce security architecture, which question is answered by authentication?

- [ ] **A)** Who the client is
- [ ] **B)** What the client can do
- [ ] **C)** Which resources the client can access
- [ ] **D)** When the client session expires

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Authentication verifies identity; authorization determines permitted actions and resource access.
 
 
</details>

### 14. Which practices are common mistakes when implementing CSRF protection in Adobe Commerce custom code?

- [ ] **A)** Hardcoding form keys or using static tokens
- [ ] **B)** Relying solely on isAllowed() without checking request type
- [ ] **C)** Assuming HTTPS alone prevents CSRF
- [ ] **D)** Using session-bound random form keys

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> CSRF protection depends on session-bound random form keys; static keys, missing request-type checks, and assuming HTTPS are common mistakes.
 
 
</details>

### 15. The code block shows an HTTP response header from Adobe Commerce. Which browser-level CSRF defense is being configured?

```http
Set-Cookie: PHPSESSID=abc123; HttpOnly; SameSite=Lax
```

- [ ] **A)** SameSite Cookie Attribute
- [ ] **B)** Form Key Validation
- [ ] **C)** Content Security Policy
- [ ] **D)** HTTP Strict Transport Security

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SameSite instructs the browser to restrict cookie sending on cross-site requests, adding a layer of CSRF defense.
 
 
</details>


---

### **Integration**

### 16. Which Escaper method is used to neutralize output when a value is rendered inside a JavaScript block?

- [ ] **A)** escapeHtml
- [ ] **B)** escapeJs
- [ ] **C)** escapeCss
- [ ] **D)** escapeUrl

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The escapeJs method is required for JavaScript contexts. Using escapeHtml in JS is not sufficient, and escapeUrl is for URLs, while escapeCss is for stylesheets.
 
 
</details>

### 17. Which two statements correctly describe input filtering and output escaping?

- [ ] **A)** Input filtering cleans data as it enters the system.
- [ ] **B)** Output escaping neutralizes data when it is rendered in the browser.
- [ ] **C)** Output escaping is only needed for GET requests.
- [ ] **D)** Input filtering replaces output escaping in all scenarios.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Input filtering sanitizes data at entry; output escaping neutralizes it at render time. Both layers are part of defense-in-depth; output escaping cannot be replaced by input filtering.
 
 
</details>

### 18. Examine the XML in the code block. What does this ACL resource definition accomplish?

```xml
<config xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="urn:magento:framework:Acl/etc/acl.xsd">
    <acl>
        <resources>
            <resource id="Magento_Sales::sales" title="Sales" sortOrder="10">
                <resource id="Vendor_Module::view_orders" title="View Orders" sortOrder="20" />
            </resource>
        </resources>
    </acl>
</config>
```

- [ ] **A)** Adds a custom ACL resource under Sales.
- [ ] **B)** Creates an admin user role named View Orders.
- [ ] **C)** Creates a new database table for orders.
- [ ] **D)** Removes the Sales resource permission.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The XML declares a child resource under Magento_Sales::sales. This custom ACL resource must be defined before it can be assigned to admin roles.
 
 
</details>


---

### **Performance Optimization**

### 19. What is the primary purpose of the Escaper class in Adobe Commerce?

- [ ] **A)** Prevents XSS by providing context-specific escaping
- [ ] **B)** Validates database queries before execution
- [ ] **C)** Manages user authentication and session tokens
- [ ] **D)** Compresses JavaScript and CSS assets to improve page speed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Escaper class prevents cross-site scripting (XSS) by applying the correct escaping method for the output context, such as HTML, JavaScript, or CSS.
 
 
</details>

### 20. What two options accurately characterize input filtering and output escaping as security measures?

- [ ] **A)** Input filtering cleans data as it enters the system.
- [ ] **B)** Output escaping neutralizes data when it is rendered in the browser.
- [ ] **C)** Output escaping alone is sufficient for a defense-in-depth strategy.
- [ ] **D)** Input filtering should only be applied to stored credit card numbers.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Both techniques are required for defense-in-depth: input filtering cleans incoming data, while output escaping protects data during browser rendering.
 
 
</details>

### 21. The code block renders a variable inside a JavaScript context in a template. Which Escaper method should replace METHOD_NAME?

```php
<script>
    var userInput = '<?= $escaper->METHOD_NAME($userInput) ?>';
</script>
```

- [ ] **A)** escapeJs
- [ ] **B)** escapeHtml
- [ ] **C)** escapeUrl
- [ ] **D)** escapeCss

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Use escapeJs for data rendered inside JavaScript contexts so that script-breaking characters are neutralized.
 
 
</details>

### 22. What is the recommended technique for preventing SQL injection when using the Magento Resource Connection?

- [ ] **A)** Use parameterized queries or prepared statements.
- [ ] **B)** Concatenate user input directly into the SQL string.
- [ ] **C)** Strip or blacklist SQL keywords from the input.
- [ ] **D)** Disable SQL error reporting in production.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Parameterized queries or prepared statements treat user input as data, not executable SQL, preventing SQL injection.
 
 
</details>


---

### **Security**

### 23. Which Escaper class method should be used to safely render a variable in an HTML body context in Adobe Commerce?

- [ ] **A)** escapeHtml()
- [ ] **B)** escapeJs()
- [ ] **C)** escapeCss()
- [ ] **D)** escapeAttribute()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> EscapeHtml is designed for HTML body output. Other methods apply to JavaScript, CSS, and attribute contexts respectively.
 
 
</details>

### 24. Select the two statements that correctly describe input filtering and output escaping in Adobe Commerce.

- [ ] **A)** Input filtering cleans data as it enters the system.
- [ ] **B)** Output escaping neutralizes data as it is rendered in the browser.
- [ ] **C)** Input filtering alone is sufficient if the field length is limited.
- [ ] **D)** Output escaping should only be applied to data entered by administrators.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Input filtering and output escaping both are required. Length limits are validation, not sanitization, and all rendered output needs escaping.
 
 
</details>

### 25. Review the code_block. Which security practice is missing from this Adobe Commerce database query?

```php
<?php
$id = $_GET['id'];
$result = $connection->query("SELECT * FROM catalog_product_entity WHERE entity_id = " . $id);
?>
```

- [ ] **A)** Parameterized query or prepared statement
- [ ] **B)** Output escaping
- [ ] **C)** Form key validation
- [ ] **D)** Input length validation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Concatenating user input into SQL allows injection. Use parameterized queries or prepared statements so input is treated as data only.
 
 
</details>


---

### **Testing and Debugging**

### 26. Which Escaper method should be used to render user input inside a JavaScript block?

- [ ] **A)** escapeHtml()
- [ ] **B)** escapeJs()
- [ ] **C)** escapeCss()
- [ ] **D)** escapeUrl()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> JavaScript context requires escapeJs(); using escapeHtml would not neutralize JavaScript-specific payloads.
 
 
</details>

### 27. Which approaches help prevent SQL injection when using the Adobe Commerce Resource Connection?

- [ ] **A)** Parameterized queries
- [ ] **B)** Prepared statements
- [ ] **C)** Strict type casting and whitelisting
- [ ] **D)** Direct string concatenation of user input

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Parameterized queries and prepared statements treat input as data; type casting and whitelisting reduce malicious input. Direct concatenation creates SQL injection risk.
 
 
</details>

### 28. The PHP template in the code block applies an Escaper method before printing a variable. Which output context is this method designed to protect?

```php
<?php
$userInput = $block->getUserInput();
echo $escaper->escapeJs($userInput);
?>
```

- [ ] **A)** HTML body
- [ ] **B)** JavaScript
- [ ] **C)** CSS
- [ ] **D)** URL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code calls escapeJs(), which is specifically designed for JavaScript contexts.
 
 
</details>

### 29. Which statement best describes output escaping in Adobe Commerce?

- [ ] **A)** Storing data after removing tags
- [ ] **B)** Neutralizing data as it is rendered in the browser
- [ ] **C)** Validating that data fits a maximum length
- [ ] **D)** Encrypting data during transit

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Output escaping handles data at the point of rendering; input filtering and validation happen before storage.
 
 
</details>

### 30. Which protocols are used to verify an end-user's identity for Single Sign-On?

- [ ] **A)** OpenID Connect (OIDC)
- [ ] **B)** SAML
- [ ] **C)** JWT
- [ ] **D)** OAuth 2.0

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OIDC and SAML are identity protocols for SSO. JWT is a token format, and OAuth 2.0 is an authorization framework.
 
 
</details>

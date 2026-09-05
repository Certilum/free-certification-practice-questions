<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Adobe/Adobe%20Certified%20Expert.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Adobe Commerce Developer Expert</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Configuration and Deployment](#configuration-and-deployment) (7 questions)
- [Development](#development) (9 questions)
- [Integration](#integration) (3 questions)
- [Performance and Optimization](#performance-and-optimization) (6 questions)
- [Security](#security) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:43:52.980Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Configuration and Deployment | 7 |
| Development | 9 |
| Integration | 3 |
| Performance and Optimization | 6 |
| Security | 5 |

---

### **Configuration and Deployment**

### 1. What is the immediate consequence if the crypt key stored in app/etc/env.php is lost?

- [ ] **A)** All previously encrypted data becomes unreadable
- [ ] **B)** The system automatically re-encrypts all data with a new key
- [ ] **C)** Only passwords become unrecoverable
- [ ] **D)** Only payment information remains accessible

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The crypt key in env.php is required for all cryptographic operations. Losing it means previously encrypted data cannot be decrypted, while a compromised key exposes the database.
 
 
</details>

### 2. Which session storage backends should be considered for Adobe Commerce production environments that use multiple web nodes?

- [ ] **A)** Redis
- [ ] **B)** Memcached
- [ ] **C)** Local file-based storage on each web node
- [ ] **D)** PHP default session files

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> File-based storage is the default for single-node environments, but multi-node production requires centralized distributed storage such as Redis or Memcached to ensure session consistency.
 
 
</details>

### 3. Review the session cookie configuration shown in the code block. Which flag should be set to true to prevent JavaScript from reading the session ID?

```php
'session' => [
    'save' => 'redis',
    'cookie' => [
        'lifetime' => 86400,
        'path' => '/',
        'domain' => 'example.com',
        'secure' => false,
        'httponly' => false,
        'samesite' => 'Lax'
    ]
]
```

- [ ] **A)** httponly
- [ ] **B)** secure
- [ ] **C)** samesite
- [ ] **D)** lifetime

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The HttpOnly flag prevents JavaScript from accessing the session ID, reducing the risk of session theft via cross-site scripting. The Secure flag is also important, but the specific issue described is JavaScript access.
 
 
</details>

### 4. How does hashing differ from encryption in Adobe Commerce data protection?

- [ ] **A)** Hashing is one-way; the original value is not meant to be recovered
- [ ] **B)** Hashing can be reversed with the same key
- [ ] **C)** Encryption is used for password verification
- [ ] **D)** Hashing and encryption are interchangeable terms

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Hashing is a one-way function used for password verification where the original value is never recovered. Encryption is a two-way process used for data that must be retrieved in its original form.
 
 
</details>

### 5. Which practices align with Adobe Commerce's encryption and key-management security guidance?

- [ ] **A)** Store sensitive field values using application-level encryption through the Encryptor interface
- [ ] **B)** Move the crypt key out of version control
- [ ] **C)** Use the Encryptor to encrypt passwords
- [ ] **D)** Hardcode the crypt key in a module configuration file for portability

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Application-level encryption through the Encryptor interface is the standard implementation, and the crypt key should be environment-based and outside version control. Passwords must not use reversible Encryptor encryption, and hardcoding the key is a known trap.
 
 
</details>

### 6. In the code block, which Encryptor method should replace TODO to encrypt the API key using Adobe Commerce's standard symmetric encryption?

```php
use Magento\Framework\Encryption\EncryptorInterface;

class CustomService
{
    private $encryptor;

    public function __construct(EncryptorInterface $encryptor)
    {
        $this->encryptor = $encryptor;
    }

    public function storeApiKey(string $apiKey): string
    {
        return $this->encryptor->TODO;
    }
}
```

- [ ] **A)** encrypt($apiKey)
- [ ] **B)** hash($apiKey)
- [ ] **C)** mask($apiKey)
- [ ] **D)** regenerate($apiKey)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Magento\\Framework\\Encryption\\EncryptorInterface provides encrypt() to symmetrically encrypt data at rest. Hash, mask, and regenerate are not the correct encryption methods.
 
 
</details>

### 7. What is the purpose of data masking in Adobe Commerce?

- [ ] **A)** It obscures sensitive data in the UI, such as showing only the last four digits
- [ ] **B)** It replaces data with a one-way hash for storage
- [ ] **C)** It uses a public key to encrypt data in the database
- [ ] **D)** It removes sensitive data from the database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Masking obscures sensitive data for display, but it is not encryption. Developers must distinguish between storing data encrypted in the database and displaying it securely in the Admin Panel.
 
 
</details>


---

### **Development**

### 8. What happens to encrypted data if the Crypt Key in `env.php` is lost?

- [ ] **A)** Previously encrypted data becomes unreadable.
- [ ] **B)** Adobe Commerce automatically generates a new key and decrypts the data.
- [ ] **C)** Only the admin password needs to be re-entered.
- [ ] **D)** The data remains readable but cannot be re-encrypted.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The crypt key in env.php is required for all cryptographic operations. Losing it means encrypted data can no longer be decrypted, so it is effectively unreadable.
 
 
</details>

### 9. Which statements correctly describe symmetric encryption in Adobe Commerce?

- [ ] **A)** The same key is used for encryption and decryption.
- [ ] **B)** The `Magento\\Framework\\Encryption\\Encryptor` interface is the standard implementation to use.
- [ ] **C)** It is primarily used for data at rest.
- [ ] **D)** It relies on a public/private key pair.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Symmetric encryption uses one key for both operations. Adobe Commerce's Encryptor interface implements this approach and is mainly used for data at rest. Public/private key pairs are part of asymmetric encryption.
 
 
</details>

### 10. Review the code snippet. Which security flaw is present?

```php
use Magento\Framework\Encryption\EncryptorInterface;

class CustomData
{
    public function __construct(private EncryptorInterface $encryptor) {}

    public function storePassword(string $password): string
    {
        return $this->encryptor->encrypt($password);
    }
}
```

- [ ] **A)** Using reversible encryption for passwords instead of a dedicated password hashing mechanism.
- [ ] **B)** Storing the password in a class property.
- [ ] **C)** Using dependency injection for the Encryptor.
- [ ] **D)** Failing to encode the password with base64.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Passwords must be hashed, not encrypted. Encryptor is for data that must be retrieved later; using reversible encryption for passwords is a major security flaw.
 
 
</details>

### 11. What distinguishes hashing from encryption?

- [ ] **A)** Hashing is one-way; encryption is two-way.
- [ ] **B)** Encryption is one-way; hashing is two-way.
- [ ] **C)** Both are reversible with the same key.
- [ ] **D)** Hashing is used for API credentials; encryption is used for passwords.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Hashing is a one-way function used for verification, while encryption is two-way and allows data to be retrieved in its original form.
 
 
</details>

### 12. Which actions are considered security traps in Adobe Commerce development?

- [ ] **A)** Assuming MySQL-level encryption is enough for Adobe Commerce compliance.
- [ ] **B)** Using the `Encryptor` class to encrypt passwords.
- [ ] **C)** Hardcoding the crypt key in a module configuration file.
- [ ] **D)** Using application-level encryption for sensitive fields.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Developers must apply application-level encryption, use password hashing, and store the crypt key in env.php rather than hardcoding it in configs.
 
 
</details>

### 13. Inspect the configuration snippet. What security issue does it introduce?

```php
return [
    'crypt' => [
        'key' => 'Hardcoded-Crypt-Key-123'
    ]
];
```

- [ ] **A)** The crypt key should be stored in `env.php`, not in a module configuration file.
- [ ] **B)** The key should be a password hash rather than an encryption key.
- [ ] **C)** The key can only contain numeric characters.
- [ ] **D)** The key must be regenerated on every request.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The crypt key belongs in env.php and must not be committed to a module config because hardcoding it exposes the key and breaks environment-based security.
 
 
</details>

### 14. Which session storage solution should be used in a production Adobe Commerce environment with multiple web nodes?

- [ ] **A)** Redis or Memcached
- [ ] **B)** Local file-based storage
- [ ] **C)** Browser local storage
- [ ] **D)** Database-only storage without synchronization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Centralized distributed storage such as Redis or Memcached is required to avoid session inconsistencies across web nodes.
 
 
</details>

### 15. Which cookie flags help mitigate man-in-the-middle attacks on session cookies?

- [ ] **A)** HttpOnly
- [ ] **B)** Secure
- [ ] **C)** SameSite
- [ ] **D)** Domain

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> HttpOnly blocks JavaScript access and Secure restricts the cookie to HTTPS, both reducing MitM risk.
 
 
</details>

### 16. The code snippet sets session cookie metadata. What is misconfigured?

```php
$cookieMetadata = $this->cookieMetadataFactory->createPublicCookieMetadata();
$cookieMetadata->setHttpOnly(false);
$cookieMetadata->setSecure(true);
$cookieMetadata->setPath('/');
```

- [ ] **A)** HttpOnly is disabled, allowing JavaScript to access the cookie.
- [ ] **B)** Secure is enabled when it should be disabled.
- [ ] **C)** The path is not restricted to a secure path.
- [ ] **D)** Public cookies cannot have metadata.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> HttpOnly must be enabled to prevent client-side scripts from accessing the session cookie; disabling it weakens MitM defenses.
 
 
</details>


---

### **Integration**

### 17. What is the primary risk if the encryption key stored in the env.php file is lost?

- [ ] **A)** All previously encrypted data becomes unreadable.
- [ ] **B)** The database automatically creates a new key.
- [ ] **C)** Only the admin password needs to be reset.
- [ ] **D)** The application switches to asymmetric encryption.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The encryption key in env.php is required for all cryptographic operations. If it is lost, encrypted data cannot be decrypted, making it unreadable.
 
 
</details>

### 18. Which statements about session storage in Adobe Commerce are correct? (Select all that apply)

- [ ] **A)** File-based storage is the default backend.
- [ ] **B)** Redis and Memcached are centralized distributed storage options for multi-node environments.
- [ ] **C)** File-based storage is recommended for load-balanced production environments.
- [ ] **D)** Session data is stored in the client-side cookie.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Adobe Commerce uses file-based storage by default. For multiple web nodes, centralized storage like Redis or Memcached is required to maintain session consistency. Session data is stored server-side; only the session ID is in the cookie.
 
 
</details>

### 19. Review the code snippet. Which security principle is being violated?

```php
use Magento\Framework\Encryption\EncryptorInterface;

class CustomService
{
    private $encryptor;

    public function __construct(EncryptorInterface $encryptor)
    {
        $this->encryptor = $encryptor;
    }

    public function storePassword(string $password): string
    {
        return $this->encryptor->encrypt($password);
    }
}
```

- [ ] **A)** Passwords must be hashed, not reversibly encrypted.
- [ ] **B)** The encryptor should not be injected via dependency injection.
- [ ] **C)** The crypt key should be hardcoded in the class.
- [ ] **D)** Symmetric encryption should never be used in custom modules.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Using the Encryptor class for passwords is a trap. Passwords must be protected with a dedicated password hashing mechanism, not reversible encryption.
 
 
</details>


---

### **Performance and Optimization**

### 20. Which sensitive value is stored in the env.php file and required for all cryptographic operations?

- [ ] **A)** Encryption key
- [ ] **B)** Database password
- [ ] **C)** Session storage driver
- [ ] **D)** Cache backend

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The env.php file contains the encryption key used for all cryptographic operations. Losing it makes encrypted data unreadable, and exposing it compromises data security.
 
 
</details>

### 21. Which statements about symmetric encryption in Adobe Commerce are true?

- [ ] **A)** The same key is used for encryption and decryption.
- [ ] **B)** It is the primary method for encrypting data at rest.
- [ ] **C)** Custom modules should use the Magento\\Framework\\Encryption\\Encryptor interface.
- [ ] **D)** It uses a public and private key pair for database fields.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Symmetric encryption uses one shared key for encryption and decryption and is used for data at rest. Adobe Commerce implements it through the Encryptor interface; public and private key pairs are asymmetric.
 
 
</details>

### 22. Review the PHP service snippet. What cryptographic operation is being performed on the provided value?

```php
use Magento\Framework\Encryption\EncryptorInterface;

class SensitiveDataService
{
    public function __construct(
        private EncryptorInterface $encryptor
    ) {
    }

    public function protect(string $value): string
    {
        return $this->encryptor->encrypt($value);
    }
}
```

- [ ] **A)** It encrypts the value using symmetric encryption.
- [ ] **B)** It hashes the value with SHA-256.
- [ ] **C)** It creates a digital signature using a private key.
- [ ] **D)** It validates the value against a whitelist.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The EncryptorInterface is Adobe Commerce's standard implementation for symmetric encryption, used to encrypt data at rest.
 
 
</details>

### 23. Which session cookie flag prevents JavaScript from accessing the session ID?

- [ ] **A)** HttpOnly
- [ ] **B)** Secure
- [ ] **C)** SameSite
- [ ] **D)** Domain

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> HttpOnly prevents client-side scripts from reading the session cookie, reducing the risk of XSS-based session theft.
 
 
</details>

### 24. Which session storage backends are appropriate for a multi-node production environment?

- [ ] **A)** Redis
- [ ] **B)** Memcached
- [ ] **C)** File-based storage
- [ ] **D)** Local memory

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> File-based storage is the default but does not provide shared session state across nodes. Redis and Memcached provide centralized distributed storage for multi-node production.
 
 
</details>

### 25. Look at the configuration file fragment. Which value is critical for cryptographic operations and must be protected from version control?

```php
<?php
return [
    'crypt' => [
        'key' => '326a4a4e2f1c0d9b8a7f6e5d4c3b2a1f'
    ],
    'session' => [
        'save' => 'redis'
    ],
    'cache' => [
        'frontend' => [
            'default' => ['backend' => 'Magento\\Framework\\Cache\\Backend\\Redis']
        ]
    ]
];
```

- [ ] **A)** The crypt key value
- [ ] **B)** The session save value
- [ ] **C)** The cache backend value
- [ ] **D)** The frontend name

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The encryption key in env.php is required for cryptographic operations. Hardcoding or committing it to version control exposes the encrypted database.
 
 
</details>


---

### **Security**

### 26. In which Adobe Commerce file is the encryption key for cryptographic operations stored?

- [ ] **A)** app/etc/env.php
- [ ] **B)** app/etc/config.php
- [ ] **C)** composer.json
- [ ] **D)** auth.json

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The encryption key lives in app/etc/env.php. Losing it makes encrypted data unreadable, and a compromised key can expose the entire database.
 
 
</details>

### 27. Which statements correctly describe hashing and encryption in Adobe Commerce?

- [ ] **A)** Hashing is a one-way function used for password verification
- [ ] **B)** Encryption is a two-way process appropriate for API credentials
- [ ] **C)** The Encryptor class should be used to store passwords
- [ ] **D)** Symmetric encryption uses different keys to encrypt and decrypt

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Hashing is one-way and intended for password verification; encryption is two-way and used for API credentials. Passwords must never be stored with the Encryptor.
 
 
</details>

### 28. The code snippet injects an encryption service and calls its encrypt method. Which category of cryptographic operation does this represent?

```php
use Magento\Framework\Encryption\EncryptorInterface;

class CustomService
{
    private $encryptor;

    public function __construct(EncryptorInterface $encryptor)
    {
        $this->encryptor = $encryptor;
    }

    public function protect(string $value): string
    {
        return $this->encryptor->encrypt($value);
    }
}
```

- [ ] **A)** Symmetric encryption using the same key for encryption and decryption
- [ ] **B)** Asymmetric encryption using a public/private key pair
- [ ] **C)** One-way password hashing
- [ ] **D)** Data masking for UI display

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Encryptor applies symmetric encryption, using the same key for encryption and decryption. This is the standard implementation for custom module data.
 
 
</details>

### 29. Which session storage backend is recommended for Adobe Commerce production environments with multiple web nodes?

- [ ] **A)** File-based session storage on the local web node
- [ ] **B)** Redis or Memcached centralized storage
- [ ] **C)** Browser sessionStorage
- [ ] **D)** Database sessions on the origin server only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> In distributed production environments, file-based storage cannot keep sessions consistent. Redis or Memcached centralizes session data across web nodes.
 
 
</details>

### 30. Which two cookie flags help protect the session identifier from man-in-the-middle attacks?

- [ ] **A)** HttpOnly
- [ ] **B)** Secure
- [ ] **C)** Domain
- [ ] **D)** Path

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> HttpOnly prevents JavaScript access to the session ID, while Secure ensures the cookie is sent only over HTTPS, mitigating MitM attacks.
 
 
</details>

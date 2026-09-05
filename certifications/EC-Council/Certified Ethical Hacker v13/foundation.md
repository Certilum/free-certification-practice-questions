<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/EC-Council/Certified%20Ethical%20Hacker%20v13.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Certified Ethical Hacker v13</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [AI and Machine Learning](#ai-and-machine-learning) (3 questions)
- [Cloud Hacking](#cloud-hacking) (2 questions)
- [Cryptography](#cryptography) (1 questions)
- [Network and Perimeter](#network-and-perimeter) (7 questions)
- [Reconnaissance and Footprinting](#reconnaissance-and-footprinting) (4 questions)
- [Scanning and Enumeration](#scanning-and-enumeration) (4 questions)
- [System Hacking](#system-hacking) (4 questions)
- [Web Application Hacking](#web-application-hacking) (3 questions)
- [Wireless, Mobile and IoT Hacking](#wireless-mobile-and-iot-hacking) (2 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:32.509Z |
| Domains | 9 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| AI and Machine Learning | 3 |
| Cloud Hacking | 2 |
| Cryptography | 1 |
| Network and Perimeter | 7 |
| Reconnaissance and Footprinting | 4 |
| Scanning and Enumeration | 4 |
| System Hacking | 4 |
| Web Application Hacking | 3 |
| Wireless, Mobile and IoT Hacking | 2 |

---

### **AI and Machine Learning**

### 1. In a public key infrastructure, what is the primary responsibility of the Certificate Authority (CA) as the root of trust?

- [ ] **A)** Issues, signs, and manages digital certificates
- [ ] **B)** Verifies identities before certificate issuance
- [ ] **C)** Stores users' private keys in a central database
- [ ] **D)** Provides real-time certificate status checks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CA is the trusted third party that issues, signs, and manages certificates. A compromised CA invalidates the entire security domain and all certificates it issued.
 
 
</details>

### 2. Which two duties are typically assigned to the Registration Authority (RA) during the certificate issuance lifecycle?

- [ ] **A)** Vets certificate requests before issuance
- [ ] **B)** Verifies identity of certificate applicants
- [ ] **C)** Cryptographically signs issued certificates
- [ ] **D)** Maintains the root trust anchor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The RA verifies identities and acts as the administrative vetting layer; it does not sign certificates. Cryptographic signing is performed by the CA.
 
 
</details>

### 3. Based on the code block, which certificate validation mechanism is being used to check whether a specific certificate has been revoked?

```python
cert_id = "serial-123"
status = ocsp_responder.check(cert_id)
if status == "revoked":
    deny_access()
else:
    allow_access()
```

- [ ] **A)** Online Certificate Status Protocol (OCSP)
- [ ] **B)** Certificate Revocation List (CRL)
- [ ] **C)** Registration Authority (RA) vetting
- [ ] **D)** Certificate Authority (CA) signing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code queries an OCSP responder for a single certificate's status. OCSP is real-time and avoids downloading the complete CRL list.
 
 
</details>


---

### **Cloud Hacking**

### 4. Which entity is responsible for issuing and signing digital certificates?

- [ ] **A)** Certificate Authority (CA)
- [ ] **B)** Registration Authority (RA)
- [ ] **C)** Certificate Revocation List (CRL)
- [ ] **D)** Public key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CA is the trusted third-party entity responsible for issuing, signing, and managing digital certificates. The RA verifies identity but does not sign certificates, while CRLs and public keys are not certificate issuers.
 
 
</details>

### 5. Which two statements accurately describe a Certificate Revocation List (CRL)?

- [ ] **A)** Contains certificates revoked before expiration
- [ ] **B)** Updated periodically and cached
- [ ] **C)** Provides real-time status responses
- [ ] **D)** More efficient than OCSP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A CRL is a periodically updated list of revoked certificates. It is not real-time and is generally less efficient than OCSP, which queries a single certificate status on demand.
 
 
</details>


---

### **Cryptography**

### 6. In a public key infrastructure, which entity serves as the trusted third party that issues and signs digital certificates?

- [ ] **A)** Certificate Authority (CA)
- [ ] **B)** Registration Authority (RA)
- [ ] **C)** Online Certificate Status Protocol (OCSP) responder
- [ ] **D)** Certificate Revocation List (CRL) distributor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CA is the root of trust; it issues, signs, and manages digital certificates. The RA only verifies identity, while CRL and OCSP handle revocation status.
 
 
</details>


---

### **Network and Perimeter**

### 7. What is the primary responsibility of a Certificate Authority in a PKI?

- [ ] **A)** Issuing, signing, and managing digital certificates
- [ ] **B)** Verifying the identity of certificate requestors
- [ ] **C)** Generating all users' private keys
- [ ] **D)** Storing private keys on behalf of users

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Certificate Authority is the trusted third-party issuer and manager of digital certificates. The RA handles identity verification, and private key storage is not the CA core role.
 
 
</details>

### 8. Which statements correctly describe the Registration Authority?

- [ ] **A)** Verifies the identity of entities requesting certificates
- [ ] **B)** Signs certificates using the CA's private key
- [ ] **C)** Acts as an intermediary vetting layer before issuance
- [ ] **D)** Performs cryptographic key generation for all certificates

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The RA verifies identities and acts as a vetting layer but does not sign certificates. The CA handles the cryptographic side of issuance.
 
 
</details>

### 9. Examine the provided command. What artifact is being inspected?

```bash
openssl x509 -in certificate.crt -text -noout
```

- [ ] **A)** Digital certificate details
- [ ] **B)** Certificate revocation list
- [ ] **C)** Encrypted private key
- [ ] **D)** OCSP response

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command displays the contents of an X.509 certificate, including identity, public key, expiration, and CA signature.
 
 
</details>

### 10. What is the main purpose of a Certificate Revocation List?

- [ ] **A)** Lists certificates revoked before expiration
- [ ] **B)** Provides real-time certificate status
- [ ] **C)** Signs digital certificates
- [ ] **D)** Encrypts network traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A CRL is a periodically updated list of certificates revoked before their scheduled expiration. Real-time status is provided by OCSP.
 
 
</details>

### 11. Which statements correctly contrast CRL and OCSP?

- [ ] **A)** OCSP provides real-time certificate status
- [ ] **B)** CRL is periodically updated and cached
- [ ] **C)** OCSP requires downloading the full revocation list
- [ ] **D)** CRL provides real-time revocation updates

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> OCSP queries a responder for real-time status of a single certificate, while CRL is cached and periodically updated, making it stale.
 
 
</details>

### 12. What does the command in the code block perform?

```bash
openssl ocsp -issuer ca.crt -cert user.crt -url http://ocsp.example.com
```

- [ ] **A)** Checks real-time revocation status
- [ ] **B)** Downloads the complete revocation list
- [ ] **C)** Creates a new digital certificate
- [ ] **D)** Encrypts the user's private key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This OCSP command queries an OCSP responder to check whether a specific certificate is valid or revoked in real time.
 
 
</details>

### 13. Which key is distributed to other parties through a digital certificate?

- [ ] **A)** Public key
- [ ] **B)** Private key
- [ ] **C)** Symmetric key
- [ ] **D)** Pre-shared key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The certificate distributes the public key, while the private key must never leave the owner's secure storage.
 
 
</details>


---

### **Reconnaissance and Footprinting**

### 14. Which entity acts as the trusted third party that issues, signs, and manages digital certificates?

- [ ] **A)** Certificate Authority
- [ ] **B)** Registration Authority
- [ ] **C)** Certificate Revocation List
- [ ] **D)** Online Certificate Status Protocol

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CA is the trusted third party that issues, signs, and manages certificates. If the CA is compromised, the entire security domain is invalidated.
 
 
</details>

### 15. Which statements correctly describe the Registration Authority (RA)? Select all that apply.

- [ ] **A)** Verifies requester identities
- [ ] **B)** Signs certificates
- [ ] **C)** Vetting layer before issuance
- [ ] **D)** Maintains the CRL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The RA verifies identity and acts as an administrative vetting layer, but it does not sign certificates or maintain CRLs.
 
 
</details>

### 16. Referring to the code block, what certificate field is printed by the script?

```python
from cryptography import x509

with open('server.crt', 'rb') as f:
    cert = x509.load_pem_x509_certificate(f.read())

print(cert.issuer)
```

- [ ] **A)** Subject
- [ ] **B)** Issuer
- [ ] **C)** Serial number
- [ ] **D)** Validity period

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code loads a certificate and prints cert.issuer, which is the issuing CA's identifier.
 
 
</details>

### 17. How does OCSP differ from a Certificate Revocation List (CRL)?

- [ ] **A)** Queries single certificate status
- [ ] **B)** Downloads full revoked list
- [ ] **C)** Updates only once per week
- [ ] **D)** Performs certificate enrollment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OCSP provides real-time, single-certificate status checks, while CRLs are periodically updated lists that can be stale.
 
 
</details>


---

### **Scanning and Enumeration**

### 18. What is the primary responsibility of a Certificate Authority (CA) in a PKI?

- [ ] **A)** Issuing, signing, and managing digital certificates
- [ ] **B)** Verifying identity without signing certificates
- [ ] **C)** Creating private keys for every user
- [ ] **D)** Maintaining a list of common passwords

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Certificate Authority is the trusted third party responsible for issuing, signing, and managing digital certificates. It acts as the root of trust in a PKI.
 
 
</details>

### 19. Which statements correctly describe the role of a Registration Authority (RA)?

- [ ] **A)** It verifies the identity of entities requesting certificates.
- [ ] **B)** It signs certificates before they are issued.
- [ ] **C)** It acts as a vetting layer in the certificate lifecycle.
- [ ] **D)** It is the trusted third-party root of trust.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The Registration Authority verifies identities and acts as the administrative vetting layer, but it does not sign certificates. The Certificate Authority performs cryptographic issuance.
 
 
</details>

### 20. Use the command output to determine which standard defines the digital certificate structure shown.

```bash
openssl x509 -in server.crt -noout -text | grep -E 'Subject:|Issuer:|Public Key Algorithm:|Signature Algorithm:'
```

- [ ] **A)** X.509
- [ ] **B)** PKCS#12
- [ ] **C)** CRL
- [ ] **D)** OCSP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command displays an X.509 certificate's standard fields such as subject, issuer, and public key algorithm.
 
 
</details>

### 21. What is a Certificate Revocation List (CRL)?

- [ ] **A)** A periodically updated list of certificates revoked before their expiration date
- [ ] **B)** A real-time query response for a single certificate status
- [ ] **C)** A list of all trusted root certificates
- [ ] **D)** A digital certificate used to prove ownership of a public key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A CRL is a periodically updated list of certificates revoked early. It is not real-time; OCSP provides real-time status.
 
 
</details>


---

### **System Hacking**

### 22. Which entity is the trusted third-party responsible for issuing, signing, and managing digital certificates?

- [ ] **A)** Certificate Authority
- [ ] **B)** Registration Authority
- [ ] **C)** Certificate Revocation List
- [ ] **D)** Online Certificate Status Protocol

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Certificate Authority is the trusted third-party that issues, signs, and manages digital certificates; compromise of the CA invalidates the security domain.
 
 
</details>

### 23. Which responsibilities are performed by a Registration Authority? Select all that apply.

- [ ] **A)** Verifies the identity of entities requesting certificates
- [ ] **B)** Signs digital certificates using the CA private key
- [ ] **C)** Acts as an intermediary vetting layer before certificate issuance
- [ ] **D)** Maintains the Certificate Revocation List

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The RA handles administrative identity verification and vetting, but it does not sign certificates or maintain the CRL; those duties belong to the CA.
 
 
</details>

### 24. Review the X.509 certificate structure in the code block. Which field most directly proves that the holder owns the public key?

```json
{
  "version": "X.509 v3",
  "serial_number": "0C:82:4E",
  "subject": {
    "common_name": "server.example.com",
    "organization": "Example Inc."
  },
  "public_key_algorithm": "RSA",
  "public_key": "3081 89 02 81 81 00 B2 A4 ...",
  "signature_algorithm": "sha256WithRSAEncryption",
  "issuer": "TrustRoot CA",
  "validity": {
    "not_before": "2024-01-01",
    "not_after": "2025-01-01"
  }
}
```

- [ ] **A)** public_key
- [ ] **B)** signature_algorithm
- [ ] **C)** issuer
- [ ] **D)** validity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The public_key field carries the key itself inside the X.509 certificate, and the certificate is the electronic document used to prove ownership of that public key.
 
 
</details>

### 25. Which mechanism is the primary method for handling digital certificates that have been compromised before their expiration date?

- [ ] **A)** Certificate Revocation List
- [ ] **B)** Registration Authority log
- [ ] **C)** X.509 extension
- [ ] **D)** Digital signature

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A CRL is a periodically updated list of certificates revoked by the CA, normally due to key compromise or affiliation changes.
 
 
</details>


---

### **Web Application Hacking**

### 26. What is the primary responsibility of a Certificate Authority in a public key infrastructure?

- [ ] **A)** Issue, sign, and manage digital certificates
- [ ] **B)** Verify certificate requesters' identities
- [ ] **C)** Provide real-time certificate revocation status
- [ ] **D)** Store users' private keys

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CA issues, signs, and manages certificates. Identity verification before issuance is the RA's role, while OCSP handles real-time status. The CA is the root of trust.
 
 
</details>

### 27. Which statements about CRL and OCSP are correct? Select all that apply.

- [ ] **A)** CRLs are cached and updated periodically
- [ ] **B)** OCSP queries the status of a single certificate in real time
- [ ] **C)** CRL provides faster real-time updates than OCSP
- [ ] **D)** OCSP requires downloading a complete list of revoked certificates

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CRLs are periodically updated, stale lists; OCSP responds in real time for one certificate. Therefore the first two choices are correct.
 
 
</details>

### 28. Analyze the provided code snippet. Which security mechanism is being demonstrated?

```javascript
const digest = hash(message);
const decrypted = decrypt(signature, publicKey);
return digest === decrypted;
```

- [ ] **A)** Digital signature verification
- [ ] **B)** Symmetric encryption
- [ ] **C)** Hash-only integrity check
- [ ] **D)** Certificate revocation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code decrypts the signature with the public key and compares it to the message's hash. This is the standard digital signature verification process.
 
 
</details>


---

### **Wireless, Mobile and IoT Hacking**

### 29. Which trusted third-party entity is responsible for issuing, signing, and managing digital certificates in a typical PKI environment?

- [ ] **A)** Registration Authority
- [ ] **B)** Certificate Authority
- [ ] **C)** Certificate Revocation List
- [ ] **D)** Online Certificate Status Protocol

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The CA issues, signs, and manages digital certificates. RA vets requests but does not sign; CRL and OCSP are status mechanisms.
 
 
</details>

### 30. Which tasks are performed by a Registration Authority before a certificate is issued by the certificate authority?

- [ ] **A)** Verifies identity of certificate requesters
- [ ] **B)** Signs certificates with its own private key
- [ ] **C)** Handles administrative vetting before issuance
- [ ] **D)** Acts as the ultimate root of trust

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The RA verifies identity and handles administrative vetting, but does not sign certificates. The CA signs and is the ultimate root of trust.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Confluent/Confluent%20Certified%20Administrator%20for%20Apache%20Kafka.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Confluent Certified Administrator for Apache Kafka</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Cluster Installation and Configuration](#cluster-installation-and-configuration) (6 questions)
- [Kafka Architecture and Fundamentals](#kafka-architecture-and-fundamentals) (6 questions)
- [Kafka Connect and kDB](#kafka-connect-and-kdb) (4 questions)
- [Operations and Monitoring](#operations-and-monitoring) (6 questions)
- [Performance Tuning and Troubleshooting](#performance-tuning-and-troubleshooting) (3 questions)
- [Security](#security) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:24.798Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Cluster Installation and Configuration | 6 |
| Kafka Architecture and Fundamentals | 6 |
| Kafka Connect and kDB | 4 |
| Operations and Monitoring | 6 |
| Performance Tuning and Troubleshooting | 3 |
| Security | 5 |

---

### **Cluster Installation and Configuration**

### 1. Which repository contains the private key and certificate that identifies a Kafka broker during a TLS handshake?

- [ ] **A)** Keystore
- [ ] **B)** Truststore
- [ ] **C)** Certificate Revocation List
- [ ] **D)** Key Distribution Center

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A keystore holds the local identity's private key and certificate. A truststore holds public CA certificates used to verify remote parties during TLS.
 
 
</details>

### 2. Which statements about SASL mechanisms are correct?

- [ ] **A)** SASL/SCRAM stores credentials using salted hashes.
- [ ] **B)** SASL/GSSAPI uses a Key Distribution Center and tickets.
- [ ] **C)** SASL/PLAIN should always be combined with SSL/TLS to protect credentials.
- [ ] **D)** SASL/OAUTHBEARER relies on Kerberos tickets.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> SASL/SCRAM uses salted hashes, SASL/GSSAPI uses Kerberos tickets, and SASL/PLAIN must be protected with TLS. OAUTHBEARER uses OAuth2 bearer tokens, not Kerberos.
 
 
</details>

### 3. Given the JAAS configuration shown in the code block, which SASL mechanism is being configured?

```properties
sasl.jaas.config=org.apache.kafka.common.security.scram.ScramLoginModule required
username="admin"
password="secret";
sasl.mechanism=SCRAM-SHA-256
```

- [ ] **A)** SCRAM-SHA-256
- [ ] **B)** PLAIN
- [ ] **C)** GSSAPI
- [ ] **D)** OAUTHBEARER

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The JAAS configuration uses ScramLoginModule and explicitly sets sasl.mechanism to SCRAM-SHA-256, so the mechanism is SCRAM-SHA-256.
 
 
</details>

### 4. In Kafka's ACL model, what happens when a client request has no explicit Allow rule?

- [ ] **A)** It is denied.
- [ ] **B)** It is allowed.
- [ ] **C)** It is queued for approval.
- [ ] **D)** It depends on an existing Deny rule.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Kafka's ACL model uses implicit deny; without an explicit Allow rule, access is denied. Kafka does not use explicit Deny rules.
 
 
</details>

### 5. Which resources can be governed by Kafka ACLs beyond topics?

- [ ] **A)** Consumer Groups
- [ ] **B)** Transactional IDs
- [ ] **C)** Schemas
- [ ] **D)** The Cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Kafka ACLs can be applied to Consumer Groups, Transactional IDs, and the Cluster itself. Schemas are typically governed by Confluent RBAC rather than raw Kafka ACLs.
 
 
</details>

### 6. Review the broker security settings in the code block. Which conclusions are accurate?

```properties
# broker configuration
ssl.client.auth=required
security.inter.broker.protocol=SSL
```

- [ ] **A)** Clients must present a valid certificate to the broker.
- [ ] **B)** Mutual TLS is enabled for client connections.
- [ ] **C)** No client authentication is needed because encryption alone is sufficient.
- [ ] **D)** This configuration disables TLS for inter-broker communication.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> With ssl.client.auth=required, the broker demands a client certificate, enabling mutual TLS. The inter-broker protocol remains SSL, so TLS is not disabled.
 
 
</details>


---

### **Kafka Architecture and Fundamentals**

### 7. In a Kafka TLS configuration, what type of cryptographic material is stored inside a truststore used for broker authentication?

- [ ] **A)** Private key and certificate
- [ ] **B)** Public certificates of trusted CAs
- [ ] **C)** SASL/SCRAM password hashes
- [ ] **D)** Consumer group offset metadata

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A truststore holds public CA certificates used to verify remote parties during the TLS handshake. A keystore contains the private key and certificate that identify the local entity.
 
 
</details>

### 8. Which two statements correctly describe the authentication behavior required by mutual TLS in a Kafka deployment?

- [ ] **A)** Only the broker presents a certificate
- [ ] **B)** Both broker and client present valid certificates
- [ ] **C)** mTLS requires two-way authentication
- [ ] **D)** mTLS uses SASL/PLAIN for encryption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> mTLS requires both broker and client to present certificates, providing strong two-way authentication. It does not replace SASL/PLAIN, and standard TLS only authenticates the server.
 
 
</details>

### 9. In the JAAS configuration shown in the code block, which Kafka security component is being defined for the broker?

```plaintext
KafkaServer {
  org.apache.kafka.common.security.plain.PlainLoginModule required
  username="admin"
  password="admin-secret"
  user_admin="admin-secret";
};
```

- [ ] **A)** Authentication credentials and mechanism
- [ ] **B)** Authorization permissions for resources
- [ ] **C)** Disk-level encryption keys
- [ ] **D)** Topic replication settings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> JAAS defines the SASL mechanism, login module, and credentials needed to authenticate. Permissions and authorization are handled separately by ACLs or RBAC.
 
 
</details>

### 10. What is a common consequence when a client trusts only the root CA but an intermediate CA certificate is absent from the broker's keystore?

- [ ] **A)** Clients fail to validate the broker's certificate
- [ ] **B)** Clients automatically fetch the missing certificate
- [ ] **C)** No impact because the root CA is trusted
- [ ] **D)** The broker rejects all SASL connections

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The trust chain must be complete. If the intermediate CA is absent from the keystore, clients cannot validate the presented chain even if they trust the root CA.
 
 
</details>

### 11. Which of these authentication mechanisms are valid SASL mechanisms that a Kafka client can use during the connection handshake?

- [ ] **A)** SASL/PLAIN
- [ ] **B)** SASL/SCRAM
- [ ] **C)** SASL/GSSAPI
- [ ] **D)** SASL/TLS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Kafka supports SASL/PLAIN, SASL/SCRAM, SASL/GSSAPI, and SASL/OAUTHBEARER. TLS is an encryption protocol, not a SASL mechanism.
 
 
</details>

### 12. Based on the SSLHandshakeException in the code block, which area should a Kafka administrator investigate before changing network settings?

```plaintext
ERROR [Producer clientId=producer-1] Connection to node -1 could not be established. Broker may not be available.
Caused by: javax.net.ssl.SSLHandshakeException: sun.security.validator.ValidatorException: PKIX path building failed: unable to find valid certification path to requested target
```

- [ ] **A)** Network connectivity and firewall rules
- [ ] **B)** Truststore contents and certificate chain
- [ ] **C)** Kafka consumer group offsets
- [ ] **D)** Disk space on the broker

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SSLHandshakeException is often caused by an untrusted certificate chain. Administrators should inspect the truststore and ensure all required CA certificates are present before checking the network.
 
 
</details>


---

### **Kafka Connect and kDB**

### 13. In TLS configuration, what is the main purpose of a truststore?

- [ ] **A)** To hold the private key and certificate that identify the local broker
- [ ] **B)** To store public certificates of trusted certificate authorities used to verify remote parties
- [ ] **C)** To store the usernames and passwords for SASL authentication
- [ ] **D)** To encrypt the Kafka topic data at rest using KMS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A truststore contains the public certificates of trusted certificate authorities that a broker or client uses to verify remote identities during the TLS handshake. The keystore, not the truststore, holds the private key and local certificate.
 
 
</details>

### 14. Which two statements correctly distinguish SASL from SSL?

- [ ] **A)** SASL handles authentication or identity verification.
- [ ] **B)** SSL/TLS provides encryption and integrity for the communication channel.
- [ ] **C)** SASL encrypts data stored in Kafka log segments.
- [ ] **D)** SSL/TLS primarily manages ACLs and authorization.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SASL is an authentication framework that verifies identity, while SSL/TLS secures the channel between client and broker by providing encryption and integrity. SASL does not encrypt data at rest, and TLS does not manage authorization.
 
 
</details>

### 15. Based on the JAAS configuration shown in the code block, and knowing that encryption is not enabled, what security issue is most likely to occur?

```java
Client {
  org.apache.kafka.common.security.plain.PlainLoginModule required
  username="admin"
  password="secret";
};
```

- [ ] **A)** The username and password are transmitted in plaintext over the network.
- [ ] **B)** The broker will reject the certificate chain because no truststore exists.
- [ ] **C)** The principal will be denied authorization because no ACLs are defined.
- [ ] **D)** The client will be forced to use Kerberos tickets instead of a password.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SASL/PLAIN sends username and password in clear text unless protected by SSL/TLS. The other choices describe certificate or authorization issues that are not directly caused by this JAAS/PLAIN setup.
 
 
</details>

### 16. What value must be set for ssl.client.auth to enforce mutual TLS on a Kafka broker?

- [ ] **A)** none
- [ ] **B)** requested
- [ ] **C)** required
- [ ] **D)** certificate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> ssl.client.auth=required enforces mutual TLS by requiring every client to present a valid certificate. With ssl.client.auth=none, only the server presents a certificate and encryption is not mutual.
 
 
</details>


---

### **Operations and Monitoring**

### 17. What type of material is stored in a truststore in a Kafka TLS configuration?

- [ ] **A)** Public certificates of trusted CAs
- [ ] **B)** The local entity's private key
- [ ] **C)** Username and password pairs
- [ ] **D)** Consumer group offsets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A truststore stores public certificates of trusted certificate authorities so a peer can be verified during the TLS handshake. Private keys and certificates identifying the local entity are kept in a keystore.
 
 
</details>

### 18. Which actions are performed during the SSL/TLS handshake? Select all that apply.

- [ ] **A)** Negotiation of encryption parameters
- [ ] **B)** Exchange of certificates
- [ ] **C)** Establishment of a secure session
- [ ] **D)** Commit of consumer offsets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The handshake negotiates algorithms, exchanges certificates for authentication, and establishes the secure session. Committing offsets is a Kafka protocol operation, not part of TLS.
 
 
</details>

### 19. Examine the broker setting shown in the exhibit. What security behavior does this configuration enforce?

```properties
ssl.client.auth=required
```

- [ ] **A)** Both the broker and the client must present valid certificates
- [ ] **B)** Only the broker must present a certificate
- [ ] **C)** No TLS encryption is required
- [ ] **D)** Only the client must present a certificate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Setting ssl.client.auth=required enforces mutual TLS, meaning the broker also requires a valid client certificate. Setting it to none would only allow server-side TLS.
 
 
</details>

### 20. What is the primary security benefit of SASL/SCRAM compared with SASL/PLAIN?

- [ ] **A)** It stores credentials as salted hashes
- [ ] **B)** It disables SSL/TLS encryption
- [ ] **C)** It does not require a jaas config
- [ ] **D)** It sends passwords in clear text

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SCRAM uses salted hashed passwords, reducing risks like rainbow table attacks. PLAIN transmits username and password in clear text unless protected by TLS.
 
 
</details>

### 21. Which statements correctly describe SASL and SSL in Kafka? Select all that apply.

- [ ] **A)** SASL verifies identity while SSL protects channel security
- [ ] **B)** SSL is responsible for encryption and integrity
- [ ] **C)** SASL/PLAIN should always be protected with SSL/TLS
- [ ] **D)** SSL can replace SASL as an authentication mechanism

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> SASL handles authentication and identity while SSL/TLS handles channel security and encryption. SASL/PLAIN sends plaintext credentials, so TLS must wrap it; SSL does not provide Kafka SASL identity verification.
 
 
</details>

### 22. According to the displayed JAAS configuration, what does this entry define?

```java
KafkaClient {
    org.apache.kafka.common.security.plain.PlainLoginModule required
    username="alice"
    password="secret";
};
```

- [ ] **A)** Credentials and login module for authentication
- [ ] **B)** ACL permissions for resource access
- [ ] **C)** TLS certificate trust list
- [ ] **D)** Encryption keys for data at rest

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> JAAS defines the login module, username, and password used during authentication. It does not define permissions or encryption; ACLs and TLS handle those separately.
 
 
</details>


---

### **Performance Tuning and Troubleshooting**

### 23. In a Kafka broker's TLS configuration, what is stored in the keystore?

- [ ] **A)** The private key and certificate that identify the broker
- [ ] **B)** The public certificates of trusted certificate authorities
- [ ] **C)** SASL usernames and passwords
- [ ] **D)** The listener name and port configuration

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A keystore stores the local entity's private key and associated certificate. A truststore stores CA public certificates used to validate remote peers.
 
 
</details>

### 24. Which of the following statements about SASL mechanisms are correct?

- [ ] **A)** SASL/GSSAPI uses a Key Distribution Center for Kerberos authentication
- [ ] **B)** SASL/OAUTHBEARER uses bearer tokens from an external Identity Provider
- [ ] **C)** SASL/PLAIN is inherently secure without additional TLS/SSL encryption
- [ ] **D)** SASL/SCRAM stores credentials as salted hashes to protect against rainbow table attacks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Kerberos relies on a KDC, OAUTHBEARER uses tokens from an IdP, and SCRAM uses salted hashes. PLAIN is insecure unless protected by TLS.
 
 
</details>

### 25. The JAAS configuration shown in the code block is used by a Kafka client. Which SASL mechanism is being configured?

```properties
KafkaClient { org.apache.kafka.common.security.plain.PlainLoginModule required username="alice" password="secret"; };
```

- [ ] **A)** SASL/PLAIN
- [ ] **B)** SASL/SCRAM
- [ ] **C)** SASL/GSSAPI
- [ ] **D)** SASL/OAUTHBEARER

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The PlainLoginModule is the JAAS module for SASL/PLAIN, using a username and password that must be protected by SSL/TLS encryption.
 
 
</details>


---

### **Security**

### 26. In the context of Kafka TLS configuration, what is the primary difference between a keystore and a truststore?

- [ ] **A)** A keystore verifies remote CAs; a truststore stores the private key.
- [ ] **B)** A keystore stores the private key and certificate for the local entity; a truststore stores trusted CA certificates.
- [ ] **C)** A keystore stores encrypted passwords; a truststore stores plaintext credentials.
- [ ] **D)** A keystore is used only by clients; a truststore is used only by brokers.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The keystore holds identity material such as the private key and certificate for the local entity, while the truststore holds CA certificates used to validate remote parties.
 
 
</details>

### 27. Which of the following are supported SASL mechanisms for authentication in Kafka? (Select all that apply.)

- [ ] **A)** SASL/PLAIN
- [ ] **B)** SASL/SCRAM
- [ ] **C)** SASL/GSSAPI
- [ ] **D)** SASL/OAUTHBEARER

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> Kafka supports SASL/PLAIN, SCRAM, GSSAPI/Kerberos, and OAUTHBEARER as authentication mechanisms.
 
 
</details>

### 28. Refer to the broker configuration in the code block. What security behavior does this setting enforce?

```properties
ssl.client.auth=required
```

- [ ] **A)** It disables TLS encryption.
- [ ] **B)** It enforces mutual TLS, requiring clients to provide valid certificates.
- [ ] **C)** It allows anonymous TLS connections.
- [ ] **D)** It only enables server-side TLS.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The value 'required' for ssl.client.auth enforces mutual TLS, meaning clients must present a valid certificate during the handshake.
 
 
</details>

### 29. What is the primary purpose of SASL/GSSAPI (Kerberos) authentication in Kafka?

- [ ] **A)** It uses tickets from a Key Distribution Center to authenticate users without sending passwords to the broker.
- [ ] **B)** It sends the user's password directly to the broker for validation.
- [ ] **C)** It encrypts the broker's keystore with a shared secret.
- [ ] **D)** It provides ACL-based authorization after the TLS handshake.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SASL/GSSAPI relies on a KDC and ticket-based authentication, so passwords are not transmitted directly to the broker.
 
 
</details>

### 30. To which resource types can Kafka ACLs be applied? (Select all that apply.)

- [ ] **A)** Topics
- [ ] **B)** Consumer Groups
- [ ] **C)** Transactional IDs
- [ ] **D)** Cluster

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> ACLs apply to topics, consumer groups, transactional IDs, and the cluster itself.
 
 
</details>

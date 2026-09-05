<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Microsoft%20Certified-%20Cybersecurity%20Architect%20Expert.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Microsoft Certified: Cybersecurity Architect Expert</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Design security operations, identity, and compliance capabilities](#design-security-operations-identity-and-compliance-capabilities) (8 questions)
- [Design security solutions for applications and data](#design-security-solutions-for-applications-and-data) (7 questions)
- [Design security solutions for infrastructure](#design-security-solutions-for-infrastructure) (8 questions)
- [Design solutions that align with security best practices and priorities](#design-solutions-that-align-with-security-best-practices-and-priorities) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:13.638Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Design security operations, identity, and compliance capabilities | 8 |
| Design security solutions for applications and data | 7 |
| Design security solutions for infrastructure | 8 |
| Design solutions that align with security best practices and priorities | 7 |

---

### **Design security operations, identity, and compliance capabilities**

### 1. Which Azure security capability is specifically designed to provide Layer 7 application traffic inspection?

- [ ] **A)** Network Security Group (NSG)
- [ ] **B)** WAF/Azure Firewall application rules
- [ ] **C)** Azure DNS
- [ ] **D)** Azure Traffic Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> WAF and Azure Firewall application rules inspect Layer 7 data such as HTTP headers. NSGs filter at Layer 4 using IPs and ports, which is the common confusion described in the playbook.
 
 
</details>

### 2. According to the common traps, which scenarios are recognized architecture mistakes?

- [ ] **A)** Confusing Layer 4 NSG rules with Layer 7 WAF capabilities
- [ ] **B)** Selecting a hub-and-spoke topology for simplicity while ignoring central inspection
- [ ] **C)** Prioritizing connectivity over inspecting traffic
- [ ] **D)** Implementing policy-driven security deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The playbook lists layer confusion, topology simplification over inspection, and connectivity before security as common traps. Policy-driven security is recommended, not a trap.
 
 
</details>

### 3. You are reviewing a network rule that only inspects IP addresses and TCP port 80. Which security capability does this rule represent?

```json
{
  "name": "Allow-HTTP-80",
  "properties": {
    "access": "Allow",
    "protocol": "Tcp",
    "direction": "Inbound",
    "sourceAddressPrefix": "*",
    "destinationAddressPrefix": "*",
    "destinationPortRange": "80"
  }
}
```

- [ ] **A)** Layer 4 Network Security Group
- [ ] **B)** Layer 7 Web Application Firewall
- [ ] **C)** Azure Policy assignment
- [ ] **D)** Azure Active Directory conditional access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The rule filters by TCP port and IP prefixes, which is Layer 4 behavior. Application-layer inspection would require a WAF or Azure Firewall application rule.
 
 
</details>

### 4. What is the main risk of making connectivity a higher priority than security inspection in a cloud architecture?

- [ ] **A)** Traffic flows quickly but may bypass required security inspection
- [ ] **B)** Inspection improves automatically as traffic flow increases
- [ ] **C)** Network latency always increases
- [ ] **D)** Compliance is easier to prove

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> When connectivity is prioritized, traffic may be allowed to flow without being directed through required inspection points, creating security gaps.
 
 
</details>

### 5. Which statements about IaaS and PaaS security responsibilities are correct?

- [ ] **A)** IaaS gives customers more control over operating systems and middleware
- [ ] **B)** PaaS shifts more infrastructure security responsibility to the provider
- [ ] **C)** Treating PaaS like IaaS can cause over-provisioning of security controls
- [ ] **D)** PaaS customers must patch the host operating system

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> PaaS transfers more underlying infrastructure responsibility to the provider. Applying IaaS-level controls to PaaS can lead to unnecessary security provisioning.
 
 
</details>

### 6. An Azure Policy definition is used to continuously audit deployed resources for compliance. Which security strategy does this demonstrate?

```json
{
  "policyRule": {
    "if": {
      "field": "kind",
      "equals": "SQLDatabase"
    },
    "then": {
      "effect": "audit",
      "details": {
        "type": "Microsoft.Sql/servers/databases"
      }
    }
  }
}
```

- [ ] **A)** Reactive manual remediation
- [ ] **B)** Proactive policy-driven architectural design
- [ ] **C)** Layer 4 network inspection
- [ ] **D)** Hub-and-spoke connectivity planning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Automated policy audit is a proactive architectural design. It continuously checks resources instead of relying on manual remediation after an issue appears.
 
 
</details>

### 7. What happens when an organization selects a visibility tool that deeply monitors only one cloud while using multiple cloud providers?

- [ ] **A)** It will likely fail to meet centralized security monitoring requirements
- [ ] **B)** It will automatically unify all cloud security data
- [ ] **C)** It reduces the need for identity management
- [ ] **D)** It is always the best choice for compliance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A single-cloud tool cannot deliver the required centralized visibility across a multi-cloud environment, causing gaps in security operations.
 
 
</details>

### 8. Which considerations are important when using a hub-and-spoke topology for security?

- [ ] **A)** Centralized inspection may require traffic to pass through a hub
- [ ] **B)** A simplistic hub-and-spoke design can ignore inspection needs
- [ ] **C)** Enabling connectivity alone does not secure the traffic
- [ ] **D)** A hub-and-spoke network automatically applies WAF policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Hub-and-spoke networks support centralized inspection only if traffic is intentionally routed through the hub. Simplicity and connectivity do not guarantee security.
 
 
</details>


---

### **Design security solutions for applications and data**

### 9. At which OSI layer do Network Security Groups (NSGs) filter traffic in an Azure environment?

- [ ] **A)** Layer 4 (Transport)
- [ ] **B)** Layer 7 (Application)
- [ ] **C)** Layer 2 (Data Link)
- [ ] **D)** Layer 5 (Session)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NSGs filter traffic by source/destination IP, port, and protocol, so they operate at Layer 4 of the OSI model rather than at Layer 7.
 
 
</details>

### 10. Which two Azure services are commonly used for Layer 7 application-level inspection and protection?

- [ ] **A)** Azure Web Application Firewall (WAF)
- [ ] **B)** Azure Firewall
- [ ] **C)** Network Security Group (NSG)
- [ ] **D)** Azure Traffic Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure WAF protects web apps from application-layer attacks, and Azure Firewall supports Layer 7 FQDN-based rules. NSGs operate at Layer 4.
 
 
</details>

### 11. Review the JSON rule in the code block. At which OSI layer does this rule operate?

```json
{
  "name": "AllowTCP80",
  "properties": {
    "access": "Allow",
    "destinationPortRange": "80",
    "protocol": "Tcp",
    "direction": "Inbound",
    "priority": 100
  }
}
```

- [ ] **A)** Layer 4 (Transport)
- [ ] **B)** Layer 7 (Application)
- [ ] **C)** Layer 2 (Data Link)
- [ ] **D)** Layer 5 (Session)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The rule filters TCP port 80, which is a transport-layer characteristic, so this NSG rule operates at Layer 4.
 
 
</details>

### 12. Which network topology is typically used to route traffic through a central security inspection point?

- [ ] **A)** Hub-and-spoke
- [ ] **B)** Full mesh
- [ ] **C)** Point-to-point
- [ ] **D)** Flat network

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Hub-and-spoke centralizes connectivity in a hub, allowing traffic to be inspected before reaching spokes. Other topologies complicate centralized enforcement.
 
 
</details>

### 13. Which two security outcomes should be prioritized instead of only ensuring traffic flows?

- [ ] **A)** Ensure traffic is inspected
- [ ] **B)** Centralize security inspection
- [ ] **C)** Minimize latency above all
- [ ] **D)** Let traffic flow freely

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Security architecture must inspect traffic and centralize enforcement; only ensuring traffic flows without inspection can create security gaps.
 
 
</details>

### 14. The code block contains a resource definition. Which cloud service model does this resource represent?

```json
{
  "type": "Microsoft.Web/sites",
  "name": "myAppService",
  "location": "eastus",
  "properties": {
    "serverFarmId": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/myRG/providers/Microsoft.Web/serverfarms/myPlan"
  }
}
```

- [ ] **A)** Platform as a Service (PaaS)
- [ ] **B)** Infrastructure as a Service (IaaS)
- [ ] **C)** Software as a Service (SaaS)
- [ ] **D)** On-premises

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Microsoft.Web/sites represents Azure App Service, a PaaS offering in which the platform manages infrastructure and the customer manages applications and data.
 
 
</details>

### 15. What common trap occurs when a security tool provides excellent visibility in one cloud but does not meet multi-cloud requirements?

- [ ] **A)** Single-cloud visibility trap
- [ ] **B)** IaaS/PaaS responsibility confusion
- [ ] **C)** Connectivity over security
- [ ] **D)** Reactive security

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Using a tool that only meets single-cloud visibility fails to protect distributed environments when multi-cloud visibility is required by the architecture.
 
 
</details>


---

### **Design security solutions for infrastructure**

### 16. Which common trap refers to confusing the security capabilities of NSG with those of WAF or Azure Firewall when dealing with application-level threats?

- [ ] **A)** Selecting hub-and-spoke for simplicity and no inspection
- [ ] **B)** Confusing NSG (Layer 4) with WAF (Layer 7)
- [ ] **C)** Prioritizing connectivity over security inspection
- [ ] **D)** Mixing IaaS and PaaS security responsibilities

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The document lists this exact trap as confusing Layer 4 (NSG) with Layer 7 (WAF/Azure Firewall) capabilities, especially for application-level threats.
 
 
</details>

### 17. Which of the following are common traps when designing security solutions for infrastructure? Select all that apply.

- [ ] **A)** Confusing NSG (Layer 4) with WAF (Layer 7)
- [ ] **B)** Selecting hub-and-spoke while ignoring inspection
- [ ] **C)** Prioritizing reactive over proactive design
- [ ] **D)** Centralizing inspection before enabling traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The first three options match common traps listed in the playbook. The fourth is a recommended practice, not a trap.
 
 
</details>

### 18. Which common trap is illustrated by the scenario in the code block?

```javascript
// Planning note:
// The architecture uses a hub-and-spoke model to keep the design simple.
// There is no planned network virtual appliance or firewall for traffic inspection.
// The team is proud that traffic will flow efficiently between spokes.
```

- [ ] **A)** Confusing NSG with WAF/Azure Firewall layers
- [ ] **B)** Using hub-and-spoke without centralized inspection
- [ ] **C)** Prioritizing reactive manual response
- [ ] **D)** Mixing IaaS and PaaS responsibilities

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code block describes a simple hub-and-spoke deployment without centralized inspection, which matches the hub-and-spoke trap.
 
 
</details>

### 19. What is the main risk of prioritizing connectivity over security when designing infrastructure?

- [ ] **A)** Connectivity guarantees traffic inspection
- [ ] **B)** Traffic flows without mandatory inspection
- [ ] **C)** Firewall required for connectivity
- [ ] **D)** NSGs block all Layer 7 threats

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The playbook warns against prioritizing connectivity for the sake of traffic flow while ignoring security inspection, which can leave traffic uninspected.
 
 
</details>

### 20. Which of the following are consequences of confusing IaaS and PaaS security responsibilities? Select all that apply.

- [ ] **A)** Over-provisioning security controls
- [ ] **B)** Security gaps from missed responsibilities
- [ ] **C)** Clearer platform security boundaries
- [ ] **D)** Same security posture in all models

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The playbook states this confusion can lead to over-provisioning or security gaps, not to clearer boundaries or identical posture.
 
 
</details>

### 21. Which common trap is represented by the selection logic in the code block?

```python
candidate_tool = 'single-cloud monitoring'
environment = ['azure', 'aws', 'on-premises']
selected = candidate_tool
# No validation for multi-cloud or hybrid coverage
```

- [ ] **A)** Single-cloud tool that misses hybrid coverage
- [ ] **B)** Confusing NSG with WAF
- [ ] **C)** Reactive instead of proactive design
- [ ] **D)** Hub-and-spoke without inspection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code selects a single-cloud tool even though the environment includes multiple clouds and on-premises, matching the tool-selection trap.
 
 
</details>

### 22. Which approach best represents proactive architectural design for infrastructure security?

- [ ] **A)** Manual remediation after incidents
- [ ] **B)** Policy-driven security in the architecture
- [ ] **C)** Waiting for alerts before acting
- [ ] **D)** Connecting before planning inspection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The playbook contrasts reactive manual remediation with proactive architectural design, specifically policy-driven security.
 
 
</details>

### 23. Which of the following accurately describe the hub-and-spoke common trap? Select all that apply.

- [ ] **A)** Hub-and-spoke chosen for simplicity
- [ ] **B)** Centralized inspection requirements ignored
- [ ] **C)** Only a trap when spokes are disconnected
- [ ] **D)** Eliminates need for WAF/Azure Firewall

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The trap is choosing hub-and-spoke for simplicity and ignoring centralized inspection; connectivity alone does not avoid the trap.
 
 
</details>


---

### **Design solutions that align with security best practices and priorities**

### 24. At which network layer does a Network Security Group (NSG) primarily inspect and filter traffic?

- [ ] **A)** Layer 4
- [ ] **B)** Layer 7
- [ ] **C)** Layer 2
- [ ] **D)** Layer 5

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NSGs filter traffic based on source/destination IP, port, and protocol, which aligns with Layer 4 transport-layer information.
 
 
</details>

### 25. According to the playbook, which of the following are common traps when designing security solutions? (Select all that apply.)

- [ ] **A)** Confusing NSG with WAF capabilities
- [ ] **B)** Ignoring centralized inspection when choosing hub-and-spoke
- [ ] **C)** Using a single-cloud tool for multi-cloud visibility
- [ ] **D)** Prioritizing security over connectivity in all designs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The playbook warns about confusing Layer 4 with Layer 7, ignoring centralized inspection, and choosing single-cloud tools when multi-cloud visibility is needed.
 
 
</details>

### 26. Review the filtering rule in the exhibit. At which OSI layer is this network security rule operating?

```bash
az network nsg rule create --resource-group rg-app --nsg-name app-nsg --name Allow-HTTPS --direction Inbound --priority 100 --access Allow --protocol Tcp --destination-port-ranges 443
```

- [ ] **A)** Layer 4
- [ ] **B)** Layer 7
- [ ] **C)** Session layer
- [ ] **D)** Application layer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The rule filters by protocol TCP and destination port 443, which is transport-layer information, so it operates at Layer 4.
 
 
</details>

### 27. When a designer prioritizes connectivity over security, what should be reviewed to avoid this trap?

- [ ] **A)** Ensuring traffic is inspected
- [ ] **B)** Making traffic flow quickly
- [ ] **C)** Reducing network latency
- [ ] **D)** Minimizing route complexity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The playbook warns against prioritizing connectivity before security; the correct emphasis is that traffic must be inspected, not just allowed to flow.
 
 
</details>

### 28. Which of the following reflect the IaaS/PaaS responsibility confusion mentioned in the playbook? (Select all that apply.)

- [ ] **A)** Applying host-level controls to a PaaS service
- [ ] **B)** Over-provisioning controls due to responsibility confusion
- [ ] **C)** Reviewing the shared responsibility model
- [ ] **D)** Using built-in PaaS security features

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> IaaS/PaaS confusion appears when host-level controls are applied to PaaS or when security controls are over-provisioned because responsibility boundaries are unclear.
 
 
</details>

### 29. The exhibit shows an action taken by a security team. Does this action represent proactive architecture or reactive remediation?

```bash
az policy assignment create --name require-sql-encryption --policy /subscriptions/123/resourceGroups/rg/providers/Microsoft.Authorization/policyDefinitions/require-sql-encryption --scope /subscriptions/123/resourceGroups/prod
```

- [ ] **A)** Proactive policy-driven design
- [ ] **B)** Reactive manual remediation
- [ ] **C)** Layer 4 filtering
- [ ] **D)** Hub-and-spoke simplification

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Assigning a policy is a proactive architectural control; it prevents misconfiguration instead of manually fixing issues after detection.
 
 
</details>

### 30. Why is selecting a single-cloud visibility tool dangerous when multi-cloud visibility is required?

- [ ] **A)** It lacks required multi-cloud coverage
- [ ] **B)** It increases latency in every cloud
- [ ] **C)** It filters at the wrong OSI layer
- [ ] **D)** It eliminates the need for a WAF

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A tool focused on one cloud cannot monitor workloads and threats across all providers, violating the overarching visibility requirement.
 
 
</details>

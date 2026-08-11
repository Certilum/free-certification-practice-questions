<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/ISACA/Certified%20Data%20Privacy%20Solutions%20Engineer%E2%84%A2%20(CDPSE%E2%84%A2)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>ISACA CDPSE</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Data Life Cycle Management](#data-life-cycle-management) (7 questions)
- [Privacy Engineering](#privacy-engineering) (12 questions)
- [Privacy Governance](#privacy-governance) (6 questions)
- [Privacy Risk Management and Compliance](#privacy-risk-management-and-compliance) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-11T02:41:50.466Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Data Life Cycle Management | 7 |
| Privacy Engineering | 12 |
| Privacy Governance | 6 |
| Privacy Risk Management and Compliance | 5 |

---

### **Data Life Cycle Management**

### 1. In the CDPSE framework, what is the primary purpose of creating and maintaining a data inventory?

- [ ] **A)** Structured record of personal data, locations, purposes, and legal bases
- [ ] **B)** Diagram of network connections and packet flows
- [ ] **C)** List of software licenses and hardware assets
- [ ] **D)** List of employee salaries and performance reviews

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A data inventory is a structured record of personal data, including location, purposes, legal bases, retention, and data subject categories, enabling governance and compliance.
 
 
</details>

### 2. Which factors should drive the classification of personal data in a privacy context?

- [ ] **A)** Potential harm to the data subject
- [ ] **B)** Processing context and regulatory impact
- [ ] **C)** Only the organization's trade secret value
- [ ] **D)** Database vendor's support tier

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Classification in privacy must consider data subject harm, processing context, and regulatory impact. Trade secret value alone is not sufficient.
 
 
</details>

### 3. Review the data inventory entry in the code block. Which privacy-specific attribute is missing?

```json
{
  "data_element": "email_address",
  "system_of_record": "CRM",
  "business_process": "customer support",
  "format": "structured",
  "owner": "support_manager"
}
```

- [ ] **A)** Lawful basis
- [ ] **B)** IP address
- [ ] **C)** Server room location
- [ ] **D)** Database version

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A privacy data inventory must document lawful basis, not just system details such as owner, format, and location.
 
 
</details>

### 4. Which foundational artifact visually represents the movement of personal data across systems, vendors, and jurisdictions?

- [ ] **A)** Data-flow map
- [ ] **B)** Data inventory
- [ ] **C)** Classification scheme
- [ ] **D)** Retention schedule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A data-flow map traces movement from collection through sharing, storage, and destruction, including third parties and jurisdictions.
 
 
</details>

### 5. Which events should trigger an update to data inventories and data-flow maps?

- [ ] **A)** Deployment of a new system
- [ ] **B)** Amendment of a third-party contract
- [ ] **C)** Adoption of a new privacy regulation
- [ ] **D)** Replacement of a network router

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> New systems, third-party changes, and regulatory updates change processing; inventory and flow maps must be revised to remain accurate.
 
 
</details>

### 6. Identify the foundational artifact represented in the code block.

```text
Sources: web forms and mobile apps
Destinations: CRM, US data center, marketing database
Intermediate processing: CRM validation
Transfer: EU to US
```

- [ ] **A)** Data-flow map
- [ ] **B)** Data inventory
- [ ] **C)** Data classification scheme
- [ ] **D)** Consent log

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block describes sources, destinations, and transfers, which are the defining properties of a data-flow map.
 
 
</details>

### 7. What does the principle of collection limitation require an organization to do?

- [ ] **A)** Collect only data needed for the stated purpose
- [ ] **B)** Collect as much data as possible for later analytics
- [ ] **C)** Collect data without documenting a lawful basis
- [ ] **D)** Collect data after receiving an informal request

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Collection limitation requires gathering only data that is adequate and necessary for the stated purpose; extra collection is prohibited.
 
 
</details>


---

### **Privacy Engineering**

### 8. What does privacy by design require in solution development?

- [ ] **A)** Treat privacy as an after-the-fact compliance activity
- [ ] **B)** Embed privacy controls into every development stage
- [ ] **C)** Apply privacy only during final acceptance testing
- [ ] **D)** Add privacy measures immediately after a breach

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Privacy by design requires proactive, continuous embedding of privacy into every stage of solution development, not a final review.
 
 
</details>

### 9. Which practices are part of privacy by default? (Select all that apply.)

- [ ] **A)** Most protective configuration automatically enabled
- [ ] **B)** Default opt-out for non-essential processing
- [ ] **C)** Requiring users to manually adjust many settings
- [ ] **D)** Short data retention periods by default

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Privacy by default means the most protective settings are already active, including opt-out defaults and limited retention.
 
 
</details>

### 10. Review the configuration. Which change makes it privacy protective by default?

```python
config = {
    "data_sharing": True,
    "retention_days": 3650,
    "opt_in_required": False,
    "location_access": "Always"
}
```

- [ ] **A)** Set data_sharing to False and retention_days to 30
- [ ] **B)** Set data_sharing to True and retention_days to 3650
- [ ] **C)** Set opt_in_required to False and data_sharing to True
- [ ] **D)** Set retention_days to 3650 and location_access to Always

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Privacy by default requires minimizing sharing, limiting retention, and requiring opt-in for non-essential processing.
 
 
</details>

### 11. What is the main difference between privacy by design and security?

- [ ] **A)** Security ensures privacy automatically
- [ ] **B)** Security is necessary but not sufficient for privacy
- [ ] **C)** Security and privacy are identical
- [ ] **D)** Security removes the need for privacy controls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Security protects confidentiality, but privacy also requires minimization, purpose limitation, and lawful processing.
 
 
</details>

### 12. Which outputs are created during privacy requirements elicitation? (Select all that apply.)

- [ ] **A)** Personal data stream inventory
- [ ] **B)** Legal bases for processing
- [ ] **C)** Data subject rights and retention obligations
- [ ] **D)** Marketing campaign design

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Privacy requirements elicitation captures data streams, legal bases, rights, transfer restrictions, and retention obligations.
 
 
</details>

### 13. A service needs only an age range. Which field is excessive?

```python
fields = ["full_name", "exact_date_of_birth", "age_band"]
```

- [ ] **A)** full_name
- [ ] **B)** exact_date_of_birth
- [ ] **C)** age_band
- [ ] **D)** all fields

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Collecting exact date of birth is excessive when only an age range is needed for the declared purpose.
 
 
</details>

### 14. When should a data protection impact assessment begin?

- [ ] **A)** Only after deployment
- [ ] **B)** Early and evolve with design
- [ ] **C)** After a regulator complaint
- [ ] **D)** At final acceptance testing only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A DPIA is a decision-making method that begins early and evolves with the system design.
 
 
</details>

### 15. Which controls help enforce data minimization? (Select all that apply.)

- [ ] **A)** Field-level access controls
- [ ] **B)** Schema validation
- [ ] **C)** Alerting on over-collection
- [ ] **D)** Unlimited data retention

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Schema validation, field-level access, and alerting help limit collection to only necessary personal data.
 
 
</details>

### 16. Which query demonstrates purpose limitation?

```sql
-- Query 1
SELECT * FROM patients;
-- Query 2
SELECT patient_id, condition FROM patients;
-- Query 3
SELECT patient_id FROM patients WHERE purpose = 'treatment' AND consent = TRUE;
```

- [ ] **A)** Query 1
- [ ] **B)** Query 2
- [ ] **C)** Query 3
- [ ] **D)** None

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Query 3 limits access by declared purpose and consent, directly supporting purpose limitation.
 
 
</details>

### 17. What is the joiner-mover-leaver lifecycle used for?

- [ ] **A)** Identity lifecycle management
- [ ] **B)** Firewall management
- [ ] **C)** Patch management
- [ ] **D)** Consent management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Identity lifecycle management covers creating, updating, and deleting identities as people join, move, or leave.
 
 
</details>

### 18. Which components are part of a privacy-aware identity and access architecture? (Select all that apply.)

- [ ] **A)** Identity lifecycle management
- [ ] **B)** Authorization policy enforcement
- [ ] **C)** Purpose limitation enforcement
- [ ] **D)** Network topology mapping

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Privacy-aware architectures include lifecycle management, authorization, and purpose limitation as a single control system.
 
 
</details>

### 19. Given this account state, which action best reduces privacy risk?

```python
user_status = "terminated"
account_enabled = True
```

- [ ] **A)** Disable the account automatically
- [ ] **B)** Rotate the password
- [ ] **C)** Keep the account active
- [ ] **D)** Add the account to more roles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Automated de-provisioning prevents orphaned accounts from accessing personal data after a contractor leaves.
 
 
</details>


---

### **Privacy Governance**

### 20. Which statement best defines risk appetite in privacy governance?

- [ ] **A)** The broad-level amount of risk the enterprise is willing to accept while pursuing objectives
- [ ] **B)** A quantitative limit applied to every individual data processing activity
- [ ] **C)** The total legal liability an organization has accumulated in the past year
- [ ] **D)** A mandatory regulatory requirement to disclose all data processing to regulators

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Risk appetite is the broad amount of risk an organization accepts; risk tolerance sets measurable deviations from that appetite.
 
 
</details>

### 21. Which two actions support aligning privacy strategy with enterprise mission?

- [ ] **A)** Map privacy objectives to the enterprise's strategic goals
- [ ] **B)** Apply the strictest privacy controls to every department regardless of risk appetite
- [ ] **C)** Gain executive sponsorship and board approval for the privacy strategy
- [ ] **D)** Keep privacy strategy separate from business strategy to avoid conflicts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Privacy alignment requires mapping objectives to mission and obtaining executive sponsorship. Over-restrictive or isolated strategies contradict risk appetite and integration.
 
 
</details>

### 22. Examine the decision logic in the code block. Which governance principle does it apply?

```sql
SELECT 
  CASE 
    WHEN risk_appetite = 'MODERATE' THEN 'Approve project with privacy controls'
    WHEN risk_appetite = 'LOW' THEN 'Restrict processing'
    ELSE 'Escalate to board'
  END AS privacy_strategy
FROM governance_register;
```

- [ ] **A)** Aligning processing decisions with the enterprise risk appetite
- [ ] **B)** Eliminating the need for executive oversight
- [ ] **C)** Substituting human judgment with automated decisions
- [ ] **D)** Applying identical controls to all projects

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The logic maps risk appetite to strategy. It allows processing with safeguards, restricted processing, or board escalation, reflecting appetite-based governance.
 
 
</details>

### 23. Who is ultimately accountable for approving the enterprise privacy strategy and risk appetite?

- [ ] **A)** Data Protection Officer
- [ ] **B)** Board of Directors
- [ ] **C)** IT Security Director
- [ ] **D)** Business Unit Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The board owns risk appetite and approves the privacy strategy. The DPO advises; senior management authorizes.
 
 
</details>

### 24. Which two role-to-responsibility pairings are correct under CDPSE privacy governance?

- [ ] **A)** Board of Directors – sets risk appetite and oversees strategy
- [ ] **B)** DPO – makes unilateral business decisions on all data processing
- [ ] **C)** Legal Counsel – provides consultative interpretation of privacy law
- [ ] **D)** Security Team – has final accountability for legal compliance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Board sets strategy and risk appetite; legal is consulted for law. DPO advises, and security implements technical controls, not legal accountability.
 
 
</details>

### 25. The code block shows a RACI matrix for privacy governance. Which two entries are NOT aligned with CDPSE guidance?

```python
raci = {
    'Board': 'informed',
    'DPO': 'accountable for privacy compliance',
    'IT Security': 'responsible for implementing technical controls',
    'Legal': 'consulted on legal interpretation',
    'Product Manager': 'accountable for overall legal compliance'
}
```

- [ ] **A)** Board is listed as informed
- [ ] **B)** DPO is listed as accountable for privacy compliance
- [ ] **C)** Product Manager is listed as accountable for overall legal compliance
- [ ] **D)** Legal is listed as consulted

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The board should approve and oversee strategy, not merely be informed, and legal compliance accountability cannot sit with a product manager.
 
 
</details>


---

### **Privacy Risk Management and Compliance**

### 26. In privacy risk management, what is the primary focus of a privacy risk assessment when personal data is processed?

- [ ] **A)** Harm to data subjects' rights and freedoms
- [ ] **B)** Harm to the organization's profit
- [ ] **C)** Damage to brand reputation only
- [ ] **D)** Loss of vendor contract value

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A privacy risk assessment focuses on likelihood and severity of harm to individuals, including loss of control, discrimination, or intrusion.
 
 
</details>

### 27. Which elements are typically included in a data flow map used for a privacy risk assessment? Select all that apply.

- [ ] **A)** Data subjects
- [ ] **B)** Retention periods
- [ ] **C)** Data categories
- [ ] **D)** Organizational chart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A data flow map records data subjects, data categories, processing systems, retention periods, and technical and organizational controls.
 
 
</details>

### 28. Review the DPIA decision record shown in the code block. Which processing activity is an example of the documented trigger?

```yaml
dpia_trigger: likely_to_result_in_high_risk
timing: prior_to_processing
```

- [ ] **A)** Systematic monitoring of a public area
- [ ] **B)** Any processing with consent
- [ ] **C)** Occasional manual record keeping
- [ ] **D)** Fully outsourced payroll processing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The DPIA trigger is processing likely to result in high risk; systematic monitoring of publicly accessible areas is an Article 35(3) example.
 
 
</details>

### 29. What distinguishes a data protection impact assessment from a general privacy impact assessment under data protection law?

- [ ] **A)** Required for high-risk processing and has mandatory content
- [ ] **B)** Optional for all projects
- [ ] **C)** Focuses only on security incidents
- [ ] **D)** Requires the regulator to approve every product

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A DPIA is legally required for high-risk processing and includes mandatory content, while a general PIA is flexible and internally driven.
 
 
</details>

### 30. Which steps are mandatory or expected when performing a DPIA? Select all that apply.

- [ ] **A)** Involve the data protection officer
- [ ] **B)** Consult data subjects when feasible
- [ ] **C)** Consult supervisory authority if high residual risk remains
- [ ] **D)** Obtain consent from every data subject

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A DPIA requires DPO involvement, feasible data subject consultation, and supervisory authority consultation when high residual risk remains.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Salesforce/Salesforce%20Certified%20Platform%20Administrator.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Salesforce Certified Advanced Administrator</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Analytics and Reporting](#analytics-and-reporting) (3 questions)
- [AppExchange](#appexchange) (1 questions)
- [Configuration and Setup](#configuration-and-setup) (6 questions)
- [Data Management](#data-management) (3 questions)
- [Object Manager and Lightning Apps](#object-manager-and-lightning-apps) (6 questions)
- [Productivity and Collaboration](#productivity-and-collaboration) (2 questions)
- [User Management](#user-management) (4 questions)
- [Workflow/Process Automation](#workflow-process-automation) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:47:09.493Z |
| Domains | 8 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Analytics and Reporting | 3 |
| AppExchange | 1 |
| Configuration and Setup | 6 |
| Data Management | 3 |
| Object Manager and Lightning Apps | 6 |
| Productivity and Collaboration | 2 |
| User Management | 4 |
| Workflow/Process Automation | 5 |

---

### **Analytics and Reporting**

### 1. In the AppExchange ecosystem, what is the primary purpose of a managed package that vendors release?

- [ ] **A)** Providing freely modifiable source code
- [ ] **B)** Creating static org templates
- [ ] **C)** Distributing protected, upgradeable code
- [ ] **D)** Replacing all custom metadata

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Managed packages allow vendors to distribute updates while protecting source code and letting customers customize supported metadata without breaking upgrades.
 
 
</details>

### 2. Which factors should an Advanced Administrator evaluate when assessing the security posture of a third-party AppExchange solution?

- [ ] **A)** OAuth scopes requested
- [ ] **B)** Number of Salesforce users
- [ ] **C)** Data encryption standards
- [ ] **D)** Compliance certifications

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Security reviews focus on encryption, OAuth scopes, and certifications. A user count is not a security posture attribute.
 
 
</details>

### 3. Review the Apex trigger snippet. What is the primary scalability risk when this code runs on large data volumes?

```apex
trigger OpportunityTrigger on Opportunity (before insert, before update) {
    for (Opportunity opp : Trigger.new) {
        opp.Amount__c = opp.Amount * 1.2;
    }
}
```

- [ ] **A)** Asynchronous processing will scale without limits
- [ ] **B)** Synchronous execution nearing governor limits
- [ ] **C)** Triggers have no governor limits
- [ ] **D)** No DML means no performance risk

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> This trigger runs synchronously in the transaction and counts against governor limits, so it is a scalability concern as data volumes grow.
 
 
</details>


---

### **AppExchange**

### 4. What is a defining characteristic of a managed package in the AppExchange ecosystem?

- [ ] **A)** Vendors can push updates without impacting the customer's ability to customize certain metadata.
- [ ] **B)** It becomes a static template that the vendor can no longer update.
- [ ] **C)** It requires the customer to manually reinstall the package after every release.
- [ ] **D)** It removes all customer control over the package's metadata.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Managed packages allow vendors to release updates while still permitting customers to customize specific metadata. Unmanaged packages, in contrast, are essentially templates that become part of the org and increase long-term maintenance responsibilities.
 
 
</details>


---

### **Configuration and Setup**

### 5. What is the primary difference between managed and unmanaged packages when installed in the AppExchange ecosystem?

- [ ] **A)** Vendors can update it without destroying customer customizations.
- [ ] **B)** It cannot be modified by the customer ever.
- [ ] **C)** It remains fully editable source code.
- [ ] **D)** It never requires vendor updates.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Managed packages allow vendors to push updates while customers keep certain customizations; unmanaged packages become static, customer-owned templates.
 
 
</details>

### 6. Which areas should an Advanced Administrator review when assessing a solution's security and compliance posture?

- [ ] **A)** Data encryption standards
- [ ] **B)** OAuth scopes
- [ ] **C)** Compliance certifications such as SOC2 or HIPAA
- [ ] **D)** The color scheme of the user interface

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Security reviews must inspect encryption, OAuth scopes, and compliance certifications. User interface styling is not a security consideration.
 
 
</details>

### 7. The code block lists OAuth scopes requested by a Connected App. Which scope should be removed to align with least privilege?

```json
{
  "app": "Vendor Tool",
  "oauthScopes": ["profile", "email", "api", "full"]
}
```

- [ ] **A)** full
- [ ] **B)** api
- [ ] **C)** email
- [ ] **D)** profile

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'full' scope grants broad access to Salesforce data, violating least privilege; only the necessary scopes should be kept.
 
 
</details>

### 8. What is the primary risk of choosing an unmanaged package when frequent vendor updates are required?

- [ ] **A)** A massive maintenance burden
- [ ] **B)** Automatic loss of custom objects
- [ ] **C)** Immediate license expiration
- [ ] **D)** Cloud-based backup failure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An unmanaged package becomes part of the customer's org, so applying frequent vendor updates manually creates a significant maintenance burden.
 
 
</details>

### 9. Which items should be included when calculating the total cost of ownership for a third-party AppExchange solution?

- [ ] **A)** Implementation and training costs
- [ ] **B)** Specialized administration effort
- [ ] **C)** Impact on storage limits
- [ ] **D)** The vendor's logo design

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> TCO calculations include implementation, training, specialized administration, storage impact, and long-term migration costs, not branding elements.
 
 
</details>

### 10. The code block demonstrates a processing pattern for an external integration. What type of processing is shown?

```apex
trigger AccountScoreTrigger on Account (after insert) {
    for (Account acc : Trigger.new) {
        HttpRequest req = new HttpRequest();
        req.setEndpoint('https://scoring.example.com/api');
        Http http = new Http();
        http.send(req);
    }
}
```

- [ ] **A)** Synchronous trigger processing
- [ ] **B)** Asynchronous queueable processing
- [ ] **C)** Scheduled batch processing
- [ ] **D)** Platform event streaming

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code shows a synchronous callout inside a trigger, which can consume limits and reduce scalability. Asynchronous processing is often preferred.
 
 
</details>


---

### **Data Management**

### 11. What is the fundamental difference between managed and unmanaged packages on the AppExchange?

- [ ] **A)** Managed packages allow vendors to push updates while preserving customer customizations; unmanaged packages become part of the org and increase maintenance.
- [ ] **B)** Unmanaged packages are encrypted and require no maintenance; managed packages are always open source.
- [ ] **C)** Managed packages cannot be customized by customers; unmanaged packages allow full vendor updates automatically.
- [ ] **D)** Unmanaged packages are automatically upgraded by Salesforce; managed packages require manual customer upgrades.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Managed packages enable vendors to release updates without destroying customer metadata, whereas unmanaged packages are templates that become part of the org and create long-term maintenance responsibilities.
 
 
</details>

### 12. Which aspects should be scrutinized during a security and compliance assessment of an AppExchange solution? Select all that apply.

- [ ] **A)** Data encryption standards
- [ ] **B)** OAuth scopes and access permissions
- [ ] **C)** Compliance certifications such as SOC2 or HIPAA
- [ ] **D)** The number of end users in the customer org

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A security and compliance assessment should cover encryption standards, OAuth scopes, and certifications such as SOC2 or HIPAA. The number of end users is not part of this assessment.
 
 
</details>

### 13. Review the requested scopes in the provided configuration. Which security best practice is being violated?

```json
{
  "app": "Example App",
  "requested_oauth_scopes": [
    "full_access_all_data",
    "offline_access",
    "read_only"
  ],
  "compliance": ["SOC2"]
}
```

- [ ] **A)** Least privilege
- [ ] **B)** Single sign-on
- [ ] **C)** Data residency
- [ ] **D)** License assignment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The app requests full access to all data, which goes beyond the minimum necessary access and violates the principle of least privilege.
 
 
</details>


---

### **Object Manager and Lightning Apps**

### 14. In the context of Salesforce packaging, what key difference distinguishes a managed package from an unmanaged package?

- [ ] **A)** Vendor can push updates without breaking customizations
- [ ] **B)** Unmanaged packages support vendor-controlled updates
- [ ] **C)** Managed packages become part of the customer org
- [ ] **D)** Unmanaged packages preserve all custom metadata

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Managed packages allow vendor updates while preserving customer customizations; unmanaged packages become part of the org and increase maintenance responsibilities.
 
 
</details>

### 15. When evaluating Salesforce package types, which two true statements describe the nature and long-term impact of unmanaged packages?

- [ ] **A)** Become part of the customer org
- [ ] **B)** Increase long-term maintenance responsibilities
- [ ] **C)** Provide vendor-managed update paths
- [ ] **D)** Prevent all customer customizations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Unmanaged packages become part of the customer org, so they increase maintenance responsibilities and lack vendor-controlled upgrades.
 
 
</details>

### 16. Review the Apex trigger snippet. Which scalability concern should you associate with this synchronous processing approach?

```apex
trigger OpportunitySync on Opportunity (after insert) {
    for (Opportunity opp : Trigger.new) {
        update new Account(Id = opp.AccountId, Description = 'Synced');
    }
}
```

- [ ] **A)** May consume DML and CPU limits
- [ ] **B)** Avoids all governor limits
- [ ] **C)** Has no effect on performance
- [ ] **D)** Eliminates the need for asynchronous code

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Performing synchronous DML in a loop can consume DML and CPU governor limits; asynchronous processing is more scalable for growing data volumes.
 
 
</details>

### 17. During an AppExchange solution evaluation, which security-related aspect should an advanced administrator carefully examine before approving the app?

- [ ] **A)** Data encryption and OAuth scopes
- [ ] **B)** Feature list only
- [ ] **C)** Vendor office location
- [ ] **D)** Number of end users

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Security assessment should focus on encryption standards, OAuth scopes, and compliance certifications like SOC2 and HIPAA.
 
 
</details>

### 18. Which two elements should be included when evaluating the security and compliance posture of an AppExchange solution?

- [ ] **A)** Data encryption standards
- [ ] **B)** OAuth scopes
- [ ] **C)** Price per user
- [ ] **D)** Logo and branding

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Encryption standards and OAuth scopes are key security and compliance factors; pricing and branding are not part of this evaluation.
 
 
</details>

### 19. Review the Connected App configuration and identify the security principle violated by its broad OAuth scope request.

```json
{
  "oauthScopes": ["full", "refresh_token"],
  "adminConsentRequired": true
}
```

- [ ] **A)** Principle of least privilege
- [ ] **B)** Single sign-on
- [ ] **C)** Data residency
- [ ] **D)** Managed package updates

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Requesting broad scopes such as full and refresh_token violates least privilege; access should be limited to required objects and fields.
 
 
</details>


---

### **Productivity and Collaboration**

### 20. What is the fundamental distinction between managed and unmanaged packages in the AppExchange ecosystem?

- [ ] **A)** Managed packages can be edited directly by the installer; unmanaged packages remain independent of the org.
- [ ] **B)** Managed packages allow vendors to push upgrades while customers retain flexibility to customize certain metadata; unmanaged packages merge into the org and become the customer's responsibility.
- [ ] **C)** Managed packages are only available to Salesforce ISV partners; unmanaged packages are available to any admin.
- [ ] **D)** Managed packages do not count against data storage limits; unmanaged packages consume storage.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Managed packages are versioned and upgradeable, allowing the vendor to release code updates without taking over all customer customizations. Unmanaged packages become part of the org and are the customer's responsibility to maintain.
 
 
</details>

### 21. When evaluating a third-party AppExchange solution, which two factors directly relate to the principle of least privilege?

- [ ] **A)** OAuth scopes
- [ ] **B)** Requested permissions on Salesforce objects and fields
- [ ] **C)** Visualforce page styling
- [ ] **D)** Package version number

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Least privilege means the app should only request access needed to function. OAuth scopes define broad capabilities, while object and field permissions control specific data access.
 
 
</details>


---

### **User Management**

### 22. What is the key difference between managed and unmanaged packages in AppExchange?

- [ ] **A)** Managed packages allow vendors to update code without preventing customers from customizing certain metadata; unmanaged packages become part of the org and add maintenance responsibility.
- [ ] **B)** Managed packages are fully customizable at source-code level; unmanaged packages are code-locked.
- [ ] **C)** Both package types are maintained by the vendor, so there is no maintenance impact on the customer.
- [ ] **D)** Unmanaged packages allow vendor updates without touching customer data; managed packages require manual migration.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Managed packages support vendor updates while permitting selected customer customizations, whereas unmanaged packages are copied into the org and require the customer to maintain them.
 
 
</details>

### 23. Which evaluation areas are part of a security and compliance assessment for a third-party AppExchange solution? Select all that apply.

- [ ] **A)** Data encryption standards
- [ ] **B)** OAuth scopes
- [ ] **C)** App listing popularity
- [ ] **D)** Compliance certifications such as SOC2 and HIPAA

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> A security and compliance assessment includes data encryption standards, OAuth scopes, and compliance certifications such as SOC2 or HIPAA, but not the app listing popularity.
 
 
</details>

### 24. Review the Apex trigger snippet in the code block. Which AppExchange evaluation concern is most closely associated with this implementation pattern?

```apex
trigger ThirdPartyCallout on Account (after insert) {
    List<Account> accounts = Trigger.new;
    for (Account acct : accounts) {
        // Synchronous callout to external system
    }
}
```

- [ ] **A)** Technical Debt & Scalability – synchronous callouts inside a loop may hit governor limits
- [ ] **B)** The Feature Trap – this trigger makes the app feature-rich
- [ ] **C)** The Integration Blindspot – the trigger uses point-to-point integration only
- [ ] **D)** License assignment neglect – users will not automatically receive the package license

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A trigger that performs synchronous external callouts per record can consume DML, callout, and CPU limits, creating scalability and performance risk as data volume grows.
 
 
</details>

### 25. Why is it important to review the OAuth scopes requested by a Connected App during an AppExchange evaluation?

- [ ] **A)** To ensure the app has the maximum possible permissions for future integrations
- [ ] **B)** To comply with the principle of least privilege
- [ ] **C)** To confirm the app can access all custom objects without restrictions
- [ ] **D)** To guarantee the app is a managed package

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Reviewing OAuth scopes ensures the third-party tool requests only the access it truly needs, aligning with the principle of least privilege.
 
 
</details>


---

### **Workflow/Process Automation**

### 26. What is a key characteristic of managed packages?

- [ ] **A)** Vendors can update code without affecting customizations
- [ ] **B)** Becomes part of the org, increasing maintenance
- [ ] **C)** Cannot receive updates from the vendor
- [ ] **D)** Requires modifying source code for every change

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Managed packages allow vendors to release updates while leaving the customer's ability to customize certain metadata intact, unlike unmanaged packages.
 
 
</details>

### 27. Which security aspects must be evaluated for an AppExchange solution?

- [ ] **A)** Data encryption standards
- [ ] **B)** OAuth scopes
- [ ] **C)** Compliance certifications
- [ ] **D)** User interface color scheme

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Security assessments must include data encryption standards, OAuth scopes, and compliance certifications such as SOC2 or HIPAA.
 
 
</details>

### 28. An administrator is reviewing a solution with the following automation pattern. What risk should be flagged?

```apex
trigger AccountTrigger on Account (after insert) { for (Account acc : Trigger.new) { makeCallout(acc.Id); } }
```

- [ ] **A)** It may hit governor limits due to synchronous processing
- [ ] **B)** It is fully secure
- [ ] **C)** It improves data storage
- [ ] **D)** It eliminates the need for testing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The pattern processes work synchronously inside a loop, increasing the risk of hitting governor limits as data volume grows.
 
 
</details>

### 29. Which element should be considered when calculating total cost of ownership?

- [ ] **A)** Implementation and training costs
- [ ] **B)** Only the monthly license fee
- [ ] **C)** The vendor's office location
- [ ] **D)** The number of app colors

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TCO includes implementation, training, specialized administration, potential storage impact, and the long-term cost of migrating away from the tool.
 
 
</details>

### 30. Which are common traps when evaluating AppExchange solutions?

- [ ] **A)** Feature Trap
- [ ] **B)** Unmanaged Package Oversight
- [ ] **C)** Integration Blindspot
- [ ] **D)** Reviewing OAuth scopes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Common traps include focusing on features only, choosing unmanaged packages when updates are needed, and ignoring integration overhead.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Salesforce/Salesforce%20Certified%20Platform%20Developer%20I.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Salesforce Certified Platform Developer I</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Developer Fundamentals](#developer-fundamentals) (8 questions)
- [Process Automation and Logic](#process-automation-and-logic) (8 questions)
- [Testing, Debugging, and Deployment](#testing-debugging-and-deployment) (6 questions)
- [User Interface](#user-interface) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-24T21:53:30.214Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Developer Fundamentals | 8 |
| Process Automation and Logic | 8 |
| Testing, Debugging, and Deployment | 6 |
| User Interface | 8 |

---

### **Developer Fundamentals**

### 1. What type of cloud architecture is the Salesforce platform built on?

- [ ] **A)** Peer-to-peer cloud architecture
- [ ] **B)** Multi-tenant cloud architecture
- [ ] **C)** Single-tenant dedicated infrastructure
- [ ] **D)** Client-server architecture with isolated resources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Salesforce is built on a multi-tenant architecture where compute, storage, and application resources are shared securely among customers while data is logically isolated.
 
 
</details>

### 2. Which of the following are true about Lightning Experience? Select all that apply.

- [ ] **A)** It is built natively on the Salesforce Lightning Design System (SLDS)
- [ ] **B)** It requires all customizations to be written in Apex
- [ ] **C)** It is a component-based user interface framework using LWC and Aura
- [ ] **D)** It replaced Salesforce Classic as the modern user interface

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Lightning Experience is a modern, component-based UI framework built on LWC and Aura, uses SLDS, and replaced Salesforce Classic.
 
 
</details>

### 3. Examine the Apex trigger in the code block. What is the main problem with this implementation?

```apex
trigger AccountExample on Account (after insert, after update) {
    for (Account acc : Trigger.new) {
        List<Contact> contacts = [SELECT Id FROM Contact WHERE AccountId = :acc.Id];
    }
}
```

- [ ] **A)** SOQL query is executed inside a for loop
- [ ] **B)** The trigger is missing a try-catch block
- [ ] **C)** No sharing keyword is used
- [ ] **D)** The variable 'contacts' is undeclared

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The SOQL query inside the for loop can exhaust the 100-query limit when many records are processed.
 
 
</details>

### 4. What is the maximum number of SOQL queries allowed in a single synchronous transaction?

- [ ] **A)** 50
- [ ] **B)** 100
- [ ] **C)** 150
- [ ] **D)** 200

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Salesforce enforces a maximum of 100 SOQL queries per synchronous transaction.
 
 
</details>

### 5. Which statements about master-detail relationships are correct? Select all that apply.

- [ ] **A)** Child records inherit security and sharing from the parent record
- [ ] **B)** Deleting a parent record automatically deletes its child records
- [ ] **C)** Roll-up summary fields can be created on the parent object
- [ ] **D)** Child records keep an owner independent from the parent record

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Master-detail relationships cascade deletes, inherit sharing and ownership from the parent, and allow roll-up summary fields on the parent.
 
 
</details>

### 6. Review the validation rule formula in the code block. What business rule does it enforce?

```formula
AND(ISPICKVAL(Status__c, 'Active'), ISBLANK(Region__c))
```

- [ ] **A)** Region is required whenever Status is Active
- [ ] **B)** Status must be Active before Region can be entered
- [ ] **C)** Only Active records may have a Region
- [ ] **D)** Active records must always have an empty Region

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The formula returns true when Status is Active and Region is blank, so the validation rule blocks saves in that situation.
 
 
</details>

### 7. What is the purpose of Organization-Wide Defaults (OWDs)?

- [ ] **A)** They grant additional record access based on criteria
- [ ] **B)** They set the baseline record access for users who do not own a record
- [ ] **C)** They provide ad-hoc sharing for individual records
- [ ] **D)** They define field-level security for profiles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Organization-Wide Defaults establish the most restrictive baseline level of record access for users who do not own a record.
 
 
</details>

### 8. Which statements about sharing rules are true? Select all that apply.

- [ ] **A)** Sharing rules can restrict access below the OWD baseline
- [ ] **B)** Sharing rules can be based on record ownership or criteria
- [ ] **C)** Sharing rules are additive and cannot restrict access further than OWD
- [ ] **D)** Sharing rules can grant additional access to groups of users

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C, D**
 
> 💡  **Explanation** 
> 
> Sharing rules only extend access beyond OWD baselines and can be ownership-based or criteria-based.
 
 
</details>


---

### **Process Automation and Logic**

### 9. What is the primary purpose of the Trigger Handler pattern in Apex, and why do developers use it?

- [ ] **A)** To delegate execution to a dedicated handler class
- [ ] **B)** To write all logic inline inside the trigger body
- [ ] **C)** To create multiple triggers per object
- [ ] **D)** To replace Flow and Process Builder entirely

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Trigger Handler pattern moves business logic out of the trigger body into a dedicated handler class, improving testability, maintainability, and execution control.
 
 
</details>

### 10. Which two statements correctly describe Apex interfaces and their role in maintainable business logic in Salesforce applications?

- [ ] **A)** Interfaces define method signatures without implementation
- [ ] **B)** Interfaces enable polymorphic behavior across classes
- [ ] **C)** Interfaces can contain concrete method bodies
- [ ] **D)** Interfaces can be instantiated directly

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Interfaces define contracts of method signatures without implementation and enable polymorphic, decoupled design. They cannot be instantiated or contain concrete method bodies.
 
 
</details>

### 11. What architectural pattern is demonstrated by the Apex trigger and handler class code block below?

```apex
trigger AccountTrigger on Account (after insert) {
    AccountHandler.handleAfterInsert(Trigger.new);
}
```

- [ ] **A)** Trigger Handler pattern
- [ ] **B)** Singleton pattern
- [ ] **C)** Strategy pattern
- [ ] **D)** Factory pattern

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The trigger delegates its after-insert logic to AccountHandler, which is the core of the Trigger Handler pattern.
 
 
</details>

### 12. What does bulkification in Apex require developers to do when processing records in triggers, and why is it important?

- [ ] **A)** Process collections of records instead of single records
- [ ] **B)** Always use one DML statement per record
- [ ] **C)** Avoid using collections in triggers
- [ ] **D)** Write a separate trigger for each record type

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Bulkification requires processing collections of records together to avoid hitting Salesforce governor limits during large data operations.
 
 
</details>

### 13. Which two items are valid Apex trigger context variables used to evaluate record state during execution?

- [ ] **A)** Trigger.new
- [ ] **B)** Trigger.isExecuting
- [ ] **C)** Trigger.query
- [ ] **D)** Trigger.result

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Trigger.new and Trigger.isExecuting are valid context variables. Trigger.query and Trigger.result are not part of the Apex trigger context.
 
 
</details>

### 14. What does the Apex code block below define as an Apex programming construct for business logic?

```apex
public interface FinancialValidation {
    Boolean validate(Account acc);
}
```

- [ ] **A)** An interface
- [ ] **B)** A concrete class
- [ ] **C)** An abstract class
- [ ] **D)** A trigger

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code defines an interface with an abstract method signature and no implementation, enabling polymorphic behavior.
 
 
</details>

### 15. What is a common drawback of putting complex business logic directly inside a trigger body in Salesforce?

- [ ] **A)** It prevents code reuse and makes testing difficult
- [ ] **B)** It guarantees better execution order across triggers
- [ ] **C)** It automatically bulkifies all DML operations
- [ ] **D)** It eliminates the need for handler classes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Inline logic prevents reuse and hampers testing. The Trigger Handler pattern avoids this by separating business logic into dedicated classes.
 
 
</details>

### 16. Which two practices are recommended when designing a trigger framework for multiple trigger events and bulk records?

- [ ] **A)** Use a single trigger per sObject
- [ ] **B)** Delegate execution to handler classes
- [ ] **C)** Create multiple triggers per object to control order
- [ ] **D)** Place SOQL queries directly inside for loops

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A trigger framework uses one trigger per object and delegates logic to handler classes, ensuring orderly, maintainable, and bulkified execution.
 
 
</details>


---

### **Testing, Debugging, and Deployment**

### 17. What is the minimum Apex code coverage percentage required by Salesforce before a deployment to production can succeed?

- [ ] **A)** 75%
- [ ] **B)** 100%
- [ ] **C)** 50%
- [ ] **D)** 85%

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Salesforce requires at least 75% aggregate coverage of all Apex code before deployment. Every trigger must also have coverage.
 
 
</details>

### 18. Which of the following are valid System.assert methods used in Apex unit tests? Select all that apply.

- [ ] **A)** System.assertEquals()
- [ ] **B)** System.assertNotEquals()
- [ ] **C)** System.assert()
- [ ] **D)** System.debug()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Apex tests validate expected outcomes with System.assertEquals(), System.assertNotEquals(), and System.assert(). System.debug() writes logs rather than making assertions.
 
 
</details>

### 19. Review the Apex test method below. What is the primary purpose of the two calls that surround the update operation?

```apex
@IsTest
private class OpportunityTest {
    @IsTest
    static void testBulkUpdate() {
        List<Opportunity> opps = new List<Opportunity>();
        for (Integer i = 0; i < 200; i++) {
            opps.add(new Opportunity(Name='Opp' + i, StageName='Prospecting', CloseDate=Date.today(), Amount=100));
        }
        insert opps;
        Test.startTest();
        update opps;
        Test.stopTest();
    }
}
```

- [ ] **A)** Reset governor limits for the core test transaction
- [ ] **B)** Insert test data more quickly
- [ ] **C)** Generate a debug log
- [ ] **D)** Increase code coverage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Test.startTest() and Test.stopTest() reset governor limits for the tested transaction and isolate asynchronous operations so bulk behavior is measured accurately.
 
 
</details>

### 20. Which Developer Console feature allows a developer to group and execute multiple Apex test classes together?

- [ ] **A)** Test Suite
- [ ] **B)** Trace Flag
- [ ] **C)** Query Editor
- [ ] **D)** Execution Overview

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Test suites group related Apex test classes and can be executed together in the Developer Console to validate functional areas.
 
 
</details>

### 21. Which statements about Salesforce code coverage are true? Select all that apply.

- [ ] **A)** It is measured across all non-test Apex code in the organization.
- [ ] **B)** Every Apex trigger must have some test coverage to be deployed.
- [ ] **C)** The Developer Console shows line-by-line coverage information.
- [ ] **D)** Every class must individually meet the 75% requirement.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Coverage is calculated across all non-test Apex code; each trigger needs coverage, and the Developer Console shows line-by-line coverage. It is not per-class.
 
 
</details>

### 22. Examine the Apex code below. What is the primary effect of the second line?

```apex
String accountName = 'Acme';
System.debug(LoggingLevel.ERROR, 'Account name: ' + accountName);
```

- [ ] **A)** Adds a diagnostic message to the debug log
- [ ] **B)** Updates the Account record in the database
- [ ] **C)** Increases the organization's Apex code coverage
- [ ] **D)** Raises the governor limit for SOQL queries

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> System.debug() writes diagnostic runtime information to the debug log. It does not modify data, coverage, or governor limits.
 
 
</details>


---

### **User Interface**

### 23. What is Lightning App Builder primarily used for?

- [ ] **A)** Point-and-click UI creation
- [ ] **B)** Writing custom Apex code
- [ ] **C)** Managing data backups
- [ ] **D)** Creating email templates

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Lightning App Builder is a point-and-click tool for assembling custom user interfaces for Lightning Experience and mobile applications.
 
 
</details>

### 24. Which component types can be added to a Lightning record page using Lightning App Builder? Select all that apply.

- [ ] **A)** Lightning Web Components
- [ ] **B)** Aura components
- [ ] **C)** Standard components
- [ ] **D)** Apex trigger classes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Lightning App Builder allows developers to assemble standard components, custom Lightning Web Components, and Aura components onto pages.
 
 
</details>

### 25. A developer adds a custom component to an Opportunity Lightning Record Page. Looking at the placeholder metadata snippet, what declarative configuration should be used to show the component only when Stage equals Negotiation?

```xml
<flexiPage>
    <itemInstances>
        <componentName>cCommissionCalculator</componentName>
    </itemInstances>
</flexiPage>
```

- [ ] **A)** Component visibility filters
- [ ] **B)** Custom JavaScript condition
- [ ] **C)** Apex controller override
- [ ] **D)** Page layout assignment rule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Component visibility filters in Lightning App Builder conditionally show components based on field values without requiring custom code.
 
 
</details>

### 26. What is the underlying metadata architecture for customizable page layouts in Lightning App Builder?

- [ ] **A)** FlexiPage
- [ ] **B)** Compact Layout
- [ ] **C)** Page Layout
- [ ] **D)** Record Type

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> FlexiPages are the metadata architecture used by Lightning App Builder for customizable page layouts and can be deployed via Metadata API.
 
 
</details>

### 27. Which criteria can dynamic component visibility filters use in Lightning App Builder? Select all that apply.

- [ ] **A)** Record field values
- [ ] **B)** Device type
- [ ] **C)** User permissions
- [ ] **D)** Browser history

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Visibility filters can evaluate record fields, device type, and user permissions to show or hide components dynamically.
 
 
</details>

### 28. This configuration file defines a Lightning Web Component's metadata. What does the target declaration allow the component to do?

```xml
<?xml version="1.0" encoding="UTF-8"?>
<LightningComponentBundle xmlns="http://soap.sforce.com/2006/04/metadata">
    <apiVersion>58.0</apiVersion>
    <isExposed>true</isExposed>
    <targets>
        <target>lightning__RecordPage</target>
    </targets>
</LightningComponentBundle>
```

- [ ] **A)** Be placed on a Lightning record page
- [ ] **B)** Run as a batch Apex job
- [ ] **C)** Be used only inside Visualforce
- [ ] **D)** Automatically create a custom object

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The target lightning__RecordPage exposes the component as an available option for Lightning record page customization.
 
 
</details>

### 29. Which decorator exposes a JavaScript property as a public property in a Lightning Web Component?

- [ ] **A)** @api
- [ ] **B)** @track
- [ ] **C)** @wire
- [ ] **D)** @salesforce

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The @api decorator marks a property as public, allowing parent components to pass values into the LWC.
 
 
</details>

### 30. Which files are part of a Lightning Web Component bundle? Select all that apply.

- [ ] **A)** .html template
- [ ] **B)** .js class
- [ ] **C)** .js-meta.xml configuration
- [ ] **D)** .controller.js file

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> An LWC bundle contains an HTML template, a JavaScript class, and a JavaScript metadata configuration file, plus optional resources such as CSS.
 
 
</details>

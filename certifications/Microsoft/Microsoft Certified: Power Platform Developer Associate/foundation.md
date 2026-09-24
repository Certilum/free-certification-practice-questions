<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Microsoft%20Certified-%20Power%20Platform%20Developer%20Associate.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Microsoft Certified: Power Platform Developer Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Build Power Platform solutions](#build-power-platform-solutions) (8 questions)
- [Create a technical design](#create-a-technical-design) (4 questions)
- [Develop integrations](#develop-integrations) (5 questions)
- [Extend the platform](#extend-the-platform) (4 questions)
- [Extend the user experience](#extend-the-user-experience) (4 questions)
- [Implement Power Apps improvements](#implement-power-apps-improvements) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:21.280Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Build Power Platform solutions | 8 |
| Create a technical design | 4 |
| Develop integrations | 5 |
| Extend the platform | 4 |
| Extend the user experience | 4 |
| Implement Power Apps improvements | 5 |

---

### **Build Power Platform solutions**

### 1. In Microsoft Power Platform Dataverse development, which interface must every plug-in class implement to satisfy the required contract?

- [ ] **A)** The IPlugin interface
- [ ] **B)** The IPluginExecutionContext object
- [ ] **C)** The IOrganizationService interface
- [ ] **D)** The CodeActivity base class

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Every plug-in must implement the IPlugin interface and provide the Execute method, which receives the IPluginExecutionContext to perform Dataverse logic.
 
 
</details>

### 2. Based on the playbook, in Dataverse plug-in development, which execution pipeline stages are valid for registering a plug-in?

- [ ] **A)** Pre-validation stage
- [ ] **B)** Pre-operation stage
- [ ] **C)** Post-operation stage
- [ ] **D)** Post-retrieval stage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Dataverse plug-ins can be registered in Pre-validation, Pre-operation, or Post-operation stages. These stages define when logic runs in relation to the transaction.
 
 
</details>

### 3. Review the plug-in code example below. Which critical safeguard is missing to prevent recursive execution?

```csharp
public class MyPlugin : IPlugin
{
    public void Execute(IServiceProvider serviceProvider)
    {
        var context = (IPluginExecutionContext)serviceProvider.GetService(typeof(IPluginExecutionContext));
        var serviceFactory = (IOrganizationServiceFactory)serviceProvider.GetService(typeof(IOrganizationServiceFactory));
        var service = serviceFactory.CreateOrganizationService(context.UserId);
    }
}
```

- [ ] **A)** Depth check
- [ ] **B)** Stage check
- [ ] **C)** Transaction check
- [ ] **D)** Entity check

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A depth check is required to prevent recursive self-triggering. Without it, a plug-in can create an infinite loop and cause a platform timeout.
 
 
</details>

### 4. According to the playbook, what runtime information does the IPluginExecutionContext make available to a plug-in during execution?

- [ ] **A)** Entity, attributes, and user identity
- [ ] **B)** Browser and UI components
- [ ] **C)** Azure subscription credentials
- [ ] **D)** Workflow process definitions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IPluginExecutionContext provides vital metadata such as the entity, attributes, and user identity needed to perform logic in a Dataverse plug-in.
 
 
</details>

### 5. According to the playbook, which statements about transaction management in Dataverse plug-in execution are correct?

- [ ] **A)** Runs in the database transaction
- [ ] **B)** Failure rolls back the operation
- [ ] **C)** Pre-validation runs before transaction
- [ ] **D)** All exceptions are ignored

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Plug-ins execute inside the database transaction. If an exception is thrown, the original data change is rolled back. Pre-validation runs before the transaction starts.
 
 
</details>

### 6. In the custom activity code presented, which method must be implemented to satisfy the activity contract?

```csharp
public class MyActivity : CodeActivity
{
    // TODO: implement required method
}
```

- [ ] **A)** Execute(CodeActivityContext context)
- [ ] **B)** Execute(IServiceProvider serviceProvider)
- [ ] **C)** Run(WorkflowContext context)
- [ ] **D)** Start(ActivityContext context)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A custom activity inherits from CodeActivity and must override Execute(CodeActivityContext context), or the class will fail to compile and run.
 
 
</details>

### 7. According to the playbook, what service is primarily used to perform CRUD operations on Dataverse entities from within a plug-in?

- [ ] **A)** IOrganizationService interface
- [ ] **B)** IOrganizationServiceFactory interface
- [ ] **C)** IPluginExecutionContext object
- [ ] **D)** CodeActivityContext object

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IOrganizationService is the primary gateway for CRUD operations on Dataverse entities inside plug-in code, created via the service factory.
 
 
</details>

### 8. Based on the playbook, which of the following are common traps when developing Dataverse plug-ins?

- [ ] **A)** Confusing Pre-operation with Pre-validation
- [ ] **B)** Forgetting the depth check
- [ ] **C)** Using client-side libraries
- [ ] **D)** Calling IOrganizationService.Create

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Common traps include confusing Pre-operation with Pre-validation, forgetting depth checks, and attempting to use client-side libraries in plug-ins.
 
 
</details>


---

### **Create a technical design**

### 9. Which interface must every Dataverse plug-in implement?

- [ ] **A)** IPlugin
- [ ] **B)** IPluginExecutionContext
- [ ] **C)** IOrganizationService
- [ ] **D)** CodeActivity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Every plug-in must implement the IPlugin interface, whose Execute method receives the execution context.
 
 
</details>

### 10. Which stages of the event execution pipeline can a plug-in be registered in? Select all that apply.

- [ ] **A)** Pre-validation
- [ ] **B)** Pre-operation
- [ ] **C)** Post-operation
- [ ] **D)** Pre-delete

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Plug-ins are registered in Pre-validation, Pre-operation, or Post-operation; Pre-delete is not a pipeline stage.
 
 
</details>

### 11. Review the code block. Which execution context type is being retrieved for the plug-in logic?

```csharp
public void Execute(IServiceProvider serviceProvider)
{
    var context = (IPluginExecutionContext)serviceProvider.GetService(typeof(IPluginExecutionContext));
}
```

- [ ] **A)** IPluginExecutionContext
- [ ] **B)** IWorkflowContext
- [ ] **C)** CodeActivityContext
- [ ] **D)** IServiceProvider

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code casts the service provider to IPluginExecutionContext, the interface that provides plug-in runtime data.
 
 
</details>

### 12. Which base class must a custom workflow activity inherit from?

- [ ] **A)** System.Activities.CodeActivity
- [ ] **B)** Microsoft.Xrm.Sdk.Client.ServiceContext
- [ ] **C)** System.Activities.NativeActivity
- [ ] **D)** System.Workflow.ComponentModel.Activity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Custom workflow activities inherit from System.Activities.CodeActivity and implement its Execute method.
 
 
</details>


---

### **Develop integrations**

### 13. In the Dataverse event execution pipeline, before the database transaction starts, which stage occurs?

- [ ] **A)** Pre-validation
- [ ] **B)** Pre-operation
- [ ] **C)** Post-operation
- [ ] **D)** Post-validation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Pre-validation is the stage that occurs before the database transaction starts. Pre-operation occurs within the transaction, and Post-operation occurs after the core operation.
 
 
</details>

### 14. Which two statements correctly describe plug-in execution and the context depth trap?

- [ ] **A)** Plug-ins run within the database transaction of the triggering event.
- [ ] **B)** Plug-ins can safely use client-side libraries to access the user's browser components.
- [ ] **C)** Checking the context depth prevents a plug-in from recursively triggering itself.
- [ ] **D)** Pre-operation executes before the database transaction starts.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The playbook states that plug-ins run within the database transaction of the triggering event, and checking depth prevents infinite recursive calls. Client-side libraries are not available in plug-ins, and Pre-operation occurs within the transaction, not before it.
 
 
</details>

### 15. Review the plug-in code excerpt. What condition should be added at the start of the Execute method to prevent recursive execution?

```csharp
public void Execute(IServiceProvider serviceProvider)
{
    var context = (IPluginExecutionContext)serviceProvider.GetService(typeof(IPluginExecutionContext));
    var serviceFactory = (IOrganizationServiceFactory)serviceProvider.GetService(typeof(IOrganizationServiceFactory));
    var service = serviceFactory.CreateOrganizationService(context.UserId);
    // Missing guard condition
    // Remaining plug-in logic
}
```

- [ ] **A)** context.Depth > 1
- [ ] **B)** context.MessageName == "Create"
- [ ] **C)** context.Stage == 10
- [ ] **D)** context.IsInTransaction == true

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The context depth property indicates how many times the plug-in has been called in the current operation. Checking depth prevents a plug-in from triggering itself recursively, which can cause a platform timeout.
 
 
</details>

### 16. What programmatic contract must every plug-in implement?

- [ ] **A)** IPlugin
- [ ] **B)** IWorkflowContext
- [ ] **C)** IOrganizationServiceFactory
- [ ] **D)** CodeActivity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IPlugin is the core programmatic contract for plug-ins. It requires the Execute method, which receives an IPluginExecutionContext.
 
 
</details>

### 17. Which three statements are true regarding custom workflow activities?

- [ ] **A)** Custom workflow activities inherit from System.Activities.CodeActivity.
- [ ] **B)** InputArgument<T> and OutputArgument<T> are used for data exchange with the workflow engine.
- [ ] **C)** Custom workflow activities are triggered directly by Dataverse record events such as Create or Update.
- [ ] **D)** The IWorkflowContext exposes runtime information such as the target entity and the triggering user.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> CodeActivity inheritance, typed input/output arguments, and IWorkflowContext are core to custom workflow activities. Direct event triggering describes plug-ins, not workflow activities.
 
 
</details>


---

### **Extend the platform**

### 18. In which execution pipeline stage does a plug-in run after the main data operation has completed?

- [ ] **A)** Pre-validation
- [ ] **B)** Pre-operation
- [ ] **C)** Post-operation
- [ ] **D)** Pre-commit

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Post-operation is the stage after the main operation, allowing plug-in logic to run once data changes have been made.
 
 
</details>

### 19. Which of the following are registered execution pipeline stages for plug-ins according to the document? Select all that apply.

- [ ] **A)** Pre-validation
- [ ] **B)** Pre-operation
- [ ] **C)** Post-operation
- [ ] **D)** Post-validation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The document lists Pre-validation, Pre-operation, and Post-operation as the execution pipeline stages. Post-validation is not a valid stage.
 
 
</details>

### 20. Given the following C# code block, which pattern is used to create an IOrganizationService inside a plug-in?

```csharp
var serviceFactory = (IOrganizationServiceFactory)serviceProvider.GetService(typeof(IOrganizationServiceFactory));
var service = serviceFactory.CreateOrganizationService(context.UserId);
```

- [ ] **A)** Service Provider Pattern
- [ ] **B)** Singleton Pattern
- [ ] **C)** Adapter Pattern
- [ ] **D)** Event Pipeline Pattern

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code uses IOrganizationServiceFactory from the service provider to create IOrganizationService, which demonstrates the Service Provider Pattern.
 
 
</details>

### 21. According to the document, what happens if a plug-in fails and throws an exception during execution?

- [ ] **A)** Only the plug-in's data modifications are rolled back
- [ ] **B)** The entire operation, including the original data change, is rolled back
- [ ] **C)** The transaction is committed but the exception is recorded
- [ ] **D)** The database transaction is paused for manual handling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Plug-ins run within the database transaction of the triggering event, so an exception rolls back the entire operation, preserving data consistency.
 
 
</details>


---

### **Extend the user experience**

### 22. In Dataverse, what is the core programmatic contract that every custom plug-in must implement?

- [ ] **A)** IPlugin
- [ ] **B)** IWorkflowContext
- [ ] **C)** IOrganizationService
- [ ] **D)** CodeActivity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Every plug-in must implement the IPlugin interface, which defines the Execute method. This is the core programmatic contract for plug-in execution.
 
 
</details>

### 23. Which two statements correctly describe the differences between Pre-validation and Pre-operation stages?

- [ ] **A)** Pre-validation occurs before the database transaction starts
- [ ] **B)** Pre-operation runs inside the database transaction
- [ ] **C)** Pre-operation occurs before Pre-validation
- [ ] **D)** Post-operation runs before the database transaction

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Pre-validation runs before the transaction starts; Pre-operation runs inside the transaction. Mixing these up can cause logic to execute at the wrong time.
 
 
</details>

### 24. Review the code sample and explain what runtime problem the depth check prevents in this plug-in.

```csharp
public class OpportunityPlugin : IPlugin
{
    public void Execute(IServiceProvider serviceProvider)
    {
        var context = (IPluginExecutionContext)serviceProvider.GetService(typeof(IPluginExecutionContext));
        if (context.Depth > 1)
        {
            return;
        }
        // Additional business logic here
    }
}
```

- [ ] **A)** Prevents recursive execution
- [ ] **B)** Measures database transaction timeout
- [ ] **C)** Verifies the user is the system admin
- [ ] **D)** Checks if the entity exists

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Checking Depth prevents a plug-in from recursively triggering itself, which can cause an infinite loop and platform timeout.
 
 
</details>

### 25. What happens to the complete Dataverse transaction if a plug-in throws an unhandled exception?

- [ ] **A)** Entire transaction is rolled back
- [ ] **B)** Only the plug-in’s changes are rolled back
- [ ] **C)** The operation is committed with an error log
- [ ] **D)** The exception is ignored and execution continues

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Plug-ins run inside the triggering event’s database transaction. If a plug-in throws an exception, the whole transaction is rolled back, preserving consistency.
 
 
</details>


---

### **Implement Power Apps improvements**

### 26. In the Dataverse event pipeline, which interface must every plug-in implement to define its execution logic?

- [ ] **A)** IPlugin
- [ ] **B)** IPluginExecutionContext
- [ ] **C)** IOrganizationService
- [ ] **D)** IOrganizationServiceFactory

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The IPlugin interface defines the Execute method, which every plug-in must implement to handle Dataverse events. This is the core programmatic contract for all plug-ins.
 
 
</details>

### 27. Within the plug-in execution pipeline, which two stages run while the database transaction is active?

- [ ] **A)** Pre-validation
- [ ] **B)** Pre-operation
- [ ] **C)** Post-operation
- [ ] **D)** Post-validation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Pre-validation occurs before the database transaction begins. Pre-operation and Post-operation run while the transaction is active, so failures can roll back the full operation.
 
 
</details>

### 28. Review the plug-in code snippet. What is the purpose of the service variable created through the service factory?

```csharp
var serviceFactory = (IOrganizationServiceFactory)serviceProvider.GetService(typeof(IOrganizationServiceFactory));
var service = serviceFactory.CreateOrganizationService(context.UserId);
```

- [ ] **A)** Perform CRUD operations on Dataverse records
- [ ] **B)** Register the plug-in for an event
- [ ] **C)** Access browser UI components
- [ ] **D)** Start a database transaction

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The IOrganizationServiceFactory creates an IOrganizationService instance, which is the primary gateway for CRUD operations on Dataverse records within plug-in code.
 
 
</details>

### 29. Which administrative tool is used to deploy, register, and configure plug-in assemblies and steps in Dataverse?

- [ ] **A)** Plugin Registration Tool
- [ ] **B)** Power Apps Checker
- [ ] **C)** Solution Packager
- [ ] **D)** Data Migration Tool

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Plugin Registration Tool (PRT) is the administrative utility used to deploy, register, and configure plug-in assemblies, including defining the message, entity, and stage.
 
 
</details>

### 30. According to common plug-in development traps, which two practices should a developer apply to avoid platform issues?

- [ ] **A)** Check the execution context depth
- [ ] **B)** Use client-side libraries in server-side code
- [ ] **C)** Assume rollback is handled automatically
- [ ] **D)** Avoid UI libraries in server-side logic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Checking the Depth property prevents recursive plug-in execution and platform timeouts. Plug-ins cannot access client-side UI components, so UI-centric libraries should not be used.
 
 
</details>

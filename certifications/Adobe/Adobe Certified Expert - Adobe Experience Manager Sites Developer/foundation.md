<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Adobe/Adobe%20Certified%20Expert.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Adobe Certified Expert - Adobe Experience Manager Sites Developer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [AEM Development](#aem-development) (10 questions)
- [Building Accessible and Responsive Sites](#building-accessible-and-responsive-sites) (6 questions)
- [Configuring AEM for a Project](#configuring-aem-for-a-project) (7 questions)
- [Site Administration and Content Management](#site-administration-and-content-management) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:02.144Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| AEM Development | 10 |
| Building Accessible and Responsive Sites | 6 |
| Configuring AEM for a Project | 7 |
| Site Administration and Content Management | 7 |

---

### **AEM Development**

### 1. What is the purpose of the sling:resourceSuperType property in a proxy component?

- [ ] **A)** Defines the resource type for rendering
- [ ] **B)** Points to a parent component to inherit behavior
- [ ] **C)** Sets the default category for client libraries
- [ ] **D)** Stores the component's dialog definition

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The sling:resourceSuperType sets the parent component for inheritance, enabling the proxy pattern without copying resource types.
 
 
</details>

### 2. Which annotations are valid for creating a Sling Model? (Select two)

- [ ] **A)** @Model
- [ ] **B)** @SlingServlet
- [ ] **C)** @Inject
- [ ] **D)** @Component

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> @Model marks the class as a Sling Model; @Inject is used for dependency injection into the model.
 
 
</details>

### 3. Review the HTL code snippet. What does the data-sly-use attribute do?

```html
<div data-sly-use.myModel="com.example.models.MyModel">${myModel.title}</div>
```

- [ ] **A)** Includes a client-side JavaScript library
- [ ] **B)** Loads a Java Use-API object and makes it available in the template
- [ ] **C)** Applies a CSS class to the element
- [ ] **D)** Defines a reusable template fragment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> data-sly-use instantiates a server-side Java or JavaScript object, exposing its methods and properties to the HTL template.
 
 
</details>

### 4. Where are editable template policies stored in the AEM repository?

- [ ] **A)** /apps/
- [ ] **B)** /content/
- [ ] **C)** /conf/
- [ ] **D)** /etc/designs/

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Editable template policies are stored under /conf/<project>/settings/wcm/policies/.
 
 
</details>

### 5. Which properties must be set for a client library folder under /apps to be served via the proxy path? (Select two)

- [ ] **A)** allowProxy = true
- [ ] **B)** categories
- [ ] **C)** jcr:primaryType = cq:ClientLibraryFolder
- [ ] **D)** dependencies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> allowProxy=true enables the proxy path; categories is needed for the clientlib to be included by components.
 
 
</details>

### 6. Refer to the overlay path: /apps/project/components/text. What does the Sling Resource Merger do when a component requests a resource from /libs?

```none
/apps/project/components/text (overlay) -> sling:resourceSuperType = core/wcm/components/text/v2/text
```

- [ ] **A)** It only looks in /libs, ignoring the overlay.
- [ ] **B)** It merges properties from both, with /apps taking precedence.
- [ ] **C)** It replaces /libs entirely with the overlay.
- [ ] **D)** It throws an error if both paths exist.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Sling Resource Merger checks /apps first; if nodes exist, they override /libs. Non-overridden parts fall back to /libs.
 
 
</details>

### 7. Which interface must a custom workflow step implement?

- [ ] **A)** WorkflowProcess
- [ ] **B)** JobConsumer
- [ ] **C)** EventHandler
- [ ] **D)** SlingSafeMethodsServlet

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Custom workflow steps must implement the com.adobe.granite.workflow.exec.WorkflowProcess interface.
 
 
</details>

### 8. Which two statements are true about AEM tags? (Select two)

- [ ] **A)** Tags are stored as cq:Tag nodes under /content/cq:tags.
- [ ] **B)** Tags must be created using the TagManager API.
- [ ] **C)** Tags are automatically inherited by child pages.
- [ ] **D)** The cq:tags property stores a single string value.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Tags reside under /content/cq:tags (or legacy /etc/tags) and are created via TagManager. They are not inherited and cq:tags is a string array.
 
 
</details>

### 9. Given this client-side custom event creation: new CustomEvent('aem:filterupdate', { detail: { key: 'color', value: 'red' } }). What is the correct way to listen for this event?

```javascript
const event = new CustomEvent('aem:filterupdate', { detail: { key: 'color', value: 'red' } }); document.dispatchEvent(event);
```

- [ ] **A)** document.addEventListener('aem:filterupdate', handler)
- [ ] **B)** addEventListener('CustomEvent', handler)
- [ ] **C)** EventAdmin.onEvent('aem:filterupdate', handler)
- [ ] **D)** window.on('customEvent', handler)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> CustomEvent creates a named event; to listen, use standard DOM addEventListener on the document or element with the same event name.
 
 
</details>

### 10. What is the primary advantage of using a Job over an Event for long-running tasks?

- [ ] **A)** Jobs provide reliable, persistent execution with retries.
- [ ] **B)** Events are more secure and require less configuration.
- [ ] **C)** Jobs can only run on publish instances.
- [ ] **D)** Events support parallel execution by default.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Jobs are persisted in the repository and can be retried, making them suitable for long-running or unreliable operations.
 
 
</details>


---

### **Building Accessible and Responsive Sites**

### 11. What does the CSS class 'aem-GridColumn--default--6' represent in the AEM Responsive Grid?

- [ ] **A)** A column spanning 6 columns on the default breakpoint
- [ ] **B)** A column spanning 6 columns on the tablet breakpoint
- [ ] **C)** A column offset of 6 on the default breakpoint
- [ ] **D)** A row containing 6 default columns

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The naming convention 'default--6' means the column spans 6 columns on the default (desktop) breakpoint.
 
 
</details>

### 12. According to WCAG 2.1 AA, which contrast ratios are required for normal and large text? (Select two)

- [ ] **A)** 4.5:1 for normal text
- [ ] **B)** 3:1 for large text
- [ ] **C)** 2:1 for normal text
- [ ] **D)** 4:1 for large text

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> WCAG 2.1 AA requires at least 4.5:1 contrast for normal text and 3:1 for large text.
 
 
</details>

### 13. Given the following JCR node structure, where must the 'cq:styleSystem' node be placed for the AEM Style System to work?

```xml
<root jcr:primaryType="nt:unstructured">
  <policies>
    <text-policy>
      <cq:styleSystem jcr:primaryType="nt:unstructured"/>
    </text-policy>
  </policies>
</root>
```

- [ ] **A)** Under the component's policy node in /conf
- [ ] **B)** Under the component's resource node in /apps
- [ ] **C)** Under the template's jcr:content node
- [ ] **D)** Under the page node in /content

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Style System is configured at the template policy level, not at the component or page level.
 
 
</details>

### 14. How should you translate UI strings like 'Read More' in an AEM component?

- [ ] **A)** Use resource bundles placed under /apps/.../i18n
- [ ] **B)** Use the Translation Integration Framework (TIF)
- [ ] **C)** Use MSM rollout configurations
- [ ] **D)** Use language copies with manual editing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Component UI strings are internationalized via resource bundles, not through TIF which is for page content.
 
 
</details>

### 15. Which conditions should a Sling Rewriter transformer check before injecting a canonical tag? (Select two)

- [ ] **A)** The response content type is HTML
- [ ] **B)** The page property cq:noIndex is false
- [ ] **C)** The page has a vanity URL configured
- [ ] **D)** The request contains query parameters

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Canonical tags should only be injected for HTML responses and when the page is not marked noindex.
 
 
</details>

### 16. Given this RTE configuration snippet, what will be the effect on the 'link' plugin?

```xml
<rtePlugins jcr:primaryType="nt:unstructured">
  <link jcr:primaryType="nt:unstructured">
    <features/>
  </link>
</rtePlugins>
```

- [ ] **A)** The plugin remains active but no toolbar buttons appear
- [ ] **B)** The plugin is completely disabled and cannot be used
- [ ] **C)** The plugin shows its default toolbar buttons
- [ ] **D)** The configuration is invalid and causes an error

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An empty 'features' array hides toolbar buttons but the plugin stays active; to disable it fully, omit the node.
 
 
</details>


---

### **Configuring AEM for a Project**

### 17. What node type is used to store OSGi configurations in the AEM JCR repository?

- [ ] **A)** sling:OsgiConfig
- [ ] **B)** nt:unstructured
- [ ] **C)** cq:Page
- [ ] **D)** oak:Unstructured

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OSGi configurations in AEM are stored using the sling:OsgiConfig node type, typically under config folders.
 
 
</details>

### 18. Which of the following are valid methods to configure OSGi components in AEM? (Select all that apply)

- [ ] **A)** Using the Web Console (ConfigMgr)
- [ ] **B)** Creating sling:OsgiConfig nodes via CRXDE
- [ ] **C)** Defining repoinit statements in a config.xml file
- [ ] **D)** Setting environment variables on the server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> OSGi configs can be set via Web Console, sling:OsgiConfig nodes, or repoinit. Environment variables are not a direct method for AEM OSGi configs.
 
 
</details>

### 19. Given the following Query Builder predicate map, what does the query return? The snippet uses the 'property' predicate with 'operation=like'.

```java
Map<String, String> predicates = new HashMap<>();
predicates.put("path", "/content");
predicates.put("property", "jcr:title");
predicates.put("property.value", "About");
predicates.put("property.operation", "like");
```

- [ ] **A)** All pages under /content that have a title starting with 'About'
- [ ] **B)** All pages under /content with a title exactly equal to 'About'
- [ ] **C)** All resources under /content with a description containing 'About'
- [ ] **D)** All resources under /content that do not have a title

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The predicate 'property.operation=like' performs a prefix match, so it retrieves nodes where the property starts with the given value.
 
 
</details>

### 20. Where should a reverse replication agent be configured in AEM?

- [ ] **A)** On the author instance
- [ ] **B)** On the publish instance
- [ ] **C)** On the dispatcher server
- [ ] **D)** On a separate replication server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Reverse replication agents are configured on the publish instance to send content back to the author instance.
 
 
</details>

### 21. Which event types can trigger a workflow launcher in AEM? (Select all that apply)

- [ ] **A)** Created
- [ ] **B)** Changed
- [ ] **C)** Deleted
- [ ] **D)** Workflow Completed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> Launchers listen to Created, Changed, Deleted, and WorkflowCompleted events as defined by the event type integers.
 
 
</details>

### 22. Examine the package filter configuration below. Which repository path will be included in the package? The XML excerpt shows the filter.xml content.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<workspaceFilter version="1.0">
    <filter root="/apps/myproject"/>
</workspaceFilter>
```

- [ ] **A)** /apps/myproject
- [ ] **B)** /apps/myproject/components
- [ ] **C)** /apps
- [ ] **D)** /apps/myproject/config

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The filter's root path is '/apps/myproject', and no sub-path excludes it, so the entire subtree under that path is included.
 
 
</details>

### 23. In Multi-Site Manager (MSM), what is the direction of content inheritance?

- [ ] **A)** From live copy to blueprint
- [ ] **B)** From blueprint to live copy
- [ ] **C)** Bidirectional between blueprint and live copy
- [ ] **D)** Inheritance is disabled by default

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> MSM inheritance is one-way: changes in the blueprint can be rolled out to live copies; live copy changes do not propagate back.
 
 
</details>


---

### **Site Administration and Content Management**

### 24. What is the default maximum number of versions AEM keeps per page?

- [ ] **A)** 10
- [ ] **B)** 20
- [ ] **C)** 50
- [ ] **D)** 100

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AEM keeps up to 20 versions per page by default, as stated in the playbook document.
 
 
</details>

### 25. Which statements are correct regarding workflow participants in AEM? (Select all that apply)

- [ ] **A)** Workflow participants automatically have read and write access to the payload page.
- [ ] **B)** The assignment type can be configured so that any single user in a group can approve.
- [ ] **C)** Participants require explicit JCR write permission on the content path to edit the payload.
- [ ] **D)** Only users in the workflow-administrators group can be assigned as participants.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Workflow participants need explicit write permissions on the payload, and the assignment type can be set to 'Single Participant' (any one user). The other options are false.
 
 
</details>

### 26. In the provided dialog snippet, what is the name of the property that stores the link to the DAM asset?

```xml
<imageReference jcr:primaryType="nt:unstructured" sling:resourceType="granite/ui/components/coral/foundation/form/hidden" name="./imageReference" value="${empty}" />
```

- [ ] **A)** imageReference
- [ ] **B)** assetReference
- [ ] **C)** damReference
- [ ] **D)** jcr:reference

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The hidden field in the component dialog uses the name 'imageReference' to store the asset reference, as shown in the playbook example.
 
 
</details>

### 27. Which framework acts as the bridge between AEM and third-party translation providers?

- [ ] **A)** Translation Integration Framework (TIF)
- [ ] **B)** Multi Site Manager (MSM)
- [ ] **C)** Launches
- [ ] **D)** ContextHub

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Translation Integration Framework (TIF) is the backbone that connects AEM to external translation services, as described in the playbook.
 
 
</details>

### 28. Which persistence modes are supported by ContextHub stores? (Choose all that apply.)

- [ ] **A)** local
- [ ] **B)** session
- [ ] **C)** cookie
- [ ] **D)** database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> ContextHub supports local (localStorage), session (sessionStorage), and cookie persistence modes. 'Database' is not a supported persistence mode.
 
 
</details>

### 29. In the provided node definition, what mixin type is required for a node to be recognized as a custom report in AEM?

```xml
<jcr:node jcr:primaryType="nt:file" jcr:mixinTypes="[cq:ReportDefinition]">
  <jcr:content jcr:primaryType="nt:resource" jcr:data="..."/>
</jcr:node>
```

- [ ] **A)** cq:ReportDefinition
- [ ] **B)** cq:Page
- [ ] **C)** sling:Folder
- [ ] **D)** nt:unstructured

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A custom report definition node must have the mixin type 'cq:ReportDefinition' to be recognized by the AEM Dashboard, as stated in the playbook.
 
 
</details>

### 30. What is the primary role of an AEM Launch in site management?

- [ ] **A)** It creates a temporary fork of the content tree for future updates.
- [ ] **B)** It automatically publishes pages at a scheduled time.
- [ ] **C)** It manages multilingual content synchronization.
- [ ] **D)** It creates a live copy of a blueprint.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An AEM Launch creates a temporary fork of content for future promotion without affecting the live site. The other options describe different features (activation schedules, translation, MSM).
 
 
</details>

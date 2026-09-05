<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/ServiceNow/ServiceNow%20Certified%20System%20Administrator%20(CSA)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>ServiceNow Certified System Administrator</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Application Development](#application-development) (6 questions)
- [Collaboration](#collaboration) (3 questions)
- [Database Administration](#database-administration) (6 questions)
- [Integration and APIs](#integration-and-apis) (3 questions)
- [Security and Access Control](#security-and-access-control) (3 questions)
- [Service Management and ITSM](#service-management-and-itsm) (4 questions)
- [User Interface and Navigation](#user-interface-and-navigation) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:48:05.722Z |
| Domains | 7 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Application Development | 6 |
| Collaboration | 3 |
| Database Administration | 6 |
| Integration and APIs | 3 |
| Security and Access Control | 3 |
| Service Management and ITSM | 4 |
| User Interface and Navigation | 5 |

---

### **Application Development**

### 1. In the ServiceNow platform, what are the two primary mechanisms that are responsible for activating notifications?

- [ ] **A)** Record Changes and Events
- [ ] **B)** Business Rules and Workflows
- [ ] **C)** Email Client and Templates
- [ ] **D)** Groups and Roles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ServiceNow notifications are activated when a record changes or when an event is queued through the gs.eventQueue() API.
 
 
</details>

### 2. Which of the following statements about group membership and role inheritance are accurate in the ServiceNow platform?

- [ ] **A)** Assigning a role to a group grants that role to every member of the group.
- [ ] **B)** The hierarchy moves from User to Group to Role.
- [ ] **C)** A group can be assigned directly to a role.
- [ ] **D)** Group members inherit the roles assigned to their group.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Roles are assigned to groups, and members inherit those roles. The supported hierarchy is User -> Group -> Role; groups are not assigned to roles.
 
 
</details>

### 3. Analyze the provided script snippet and identify the primary purpose of this code within the ServiceNow notification architecture.

```javascript
gs.eventQueue('incident.critical', current, current.caller_id);
```

- [ ] **A)** It queues an event that can activate a notification.
- [ ] **B)** It immediately sends an email to the assigned user.
- [ ] **C)** It creates a new business rule for the incident.
- [ ] **D)** It updates the incident record with a new priority.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code calls gs.eventQueue() to queue an event, which then serves as a signal that can activate an existing notification.
 
 
</details>

### 4. In the configuration of a ServiceNow notification, what function do conditions serve when the notification is evaluated?

- [ ] **A)** It acts as a logic gate that must be met for the notification to fire.
- [ ] **B)** It defines the email template used in the notification.
- [ ] **C)** It specifies which users receive the notification.
- [ ] **D)** It determines whether the notification is sent by email or SMS.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Conditions determine whether the notification should fire; if they are not met, no notification is dispatched.
 
 
</details>

### 5. Which of the following options are valid targets when configuring the recipient list for a ServiceNow notification?

- [ ] **A)** Specific users
- [ ] **B)** Groups
- [ ] **C)** Fields on the record such as Caller or Assigned to
- [ ] **D)** Email templates

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Notification recipients can be users, groups, or dynamic record fields; email templates only control content, not recipients.
 
 
</details>

### 6. Analyze the provided script. What condition must be true for an associated notification to be activated?

```javascript
if (current.priority == 1) {
    gs.eventQueue('incident.critical', current, current.caller_id);
}
```

- [ ] **A)** The incident priority must be Critical.
- [ ] **B)** The notification template must contain HTML.
- [ ] **C)** The assigned group must be empty.
- [ ] **D)** The incident must be created by the system.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The if condition checks that priority equals 1 (Critical) before queuing the event, so the notification fires only when that condition is true.
 
 
</details>


---

### **Collaboration**

### 7. Which two primary mechanisms can activate a system notification in ServiceNow?

- [ ] **A)** Record changes and Events
- [ ] **B)** Business Rules and Scripts
- [ ] **C)** Email Client and Inbound Actions
- [ ] **D)** Assignment Groups and Roles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Notifications are activated by record changes, such as inserts, updates, or field value changes, and by Events queued through the gs.eventQueue() API.
 
 
</details>

### 8. Which statements about groups and role inheritance are true? Select two.

- [ ] **A)** When a role is assigned to a group, every member of that group automatically possesses that role.
- [ ] **B)** A Group cannot have more than one User as a member.
- [ ] **C)** Assigning roles to groups is an administrative best practice because updates can be applied globally.
- [ ] **D)** A Group Manager is the only group member who receives the group's roles.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Role inheritance means all group members gain any role assigned to the group. Assigning roles to groups is an efficient best practice because security updates can be made once to the group rather than to each user individually.
 
 
</details>

### 9. Review the code block. What action does the API call perform in the notification process?

```javascript
gs.eventQueue('incident.critical', current, user);
```

- [ ] **A)** It queues an event that can trigger notifications
- [ ] **B)** It immediately sends an email message
- [ ] **C)** It creates a new Business Rule
- [ ] **D)** It updates the Assignment Group on the record

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The gs.eventQueue() API queues an event. Notifications subscribe to events, and the event acts as the signal that can trigger notification delivery.
 
 
</details>


---

### **Database Administration**

### 10. Which two primary mechanisms activate ServiceNow notifications?

- [ ] **A)** Record Changes and Events
- [ ] **B)** Record Changes and Business Rules
- [ ] **C)** Events and Roles
- [ ] **D)** Email Client and Inbound Actions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Notifications are activated either by record changes or by events triggered through the eventQueue API.
 
 
</details>

### 11. Select all true statements about group membership and role inheritance.

- [ ] **A)** Assigning a role to a group grants it to all members
- [ ] **B)** Group membership allows users to inherit group properties like roles
- [ ] **C)** Assigning roles to groups is a best practice for administrative efficiency
- [ ] **D)** A role can be assigned to a group by making the group a member of the role

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A role assigned to a group is inherited by every member. The platform best practice is to assign roles to groups rather than individual users.
 
 
</details>

### 12. What does the method call in the provided code snippet do?

```javascript
gs.eventQueue('incident.critical', current, user);
```

- [ ] **A)** Fires a ServiceNow event
- [ ] **B)** Runs a business rule immediately
- [ ] **C)** Sends an email directly to the user
- [ ] **D)** Creates a new group record

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> gs.eventQueue() places an event on the queue, which the notification engine uses to trigger the corresponding notification.
 
 
</details>

### 13. In a notification, the 'Who' component is used for what purpose?

- [ ] **A)** The target audience
- [ ] **B)** The email template
- [ ] **C)** The trigger condition
- [ ] **D)** The notification event name

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The recipient list defines who receives the notification, including users, groups, or values from record fields.
 
 
</details>

### 14. Which recipient options can be used to target notifications?

- [ ] **A)** Specific users
- [ ] **B)** Specific groups
- [ ] **C)** Fields on the record, such as Caller or Assigned to
- [ ] **D)** Every record in the sys_user table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Recipients can be chosen manually, by group, or dynamically from fields such as Caller or Assigned to.
 
 
</details>

### 15. In the provided code snippet, the conditional check represents which notification concept?

```javascript
if (current.priority == '1') {
    gs.eventQueue('incident.priority.critical', current, user);
}
```

- [ ] **A)** Conditions (the 'When')
- [ ] **B)** Recipients (the 'Who')
- [ ] **C)** Email template (the 'Format')
- [ ] **D)** Event name (the 'Trigger')

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The conditional check before eventQueue acts as the logic gate, ensuring the notification is dispatched only when the defined criteria are met.
 
 
</details>


---

### **Integration and APIs**

### 16. Which mechanism triggers a notification when a field value on a record changes?

- [ ] **A)** Record Change
- [ ] **B)** Event via gs.eventQueue()
- [ ] **C)** Email Client
- [ ] **D)** Condition Builder

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Notifications are activated by record changes when a field value changes or a record is inserted/updated, or by events triggered with gs.eventQueue().
 
 
</details>

### 17. Which two statements correctly describe role inheritance and group management best practices?

- [ ] **A)** Roles assigned to a group are automatically inherited by its members.
- [ ] **B)** To update security for multiple users, modify the role on each user profile.
- [ ] **C)** Users can be members of one group only.
- [ ] **D)** Roles are assigned to groups, not groups to roles.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Roles are assigned to groups, and all members inherit them. You cannot assign a group to a role; the correct hierarchy is User -> Group -> Role.
 
 
</details>

### 18. Review the provided script. What does calling the eventQueue API accomplish in this context?

```javascript
gs.eventQueue('incident.critical', current, current.assigned_to, '');
```

- [ ] **A)** It immediately sends an email to the assigned_to user.
- [ ] **B)** It queues an event that can trigger one or more notifications.
- [ ] **C)** It creates a new business rule to run asynchronously.
- [ ] **D)** It sets the current record's priority to critical.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> An event is a signal fired via gs.eventQueue(). The notification engine receives the event and dispatches relevant communications, but it does not directly send email or alter the record.
 
 
</details>


---

### **Security and Access Control**

### 19. Which statement correctly represents the relationship between users, groups, and roles in ServiceNow?

- [ ] **A)** User -> Group -> Role
- [ ] **B)** Role -> Group -> User
- [ ] **C)** Group -> Role -> User
- [ ] **D)** User -> Role -> Group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Roles are assigned to groups, and users inherit roles through group membership. This follows the User -> Group -> Role hierarchy.
 
 
</details>

### 20. Which two mechanisms primarily activate ServiceNow notifications?

- [ ] **A)** Record changes
- [ ] **B)** Events queued with the gs.eventQueue() API
- [ ] **C)** Business Rules
- [ ] **D)** Inbound Actions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Notifications are activated by record changes or events. Although business rules can call eventQueue, they are not direct notification triggers.
 
 
</details>

### 21. What action does the provided script perform?

```javascript
gs.eventQueue('incident.critical', current, gs.getUserID(), gs.getUserID());
```

- [ ] **A)** It queues an event to activate incident-critical notifications.
- [ ] **B)** It sends an email immediately to the current user.
- [ ] **C)** It creates a new incident record.
- [ ] **D)** It assigns the incident to a group.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The gs.eventQueue() API queues an event; notification records subscribed to that event can then process the output. It does not send direct emails.
 
 
</details>


---

### **Service Management and ITSM**

### 22. In the ServiceNow platform, notifications can be activated by two distinct primary mechanisms. Which pair correctly identifies them?

- [ ] **A)** Business Rules and Scripts
- [ ] **B)** Email Client and Inbound Actions
- [ ] **C)** Assignment Groups and Roles
- [ ] **D)** Record Changes and Events

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> Notifications are activated by record changes such as field updates or inserts, and by events queued using gs.eventQueue(). Business Rules may call events but are not primary triggers.
 
 
</details>

### 23. From the options provided, select all true statements about role inheritance and group membership in ServiceNow.

- [ ] **A)** All group members inherit group roles.
- [ ] **B)** Individual user role assignment is best practice.
- [ ] **C)** Groups can be assigned to roles.
- [ ] **D)** Group role changes affect all members.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Role inheritance means group members automatically receive roles assigned to the group. Administering roles at the group level is efficient, and the hierarchy is User -> Group -> Role.
 
 
</details>

### 24. Review the provided code snippet and determine which notification component this API call represents in ServiceNow.

```javascript
gs.eventQueue('incident.updated', current, previous);
```

- [ ] **A)** Email template
- [ ] **B)** Recipient list
- [ ] **C)** Event trigger
- [ ] **D)** Condition builder

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The gs.eventQueue() API creates an event that can trigger a notification. An event is the signal object, distinct from business rules and the notification engine itself.
 
 
</details>

### 25. Which collaboration tool is optimized for workspace environments and lets technicians manage several chats at once?

- [ ] **A)** Connect Chat
- [ ] **B)** Activity Stream
- [ ] **C)** Social Profile
- [ ] **D)** Agent Chat

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> Agent Chat is optimized for workspace environments and enables technicians to manage multiple concurrent conversations while maintaining context on records.
 
 
</details>


---

### **User Interface and Navigation**

### 26. What two primary mechanisms activate ServiceNow notifications?

- [ ] **A)** Record Changes and Events
- [ ] **B)** Business Rules and Scripts
- [ ] **C)** Email Client and Reports
- [ ] **D)** User Preferences and Roles

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Notifications are activated by Record Changes or Events, such as the gs.eventQueue() API. The other choices do not represent the primary notification trigger mechanisms.
 
 
</details>

### 27. Which statements about group membership and role inheritance are correct according to the playbook? Select all that apply.

- [ ] **A)** Assigning a role to a group grants that role to every member of the group.
- [ ] **B)** Roles can be assigned to groups, so security updates can be managed globally by updating the group.
- [ ] **C)** A Group can be assigned to a Role to create a direct user-role hierarchy.
- [ ] **D)** Assignment groups and security groups are functionally identical.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Roles assigned to groups are inherited by all group members. The hierarchy is User -> Group -> Role, and not all groups are used for task assignment.
 
 
</details>

### 28. Review the provided script snippet. What mechanism is being used to initiate the notification process?

```javascript
// Trigger an event for notification processing
gs.eventQueue('incident.critical', current, 'HIGH', '');
```

- [ ] **A)** It is queuing an Event to trigger a notification
- [ ] **B)** It is sending an email directly to the caller
- [ ] **C)** It is creating a new Assignment Group
- [ ] **D)** It is updating the role inheritance for a group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The gs.eventQueue() call creates an Event, which is one of the two primary mechanisms used to fire notifications in ServiceNow.
 
 
</details>

### 29. What is the primary purpose of the Condition Builder in a notification configuration?

- [ ] **A)** To define criteria that must be met before the notification is dispatched
- [ ] **B)** To design the email template for the notification
- [ ] **C)** To manage role inheritance for group members
- [ ] **D)** To create a new Assignment Group for routing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Condition Builder acts as a logic gate, ensuring the notification only fires when defined criteria are met, avoiding unnecessary system noise.
 
 
</details>

### 30. Which two statements are identified as common traps regarding notifications in the playbook?

- [ ] **A)** Assuming that all notifications are sent via email
- [ ] **B)** Confusing Events with Business Rules
- [ ] **C)** Using Agent Chat for all real-time messaging
- [ ] **D)** Assigning roles to groups instead of individual users

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The playbook notes the traps of assuming email-only delivery and confusing Events with Business Rules. Assigning roles to groups is actually a best practice.
 
 
</details>

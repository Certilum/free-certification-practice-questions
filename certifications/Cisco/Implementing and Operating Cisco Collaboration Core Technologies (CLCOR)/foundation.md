<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Cisco/Implementing%20and%20Operating%20Cisco%20Collaboration%20Core%20Technologies.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Implementing and Operating Cisco Collaboration Core Technologies (CLCOR)</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Call Control](#call-control) (6 questions)
- [Cisco IOS XE Gateway and Media Resources](#cisco-ios-xe-gateway-and-media-resources) (6 questions)
- [Collaboration Applications](#collaboration-applications) (6 questions)
- [Infrastructure and Design](#infrastructure-and-design) (3 questions)
- [Protocols, Codecs and Endpoints](#protocols-codecs-and-endpoints) (4 questions)
- [Quality of Service](#quality-of-service) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:11.031Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Call Control | 6 |
| Cisco IOS XE Gateway and Media Resources | 6 |
| Collaboration Applications | 6 |
| Infrastructure and Design | 3 |
| Protocols, Codecs and Endpoints | 4 |
| Quality of Service | 5 |

---

### **Call Control**

### 1. What is the primary purpose of digit manipulation in a CUCM environment?

- [ ] **A)** Programmatic alteration of dialed digits
- [ ] **B)** Assignment of IP addresses to endpoints
- [ ] **C)** Creation of end-user accounts
- [ ] **D)** Upgrading device firmware

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Digit manipulation is the programmatic alteration of dialed digits to normalize or modify numbers for compatibility between systems.
 
 
</details>

### 2. Which pattern types can be used to perform digit manipulation? (Choose all that apply.)

- [ ] **A)** Translation Patterns
- [ ] **B)** Route Patterns
- [ ] **C)** Transformation Patterns
- [ ] **D)** Device Pools

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Digit manipulation uses Translation Patterns, Transformation Patterns, and Route Patterns to alter or route dialed digits.
 
 
</details>

### 3. Refer to the code block. Which pattern type changes the dialed digits during the route lookup process?

```text
Route Pattern: 9.XXXXXXXXXX
Translation Pattern: 91.XXXXXXXXXX
Transformation Pattern: +1XXXXXXXXXX
```

- [ ] **A)** Translation Pattern
- [ ] **B)** Transformation Pattern
- [ ] **C)** Route Pattern
- [ ] **D)** Route List

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Translation patterns alter digits during the search phase, unlike transformation patterns which operate after routing.
 
 
</details>

### 4. What is the main purpose of a Route Pattern?

- [ ] **A)** Direct calls toward a specific destination
- [ ] **B)** Change the digits in SIP headers
- [ ] **C)** Group devices into partitions
- [ ] **D)** Register endpoints with the server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Route Patterns direct calls to a specific destination such as a gateway or SIP trunk.
 
 
</details>

### 5. Which functions are provided by an H.323 Gatekeeper? (Choose all that apply.)

- [ ] **A)** Admission Control
- [ ] **B)** Location Service
- [ ] **C)** Call Signaling
- [ ] **D)** NAT Traversal

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The H.323 Gatekeeper provides Admission Control, Location Service, and Call Signaling.
 
 
</details>

### 6. Refer to the code block. What is the intended purpose of this SIP message?

```text
REGISTER sip:registrar.cisco.com SIP/2.0
From: sip:1001@cisco.com
To: sip:1001@cisco.com
Contact: sip:1001@192.168.1.10
Expires: 600
```

- [ ] **A)** Bind a SIP URI to an IP address
- [ ] **B)** Establish a media session
- [ ] **C)** Terminate a registered endpoint
- [ ] **D)** Query a route group status

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This is a SIP REGISTER request, which updates the location service by binding the SIP URI to the endpoint's contact address.
 
 
</details>


---

### **Cisco IOS XE Gateway and Media Resources**

### 7. What is the primary purpose of digit manipulation in a Cisco collaboration solution?

- [ ] **A)** To normalize dialed digits to meet trunk requirements
- [ ] **B)** To increase call encryption strength
- [ ] **C)** To replace gateway hardware
- [ ] **D)** To manage device registrations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Digit manipulation alters dialed digits so numbers match trunk expectations, such as adding prefixes or removing leading zeros for interoperability.
 
 
</details>

### 8. Which two statements correctly compare Route Patterns and Translation Patterns?

- [ ] **A)** Route Patterns send calls to a specific destination such as a gateway or SIP trunk.
- [ ] **B)** Translation Patterns modify digits during call routing lookup.
- [ ] **C)** Translation Patterns are used only for emergency calls.
- [ ] **D)** Route Patterns change the caller ID in the SIP message.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Route Patterns direct calls to destinations; Translation Patterns manipulate digits during the search process. They serve different roles in CUCM routing.
 
 
</details>

### 9. Refer to the exhibit. What is the resulting called party number after the translation pattern is applied?

```text
Translation Pattern: 91XXXXXXXXXX
Called Party Transform Mask: +1XXXXXXXXXX
User dialed digits: 914155551234
```

- [ ] **A)** +14155551234
- [ ] **B)** 914155551234
- [ ] **C)** 14155551234
- [ ] **D)** 4155551234

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The pattern prepends +1 while preserving the ten digits after 91, converting 914155551234 into +14155551234.
 
 
</details>

### 10. Which statement best describes a Partition in CUCM?

- [ ] **A)** A logical container that defines visibility for patterns
- [ ] **B)** A list of devices that may access patterns
- [ ] **C)** A route group containing gateways
- [ ] **D)** A SIP trunk security profile

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Partitions group patterns and define their scope of visibility; they do not control device access by themselves.
 
 
</details>

### 11. Which two statements are true about Calling Search Spaces?

- [ ] **A)** A CSS is a collection of Partitions.
- [ ] **B)** A CSS defines which Partitions a device can access.
- [ ] **C)** A CSS contains the actual route patterns.
- [ ] **D)** A CSS is used to encrypt SIP messages.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A CSS aggregates Partitions and is assigned to devices to grant access to those Partitions during routing.
 
 
</details>

### 12. Refer to the exhibit. What happens when a user dials 911 from the configured phone?

```text
Partition: Emergency_PT
Pattern: 911 in Emergency_PT
CSS: Sales_CSS contains Sales_PT
Phone CSS: Sales_CSS
```

- [ ] **A)** The call fails because Sales_CSS does not include Emergency_PT.
- [ ] **B)** The call succeeds because 911 is a global emergency route.
- [ ] **C)** The call succeeds because all partitions are visible to all phones.
- [ ] **D)** The call fails because the phone is not registered.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A device can only reach patterns in Partitions contained by its assigned CSS. Since Emergency_PT is not in Sales_CSS, the call fails.
 
 
</details>


---

### **Collaboration Applications**

### 13. Which CUCM element is used to modify the dialed digits, such as adding a prefix or stripping a leading digit, before the call is routed?

- [ ] **A)** Translation Pattern
- [ ] **B)** Calling Search Space
- [ ] **C)** Route List
- [ ] **D)** SIP Profile

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Translation Pattern is used for digit manipulation within CUCM, altering the dialed digits before the call is routed to a final destination.
 
 
</details>

### 14. Which two statements about Partitions and Calling Search Spaces (CSS) are true?

- [ ] **A)** Partitions are containers for patterns, and a CSS defines which partitions a device can access.
- [ ] **B)** A device can reach a pattern only if the pattern's partition is included in the device's CSS.
- [ ] **C)** Simply placing a pattern in a Partition makes it reachable by every device.
- [ ] **D)** A CSS is assigned to a Partition to restrict the digits in that partition.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Partitions group patterns for visibility control. A CSS must include the target partition for a device to access the patterns within it.
 
 
</details>

### 15. Refer to the code block. What is the effect of this translation pattern configuration?

```cisco
translation-pattern 9[1-9]XXXXXXXXXX
  strip 9
  prefix 1
```

- [ ] **A)** It removes the leading 9 and adds the prefix 1.
- [ ] **B)** It only adds the prefix 1 without changing the digits.
- [ ] **C)** It blocks the call after translation.
- [ ] **D)** It changes the destination to a different route list.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The translation pattern strips the initial 9 from the dialed digits and prepends 1, normalizing the number for trunk delivery.
 
 
</details>

### 16. What is the primary difference between a Route Pattern and a Translation Pattern in CUCM?

- [ ] **A)** Route Patterns direct calls to a specific destination, while Translation Patterns change the digit string.
- [ ] **B)** Translation Patterns direct calls to a gateway, while Route Patterns manipulate digits.
- [ ] **C)** Route Patterns are used only for internal calls, while Translation Patterns are used for PSTN calls.
- [ ] **D)** There is no functional difference; they are interchangeable.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Route Patterns determine where the call is sent, while Translation Patterns modify the digits before or during the routing decision.
 
 
</details>

### 17. Which two statements correctly describe Transformation Patterns in CUCM?

- [ ] **A)** They change the calling or called party number after the route has been selected.
- [ ] **B)** They are often used to normalize numbers for PSTN egress.
- [ ] **C)** They are used to add a route list to a call.
- [ ] **D)** They control which partitions a device can access.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Transformation Patterns alter party numbers after route selection, commonly to normalize caller ID or called numbers for external networks.
 
 
</details>

### 18. Review the code block showing a SIP REGISTER message. What is the meaning of the 'Expires: 3600' header?

```sip
REGISTER sip:cucm.example.com SIP/2.0
From: <sip:2001@example.com>
To: <sip:2001@example.com>
Contact: <sip:2001@192.168.1.25>
Expires: 3600
```

- [ ] **A)** The registration is valid for 3600 seconds.
- [ ] **B)** The call will last a maximum of 3600 seconds.
- [ ] **C)** The endpoint will send an INVITE after 3600 seconds.
- [ ] **D)** The message can traverse up to 3600 hops.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In SIP, the Expires header in a REGISTER request sets the validity duration of the registration. After it lapses, the endpoint must re-register.
 
 
</details>


---

### **Infrastructure and Design**

### 19. What is the primary purpose of digit manipulation in a Cisco Collaboration environment?

- [ ] **A)** To alter dialed digits so they match trunk and gateway requirements
- [ ] **B)** To restrict access to route patterns
- [ ] **C)** To provide failover between route groups
- [ ] **D)** To manage device registration intervals

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Digit manipulation changes dialed digits, such as adding prefixes or stripping leading zeros, to normalize numbers for trunk requirements and ensure compatibility between systems.
 
 
</details>

### 20. Which statements about Partitions and Calling Search Spaces (CSS) are true? (Select all that apply.)

- [ ] **A)** Partitions are containers that define visibility for patterns.
- [ ] **B)** A CSS determines which partitions a device can access.
- [ ] **C)** A device can reach a pattern if the pattern is in any partition.
- [ ] **D)** The CSS must contain the target pattern's partition for access.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Partitions contain patterns; a CSS grants a device access to selected partitions. Adding a pattern to a partition does not make it reachable unless the device's CSS includes that partition.
 
 
</details>

### 21. Refer to the pattern configuration in the code block. What does this configuration represent?

```python
pattern_config = {
    "type": "Translation",
    "matching_digits": "91XXXXXXXXXX",
    "prefix_added": "1",
}
```

- [ ] **A)** A Translation Pattern that changes digits before route selection
- [ ] **B)** A Route Pattern that selects a destination trunk
- [ ] **C)** A Transformation Pattern that changes digits after routing
- [ ] **D)** A CSS Pattern that defines device permissions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code shows a Translation Pattern, which alters the digit string during the search phase before the route is selected.
 
 
</details>


---

### **Protocols, Codecs and Endpoints**

### 22. What is the primary function of a Translation Pattern within a Cisco Unified Communications environment?

- [ ] **A)** Alters digits during the search phase
- [ ] **B)** Forwards calls to a specific trunk
- [ ] **C)** Contains a set of partitions
- [ ] **D)** Provides bandwidth management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Translation Patterns change digits during the search phase, before a destination is selected. Route Patterns, not Translation Patterns, are used to forward calls toward trunks or gateways.
 
 
</details>

### 23. Which two statements correctly describe Partitions and Calling Search Spaces (CSS)?

- [ ] **A)** A container for route patterns
- [ ] **B)** Defines the partitions a device can access
- [ ] **C)** Adding a pattern to a Partition makes it reachable
- [ ] **D)** A list of patterns and numbers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Partitions contain patterns and define visibility scope. A CSS defines which partitions a device can access; adding a pattern to a Partition does not make it reachable unless the device CSS includes that Partition.
 
 
</details>

### 24. A SIP endpoint sends the request shown to its registrar. What is the purpose of the Expires header in this request?

```text
REGISTER sip:10.1.1.1 SIP/2.0
From: sip:1000@10.1.1.1
To: sip:1000@10.1.1.1
Expires: 3600
```

- [ ] **A)** Indicates how long the registration remains valid
- [ ] **B)** Selects the audio codec for the session
- [ ] **C)** Sets the maximum number of simultaneous calls
- [ ] **D)** Determines route pattern priority

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Expires header defines the registration lifetime. If the endpoint does not refresh before expiry, the registration entry becomes stale and call routing can fail.
 
 
</details>

### 25. In which order are Route Lists evaluated when a call is placed?

- [ ] **A)** Sequentially by Route Group preference
- [ ] **B)** In parallel across all Route Groups
- [ ] **C)** Based on the calling party username
- [ ] **D)** Randomly to balance the load

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Route Lists contain Route Groups that are evaluated in preference order. If all trunks in one Route Group are unavailable, the system moves to the next Route Group in the list.
 
 
</details>


---

### **Quality of Service**

### 26. Which CUCM pattern type is used to alter dialed digits to match a different number format inside the call control system?

- [ ] **A)** Route Pattern
- [ ] **B)** Translation Pattern
- [ ] **C)** Transformation Pattern
- [ ] **D)** Calling Search Space

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Translation Patterns alter the digit string during the search phase, re-mapping the call to a different pattern inside the system. This is the key difference from route and transformation patterns.
 
 
</details>

### 27. Which two statements correctly describe Translation Patterns in a Cisco Unified CM dial plan?

- [ ] **A)** They direct calls toward a specific destination such as a SIP trunk.
- [ ] **B)** They can change a number format by adding a prefix without changing the destination.
- [ ] **C)** They are applied after the route has been selected.
- [ ] **D)** They modify digits during the search phase of call routing.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Translation Patterns modify digits during dial-plan lookup and can add a prefix without changing the destination. They are not used to direct calls or to transform digits after route selection.
 
 
</details>

### 28. Refer to the dial plan excerpt in the code block. What is the purpose of the configured pattern type?

```text
Pattern: 91.[2-9]XX[2-9]XXXXXX
Type: Translation Pattern
CSS: PSTN_Access
```

- [ ] **A)** It sends the call directly to a PSTN gateway without further lookup.
- [ ] **B)** It changes the digits and the call continues through the call-routing process.
- [ ] **C)** It blocks the call by applying a reject action.
- [ ] **D)** It only modifies the caller ID before the call is forwarded.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Translation Patterns change digits during the routing search and allow the call to continue through the dial plan. Route selection occurs after the digit change has been applied.
 
 
</details>

### 29. In Cisco Unified CM, what is the primary purpose of a Partition?

- [ ] **A)** It defines the scope of visibility for patterns.
- [ ] **B)** It determines which partitions a device can access.
- [ ] **C)** It routes calls to external gateways.
- [ ] **D)** It manages SIP registration state.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Partitions define the visibility scope for patterns. A device needs a CSS that contains the partition in order to reach the pattern.
 
 
</details>

### 30. Which two statements about Calling Search Spaces and Partitions are correct?

- [ ] **A)** A CSS contains a list of partitions that a device can access.
- [ ] **B)** A Partition acts as a container for patterns.
- [ ] **C)** A CSS can contain patterns directly without referencing a partition.
- [ ] **D)** Partitions are used to store route groups for gateway selection.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A CSS is a list of partitions that a device can access, while a Partition is a container for patterns. This separation provides permission-based routing.
 
 
</details>

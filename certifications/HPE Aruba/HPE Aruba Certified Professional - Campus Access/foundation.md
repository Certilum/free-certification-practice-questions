<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/HPE%20Aruba/HPE%20Aruba%20Certified%20Professional%20-%20Campus%20Access.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>HPE Aruba Certified Professional - Campus Access</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Campus Access Implementation](#campus-access-implementation) (9 questions)
- [Network Management](#network-management) (7 questions)
- [Network Resiliency and Device Management](#network-resiliency-and-device-management) (4 questions)
- [Network Stack](#network-stack) (1 questions)
- [Wireless LAN](#wireless-lan) (9 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:50.572Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Campus Access Implementation | 9 |
| Network Management | 7 |
| Network Resiliency and Device Management | 4 |
| Network Stack | 1 |
| Wireless LAN | 9 |

---

### **Campus Access Implementation**

### 1. What is the main purpose of SSID to VLAN mapping in an Aruba campus architecture?

- [ ] **A)** It encapsulates WLAN traffic in GRE or VXLAN and places it into the correct broadcast domain.
- [ ] **B)** It assigns IP addresses to wireless clients.
- [ ] **C)** It selects the AP transmit power.
- [ ] **D)** It creates per-user firewall rules.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SSID-to-VLAN mapping binds the wireless network to the proper wired VLAN, with GRE/VXLAN carrying traffic to the gateway.
 
 
</details>

### 2. Which two encapsulation mechanisms are used to carry WLAN traffic from an SSID to the wired VLAN in Aruba architectures?

- [ ] **A)** GRE
- [ ] **B)** VXLAN
- [ ] **C)** IPsec
- [ ] **D)** MPLS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Aruba architectures use GRE or VXLAN to encapsulate and transport WLAN traffic to the appropriate backend VLAN.
 
 
</details>

### 3. Refer to the configuration snippet. What is the effect of the vlan 100 command?

```plaintext
wlan ssid Employee
 vlan 100
 aaa authentication dot1x radius-group Corp-RADIUS
```

- [ ] **A)** Employee traffic will enter VLAN 100 at the gateway after GRE/VXLAN encapsulation.
- [ ] **B)** The AP will ignore all client traffic.
- [ ] **C)** The SSID will be hidden from probes.
- [ ] **D)** The client is assigned a static IP in VLAN 100.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The vlan command on the SSID maps that WLAN to the backend VLAN, so client traffic is delivered to the correct broadcast domain.
 
 
</details>

### 4. In Aruba RBAC, what is the primary factor that determines a user's network privileges?

- [ ] **A)** User identity
- [ ] **B)** SSID
- [ ] **C)** AP hardware model
- [ ] **D)** Radio frequency band

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RBAC uses user identity to assign privileges, not just the SSID or connection point.
 
 
</details>

### 5. Which items can an Aruba user role govern in a campus network?

- [ ] **A)** Firewall policies
- [ ] **B)** Bandwidth limits
- [ ] **C)** Access rights
- [ ] **D)** Channel assignment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> User roles govern firewall policies, bandwidth limits, and access rights regardless of client location.
 
 
</details>

### 6. Refer to the role definition. What does this configuration demonstrate about RBAC?

```plaintext
user-role employee
  vlan 20
  access-list session deny dst 10.0.0.0/8
```

- [ ] **A)** The role enforces security based on identity, independent of the physical connection point.
- [ ] **B)** The role is applied only to wired ports.
- [ ] **C)** The role changes the AP channel.
- [ ] **D)** The role affects only SSID-to-VLAN mapping.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The role includes VLAN and ACL settings that follow the user identity, not the connection point.
 
 
</details>

### 7. Which security profile is required for enterprise-grade identity management in campus WLANs?

- [ ] **A)** WPA3-Enterprise with 802.1X
- [ ] **B)** WPA2-Personal
- [ ] **C)** WEP
- [ ] **D)** Open

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Enterprise identity management requires 802.1X and WPA3-Enterprise, not pre-shared key or open security.
 
 
</details>

### 8. Which items are associated with implementing enterprise-grade security profiles for Aruba campus access?

- [ ] **A)** 802.1X
- [ ] **B)** EAP types
- [ ] **C)** RADIUS server attributes
- [ ] **D)** WPA2-Personal

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Enterprise security uses 802.1X, EAP, and RADIUS attributes to authenticate users securely.
 
 
</details>

### 9. Refer to the AAA configuration. Why are RADIUS attributes important in this setup?

```plaintext
aaa authentication dot1x employee
  radius-group Corp-RADIUS
```

- [ ] **A)** It supports secure authentication and seamless handoffs during association.
- [ ] **B)** It assigns static channel widths to APs.
- [ ] **C)** It disables client roaming.
- [ ] **D)** It provides DHCP lease information.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RADIUS attributes support 802.1X authentication, enabling secure enterprise access and smooth roaming.
 
 
</details>


---

### **Network Management**

### 10. In Aruba campus access, what is the primary purpose of SSID to VLAN mapping?

- [ ] **A)** It binds a wireless network identity to a backend wired VLAN so traffic enters the correct broadcast domain.
- [ ] **B)** It changes the physical port configuration of the access switch.
- [ ] **C)** It replaces the need for role-based access control.
- [ ] **D)** It encrypts all traffic between the AP and the internet.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SSID-to-VLAN mapping binds a WLAN identity to a wired VLAN, placing traffic into the correct broadcast domain when it reaches the gateway. It does not replace RBAC or encryption.
 
 
</details>

### 11. Which of the following are characteristics of Role-Based Access Control (RBAC) in Aruba? (Select all that apply.)

- [ ] **A)** User identity, not just the SSID, dictates network privileges.
- [ ] **B)** User roles govern firewall policies and bandwidth limits.
- [ ] **C)** Access rights are tied to the physical connection point.
- [ ] **D)** RBAC is used only for guest networks.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> RBAC uses user identity to determine privileges, with roles enforcing firewall policies and bandwidth limits. It does not tie rights to physical connection points and is not limited to guest networks.
 
 
</details>

### 12. The code block shows wireless client signal, noise, and channel details. Based on those values, what is the most accurate RF assessment?

```plaintext
Client MAC: 00:11:22:33:44:55
RSSI: -67 dBm
Noise floor: -79 dBm
SNR: 12 dB
Channel: 6
```

- [ ] **A)** The client has a strong signal and a healthy signal-to-noise ratio.
- [ ] **B)** The client has adequate signal strength but low signal quality due to a higher noise floor.
- [ ] **C)** The client has poor signal strength but excellent signal quality.
- [ ] **D)** The client is experiencing co-channel interference from Bluetooth.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The RSSI is adequate, but the SNR is low because the noise floor is relatively high. This distinction between signal strength and signal quality is a common RF trap.
 
 
</details>

### 13. What is Radio Resource Management (RRM) in Aruba wireless networks?

- [ ] **A)** Automated configuration of channel selection and transmit power
- [ ] **B)** Dynamic creation of user roles for guest access
- [ ] **C)** Encryption of management traffic between controllers
- [ ] **D)** Automatic firmware upgrades for access points

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RRM automates channel planning and transmit power to mitigate interference and maintain coverage density. It is not used for roles, encryption, or firmware.
 
 
</details>

### 14. Which of the following are RF optimization techniques described in the playbook? (Select all that apply.)

- [ ] **A)** AirMatch
- [ ] **B)** Transmit Power Control (TPC)
- [ ] **C)** Dynamic Channel Assignment (DCA)
- [ ] **D)** Static Channel Assignment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> AirMatch, TPC, and DCA are Aruba RF optimization features. Static channel assignment does not adapt to environmental changes and is not considered an optimization technique.
 
 
</details>

### 15. The code block shows an RF optimization summary for a mobility domain. What does the output reveal about AirMatch?

```plaintext
RF Optimization Mode: AirMatch
Last Run: 2025-01-15 02:00:00
Optimization Interval: 1 day
Predicted Coverage Improvement: +8%
```

- [ ] **A)** AirMatch continuously adjusts channels second by second.
- [ ] **B)** AirMatch follows a periodic, data-driven optimization cycle.
- [ ] **C)** AirMatch requires manual channel configuration before it can run.
- [ ] **D)** AirMatch only optimizes transmit power on the 2.4 GHz band.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AirMatch is centralized and data-driven, using periodic optimization cycles rather than real-time second-by-second adjustments. It does not require manual channel configuration.
 
 
</details>

### 16. What is the main purpose of 802.11k Neighbor Reports in an Aruba WLAN?

- [ ] **A)** It gives clients a list of adjacent APs, reducing the time spent scanning all channels.
- [ ] **B)** It enables the network to suggest a better AP without client involvement.
- [ ] **C)** It performs the security key handshake before a client moves.
- [ ] **D)** It increases transmit power to extend AP coverage.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> 802.11k Neighbor Reports provide candidate APs, shortening the discovery phase of roaming. 802.11v handles BSS Transition Management, and 802.11r handles fast security handoffs.
 
 
</details>


---

### **Network Resiliency and Device Management**

### 17. What does SSID-to-VLAN mapping accomplish in Aruba campus networks?

- [ ] **A)** Defines user roles for firewall filtering
- [ ] **B)** Places WLAN traffic into the correct VLAN via GRE/VXLAN
- [ ] **C)** Assigns a static IP to each wireless client
- [ ] **D)** Creates a separate management tunnel

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SSID-to-VLAN mapping binds the WLAN to a VLAN and encapsulates traffic with GRE/VXLAN so it reaches the correct broadcast domain at the gateway.
 
 
</details>

### 18. Which encapsulation methods are used to carry Aruba WLAN traffic to its mapped VLAN?

- [ ] **A)** GRE
- [ ] **B)** VXLAN
- [ ] **C)** IPsec
- [ ] **D)** MPLS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> GRE and VXLAN are the overlay encapsulation methods used to transport WLAN traffic to the mapped VLAN.
 
 
</details>

### 19. Based on the CLI configuration shown in the code block, which security profile is applied?

```text
wlan ssid campus
 security wpa2-enterprise
 security wpa2-enterprise auth-server radius1
```

- [ ] **A)** WPA2-Personal
- [ ] **B)** WPA2-Enterprise
- [ ] **C)** Captive Portal
- [ ] **D)** MAC authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The configuration specifies wpa2-enterprise with a RADIUS auth server, indicating 802.1X/WPA2-Enterprise is enabled.
 
 
</details>

### 20. In Role-Based Access Control, what determines a user's network privileges?

- [ ] **A)** User role derived from identity
- [ ] **B)** SSID in use
- [ ] **C)** AP location
- [ ] **D)** Static VLAN only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RBAC uses user identity and assigned role to shape firewall policies, bandwidth limits, and access rights.
 
 
</details>


---

### **Network Stack**

### 21. In HPE Aruba campus access, what does Role-Based Access Control (RBAC) primarily determine?

- [ ] **A)** User identity and privileges
- [ ] **B)** AP transmit power channel
- [ ] **C)** SSID broadcast state
- [ ] **D)** VLAN membership only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RBAC uses the user's identity, not just the SSID, to define firewall policies, bandwidth limits, and access rights.
 
 
</details>


---

### **Wireless LAN**

### 22. In an Aruba campus WLAN, what is the primary purpose of mapping an SSID to a backend wired VLAN?

- [ ] **A)** Places traffic in the correct broadcast domain
- [ ] **B)** Increases RF transmit power
- [ ] **C)** Hides the network from clients
- [ ] **D)** Replaces RADIUS authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SSID-to-VLAN mapping binds the wireless network identity to a backend wired VLAN so traffic is placed into the correct broadcast domain at the gateway.
 
 
</details>

### 23. Which two functions are performed by Radio Resource Management to automate RF optimization in Aruba WLANs?

- [ ] **A)** Dynamic Channel Assignment
- [ ] **B)** Transmit Power Control
- [ ] **C)** Manual channel locking
- [ ] **D)** Client OS patching

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> RRM automates dynamic channel assignment and transmit power control, adapting to environmental changes and reducing interference without manual static configuration.
 
 
</details>

### 24. Refer to the code block. What is the result of binding the WLAN profile to VLAN 25 in this configuration?

```text
wlan ssid profile CorpHQ
 vlan 25
 tunnel-mode gre

```

- [ ] **A)** Maps wireless traffic to VLAN 25 at the gateway
- [ ] **B)** Disables wireless encryption
- [ ] **C)** Assigns a static IP to every client
- [ ] **D)** Creates a new user role for each employee

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block shows SSID-to-VLAN mapping. Traffic from the WLAN is encapsulated and delivered to VLAN 25 after reaching the gateway.
 
 
</details>

### 25. In Aruba Role-Based Access Control, what is the primary factor that determines the privileges granted to a wireless user?

- [ ] **A)** User identity
- [ ] **B)** SSID name
- [ ] **C)** AP hardware model
- [ ] **D)** Radio channel

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RBAC uses user identity, not just SSID or connection point, to define firewall policies, bandwidth limits, and access rights.
 
 
</details>

### 26. Which two security profile types are appropriate for enterprise-grade identity management in an Aruba WLAN?

- [ ] **A)** WPA2-Enterprise
- [ ] **B)** WPA3-Enterprise
- [ ] **C)** WPA2-Personal
- [ ] **D)** Open authentication

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Enterprise identity management requires 802.1X authentication, which is provided by WPA2-Enterprise and WPA3-Enterprise security profiles.
 
 
</details>

### 27. The code block defines a security profile. Which authentication type is enabled when this profile is applied to an SSID?

```text
security-profile AuthNet
 authentication-server-radius internal
 dot1x eap-peap

```

- [ ] **A)** 802.1X with EAP
- [ ] **B)** Pre-shared key
- [ ] **C)** Captive portal
- [ ] **D)** MAC authentication only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The profile uses dot1x with EAP, aligning with WPA2/WPA3-Enterprise and RADIUS-based identity management.
 
 
</details>

### 28. What is the most efficient way to segment users who connect to the same SSID in an Aruba campus WLAN?

- [ ] **A)** Define user roles with RBAC
- [ ] **B)** Create a unique SSID for every user group
- [ ] **C)** Change the VLAN on one SSID
- [ ] **D)** Hide the SSID

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Changing VLAN per SSID is less efficient than role-based access control. The exam expects user identity, not SSID, to drive segmentation.
 
 
</details>

### 29. Which two statements accurately describe Aruba AirMatch and how it performs RF optimization across the mobility domain?

- [ ] **A)** It is an AI-driven engine that automates RF optimization
- [ ] **B)** It uses historical client data and RF telemetry
- [ ] **C)** It makes real-time second-by-second channel changes
- [ ] **D)** It only adjusts SSID broadcast intervals

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> AirMatch is a centralized AI engine using historical data and RF telemetry in periodic, data-driven optimization cycles.
 
 
</details>

### 30. The code block enables an automated RF feature in Aruba. What does this feature primarily optimize across the campus?

```text
rf-profile campus
 airmatch
 channel-plan auto
 power-plan auto

```

- [ ] **A)** Channel selection and transmit power
- [ ] **B)** Client web authentication
- [ ] **C)** Gateway routing tables
- [ ] **D)** DHCP address pools

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AirMatch automates optimal channel plans and transmit power across the mobility domain, moving beyond reactive adjustments.
 
 
</details>

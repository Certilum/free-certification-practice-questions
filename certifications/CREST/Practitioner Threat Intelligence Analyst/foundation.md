<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CREST/CREST%20Practitioner%20Threat%20Intelligence%20Analyst%20(CPTIA)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Practitioner Threat Intelligence Analyst</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Operationalizing Threat Intelligence](#operationalizing-threat-intelligence) (4 questions)
- [Threat Intelligence Analysis and Production](#threat-intelligence-analysis-and-production) (9 questions)
- [Threat Intelligence Collection](#threat-intelligence-collection) (6 questions)
- [Threat Intelligence Concepts and Principles](#threat-intelligence-concepts-and-principles) (6 questions)
- [Threat Intelligence Dissemination and Integration](#threat-intelligence-dissemination-and-integration) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:39.819Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Operationalizing Threat Intelligence | 4 |
| Threat Intelligence Analysis and Production | 9 |
| Threat Intelligence Collection | 6 |
| Threat Intelligence Concepts and Principles | 6 |
| Threat Intelligence Dissemination and Integration | 5 |

---

### **Operationalizing Threat Intelligence**

### 1. What is the primary goal of proactive defense in threat intelligence?

- [ ] **A)** To respond to incidents after they occur
- [ ] **B)** To anticipate and prevent attacks before they happen
- [ ] **C)** To comply with regulatory requirements
- [ ] **D)** To reduce the cost of security tools

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Proactive defense shifts from reactive incident response to anticipatory security operations, aiming to detect and prevent attacks early.
 
 
</details>

### 2. Which of the following are core pillars of proactive defense? (Select all that apply)

- [ ] **A)** Hunting
- [ ] **B)** Hardening
- [ ] **C)** Deception
- [ ] **D)** Vulnerability scanning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Proactive defense includes hunting, hardening, and deception as core pillars to detect and prevent threats.
 
 
</details>

### 3. Analyze the following scenario: An analyst searches logs for hosts that executed an Office document and then made outbound HTTPS connections to newly registered domains. What proactive defense activity is being performed?

```sql
SELECT * FROM logs WHERE process_name = 'WINWORD.EXE' AND dest_port = 443 AND dest_domain LIKE '%.xyz';
```

- [ ] **A)** Hunting
- [ ] **B)** Hardening
- [ ] **C)** Deception
- [ ] **D)** Incident response

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Hunting involves hypothesis-driven searches for undetected threats based on threat intelligence.
 
 
</details>

### 4. What type of intelligence is most suitable for proactive defense rather than reactive detection?

- [ ] **A)** Indicators of Compromise (IOCs)
- [ ] **B)** Tactics, Techniques, and Procedures (TTPs)
- [ ] **C)** IP address blocklists
- [ ] **D)** File hashes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Proactive defense requires behavioral patterns (TTPs) to hunt for unknown variants, not just known bad indicators.
 
 
</details>


---

### **Threat Intelligence Analysis and Production**

### 5. What is the primary purpose of Analysis of Competing Hypotheses (ACH) in threat intelligence?

- [ ] **A)** To confirm a single hypothesis as true
- [ ] **B)** To identify which hypotheses are least supported
- [ ] **C)** To generate as many hypotheses as possible
- [ ] **D)** To rank hypotheses by their impact on the organization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> ACH systematically evaluates each hypothesis against evidence, focusing on the least supported to avoid confirmation bias.
 
 
</details>

### 6. Which of the following are key concepts in structured analysis as per the CPTIA syllabus? (Choose two)

- [ ] **A)** MECE principle
- [ ] **B)** Pre-mortem analysis
- [ ] **C)** Bayesian inference
- [ ] **D)** Root cause analysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> MECE and Pre-mortem are listed; Bayesian and Root cause are not part of the defined key concepts.
 
 
</details>

### 7. Given a scenario where an analyst has three hypotheses for a malware campaign, which technique should be used to systematically evaluate them?

```plaintext
// Pseudocode for ACH matrix
Hypotheses = [H1, H2, H3]
Evidence = [E1, E2, E3]
For each H, assess consistency with E
Score = sum of consistent evidence / total evidence
Select H with lowest score as least supported
```

- [ ] **A)** Brainstorming
- [ ] **B)** Analysis of Competing Hypotheses
- [ ] **C)** SWOT analysis
- [ ] **D)** Root cause analysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> ACH is specifically designed to evaluate and compare multiple hypotheses using evidence, reducing bias.
 
 
</details>

### 8. What is the first step in static malware analysis?

- [ ] **A)** Dynamic execution in a sandbox
- [ ] **B)** File hashing (e.g., MD5, SHA1, SHA256)
- [ ] **C)** Network traffic capture
- [ ] **D)** Disassembly of the binary

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Static analysis begins with file hashing to generate unique identifiers for identification and lookup.
 
 
</details>

### 9. Which of the following are Indicators of Compromise (IOCs) that can be extracted from dynamic malware analysis? (Choose two)

- [ ] **A)** API calls such as CreateRemoteThread
- [ ] **B)** Embedded strings from the binary
- [ ] **C)** Registry modifications for persistence
- [ ] **D)** PE header imports and exports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Dynamic analysis observes runtime behavior: API calls and registry changes are behavioral IOCs; strings and PE headers are static.
 
 
</details>

### 10. During network traffic analysis, which tool is commonly used to capture and inspect packet captures for extracting IOCs?

```bash
# Example Zeek command
zeek -C -r capture.pcap
```

- [ ] **A)** Wireshark
- [ ] **B)** Zeek
- [ ] **C)** Nmap
- [ ] **D)** Metasploit

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Zeek is specifically designed for network traffic analysis, producing logs for security monitoring.
 
 
</details>

### 11. What is the purpose of pivot analysis in threat intelligence?

- [ ] **A)** To confirm a single IOC as malicious
- [ ] **B)** To use one indicator to find related or new indicators
- [ ] **C)** To remove false positives from a feed
- [ ] **D)** To assign a severity score to an IOC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Pivot analysis leverages one known IOC to discover other associated IOCs, expanding the threat picture.
 
 
</details>

### 12. Which two factors should analysts consider when validating an Indicator of Compromise?

- [ ] **A)** Freshness (age of the indicator)
- [ ] **B)** The color of the hacker group logo
- [ ] **C)** Fidelity (likelihood of true positive)
- [ ] **D)** The number of syllables in the domain name

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Validation depends on how recent and reliable the IOC is; freshness and fidelity are critical.
 
 
</details>

### 13. In log analysis, which Windows Event ID is associated with process creation?

```xml
// Example log entry
<EventID>4688</EventID>
<Data Name="NewProcessName">C:\Windows\System32\cmd.exe</Data>
```

- [ ] **A)** 4624
- [ ] **B)** 4688
- [ ] **C)** 4634
- [ ] **D)** 5140

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Event ID 4688 records process creation, a key indicator for monitoring execution.
 
 
</details>


---

### **Threat Intelligence Collection**

### 14. Which of the following is a key characteristic of Open Source Intelligence (OSINT)?

- [ ] **A)** Requires subscription fees
- [ ] **B)** Often requires cross-referencing for validation
- [ ] **C)** Always provides high-confidence IOCs
- [ ] **D)** Only available from government sources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> OSINT is free and abundant but requires constant cross-referencing to ensure reliability.
 
 
</details>

### 15. Which two methods are considered passive collection techniques for domains?

- [ ] **A)** WHOIS lookup
- [ ] **B)** Live DNS query
- [ ] **C)** Passive DNS
- [ ] **D)** URL scanning service

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> WHOIS and passive DNS query registry or historical records without contacting the domain's authoritative servers.
 
 
</details>

### 16. The following MISP API call uploads an indicator. What type of indicator is being uploaded?

```json
"type": "ip-dst",
"value": "198.51.100.10"
```

- [ ] **A)** IP address
- [ ] **B)** Domain name
- [ ] **C)** File hash
- [ ] **D)** URL

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'value' field contains an IP address, which is the indicator type being uploaded.
 
 
</details>

### 17. What is the primary function of Shodan in automated collection?

- [ ] **A)** Store and share structured IOCs
- [ ] **B)** Coordinate incident response
- [ ] **C)** Discover internet-facing services and assets
- [ ] **D)** Perform malware analysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Shodan indexes banners from internet-connected devices for passive reconnaissance.
 
 
</details>

### 18. Which two steps are essential before deduplication in a data processing pipeline?

- [ ] **A)** Normalization
- [ ] **B)** Encryption
- [ ] **C)** Schema mapping
- [ ] **D)** Source validation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Normalization ensures consistent format; schema mapping aligns data to a common model before duplicates can be identified.
 
 
</details>

### 19. The analyst writes: 'We have no information on the adversary's current C2 infrastructure.' This represents which type of intelligence gap?

```javascript
// Current C2 infrastructure unknown
```

- [ ] **A)** Knowledge gap
- [ ] **B)** Source gap
- [ ] **C)** Temporal gap
- [ ] **D)** Resolution gap

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The gap is a lack of information (knowledge), not due to source unavailability or timeframe.
 
 
</details>


---

### **Threat Intelligence Concepts and Principles**

### 20. What is the foundation of threat intelligence, according to the CREST CPTIA framework?

- [ ] **A)** A collection of raw Indicators of Compromise (IoCs)
- [ ] **B)** Evidence-based knowledge including context, mechanisms, indicators, implications, and actionable advice
- [ ] **C)** A list of threat actor names and their motivations
- [ ] **D)** Real-time data feeds from commercial vendors

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Threat intelligence is defined as evidence-based knowledge, including context, mechanisms, indicators, implications, and actionable advice about an existing or emerging menace or hazard to assets. Raw IoCs alone are data, not intelligence.
 
 
</details>

### 21. Which of the following are phases in the intelligence lifecycle as described in the CREST CPTIA framework? (Select all that apply.)

- [ ] **A)** Direction
- [ ] **B)** Collection
- [ ] **C)** Processing
- [ ] **D)** Automation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The intelligence lifecycle consists of Direction, Collection, Processing, Analysis, Dissemination, and Feedback. Automation is a tool, not a lifecycle phase.
 
 
</details>

### 22. Review the following intelligence report snippet. What type of intelligence does it represent?

```text
Indicators of Compromise:
- IP: 198.51.100.7
- MD5: d41d8cd98f00b204e9800998ecf8427e
- Domain: malware.example.com
```

- [ ] **A)** Strategic Intelligence
- [ ] **B)** Operational Intelligence
- [ ] **C)** Tactical Intelligence
- [ ] **D)** Technical Intelligence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> The report shows a list of specific IP addresses and file hashes (IoCs). This is technical intelligence, which is the most granular level focused on indicators of compromise.
 
 
</details>

### 23. Which phase of the intelligence lifecycle involves defining Priority Intelligence Requirements (PIRs)?

- [ ] **A)** Collection
- [ ] **B)** Direction
- [ ] **C)** Analysis
- [ ] **D)** Dissemination

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The Direction phase is where requirements are gathered and priority intelligence requirements (PIRs) are defined. This sets the 'why' for the entire intelligence cycle.
 
 
</details>

### 24. Which of the following are characteristics of strategic intelligence? (Select all that apply.)

- [ ] **A)** Focused on long-term threats and geopolitical trends
- [ ] **B)** Contains detailed Indicators of Compromise (IoCs)
- [ ] **C)** Intended for senior decision-makers such as the CISO or board
- [ ] **D)** Provides information about specific adversary TTPs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Strategic intelligence is high-level, long-term, and consumed by executives. It does not include detailed IoCs or TTPs; those are tactical/technical.
 
 
</details>

### 25. Look at the following process description. Which phase of the intelligence lifecycle is being executed?

```python
def process_data(raw_logs):
    normalized = []
    for log in raw_logs:
        entry = {
            'timestamp': log['time'],
            'source_ip': log['src'],
            'event_type': log['type']
        }
        normalized.append(entry)
    return normalized
```

- [ ] **A)** Collection
- [ ] **B)** Processing
- [ ] **C)** Analysis
- [ ] **D)** Dissemination

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Normalizing, deduplicating, and converting data into a structured format (e.g., CSV to STIX) is the Processing phase of the intelligence lifecycle.
 
 
</details>


---

### **Threat Intelligence Dissemination and Integration**

### 26. Which audience requires a report focused on business impact and financial risk?

- [ ] **A)** Executives
- [ ] **B)** SOC analysts
- [ ] **C)** Technical teams
- [ ] **D)** Threat hunters

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Executives need strategic, business-focused intelligence to make budget and risk decisions.
 
 
</details>

### 27. Which two elements are typically included in a technical team report but not in an executive summary?

- [ ] **A)** MITRE ATT&CK techniques
- [ ] **B)** Business impact analysis
- [ ] **C)** Raw indicators of compromise
- [ ] **D)** Budget recommendations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Technical teams need detailed TTPs and IOCs; executives need high-level impact and resource recommendations.
 
 
</details>

### 28. Refer to the code block. What does this TLP marking indicate?

```text
TLP:RED
```

- [ ] **A)** Limited to named recipients
- [ ] **B)** Organization-wide circulation
- [ ] **C)** Community-wide sharing
- [ ] **D)** Public disclosure allowed

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TLP:RED means intelligence is disclosed only to specific named individuals and cannot be shared further.
 
 
</details>

### 29. Which STIX domain object would you use to represent a known malicious IP address?

- [ ] **A)** Indicator
- [ ] **B)** Campaign
- [ ] **C)** Threat Actor
- [ ] **D)** Malware

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An Indicator SDO is used for observable patterns like IPs, hashes, or domains that suggest malicious activity.
 
 
</details>

### 30. Which two protocols or platforms are primarily used to transport and share threat intelligence?

- [ ] **A)** TAXII
- [ ] **B)** MISP
- [ ] **C)** STIX
- [ ] **D)** ISO 27001

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> TAXII is a transport protocol; MISP is a collaborative platform with sharing capabilities. STIX is a data model, not transport.
 
 
</details>

<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/CREST/CREST%20Registered%20Threat%20Intelligence%20Analyst%20(CRTIA)" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Registered Threat Intelligence Analyst</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Analysis and Processing](#analysis-and-processing) (7 questions)
- [Dissemination and Reporting](#dissemination-and-reporting) (6 questions)
- [Intelligence Collection and Sources](#intelligence-collection-and-sources) (9 questions)
- [Operational Intelligence and Incident Response](#operational-intelligence-and-incident-response) (3 questions)
- [Threat Intelligence Concepts and Principles](#threat-intelligence-concepts-and-principles) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:27:47.822Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Analysis and Processing | 7 |
| Dissemination and Reporting | 6 |
| Intelligence Collection and Sources | 9 |
| Operational Intelligence and Incident Response | 3 |
| Threat Intelligence Concepts and Principles | 5 |

---

### **Analysis and Processing**

### 1. What is the primary purpose of the Analysis of Competing Hypotheses (ACH) technique in threat intelligence?

- [ ] **A)** To evaluate multiple hypotheses against available evidence
- [ ] **B)** To challenge a single prevailing hypothesis without evidence
- [ ] **C)** To brainstorm as many ideas as possible in a short time
- [ ] **D)** To map intrusion events into a visual framework

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> ACH is a structured analytic technique that lists all plausible hypotheses and systematically evaluates evidence for and against each, with the goal of refuting hypotheses rather than confirming them. It is designed to reduce cognitive biases.
 
 
</details>

### 2. Which of the following are the four core vertices of the Diamond Model of Intrusion Analysis? (Select all that apply)

- [ ] **A)** Adversary
- [ ] **B)** Capability
- [ ] **C)** Infrastructure
- [ ] **D)** Victim

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> The Diamond Model has exactly four vertices: Adversary, Capability, Infrastructure, and Victim. Meta-features like social-political-economic context are additional, not vertices.
 
 
</details>

### 3. In the Diamond Model, to which vertex does the IP address in the code block most likely belong?

```python
ip_address = '192.168.1.1'
# This IP is used by C2 server
```

- [ ] **A)** Adversary
- [ ] **B)** Capability
- [ ] **C)** Infrastructure
- [ ] **D)** Victim

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Infrastructure includes network resources such as IP addresses, domains, and servers that the adversary uses to conduct operations. The IP is a network indicator, thus Infrastructure.
 
 
</details>

### 4. Which structured analytic technique involves an individual deliberately arguing against a prevailing hypothesis to test its robustness?

- [ ] **A)** Devil's Advocacy
- [ ] **B)** Red Teaming
- [ ] **C)** Brainstorming
- [ ] **D)** Premortem

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Devil's Advocacy is a structured technique where an individual (within the team) argues against the prevailing hypothesis. Red Teaming involves an external group simulating an adversary.
 
 
</details>

### 5. Which of the following are examples of structured analytic techniques used in threat intelligence? (Select all that apply)

- [ ] **A)** Analysis of Competing Hypotheses (ACH)
- [ ] **B)** Checklist Analysis
- [ ] **C)** Brainstorming
- [ ] **D)** Intuitive Judgment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> SATs include ACH, Devil's Advocacy, Brainstorming, and Checklist Analysis. Intuitive judgment is unstructured and prone to bias.
 
 
</details>

### 6. According to the Diamond Model, what is the role of the 'Capability' vertex as shown in the code block?

```python
malware_hash = 'e3b0c44b1a5c7f8d9e0f1a2b3c4d5e6f'
# SHA256 of the dropper
```

- [ ] **A)** The tool or technique used by the adversary
- [ ] **B)** The network infrastructure used for C2
- [ ] **C)** The entity being attacked
- [ ] **D)** The individual behind the attack

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Capability refers to the tools, malware, or techniques (TTPs) that the adversary employs. A malware hash is a specific indicator of a capability.
 
 
</details>

### 7. What is the primary benefit of using structured analytic techniques over unstructured intuition?

- [ ] **A)** They mitigate cognitive biases and improve accuracy
- [ ] **B)** They allow faster decision making with less data
- [ ] **C)** They eliminate the need for evidence collection
- [ ] **D)** They guarantee correct attribution every time

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Structured analytic techniques (SATs) are designed to mitigate cognitive biases such as confirmation bias and anchoring, leading to more reliable and defensible judgments.
 
 
</details>


---

### **Dissemination and Reporting**

### 8. What is the primary purpose of an executive summary in a threat intelligence report?

- [ ] **A)** To provide raw technical indicators for analysts
- [ ] **B)** To deliver a concise overview of key threats and business impact
- [ ] **C)** To list all sources used in the analysis
- [ ] **D)** To describe the methodology in detail

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The executive summary is a brief, jargon-free section that highlights critical threats and business consequences for non-technical leaders.
 
 
</details>

### 9. Which two elements are essential for a non-technical audience in a threat briefing?

- [ ] **A)** List of specific IP addresses
- [ ] **B)** Business risk and financial impact
- [ ] **C)** Strategic recommendations
- [ ] **D)** YARA rules for detection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Executives need risk context and action items, not technical details like IPs or YARA rules.
 
 
</details>

### 10. Based on the code block below, what does the TLP label indicate?

```plaintext
TLP:AMBER
This report contains sensitive information about a current phishing campaign.
```

- [ ] **A)** Only named recipients can view it
- [ ] **B)** Can be shared within the organization on need-to-know
- [ ] **C)** May be shared publicly
- [ ] **D)** Must be destroyed after 24 hours

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> TLP:AMBER restricts sharing to the organization's internal team with a legitimate need.
 
 
</details>

### 11. What is the correct TLP marking for intelligence that can be shared with industry partners but not the public?

- [ ] **A)** TLP:RED
- [ ] **B)** TLP:AMBER
- [ ] **C)** TLP:GREEN
- [ ] **D)** TLP:CLEAR

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> TLP:GREEN allows sharing within the community (e.g., ISAC members) but not public distribution.
 
 
</details>

### 12. Which two items should be included in a technical intelligence report for SOC analysts?

- [ ] **A)** MITRE ATT&CK technique IDs
- [ ] **B)** YARA rules and hashes
- [ ] **C)** Estimated financial loss
- [ ] **D)** Executive summary only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Technical audiences need actionable indicators like TTPs and detection rules, not business impact numbers.
 
 
</details>

### 13. What is the meaning of the code word 'NOFORN' in the classification label?

```plaintext
CLASSIFICATION: CONFIDENTIAL // NOFORN
```

- [ ] **A)** Not to be shared with foreign nationals
- [ ] **B)** No foreign travel allowed
- [ ] **C)** Not for public release
- [ ] **D)** No further distribution

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NOFORN indicates the intelligence cannot be shared with non-citizens or foreign entities.
 
 
</details>


---

### **Intelligence Collection and Sources**

### 14. What does the acronym OSINT stand for in threat intelligence?

- [ ] **A)** Open Source Intelligence
- [ ] **B)** Operational Security Intelligence
- [ ] **C)** Online System Intelligence
- [ ] **D)** Open System Intelligence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> OSINT stands for Open Source Intelligence, which is intelligence derived from publicly available information. The other options are incorrect and do not represent the accepted definition.
 
 
</details>

### 15. Which of the following are considered OSINT sources? (Select all that apply)

- [ ] **A)** Public social media posts
- [ ] **B)** Company internal HR databases
- [ ] **C)** Government tax records (publicly accessible)
- [ ] **D)** Classified military reports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> OSINT includes publicly available information. Social media and public government records are OSINT. Internal databases and classified material are not publicly available.
 
 
</details>

### 16. Analyze the following search operator and determine its purpose in OSINT collection.

```plaintext
site:example.com intitle:login
```

- [ ] **A)** It restricts results to a specific domain
- [ ] **B)** It searches for files of a specific type
- [ ] **C)** It shows only exact phrase matches
- [ ] **D)** It excludes certain keywords from results

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The operator 'site:' restricts search results to a particular domain (e.g., site:example.com). This is a fundamental OSINT technique to narrow down public information from a specific website.
 
 
</details>

### 17. In the TRAAP framework for evaluating OSINT sources, what does the 'R' stand for?

- [ ] **A)** Relevance
- [ ] **B)** Reliability
- [ ] **C)** Recency
- [ ] **D)** Rigour

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> TRAAP stands for Timeliness, Relevance, Authority, Accuracy, and Purpose. The 'R' is Relevance – whether the information directly addresses the intelligence requirement.
 
 
</details>

### 18. Which of the following are correct descriptions of the Admiralty Code for source reliability? (Select all that apply)

- [ ] **A)** An A-rated source is considered highly reliable
- [ ] **B)** An F-rated source is completely unreliable
- [ ] **C)** The code applies only to technical intelligence sources
- [ ] **D)** The code has six letters (A-F) for source reliability

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> The Admiralty Code rates source reliability from A (most reliable) to F (least reliable). It applies to all intelligence sources, not just technical. Options 1,2,4 are correct.
 
 
</details>

### 19. Review the following Python code snippet used for passive OSINT collection. What is its primary function?

```python
import requests
url = "https://example.com/robots.txt"
r = requests.get(url)
print(r.text)
```

- [ ] **A)** It downloads files from a remote server
- [ ] **B)** It queries a website's robots.txt file
- [ ] **C)** It performs a port scan on a target
- [ ] **D)** It extracts email addresses from a webpage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code uses the requests library to retrieve the robots.txt file from a given domain. This is a passive OSINT technique to understand what parts of a site are disallowed for crawling.
 
 
</details>

### 20. Which of the following is a passive OSINT technique?

- [ ] **A)** Performing an active port scan on a target IP
- [ ] **B)** Querying passive DNS databases for historical records
- [ ] **C)** Sending a phishing email to gather credentials
- [ ] **D)** Deploying a honeypot to capture attacker activity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Passive OSINT involves no direct interaction with the target. Querying historical DNS records is passive, whereas port scanning and honeypots are active techniques that may alert the adversary.
 
 
</details>

### 21. Which of the following are common pitfalls when evaluating OSINT sources? (Select all that apply)

- [ ] **A)** Assuming popularity equals credibility
- [ ] **B)** Cross-checking data with independent sources
- [ ] **C)** Over-relying on automated tools without manual review
- [ ] **D)** Treating all dark web content as authentic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Common traps include confusing popularity with credibility, over-reliance on automation, and assuming dark web data is genuine. Cross-checking is good practice, not a pitfall.
 
 
</details>

### 22. Examine the SQL query below. What intelligence discipline does this technique belong to?

```sql
SELECT * FROM firewall_logs WHERE src_ip = '192.168.1.100' AND timestamp > NOW() - INTERVAL 1 DAY;
```

- [ ] **A)** Human Intelligence (HUMINT)
- [ ] **B)** Technical Intelligence (TECHINT)
- [ ] **C)** Open-Source Intelligence (OSINT)
- [ ] **D)** Signals Intelligence (SIGINT)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Querying a database using SQL is a technical data collection method. TECHINT encompasses passive and active technical means such as database queries, network scans, and malware analysis.
 
 
</details>


---

### **Operational Intelligence and Incident Response**

### 23. What does the integration of threat intelligence into incident response primarily transform?

- [ ] **A)** Raw indicators into actionable triggers
- [ ] **B)** Alerts into manual ticketing
- [ ] **C)** SOCs into standalone teams
- [ ] **D)** Intelligence into static reports

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Integration transforms raw contextualised intelligence into actionable triggers, enrichments, and feedback loops for detection and response.
 
 
</details>

### 24. Which two components are essential for integrating intelligence into SOC operations?

- [ ] **A)** Seamless interoperability between TIPs and SIEMs
- [ ] **B)** Manual analyst review for every alert
- [ ] **C)** Automated indicator enrichment via APIs
- [ ] **D)** Isolated intelligence consumption without feedback

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Integration demands seamless interoperability between TIPs, SIEMs, SOARs, and automated enrichment via APIs to transform intelligence into actions.
 
 
</details>

### 25. Based on the code block, which protocol is used to transport structured threat intelligence?

```python
def query_taxii(collection):
    # TAXII client to pull STIX indicators
    discovery = TAXIIDiscovery('https://taxii.example.com')
    poll = discovery.poll(collection)
    return poll.manifest
```

- [ ] **A)** STIX
- [ ] **B)** TAXII
- [ ] **C)** OAuth
- [ ] **D)** MISP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> TAXII is the Trusted Automated Exchange of Intelligence Information protocol used to transport STIX data over HTTPS.
 
 
</details>


---

### **Threat Intelligence Concepts and Principles**

### 26. Which level of threat intelligence is primarily consumed by executive leadership such as the CISO or board of directors and focuses on long-term risk management?

- [ ] **A)** Tactical Intelligence
- [ ] **B)** Operational Intelligence
- [ ] **C)** Strategic Intelligence
- [ ] **D)** Technical Intelligence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Strategic intelligence is designed for executive leadership (CISO, board) and informs long-term risk management, resource allocation, and business strategy. It focuses on trends, geopolitical forces, and industry-level threats.
 
 
</details>

### 27. Which two of the following are characteristics of tactical intelligence? (Select two.)

- [ ] **A)** It consists of specific indicators of compromise such as IP addresses and file hashes.
- [ ] **B)** It is consumed by frontline SOC analysts for immediate detection and blocking.
- [ ] **C)** It informs long-term investment strategies and geopolitical risks.
- [ ] **D)** It covers campaign-level TTPs and adversary behaviour patterns.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Tactical intelligence provides immediate, technical IoCs (IPs, hashes) used by frontline analysts for real-time detection and blocking. It has a short shelf life and supports immediate defensive actions.
 
 
</details>

### 28. The intelligence analyst has been tasked with producing a threat report. At what step in the intelligence cycle should the analyst first define the Priority Intelligence Requirements (PIRs)?

```plaintext
// Direction phase: Define PIRs and collection plan
// Example: PIR: 'What are the top ransomware groups targeting our sector?'
```

- [ ] **A)** Collection
- [ ] **B)** Direction
- [ ] **C)** Analysis
- [ ] **D)** Dissemination

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Direction is the first phase of the intelligence cycle where PIRs are defined based on consumer needs. This sets the scope for all subsequent collection and analysis activities.
 
 
</details>

### 29. What is the key difference between information and intelligence in the context of threat intelligence?

- [ ] **A)** Information is collected automatically, while intelligence is always produced by humans.
- [ ] **B)** Intelligence is the product of analysis that answers 'so what?' and is tailored to a consumer's decision.
- [ ] **C)** Information contains more context than intelligence.
- [ ] **D)** Intelligence is raw data that has been collated without interpretation.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Intelligence results from rigorous analysis that provides context, evaluation, and actionable recommendations. It answers 'so what?' and is specifically tailored to a consumer's decision-making needs. Information is structured data that answers 'what happened?' but lacks analytical depth.
 
 
</details>

### 30. Which three of the following are valid phases of the intelligence cycle? (Select three.)

- [ ] **A)** Direction
- [ ] **B)** Collection
- [ ] **C)** Exploitation
- [ ] **D)** Dissemination

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> The intelligence cycle consists of Direction, Collection, Processing, Analysis, Dissemination, and Feedback. Exploitation is not a standard phase of the intelligence cycle; it belongs to other domains like vulnerability management.
 
 
</details>

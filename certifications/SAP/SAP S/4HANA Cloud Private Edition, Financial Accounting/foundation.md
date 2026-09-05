<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/SAP/SAP%20S%3A4HANA%20Cloud%20Private%20Edition%2C%20Financial%20Accounting.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>SAP S/4HANA Cloud Private Edition, Financial Accounting</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Accounts Payable](#accounts-payable) (4 questions)
- [Accounts Receivable](#accounts-receivable) (4 questions)
- [Asset Accounting](#asset-accounting) (3 questions)
- [Financial Accounting Overview](#financial-accounting-overview) (5 questions)
- [General Ledger](#general-ledger) (6 questions)
- [Period-End/Year-End Closing](#period-end-year-end-closing) (5 questions)
- [Reporting and Analytics](#reporting-and-analytics) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:47:04.414Z |
| Domains | 7 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Accounts Payable | 4 |
| Accounts Receivable | 4 |
| Asset Accounting | 3 |
| Financial Accounting Overview | 5 |
| General Ledger | 6 |
| Period-End/Year-End Closing | 5 |
| Reporting and Analytics | 3 |

---

### **Accounts Payable**

### 1. Which chart of accounts is assigned to company codes as the primary structure for day-to-day postings in the general ledger?

- [ ] **A)** Operating Chart of Accounts
- [ ] **B)** Group Chart of Accounts
- [ ] **C)** Country-Specific Chart of Accounts
- [ ] **D)** Account Group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The operating chart of accounts is assigned to company codes for day-to-day postings, ensuring a unified account structure for financial statements.
 
 
</details>

### 2. Which statements about charts of accounts and account groups are correct? Choose all that apply.

- [ ] **A)** A company code has one operating CoA and can use mapped group and country-specific CoAs.
- [ ] **B)** Account number is defined at CoA level, while field status can be company-code level.
- [ ] **C)** Account groups are assigned to G/L master records, not to company codes.
- [ ] **D)** A company code can use only one chart of accounts in total.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A company code uses one operating CoA plus mapped group/country-specific CoAs. Account groups are assigned to master records, and field status can differ at company code level.
 
 
</details>

### 3. The SQL snippet reads from the Universal Journal. What type of ledger data does the query select?

```sql
SELECT RLDNR, BUKRS, BELNR, DMBTR
FROM ACDOCA
WHERE RLDNR = '0L';
```

- [ ] **A)** Leading ledger postings
- [ ] **B)** Non-leading ledger postings
- [ ] **C)** Extension ledger adjustments
- [ ] **D)** Country-specific chart data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> 0L is the hardcoded leading ledger, always active and used as the basis for group valuation.
 
 
</details>

### 4. Which statement best describes the Leading Ledger (0L) in SAP S/4HANA?

- [ ] **A)** It is hardcoded and always active
- [ ] **B)** It can be deleted and replaced
- [ ] **C)** It is an optional extension ledger
- [ ] **D)** It stores only delta adjustments

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Leading Ledger 0L is hardcoded and fundamental; it cannot be deleted or replaced with another ledger.
 
 
</details>


---

### **Accounts Receivable**

### 5. What is the main purpose of the operating chart of accounts in SAP S/4HANA?

- [ ] **A)** It defines day-to-day G/L postings across assigned company codes
- [ ] **B)** It creates statutory reports for a specific country
- [ ] **C)** It maps local accounts for group consolidation
- [ ] **D)** It replaces the Universal Journal for parallel accounting

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The operating CoA is assigned to company codes and provides the unified numbering and categorization structure used for daily postings. It supports consolidated statements.
 
 
</details>

### 6. Which two statements about the group chart of accounts are correct? Select all that apply.

- [ ] **A)** It facilitates consolidation across company codes with different operating charts of accounts.
- [ ] **B)** It maps local accounts to a common structure for group-level reporting.
- [ ] **C)** It is assigned to only one company code to enforce local reporting.
- [ ] **D)** It replaces the country-specific chart of accounts for legal reporting.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The group CoA is a common language for consolidation and mapping local accounts to group reporting. It does not replace country-specific statutory requirements.
 
 
</details>

### 7. The code block contains a query against the central financial table. Which best describes the table and ledger combination used in the query?

```sql
SELECT RCLNT, RLDNR, RBUKRS, RACCT, HSL, VALTYPE FROM ACDOCA WHERE RLDNR = '0L' AND RBUKRS = '1000';
```

- [ ] **A)** Universal Journal with the leading ledger (0L)
- [ ] **B)** Classic G/L document table without extension ledgers
- [ ] **C)** Segment table containing only country-specific data
- [ ] **D)** Customer master table with accounting principle data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query reads ACDOCA, the Universal Journal, and filters on ledger 0L, which is the leading ledger. This table stores integrated financial data.
 
 
</details>

### 8. What do account groups control when a G/L account master record is created?

- [ ] **A)** Number range and field status
- [ ] **B)** Only the company code currency
- [ ] **C)** The fiscal year variant of the ledger
- [ ] **D)** The assignment of the chart of accounts to a company code

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Account groups categorize accounts and control number ranges plus field status, indicating which fields are required, optional, or suppressed.
 
 
</details>


---

### **Asset Accounting**

### 9. Which chart of accounts is assigned to a company code for day-to-day postings in the general ledger?

- [ ] **A)** Operating chart of accounts
- [ ] **B)** Group chart of accounts
- [ ] **C)** Country-specific chart of accounts
- [ ] **D)** Extension chart of accounts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The operating chart of accounts is assigned to company codes for daily postings; group and country-specific charts are mapped to it for consolidation and statutory reporting.
 
 
</details>

### 10. Which statements about leading, non-leading, and extension ledgers in SAP S/4HANA are correct? Select all that apply.

- [ ] **A)** The leading ledger 0L is always active and cannot be deleted.
- [ ] **B)** An extension ledger stores complete independent transactions.
- [ ] **C)** A non-leading ledger can use a different fiscal year variant.
- [ ] **D)** Parallel accounting requires separate subledgers for each accounting principle.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The leading ledger 0L is hardcoded and always active. Non-leading ledgers can use different fiscal year variants; extension ledgers contain only delta data.
 
 
</details>

### 11. Review the configuration snippet. Which statement about chart of accounts assignment for company code DE01 is correct?

```plaintext
CONFIGURATION
Company code: DE01
Operating CoA: SOCA
Group CoA: GCA
Country-specific CoA: DCA
```

- [ ] **A)** DE01 uses SOCA for daily postings.
- [ ] **B)** DE01 can only have one chart of accounts in total.
- [ ] **C)** DCA is the primary chart for daily postings.
- [ ] **D)** GCA is used for local statutory reporting.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The operating CoA (SOCA) is assigned to the company code for daily postings. Group and country-specific COAs are additional mapped structures, not replacements for the operating CoA.
 
 
</details>


---

### **Financial Accounting Overview**

### 12. What chart of accounts is used for day-to-day postings in the general ledger?

- [ ] **A)** Operating Chart of Accounts
- [ ] **B)** Group Chart of Accounts
- [ ] **C)** Country-Specific Chart of Accounts
- [ ] **D)** Account Groups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Operating Chart of Accounts is assigned to company codes and is used for all day-to-day postings in the general ledger.
 
 
</details>

### 13. Which statements about charts of accounts are correct?

- [ ] **A)** A company code has one Operating CoA and can also use Group and Country-Specific CoAs through mapping.
- [ ] **B)** The Group Chart of Accounts maps local accounts to a unified structure for group reporting.
- [ ] **C)** Account groups control number ranges and required or optional fields during G/L account creation.
- [ ] **D)** A Country-Specific Chart of Accounts is required in every company code.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A company code has one Operating CoA and may use mapped Group/Country-Specific CoAs. Group CoA unifies reporting, and account groups control numbering and field status. Country-specific CoA is optional.
 
 
</details>

### 14. Examine the configuration block. Which element is configured as the anchor for distributing line items?

```plaintext
DocumentSplitting:
  SplittingCharacteristic = Profit Center
  ZeroBalanceClearing = Enabled
```

- [ ] **A)** Profit Center
- [ ] **B)** Company Code
- [ ] **C)** Fiscal Year
- [ ] **D)** Ledger

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block shows Profit Center as the Splitting Characteristic, which is the anchor used to distribute line items.
 
 
</details>

### 15. Which ledger is hardcoded and cannot be deleted in SAP S/4HANA?

- [ ] **A)** Leading Ledger (0L)
- [ ] **B)** Non-leading Ledger
- [ ] **C)** Extension Ledger
- [ ] **D)** Secondary Ledger

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Leading Ledger (0L) is hardcoded, always active, and serves as the basis for group valuation.
 
 
</details>

### 16. Which statements about extension ledgers are correct?

- [ ] **A)** They extend a base ledger and do not store their own data.
- [ ] **B)** They are used to capture delta adjustments without duplicating full transaction history.
- [ ] **C)** They cannot exist independently; they need a base ledger.
- [ ] **D)** They contain complete transaction data for parallel accounting.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Extension ledgers store adjustments on top of a base ledger, avoid duplication, and cannot exist independently.
 
 
</details>


---

### **General Ledger**

### 17. Which chart of accounts is used for day-to-day postings in the general ledger?

- [ ] **A)** Operating Chart of Accounts
- [ ] **B)** Group Chart of Accounts
- [ ] **C)** Country-Specific Chart of Accounts
- [ ] **D)** Extension Ledger

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The operating chart of accounts is the primary CoA assigned to company codes for day-to-day postings, ensuring a unified numbering and categorization structure.
 
 
</details>

### 18. Which statements about the Group Chart of Accounts are correct?

- [ ] **A)** It consolidates multiple operating charts
- [ ] **B)** It maps local accounts to a common structure
- [ ] **C)** It is the primary CoA for daily postings
- [ ] **D)** It replaces the operating chart of accounts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The Group CoA facilitates consolidation by mapping different operating charts into a common structure for group reporting; it is not used for daily postings and does not replace the operating CoA.
 
 
</details>

### 19. Review the configuration snippet. Which statement correctly describes the chart of accounts assignment?

```json
{
  "companyCode": "1010",
  "operatingCoA": "INT",
  "groupCoA": "GROUP",
  "countryCoA": "LOCAL"
}
```

- [ ] **A)** The group chart maps local accounts for consolidation
- [ ] **B)** The country chart is the primary chart for daily postings
- [ ] **C)** The operating chart is used for group-level reporting only
- [ ] **D)** Company code can only have the operating chart

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In the snippet, GROUP is assigned as the group chart, enabling consolidation mapping, while INT is the operating CoA and LOCAL is the optional country-specific CoA.
 
 
</details>

### 20. What is controlled by an account group in G/L account master data?

- [ ] **A)** Number range and field status
- [ ] **B)** Ledger assignment and company code currency
- [ ] **C)** Fiscal year variant and posting period
- [ ] **D)** Tax code and payment terms

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Account groups define the number range and determine which fields are required, optional, or suppressed during G/L account master data creation.
 
 
</details>

### 21. Which statements about G/L account master data in S/4HANA are correct?

- [ ] **A)** It is managed through the Universal Journal
- [ ] **B)** It can include segment-specific information
- [ ] **C)** Account numbers are defined at company code level
- [ ] **D)** Data can be controlled at chart or company code level

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> In S/4HANA, G/L account master data is centrally managed in the Universal Journal, can include segment-specific information, and can be controlled at the chart of accounts level or company code level. Account numbers are defined at CoA level.
 
 
</details>

### 22. Review the ledger configuration snippet. Which statement is correct?

```json
{
  "leadingLedger": "0L",
  "nonLeadingLedger": "L1",
  "extensionLedger": "EX"
}
```

- [ ] **A)** 0L is mandatory and cannot be deleted
- [ ] **B)** EX can be used as a base ledger
- [ ] **C)** L1 stores only delta adjustments
- [ ] **D)** 0L can be replaced by L1

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The leading ledger 0L is hardcoded in every S/4HANA system and cannot be deleted or replaced. Non-leading ledgers contain full data, and extension ledgers contain only delta adjustments.
 
 
</details>


---

### **Period-End/Year-End Closing**

### 23. In SAP S/4HANA, what is the main purpose of the operating chart of accounts for daily accounting activities?

- [ ] **A)** Primary CoA for daily postings
- [ ] **B)** Only for local statutory reporting
- [ ] **C)** Stores extension ledger adjustments
- [ ] **D)** Replaces the group chart of accounts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The operating chart of accounts is the primary CoA used for day-to-day postings and is assigned to each company code.
 
 
</details>

### 24. Which two statements accurately describe the Leading Ledger (0L) in the SAP S/4HANA system? Select two.

- [ ] **A)** Always active in every system
- [ ] **B)** Can be deleted or replaced
- [ ] **C)** Basis for group valuation
- [ ] **D)** An extension ledger with delta data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> The leading ledger is always active and is the basis for group valuation. It cannot be deleted or replaced because 0L is hardcoded.
 
 
</details>

### 25. The SQL statement shown queries the Universal Journal. Which ledger is selected by this query?

```sql
SELECT rldnr, rbukrs, gjahr, poper, hsl
FROM acdoca
WHERE rldnr = '0L';
```

- [ ] **A)** Leading Ledger
- [ ] **B)** Extension ledger
- [ ] **C)** Non-leading ledger
- [ ] **D)** Group chart of accounts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The query selects the hardcoded primary ledger, which is always active and used for group valuation.
 
 
</details>

### 26. What is the main function of the group chart of accounts when consolidating multiple company codes?

- [ ] **A)** Enables consolidation across different operating CoAs
- [ ] **B)** Handles daily postings for one company code
- [ ] **C)** Controls G/L account number ranges
- [ ] **D)** Stores extension ledger delta data

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The group chart of accounts maps local operating charts to a common structure, enabling consolidated financial statements across the enterprise.
 
 
</details>

### 27. Which two statements about non-leading ledgers in SAP S/4HANA are true? Select two options.

- [ ] **A)** Post according to local accounting standards
- [ ] **B)** May use different fiscal year variants
- [ ] **C)** Store only delta adjustments
- [ ] **D)** Replace the leading ledger

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Non-leading ledgers support local GAAP with different valuations, fiscal year variants, and depreciation areas; they do not replace or extend the leading ledger.
 
 
</details>


---

### **Reporting and Analytics**

### 28. In SAP S/4HANA, which chart of accounts is assigned to company codes for routine day-to-day postings in the general ledger?

- [ ] **A)** Operating Chart of Accounts
- [ ] **B)** Group Chart of Accounts
- [ ] **C)** Country-Specific Chart of Accounts
- [ ] **D)** Extension Ledger

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Operating Chart of Accounts is the primary CoA assigned to company codes for day-to-day postings in the general ledger.
 
 
</details>

### 29. Which statements about the operating chart of accounts and account groups are correct in SAP S/4HANA configuration?

- [ ] **A)** A company code has one Operating CoA but can also use Group and Country-Specific CoAs through mapping.
- [ ] **B)** Account groups control the number range and field status of G/L account master data.
- [ ] **C)** The Account Group is assigned to the G/L account, while the Operating CoA is assigned to the company code.
- [ ] **D)** The account number is defined at company code level, while field status is defined at chart of accounts level.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> A company code has one Operating CoA but can be mapped to Group and Country-Specific CoAs; account groups are assigned to G/L accounts and control number ranges and field status.
 
 
</details>

### 30. Review the configuration snippet and identify the entity to which accounting principles are assigned in SAP S/4HANA.

```plaintext
Ledger 0L -> Accounting Principle IFRS
Ledger L1 -> Accounting Principle Local GAAP
```

- [ ] **A)** Ledger
- [ ] **B)** Company Code
- [ ] **C)** Operating Chart of Accounts
- [ ] **D)** Fiscal Year Variant

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In S/4HANA, accounting principles are assigned to ledgers, not to company codes, charts of accounts, or fiscal year variants.
 
 
</details>

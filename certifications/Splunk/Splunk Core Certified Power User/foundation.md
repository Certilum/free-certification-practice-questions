<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Splunk/Splunk%20Core%20Certified%20Power%20User" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Splunk Core Certified Power User</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [CIM Normalization](#cim-normalization) (3 questions)
- [Correlation (stats vs transaction)](#correlation-stats-vs-transaction) (5 questions)
- [Data Models](#data-models) (3 questions)
- [Field Aliases and Calculated Fields](#field-aliases-and-calculated-fields) (3 questions)
- [Field Extractions](#field-extractions) (3 questions)
- [Filtering and Formatting (eval, where, fillnull)](#filtering-and-formatting-eval-where-fillnull) (3 questions)
- [Macros](#macros) (3 questions)
- [Tags and Event Types](#tags-and-event-types) (3 questions)
- [Visualizations (chart, timechart)](#visualizations-chart-timechart) (1 questions)
- [Workflow Actions](#workflow-actions) (3 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:48:13.411Z |
| Domains | 10 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| CIM Normalization | 3 |
| Correlation (stats vs transaction) | 5 |
| Data Models | 3 |
| Field Aliases and Calculated Fields | 3 |
| Field Extractions | 3 |
| Filtering and Formatting (eval, where, fillnull) | 3 |
| Macros | 3 |
| Tags and Event Types | 3 |
| Visualizations (chart, timechart) | 1 |
| Workflow Actions | 3 |

---

### **CIM Normalization**

### 1. During a Splunk search, which special symbol should be placed around a macro name to invoke it correctly?

- [ ] **A)** Backtick (`)
- [ ] **B)** Parentheses ( )
- [ ] **C)** Dollar sign ($)
- [ ] **D)** Asterisk (*)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A macro is invoked by surrounding its name with backticks, such as `my_macro`; using the name alone causes syntax errors.
 
 
</details>

### 2. Which of the following mistakes can cause a macro call to fail when used in a Splunk search?

- [ ] **A)** Using backticks around the macro name
- [ ] **B)** Forgetting the backticks around the macro name
- [ ] **C)** Placing the argument outside the backticks
- [ ] **D)** Calling the macro with arguments without parentheses

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C, D**
 
> 💡  **Explanation** 
> 
> Common traps include missing backticks, placing arguments outside the backticks, and omitting parentheses when arguments are used.
 
 
</details>

### 3. Review the SPL shown in the code block. Which statement about the macro invocation is correct?

```spl
index=main `my_macro(error_code)`
```

- [ ] **A)** It calls the macro named my_macro with the argument error_code
- [ ] **B)** It calls a macro named error_code with the argument my_macro
- [ ] **C)** It is invalid because the macro name and argument are reversed
- [ ] **D)** It creates a field called my_macro with the value error_code

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The backticks surround the macro name with a parenthesized argument, so `my_macro(error_code)` invokes my_macro and passes error_code.
 
 
</details>


---

### **Correlation (stats vs transaction)**

### 4. In Splunk SPL, what symbol must surround a macro name when you invoke it?

- [ ] **A)** Backticks (`)
- [ ] **B)** Parentheses ()
- [ ] **C)** Dollar signs ($)
- [ ] **D)** Single quotes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Macro invocation requires backticks around the macro name, for example `my_macro`. Without backticks, Splunk treats the name as a field or command.
 
 
</details>

### 5. Which statements about Splunk macro arguments are true?

- [ ] **A)** Arguments are defined with placeholders such as $arg1$.
- [ ] **B)** Values are passed in parentheses inside the backticks, for example `my_macro(value)`.
- [ ] **C)** The argument value passed in a search must include the placeholder name, such as `my_macro($arg1$)`.
- [ ] **D)** Arguments must be surrounded by double quotes to be recognized.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> In macro definitions, arguments use $name$ placeholders. At invocation, only values are passed inside backticks with parentheses; the placeholder name is not supplied.
 
 
</details>

### 6. Review the SPL in the code block. What is wrong with the macro invocation shown?

```spl
index=main | `my_macro` error_code
```

- [ ] **A)** The argument must be placed inside the backticks and parentheses, like `my_macro(error_code)`.
- [ ] **B)** The macro name should be in double quotes instead of backticks.
- [ ] **C)** The argument should be enclosed in square brackets.
- [ ] **D)** The search is correct; no change is needed.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Arguments must be inside the backticks with parentheses, such as `my_macro(error_code)`. Placing the argument outside the backticks is a common macro mistake.
 
 
</details>

### 7. What syntax is used to define a placeholder for an argument inside a Splunk macro definition?

- [ ] **A)** $arg1$
- [ ] **B)** `arg1`
- [ ] **C)** (arg1)
- [ ] **D)** %arg1%

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Macro arguments use dollar-sign placeholders such as $arg1$. During invocation, Splunk replaces the placeholder with the supplied value.
 
 
</details>

### 8. Which statements about Splunk macro scope are correct?

- [ ] **A)** Macros defined at the system level are available across all apps.
- [ ] **B)** Macros defined in a specific app are primarily available within that app.
- [ ] **C)** A macro with Private permissions is visible to all users who can search.
- [ ] **D)** When a global macro and an app macro have the same name, the global macro always takes precedence.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> System-level macros are global, app-level macros are sandboxed, private macros are not shared, and namespace collisions usually resolve in favor of the more local definition.
 
 
</details>


---

### **Data Models**

### 9. Which symbol must surround a macro name to invoke it in a Splunk search?

- [ ] **A)** An asterisk (*)
- [ ] **B)** A backtick (`)
- [ ] **C)** A dollar sign ($)
- [ ] **D)** A pair of parentheses ()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Macros are invoked with backticks around the macro name. Using the name alone causes Splunk to interpret it as a field or command, leading to syntax errors.
 
 
</details>

### 10. Which two statements correctly describe arguments in Splunk macros?

- [ ] **A)** Values passed in parentheses must match the order of placeholders in the definition.
- [ ] **B)** The argument value must be the same as the placeholder name used in the definition.
- [ ] **C)** Macros do not validate argument data types before execution.
- [ ] **D)** Arguments remain visible to outer search components after the macro runs.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Macro argument order must correspond to the placeholders, and macros have no built-in data type validation. The placeholder name does not need to be used in the call, and arguments are localized to the macro.
 
 
</details>

### 11. Based on the provided SPL snippet, what does the expression inside the backticks represent?

```spl
`my_macro(error_code)`
```

- [ ] **A)** The name of a field being extracted
- [ ] **B)** An argument passed to the macro my_macro
- [ ] **C)** A second macro called before my_macro
- [ ] **D)** A subsearch that returns events

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The backtick syntax invokes my_macro and passes error_code as the argument value. It is not a field, second macro, or subsearch.
 
 
</details>


---

### **Field Aliases and Calculated Fields**

### 12. What symbol must surround a macro name when invoking it in a Splunk search?

- [ ] **A)** Backtick
- [ ] **B)** Parenthesis
- [ ] **C)** Dollar sign
- [ ] **D)** Angle bracket

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The playbook states that macro invocation requires the backtick symbol surrounding the macro name, such as `my_macro`.
 
 
</details>

### 13. Which two statements about macro scope are true?

- [ ] **A)** System-level macros are available across all apps.
- [ ] **B)** A macro defined in a local app is automatically available in all other apps.
- [ ] **C)** A macro with Private permissions is not visible to other users.
- [ ] **D)** App-level macros are always visible to all users in every app context.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> System-level macros are global, while app-level macros remain local unless shared. A macro with Private permissions is hidden from other users.
 
 
</details>

### 14. In the macro definition shown in the code block, what is the purpose of the value enclosed in dollar signs?

```ini
[error_macro]
args = field
definition = status=$field$ error
```

- [ ] **A)** It is a placeholder that receives the argument passed during macro invocation.
- [ ] **B)** It is a literal string that appears in every search result.
- [ ] **C)** It is a field alias assigned by Splunk at search time.
- [ ] **D)** It is a comment ignored by the search engine.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The placeholder uses dollar signs and a name to inject the passed argument into the macro's definition at search time.
 
 
</details>


---

### **Field Extractions**

### 15. Which symbol must surround a macro name when a user invokes a macro in a Splunk search?

- [ ] **A)** Backticks (`)
- [ ] **B)** Parentheses ( )
- [ ] **C)** Dollar signs ($)
- [ ] **D)** Square brackets [ ]

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Macros are invoked by surrounding the macro name with backticks, for example `my_macro`. Without backticks, Splunk treats the name as a field or command.
 
 
</details>

### 16. Which of the following statements about arguments in Splunk macros are true? Select all that apply.

- [ ] **A)** Placeholders are written like $arg1$
- [ ] **B)** Arguments are substituted literally before parsing
- [ ] **C)** Macros validate integer and string types
- [ ] **D)** The placeholder name must be used as the value

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Macro placeholders use dollar signs and names, and arguments are substituted literally. Macros do not validate data types, and calls pass values rather than placeholder names.
 
 
</details>

### 17. Given the macro definition in the code block, which invocation correctly passes the value 500 to the macro?

```ini
[my_macro]
args = status_code
definition = status=$status_code$
```

- [ ] **A)** `my_macro(500)`
- [ ] **B)** my_macro(500)
- [ ] **C)** `my_macro` (500)
- [ ] **D)** 500(`my_macro`)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A macro with arguments is invoked by placing the macro name and its parenthesized arguments inside the backticks, like `my_macro(500)`. The value 500 is substituted for the $status_code$ placeholder.
 
 
</details>


---

### **Filtering and Formatting (eval, where, fillnull)**

### 18. Which symbol must surround a macro name when it is invoked in a Splunk search?

- [ ] **A)** Backticks (`)
- [ ] **B)** Parentheses ()
- [ ] **C)** Dollar signs ($)
- [ ] **D)** Square brackets []

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Macros are invoked by surrounding the macro name with backtick symbols, such as `my_macro`.
 
 
</details>

### 19. Which statements about macro arguments are true? Select all that apply.

- [ ] **A)** Arguments are passed inside backticks, for example `macro(value)`.
- [ ] **B)** Placeholder names must be included when calling the macro.
- [ ] **C)** Arguments are local to the macro's execution scope.
- [ ] **D)** Macros validate argument data types.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Arguments are passed in parentheses inside the backticks, are substituted into the macro, and are local to the macro. Placeholder names are not passed, and macros do not validate data types.
 
 
</details>

### 20. Review the SPL in the code block. What is returned when this macro call is processed?

```spl
index=main | `my_macro(ERROR)`
```

- [ ] **A)** A string of SPL based on the macro definition
- [ ] **B)** A set of events matching ERROR
- [ ] **C)** A syntax error because macros are not allowed after a pipe
- [ ] **D)** A field named ERROR

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A macro returns a string of SPL that is substituted into the search before execution; it does not directly return events or field values.
 
 
</details>


---

### **Macros**

### 21. Which symbol is required when invoking a macro in a Splunk search?

- [ ] **A)** Backtick
- [ ] **B)** Parenthesis
- [ ] **C)** Dollar sign
- [ ] **D)** Pipe

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Macros are invoked by surrounding the macro name with backtick characters, distinguishing them from fields or commands.
 
 
</details>

### 22. Which statements correctly describe Splunk macros?

- [ ] **A)** Macros return a string of SPL inserted into the search.
- [ ] **B)** A macro called by name alone without symbols executes normally.
- [ ] **C)** Argument placeholders are replaced with literal text before parsing.
- [ ] **D)** Macros return a filtered result set before the main query.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Macros produce a SPL string and placeholders undergo literal substitution before parsing, not run-time filtering.
 
 
</details>

### 23. In the code block, a macro is invoked with an argument. Where is the argument placed?

```splunk
`my_macro(field)`
```

- [ ] **A)** Inside parentheses immediately after the macro name
- [ ] **B)** Inside dollar signs around the macro name
- [ ] **C)** Outside backticks, before the macro
- [ ] **D)** After the pipe command

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Valid macro calls place arguments inside parentheses, and the entire expression is wrapped in backticks.
 
 
</details>


---

### **Tags and Event Types**

### 24. What symbol is required in SPL to invoke a macro?

- [ ] **A)** Backticks (` `)
- [ ] **B)** Parentheses ()
- [ ] **C)** Dollar signs ($)
- [ ] **D)** Square brackets []

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In SPL, macros are invoked with backticks around the macro name. Omitting them makes Splunk interpret the name as something other than a macro.
 
 
</details>

### 25. Which two statements correctly describe macro invocation in Splunk SPL?

- [ ] **A)** The macro name must be surrounded by backticks.
- [ ] **B)** Arguments must be placed inside the backticks with the macro name.
- [ ] **C)** Arguments are placed outside the closing backtick.
- [ ] **D)** A macro can be invoked by simply typing its name.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Macro invocation requires backticks, and argument values must be inserted inside those backticks, as in `macro(value)`. Placing arguments outside or omitting backticks causes incorrect parsing.
 
 
</details>

### 26. Review the SPL statement shown in the code block. What will Splunk do when this statement is used in a search?

```spl
`my_macro(error_code)`
```

- [ ] **A)** It invokes the macro and passes 'error_code' as an argument.
- [ ] **B)** It treats the macro name as a field and searches for 'error_code'.
- [ ] **C)** It returns a syntax error because arguments require square brackets.
- [ ] **D)** It invokes the macro without passing any argument.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block shows a macro invocation with an argument inside the backticks. Splunk substitutes the argument value into the macro before parsing the final search.
 
 
</details>


---

### **Visualizations (chart, timechart)**

### 27. What is the correct way to invoke a macro called my_macro in a Splunk search?

- [ ] **A)** `my_macro`
- [ ] **B)** my_macro
- [ ] **C)** 
- [ ] **D)** [my_macro]

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Macros are invoked with backticks around the macro name. Without backticks, Splunk interprets the text as a field or command, causing errors.
 
 
</details>


---

### **Workflow Actions**

### 28. Which symbol must surround a macro name when invoking it in a search?

- [ ] **A)** Backtick (`)
- [ ] **B)** Parentheses ( )
- [ ] **C)** Dollar signs ($)
- [ ] **D)** 

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Macros must be invoked with backticks around the macro name. Without backticks, Splunk treats the text as a command or field name.
 
 
</details>

### 29. Which statements accurately describe macros according to the documentation?

- [ ] **A)** Macros return a string of SPL
- [ ] **B)** Macros are invoked with backticks
- [ ] **C)** Macros validate argument data types
- [ ] **D)** Macros can store repeated OR conditions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Macros return SPL text, are invoked with backticks, and can hold complex repeated logic. They do not validate argument data types.
 
 
</details>

### 30. Review the macro invocation in the code block. What issue is present?

```splunk
`my_macro` (error_code)
```

- [ ] **A)** The argument is outside the backticks
- [ ] **B)** The argument is inside the parentheses
- [ ] **C)** Backticks are missing
- [ ] **D)** The invocation is valid

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The argument appears after the backticks. It must be inside the backticks and parentheses, like `my_macro(error_code)`.
 
 
</details>

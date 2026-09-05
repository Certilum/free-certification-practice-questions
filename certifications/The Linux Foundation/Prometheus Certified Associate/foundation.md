<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/The%20Linux%20Foundation/PCA%3A%20Prometheus%20Certified%20Associate" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Prometheus Certified Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Alerting and Dashboarding](#alerting-and-dashboarding) (5 questions)
- [Instrumentation and Exporters](#instrumentation-and-exporters) (4 questions)
- [Observability Concepts](#observability-concepts) (6 questions)
- [PromQL](#promql) (9 questions)
- [Prometheus Fundamentals](#prometheus-fundamentals) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:48:21.089Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Alerting and Dashboarding | 5 |
| Instrumentation and Exporters | 4 |
| Observability Concepts | 6 |
| PromQL | 9 |
| Prometheus Fundamentals | 6 |

---

### **Alerting and Dashboarding**

### 1. Which PromQL label matcher is the most efficient and commonly used for filtering by a known label value?

- [ ] **A)** Equality matcher (=)
- [ ] **B)** Inequality matcher (!=)
- [ ] **C)** Regex matcher (=~)
- [ ] **D)** Negative regex matcher (!~)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Equality matchers provide exact matching and are the most efficient and frequently used selectors in PromQL.
 
 
</details>

### 2. Which statements about PromQL regex matchers are true?

- [ ] **A)** PromQL regex matchers use RE2 syntax.
- [ ] **B)** The =~ matcher selects series whose label value matches the pattern.
- [ ] **C)** The !~ matcher excludes series whose label value matches the pattern.
- [ ] **D)** Regex matchers always have lower computational overhead than equality matchers.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> PromQL regex matchers use RE2 syntax, =~ selects matching series, and !~ excludes matching series. Regex matching has higher overhead than equality matching.
 
 
</details>

### 3. Examine the PromQL selector in the code block. Which type of label matcher is applied to the job label?

```promql
up{job=~"api.*"}
```

- [ ] **A)** Regex matcher (=~)
- [ ] **B)** Equality matcher (=)
- [ ] **C)** Inequality matcher (!=)
- [ ] **D)** Negative regex matcher (!~)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The selector uses =~, which is a regex matcher that follows RE2 syntax and selects labels matching the pattern api.*.
 
 
</details>

### 4. Which aggregation operator should you use to determine the number of active instances reporting a metric?

- [ ] **A)** sum()
- [ ] **B)** avg()
- [ ] **C)** count()
- [ ] **D)** max()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> count() returns the number of time series in the group, whereas sum() adds the values together.
 
 
</details>

### 5. Which of the following are valid PromQL label matching operators?

- [ ] **A)** =
- [ ] **B)** !=
- [ ] **C)** =~
- [ ] **D)** !~

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> PromQL supports equality, inequality, regex, and negative regex label matchers: =, !=, =~, and !~.
 
 
</details>


---

### **Instrumentation and Exporters**

### 6. Which PromQL label matcher uses exact matching and is the most efficient selector?

- [ ] **A)** =
- [ ] **B)** !=
- [ ] **C)** =~
- [ ] **D)** !~

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Equality matchers (=) compare labels for exact equality and are the most efficient and frequently used selectors in PromQL.
 
 
</details>

### 7. Which two statements about PromQL label matchers are correct?

- [ ] **A)** The =~ matcher supports RE2 regular expressions.
- [ ] **B)** The != matcher excludes series whose label value matches the given string.
- [ ] **C)** Label matching is case-insensitive.
- [ ] **D)** Shell globbing patterns such as * are valid in every PromQL matcher.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The =~ matcher uses RE2 regex syntax, and != excludes exact label values. PromQL label matching is case-sensitive and does not use shell globbing.
 
 
</details>

### 8. Review the PromQL selector shown in the code block. Given that all available series have a lower-case environment label value, what will the expression return?

```promql
http_requests_total{env="Prod"}
```

- [ ] **A)** No time series are matched.
- [ ] **B)** All time series are matched.
- [ ] **C)** The expression returns an error.
- [ ] **D)** The label value is converted to lower case automatically.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PromQL label matching is case-sensitive, so matching against a differently cased value returns no time series.
 
 
</details>

### 9. Which aggregation operator computes the arithmetic mean of the selected time series values?

- [ ] **A)** sum
- [ ] **B)** avg
- [ ] **C)** max
- [ ] **D)** count

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The avg aggregation operator calculates the arithmetic mean of the values in the resulting time series.
 
 
</details>


---

### **Observability Concepts**

### 10. What is the primary function of the equality matcher (=) in PromQL label selection?

- [ ] **A)** It requires an exact match between the label key and the provided string value.
- [ ] **B)** It performs a case-insensitive substring match.
- [ ] **C)** It matches any label value using RE2 regular expression syntax.
- [ ] **D)** It excludes time series whose label value equals the specified string.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The equality matcher (=) selects time series by requiring an exact match between the label key and the provided string value. It is the most efficient and frequently used selector.
 
 
</details>

### 11. Which of the following are valid label matching operators in PromQL?

- [ ] **A)** =
- [ ] **B)** !=
- [ ] **C)** =~
- [ ] **D)** ==

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> PromQL uses =, !=, =~, and !~ as label matching operators. In the options shown, =, !=, and =~ are valid; == is not a PromQL label matching operator.
 
 
</details>

### 12. Review the PromQL expression in the code block. What is the label selector component?

```promql
http_requests_total{job="api-server", env="production"}
```

- [ ] **A)** The portion inside curly braces, including the braces
- [ ] **B)** The metric name only
- [ ] **C)** The function wrapping the expression
- [ ] **D)** The time duration in brackets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In a PromQL vector selector, the label selector is the component inside curly braces {}. The metric name identifies the metric, and the braces contain the label filters.
 
 
</details>

### 13. Which PromQL operator is used to exclude time series that match a regular expression pattern?

- [ ] **A)** !~
- [ ] **B)** !=
- [ ] **C)** =~
- [ ] **D)** =

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The negative regex matcher (!~) excludes time series whose label value matches the provided RE2 regular expression pattern.
 
 
</details>

### 14. Which aggregation operators are specifically used to identify boundary values for threshold monitoring?

- [ ] **A)** min()
- [ ] **B)** max()
- [ ] **C)** sum()
- [ ] **D)** count()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Min and Max aggregations identify the lowest and highest values in a group of series, making them ideal for threshold monitoring such as detecting peak load or minimum available disk space.
 
 
</details>

### 15. According to the aggregation expression in the code block, which label will be preserved in the result?

```promql
sum(rate(http_requests_total[5m])) by (job)
```

- [ ] **A)** job
- [ ] **B)** instance
- [ ] **C)** No labels are preserved
- [ ] **D)** http_requests_total

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The by clause specifies which labels to preserve in the aggregation result. Because the expression uses by (job), only the job label is retained.
 
 
</details>


---

### **PromQL**

### 16. Which label matcher in PromQL requires an exact match between the label key and the provided string value?

- [ ] **A)** =
- [ ] **B)** !=
- [ ] **C)** =~
- [ ] **D)** !~

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The equality matcher (=) is the most efficient and frequently used selector for known label values. It requires an exact match between label key and string value.
 
 
</details>

### 17. Which statements correctly describe regex matcher behavior in PromQL?

- [ ] **A)** PromQL follows RE2 syntax for regular expressions.
- [ ] **B)** =~ includes time series that match the provided pattern.
- [ ] **C)** !~ excludes time series that match the provided pattern.
- [ ] **D)** Shell glob patterns are fully supported in PromQL regex matchers.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> PromQL uses RE2 syntax, not shell globbing. =~ selects matching series, and !~ excludes them. Using * instead of .* is a common trap.
 
 
</details>

### 18. In the PromQL expression shown, which type of matcher is applied to the job label to match multiple API services?

```promql
http_requests_total{job=~"api-.*", environment!="staging"}
```

- [ ] **A)** Equality matcher
- [ ] **B)** Inequality matcher
- [ ] **C)** Regex matcher
- [ ] **D)** Negative regex matcher

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The code uses =~, a regex matcher, to select jobs beginning with api-. It follows RE2 syntax and is efficient for grouping similar entities.
 
 
</details>

### 19. Which aggregation operator counts the time series in a group instead of adding their values?

- [ ] **A)** sum()
- [ ] **B)** count()
- [ ] **C)** avg()
- [ ] **D)** max()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> count() returns the number of time series in the group. Using sum() would add values, which is a common trap when counting active targets.
 
 
</details>

### 20. Which statements about by and without aggregation modifiers are correct?

- [ ] **A)** Aggregation without a by clause strips all labels from the result.
- [ ] **B)** by specifies which labels to preserve in the aggregated output.
- [ ] **C)** without preserves only the labels listed after it.
- [ ] **D)** If each selected series has value 1, sum() and count() return the same numeric result.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Without by, all labels are erased; by preserves specified labels; without removes listed labels. Summing ones equals counting series because sum adds values and count counts series.
 
 
</details>

### 21. In the displayed PromQL query, what does the by (job) modifier do?

```promql
sum(rate(http_requests_total[5m])) by (job)
```

- [ ] **A)** It removes the job label from the result.
- [ ] **B)** It preserves the job label in the aggregated result.
- [ ] **C)** It filters out every job except one.
- [ ] **D)** It converts the labels into a regular expression.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> by specifies which labels to preserve after aggregation. Using by (job) keeps the job label while other labels are stripped away.
 
 
</details>

### 22. Which PromQL function produces the average per-second rate from a counter over a range vector?

- [ ] **A)** rate()
- [ ] **B)** irate()
- [ ] **C)** increase()
- [ ] **D)** delta()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> rate() returns the average per-second increase over a range vector. irate() uses only the last two samples, while increase() reports total increase.
 
 
</details>

### 23. Which functions in PromQL are appropriate for analyzing counter metrics?

- [ ] **A)** rate()
- [ ] **B)** irate()
- [ ] **C)** increase()
- [ ] **D)** delta()

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> rate(), irate(), and increase() are designed for counter metrics. delta() is meant for gauges, and using it on counters is generally inappropriate.
 
 
</details>

### 24. In the code block, why would applying rate() to a gauge metric be incorrect?

```promql
sum(rate(node_cpu_seconds_total[5m])) by (instance)
```

- [ ] **A)** It produces invalid rates because rate() is designed for monotonically increasing counters.
- [ ] **B)** It returns exact raw values with no modification.
- [ ] **C)** It only fails if the gauge value is zero.
- [ ] **D)** It automatically converts the gauge to a counter.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> rate() mathematically expects a monotonically increasing counter. Applying it to a gauge can produce arbitrary or misleading values, a fundamental PromQL trap.
 
 
</details>


---

### **Prometheus Fundamentals**

### 25. Which PromQL label matcher requires an exact match between the label key and the provided string value?

- [ ] **A)** =~
- [ ] **B)** =
- [ ] **C)** !=
- [ ] **D)** !~

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The equality matcher (=) requires an exact match between the label key and the provided string value, making it the most efficient and frequent selector.
 
 
</details>

### 26. Which of which of these are valid PromQL label matching operators?

- [ ] **A)** =
- [ ] **B)** !=
- [ ] **C)** =~
- [ ] **D)** !~

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> PromQL supports four label matching operators: equality (=), inequality (!=), regex match (=~), and negative regex match (!~).
 
 
</details>

### 27. Review the selector in the code block. What is true about its matching behavior?

```promql
http_requests_total{env="Production"}
```

- [ ] **A)** It matches any environment whose label contains the provided text.
- [ ] **B)** It requires an exact, case-sensitive match on the environment label.
- [ ] **C)** It matches both lowercase and capitalized environment values.
- [ ] **D)** It treats the value as a regular expression pattern.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The equality matcher requires an exact match, and label matching in PromQL is case-sensitive, so only time series with the exact environment label value are returned.
 
 
</details>

### 28. Which aggregation operator should be used to calculate the total bandwidth consumed across all instances in a fleet?

- [ ] **A)** sum
- [ ] **B)** avg
- [ ] **C)** count
- [ ] **D)** max

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The sum aggregation operator adds all values from the selected time series, which is appropriate for calculating total resource consumption.
 
 
</details>

### 29. Which statements about PromQL aggregation modifiers are correct?

- [ ] **A)** The by clause specifies which labels to preserve.
- [ ] **B)** The without clause specifies which labels to remove from the result.
- [ ] **C)** An aggregation with no by or without clause strips all labels from the result.
- [ ] **D)** Using without on a label you want to keep will remove that dimension from the output.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> The by clause preserves specified labels, without removes specified labels, and omitting both strips all labels, which can accidentally remove desired dimensions.
 
 
</details>

### 30. What is the result of the expression shown in the code block?

```promql
sum(http_requests_total) by (job)
```

- [ ] **A)** The total number of HTTP requests grouped by job, preserving only the job label.
- [ ] **B)** The average number of HTTP requests per job.
- [ ] **C)** The maximum HTTP request count for each job.
- [ ] **D)** The count of time series for each job.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The sum aggregation adds request values, and the by (job) clause preserves only the job label in the resulting instant vector.
 
 
</details>

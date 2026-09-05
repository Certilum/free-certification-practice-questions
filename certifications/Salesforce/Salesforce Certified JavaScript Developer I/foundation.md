<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Salesforce/Salesforce%20Certified%20JavaScript%20Developer%20I.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Salesforce Certified JavaScript Developer I</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Asynchronous Programming](#asynchronous-programming) (4 questions)
- [Browsers and Events](#browsers-and-events) (5 questions)
- [Debugging and Error Handling](#debugging-and-error-handling) (2 questions)
- [Objects, Functions, and Classes](#objects-functions-and-classes) (7 questions)
- [Server-side JavaScript](#server-side-javascript) (3 questions)
- [Testing](#testing) (2 questions)
- [Variables, Types, and Collections](#variables-types-and-collections) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:47:24.853Z |
| Domains | 7 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Asynchronous Programming | 4 |
| Browsers and Events | 5 |
| Debugging and Error Handling | 2 |
| Objects, Functions, and Classes | 7 |
| Server-side JavaScript | 3 |
| Testing | 2 |
| Variables, Types, and Collections | 7 |

---

### **Asynchronous Programming**

### 1. What is the main purpose of using mocks or stubs in a unit test?

- [ ] **A)** They simulate external behaviors so the test validates only the target function's logic.
- [ ] **B)** They replace the assertion library so tests run faster.
- [ ] **C)** They guarantee that every line of code is covered.
- [ ] **D)** They help the runner discover test files faster.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Mocks or stubs isolate the unit under test by simulating external dependencies. This ensures the test only validates the specific logic of the target function, not the behavior of real integrations.
 
 
</details>

### 2. Which two statements correctly describe test assertions?

- [ ] **A)** Assertions compare the actual outcome of a function with the expected outcome.
- [ ] **B)** Assertions are optional when the test executes without errors.
- [ ] **C)** Without assertions, a test executes code but does not verify correctness.
- [ ] **D)** Assertions are used mainly to control the order of test execution.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Assertions validate whether the actual result matches the expected result. Running code without assertions may not fail, but it also does not prove that the code is correct.
 
 
</details>

### 3. In the code block provided, what is the role of the `.toBe(3)` expression?

```javascript
function add(a, b) {
  return a + b;
}

test('adds numbers correctly', () => {
  expect(add(1, 2)).toBe(3);
});
```

- [ ] **A)** A matcher that defines how the actual value is compared to the expected value.
- [ ] **B)** A lifecycle hook that runs before each test.
- [ ] **C)** A global object provided by the browser.
- [ ] **D)** A test-coverage reporter.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The `.toBe()` method is a matcher attached to `expect`. Matchers define the comparison logic used to decide whether the test passes or fails.
 
 
</details>

### 4. What does test coverage measure in a test suite?

- [ ] **A)** The percentage of the codebase that was executed during the test run.
- [ ] **B)** The number of assertions that passed.
- [ ] **C)** The number of external dependencies that were mocked.
- [ ] **D)** The total time required to run the test suite.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Coverage tracks which lines or code paths were executed during the tests. It shows what was touched, not whether those lines were verified correctly.
 
 
</details>


---

### **Browsers and Events**

### 5. When writing a JavaScript unit test, why is it essential to include a test assertion in the test case?

- [ ] **A)** To make the test execute faster
- [ ] **B)** To validate that the actual outcome matches the expected outcome
- [ ] **C)** To remove all external dependencies
- [ ] **D)** To generate a coverage report

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Assertions are the heart of a test; they verify that the result of the code equals the expected result. Without assertions, a test runs code without confirming correctness.
 
 
</details>

### 6. Which of the following statements correctly describe how mocks and stubs should be used to isolate a unit under test?

- [ ] **A)** They simulate external dependencies
- [ ] **B)** They help test only the target function's logic
- [ ] **C)** They replace the unit under test with a real service
- [ ] **D)** They prevent network or complex module calls

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Mocks and stubs simulate dependencies to isolate the code under test. They allow tests to validate only the target logic without making real network calls or invoking complex modules.
 
 
</details>

### 7. The code block below shows a simple test. Which step of the AAA pattern is missing from this test?

```javascript
function multiply(a, b) {
  return a * b;
}

test('multiplies numbers', () => {
  const a = 2;
  const b = 4;
  const product = multiply(a, b);
});
```

- [ ] **A)** Arrange step
- [ ] **B)** Act step
- [ ] **C)** Assert step
- [ ] **D)** Cleanup hook

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The test sets up values and then calls the function, but it never checks that the result is correct. The missing step is Assert.
 
 
</details>

### 8. If a unit test fails because a real network request returns an error, why is it considered an integration test rather than a unit test?

- [ ] **A)** A failed unit test
- [ ] **B)** A failed integration test
- [ ] **C)** A failed load test
- [ ] **D)** A failed static analysis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A true unit test isolates dependencies. If a real network call causes failure, the test is exercising external behavior, making it an integration test.
 
 
</details>

### 9. Which of the following are standard lifecycle hooks that a test runner can execute before and after tests?

- [ ] **A)** beforeEach
- [ ] **B)** beforeAll
- [ ] **C)** afterEach
- [ ] **D)** beforeTest

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Common lifecycle hooks include beforeEach, afterEach, beforeAll, and afterAll. beforeTest is not a standard test runner hook.
 
 
</details>


---

### **Debugging and Error Handling**

### 10. According to the playbook, what is the core principle that separates the unit under test from dependencies such as API calls or complex modules?

- [ ] **A)** Isolation and mocking
- [ ] **B)** Test orchestration
- [ ] **C)** Environment simulation
- [ ] **D)** Reporting and output

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Isolation and mocking is the core unit testing principle that separates the unit under test from its dependencies. Using mocks or stubs simulates external behavior so the test validates only the logic of the target function.
 
 
</details>

### 11. According to the playbook, which two scenarios are identified as common testing traps?

- [ ] **A)** Confusing `toBe` with `toEqual` for objects and arrays
- [ ] **B)** Using `toBe()` to check if an array contains an element instead of `toContain()`
- [ ] **C)** Using coverage metrics to identify untested code
- [ ] **D)** Using mocks to simulate external dependencies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The playbook warns against confusing `toBe` with `toEqual` for objects and arrays, and against using `toBe()` to check whether an array contains an element instead of `toContain()`. It also warns about forgetting to await async assertions and over-relying on coverage metrics, but using coverage to find untested code and using mocks as intended are not traps.
 
 
</details>


---

### **Objects, Functions, and Classes**

### 12. What is the primary purpose of using mocks or stubs in unit testing?

- [ ] **A)** To make the test run faster by skipping assertions
- [ ] **B)** To isolate the unit under test by simulating external dependencies
- [ ] **C)** To permanently replace the unit being tested with a fake version
- [ ] **D)** To automatically increase test line coverage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Mocks and stubs simulate external dependencies so the test validates only the logic of the unit under test without relying on real services.
 
 
</details>

### 13. Which statements about test coverage are true?

- [ ] **A)** High coverage guarantees the logic is correct.
- [ ] **B)** Coverage indicates which lines of code were executed during the test suite.
- [ ] **C)** Coverage can help identify code that has not been tested.
- [ ] **D)** 100% line coverage means the application has no bugs.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Coverage shows which lines were executed and can reveal untested code, but it does not prove logical correctness or absence of bugs.
 
 
</details>

### 14. In the test code shown, what is the purpose of the assertion line?

```javascript
function add(a, b) {
  return a + b;
}

test('add', () => {
  expect(add(1, 2)).toBe(3);
});
```

- [ ] **A)** It executes the function once.
- [ ] **B)** It validates that the actual result equals the expected result.
- [ ] **C)** It creates a mock for the add function.
- [ ] **D)** It groups the test into a suite.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The expect function receives the actual value from add(1,2), and toBe compares it to the expected value 3, confirming correctness.
 
 
</details>

### 15. In the Arrange, Act, Assert pattern, what does the 'Act' step do?

- [ ] **A)** Sets up the environment and test data
- [ ] **B)** Executes the function under test
- [ ] **C)** Verifies that the result matches the expectation
- [ ] **D)** Cleans up after the test finishes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Arrange sets up state, Act executes the function being tested, and Assert verifies that the outcome matches the expected result.
 
 
</details>

### 16. Which of the following are common traps to avoid when writing unit tests?

- [ ] **A)** Using a real API service in a unit test and blaming network errors for failures
- [ ] **B)** Testing only happy path scenarios
- [ ] **C)** Ignoring edge cases like null and undefined inputs
- [ ] **D)** Running the test suite with 100% line coverage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Unit tests should isolate dependencies, cover edge cases, and not rely only on happy paths. High coverage alone is not a trap.
 
 
</details>

### 17. What is the purpose of the lifecycle hook shown in the code block?

```javascript
describe('suite', () => {
  beforeEach(() => {
    localStorage.clear();
  });

  it('test1', () => {
    // test code
  });

  it('test2', () => {
    // test code
  });
});
```

- [ ] **A)** It runs before each test, giving the tests a clean state.
- [ ] **B)** It replaces the assertion library for the suite.
- [ ] **C)** It generates the coverage report for the test run.
- [ ] **D)** It mocks every network request in the tests.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Lifecycle hooks like beforeEach run before every test, allowing developers to reset state and prevent side effects between tests.
 
 
</details>

### 18. What does the reporting and output feature of a test runner do?

- [ ] **A)** Transforms raw execution data into human-readable or machine-readable formats
- [ ] **B)** Provides global objects like window and document
- [ ] **C)** Runs test files in random order
- [ ] **D)** Resets the database before each test

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Reporting and output convert raw test results into CLI summaries, JUnit XML, or coverage reports for developers and CI systems.
 
 
</details>


---

### **Server-side JavaScript**

### 19. What is the primary role of a test assertion in a unit test?

- [ ] **A)** Discover test files automatically before execution.
- [ ] **B)** Validate that the actual result matches the expected result.
- [ ] **C)** Simulate dependencies such as network calls.
- [ ] **D)** Group related tests into a logical suite.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Assertions are the core validation mechanism of a test. They compare the actual outcome with the expected outcome; without them a test only executes code without proving correctness.
 
 
</details>

### 20. Which of the following are common traps to avoid when writing JavaScript unit tests? (Select all that apply.)

- [ ] **A)** Including a real service dependency in a unit test and blaming a network failure on the unit test.
- [ ] **B)** Only testing happy-path scenarios and ignoring null or thrown-error inputs.
- [ ] **C)** Treating 100% line coverage as proof that the logic is correct.
- [ ] **D)** Using beforeEach to reset mocks before each test.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> All of the first three are warned against in the playbook: real dependencies can turn a unit test into an integration test, ignoring edge cases hides bugs, and coverage does not prove logical correctness. Resetting mocks in beforeEach is a recommended practice, not a trap.
 
 
</details>

### 21. Inspect the test snippet in the code block. Why does the test fail even though the object literals appear identical?

```javascript
test('object equality', () => {
  expect({ foo: 'bar' }).toBe({ foo: 'bar' });
});
```

- [ ] **A)** The test should use a mock to simulate the object.
- [ ] **B)** .toBe() checks referential equality, and each object literal has a different memory reference.
- [ ] **C)** The assertion needs to be awaited with await expect(...).resolves.
- [ ] **D)** .toBe() should be replaced with .toContain() for this comparison.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> .toBe() performs referential equality in JavaScript. Each { foo: 'bar' } literal creates a new object in a different memory location, so the assertion fails. Use .toEqual() for deep structural equality.
 
 
</details>


---

### **Testing**

### 22. What does the `toBe` matcher verify when comparing two values in a typical JavaScript test?

- [ ] **A)** Referential equality between two values
- [ ] **B)** Deep structural equality between objects
- [ ] **C)** Whether an array includes an element
- [ ] **D)** Whether a function throws an error

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> `toBe` uses referential equality, so two variables must point to the same object in memory. Use `toEqual` when comparing object structures.
 
 
</details>

### 23. According to the playbook, which of the following are common testing traps that developers should avoid when writing JavaScript tests?

- [ ] **A)** Using `toBe` with objects instead of `toEqual`
- [ ] **B)** Forgetting to `await` asynchronous assertions
- [ ] **C)** Assuming 100% coverage proves correctness
- [ ] **D)** Using `toContain` to check array membership

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The correct choices are common traps: confusing `toBe` with `toEqual`, failing to `await` async assertions, and trusting coverage as proof of correctness. Using `toContain` for arrays is a correct practice.
 
 
</details>


---

### **Variables, Types, and Collections**

### 24. What is the primary purpose of assertions in a unit test?

- [ ] **A)** To validate that the actual output matches the expected output
- [ ] **B)** To execute the function under test
- [ ] **C)** To simulate external dependencies
- [ ] **D)** To organize test cases into suites

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Assertions compare actual outcomes to expected outcomes; without them, a test runs but does not verify correctness.
 
 
</details>

### 25. Which dependencies should typically be mocked or stubbed when writing a unit test? Select all that apply.

- [ ] **A)** An external API call
- [ ] **B)** A complex internal module that is not the target
- [ ] **C)** The function being tested itself
- [ ] **D)** A simple pure arithmetic helper

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Mocks simulate external behaviors and isolate the unit from real dependencies. The target function and simple pure helpers do not need mocking.
 
 
</details>

### 26. Review the code block. Which matcher should replace the blank to assert that two variables refer to the same object?

```javascript
const first = { id: 1 };
const second = first;
expect(second).___(first);
```

- [ ] **A)** toBe
- [ ] **B)** toEqual
- [ ] **C)** toContain
- [ ] **D)** toThrow

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> toBe checks referential equality and passes when variables point to the same memory address. toEqual would check deep structure, not identity.
 
 
</details>

### 27. What does test coverage measure in a JavaScript project?

- [ ] **A)** The percentage of codebase lines executed during tests
- [ ] **B)** The number of test assertions that pass
- [ ] **C)** The logical correctness of the test suite
- [ ] **D)** The speed at which tests run

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Coverage shows which lines were touched during test runs. It is not a guarantee of correctness.
 
 
</details>

### 28. Which of the following are lifecycle hooks provided by test runners? Select all that apply.

- [ ] **A)** beforeEach
- [ ] **B)** afterEach
- [ ] **C)** beforeAll
- [ ] **D)** setup

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Jest-style runners provide beforeEach, afterEach, beforeAll, and afterAll. setup is not one of the lifecycle hooks described.
 
 
</details>

### 29. Consider the asynchronous test in the code block. Why might the test incorrectly pass even when the Promise rejects?

```javascript
it('returns data', async () => {
  expect(fetchData()).resolves.toBe('data');
});
```

- [ ] **A)** The test is missing an await before expect
- [ ] **B)** The matcher toBe is wrong for promises
- [ ] **C)** The test lacks an assertion library
- [ ] **D)** The runner executes tests in the wrong order

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Async assertions must be awaited. Without await, the test completes before the Promise is evaluated, allowing a rejected promise to go unnoticed.
 
 
</details>

### 30. What is a test suite?

- [ ] **A)** A collection of related test cases
- [ ] **B)** A single unit test scenario
- [ ] **C)** A simulated browser environment
- [ ] **D)** A coverage report generated after tests run

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A test case is one scenario; a test suite is a structured collection of related test cases.
 
 
</details>

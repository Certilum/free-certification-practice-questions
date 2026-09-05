<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Java%20SE%2021%20Developer.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Java SE 21 Developer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Arrays and Collections](#arrays-and-collections) (3 questions)
- [Concurrency](#concurrency) (5 questions)
- [Controlling Program Flow](#controlling-program-flow) (1 questions)
- [Handling Date, Time, Text, Numeric and Boolean Values](#handling-date-time-text-numeric-and-boolean-values) (2 questions)
- [Handling Exceptions](#handling-exceptions) (2 questions)
- [I/O and NIO.2](#i-o-and-nio-2) (2 questions)
- [Localization](#localization) (1 questions)
- [Modules and Deployment](#modules-and-deployment) (2 questions)
- [Object-Oriented Concepts](#object-oriented-concepts) (7 questions)
- [Streams and Lambda Expressions](#streams-and-lambda-expressions) (4 questions)
- [Supplementary Topics](#supplementary-topics) (1 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:50.082Z |
| Domains | 11 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Arrays and Collections | 3 |
| Concurrency | 5 |
| Controlling Program Flow | 1 |
| Handling Date, Time, Text, Numeric and Boolean Values | 2 |
| Handling Exceptions | 2 |
| I/O and NIO.2 | 2 |
| Localization | 1 |
| Modules and Deployment | 2 |
| Object-Oriented Concepts | 7 |
| Streams and Lambda Expressions | 4 |
| Supplementary Topics | 1 |

---

### **Arrays and Collections**

### 1. What must be called on a Thread object to begin separate concurrent execution?

- [ ] **A)** Call the run() method directly.
- [ ] **B)** Call the start() method once.
- [ ] **C)** Create the Thread subclass.
- [ ] **D)** Override the toString() method.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Calling start() makes the JVM schedule a new thread; run() is invoked inside that new thread. Calling run() directly does not launch concurrency.
 
 
</details>

### 2. Which statements are true about calling run() versus start() on a Thread object? Select all that apply.

- [ ] **A)** A direct run() call executes the thread body in the current thread.
- [ ] **B)** A direct start() call creates a new execution context and runs the task asynchronously.
- [ ] **C)** Calling start() more than once on the same Thread object is valid.
- [ ] **D)** A direct run() call always starts a new daemon thread.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> run() is synchronous when invoked directly; start() schedules a new thread. A Thread cannot be restarted, so a second start() throws IllegalThreadStateException.
 
 
</details>

### 3. The code block submits a Callable that throws an exception, then calls Future.get() inside a try-catch. What is the class name printed by the code?

```java
import java.util.concurrent.*;

public class FutureDemo {
    public static void main(String[] args) throws Exception {
        ExecutorService executor = Executors.newSingleThreadExecutor();
        Callable<String> task = () -> { throw new IllegalStateException("boom"); };
        Future<String> future = executor.submit(task);
        executor.shutdown();

        try {
            future.get();
        } catch (Exception e) {
            System.out.println(e.getClass().getName());
        }
    }
}
```

- [ ] **A)** java.lang.IllegalStateException
- [ ] **B)** java.util.concurrent.ExecutionException
- [ ] **C)** java.lang.RuntimeException
- [ ] **D)** java.lang.Exception

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> submit() stores task failure in the Future. Future.get() surfaces the failure as ExecutionException, with IllegalStateException as its cause.
 
 
</details>


---

### **Concurrency**

### 4. In Java, what is the result of creating a Thread object without calling start()?

- [ ] **A)** It represents the thread, but execution is not started.
- [ ] **B)** It immediately invokes the run() method.
- [ ] **C)** It allocates a new running thread.
- [ ] **D)** It throws an exception until start() is called.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Thread object is a handle to the execution state. The actual task runs only after start() is called.
 
 
</details>

### 5. Which two statements are true when calling a Thread's run() method directly instead of using start()?

- [ ] **A)** It executes run() in the current thread.
- [ ] **B)** It does not create a new thread of execution.
- [ ] **C)** It starts a new daemon thread.
- [ ] **D)** It can be called only once after start().

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Directly calling run() invokes its body synchronously in the caller's thread and does not start a separate thread.
 
 
</details>

### 6. Refer to the code block. What is the behavior of the operation that retrieves the Future's result?

```java
import java.util.concurrent.*;

public class Sample {
    public static int retrieveValue() throws Exception {
        ExecutorService service = Executors.newSingleThreadExecutor();
        try {
            Future<Integer> future = service.submit(() -> 42);
            return future.get();
        } finally {
            service.shutdown();
        }
    }
}
```

- [ ] **A)** It blocks until the result is available and then returns it.
- [ ] **B)** It returns a default value if the result is not ready.
- [ ] **C)** It throws an exception only if the task was cancelled.
- [ ] **D)** It polls the task once and returns immediately.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Future.get() is blocking: it waits until the task completes and then returns the result or throws an execution-related exception.
 
 
</details>

### 7. Why can extending Thread make it harder to reuse a task class?

- [ ] **A)** A Java class can extend only one superclass.
- [ ] **B)** Thread methods cannot be overridden.
- [ ] **C)** Extending Thread prevents execution on a virtual thread.
- [ ] **D)** Thread must be subclassed inside its own file.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Java allows only one superclass, so extending Thread prevents the task class from extending another useful class.
 
 
</details>

### 8. Which two statements correctly compare the execute() and submit() methods of ExecutorService?

- [ ] **A)** execute() returns void, while submit() returns a Future.
- [ ] **B)** Both execute() and submit() can capture the exception in a Future.
- [ ] **C)** An exception from execute() cannot be read through Future.get().
- [ ] **D)** submit() rethrows task exceptions immediately on the caller's thread.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> execute() has no Future, so async exceptions are not captured for later retrieval; submit() returns a Future that can hold the exception.
 
 
</details>


---

### **Controlling Program Flow**

### 9. What happens when you instantiate a Thread object in Java?

- [ ] **A)** Immediately executes run() on the current thread.
- [ ] **B)** Starts the new execution flow immediately.
- [ ] **C)** Creates Thread instance; execution flow starts on start().
- [ ] **D)** Blocks until another thread calls notify().

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Creating a Thread object does not start a new execution; the new flow begins only when start() is called. Calling run() directly executes synchronously, so a Thread object is not the same as running code.
 
 
</details>


---

### **Handling Date, Time, Text, Numeric and Boolean Values**

### 10. Which statement correctly describes the relationship between a Thread object and the actual execution it may perform?

- [ ] **A)** Calling start() schedules separate execution.
- [ ] **B)** Constructing a Thread starts it automatically.
- [ ] **C)** Calling run() creates a new thread.
- [ ] **D)** Constructing a Thread invokes run() immediately.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Creating a Thread only creates an object; start() schedules the separate execution, while run() alone runs in the current thread.
 
 
</details>

### 11. Which statements about ExecutorService methods and Future behavior are true? Choose all that apply.

- [ ] **A)** submit() returns a Future.
- [ ] **B)** execute() returns a Future.
- [ ] **C)** Future.get() may block waiting for the result.
- [ ] **D)** Future.get() is always non-blocking.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> submit() returns a Future that can represent the task result, while execute() returns void. Calling get() can block until the computation completes.
 
 
</details>


---

### **Handling Exceptions**

### 12. Which statement accurately describes the relationship between a Thread object and the execution of its run() method?

- [ ] **A)** Creating a Thread object immediately begins execution of that thread.
- [ ] **B)** Calling start() creates a new execution path that calls run() asynchronously.
- [ ] **C)** The run() method, when called directly, executes in a new thread.
- [ ] **D)** The Thread object itself is the actual operating-system thread.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A Thread object is only a handle. Without start(), no separate thread is created. The start() method asynchronously schedules run() to execute in a new thread, while calling run() directly is just an ordinary method call in the current thread.
 
 
</details>

### 13. A developer submits tasks to an ExecutorService. Which two statements are true about exception handling with execute() and submit()?

- [ ] **A)** If a task submitted with submit() throws an exception, the underlying cause is exposed when get() is called on the returned Future.
- [ ] **B)** Tasks submitted with execute() do not return a Future, so their exceptions are not surfaced to the caller through Future.get().
- [ ] **C)** Checked exceptions from tasks submitted with submit() are wrapped in RuntimeException before being returned by get().
- [ ] **D)** Both execute() and submit() store any thrown exception until the thread that submitted the task calls get().

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> submit() returns a Future that stores the failure; get() throws an ExecutionException whose cause is the original exception. execute() returns void, so no Future exists, and task exceptions propagate to the worker thread instead of being delivered through Future.get().
 
 
</details>


---

### **I/O and NIO.2**

### 14. Which statement correctly describes the behavior of Future.get() when it is called before a submitted task has finished?

- [ ] **A)** Future.get() is non-blocking.
- [ ] **B)** Future.get() blocks until completion.
- [ ] **C)** Future.get() cancels unfinished tasks.
- [ ] **D)** Future.get() returns null when idle.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Future.get() is a blocking call. It waits until the task completes before returning the result, and it can throw ExecutionException if the task failed.
 
 
</details>

### 15. According to the playbook, which two statements are correct about exception handling in ExecutorService execute() and submit()?

- [ ] **A)** execute() cannot return a Future.
- [ ] **B)** submit() returns a Future.
- [ ] **C)** execute() always hides task exceptions.
- [ ] **D)** submit() ignores task exceptions.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> execute() returns void and cannot store a failure; submit() returns a Future, so Future.get throws ExecutionException for failed tasks.
 
 
</details>


---

### **Localization**

### 16. Which statement correctly describes creating a Thread object relative to the underlying system thread or asynchronous execution?

- [ ] **A)** Starts a new execution automatically
- [ ] **B)** Execution begins only after start() is called
- [ ] **C)** Calling run() invokes it in a new thread
- [ ] **D)** Thread object and actual execution are identical

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Creating a Thread object only creates an instance. Execution begins only when start() is invoked, while calling run() directly runs synchronously and does not start a new thread.
 
 
</details>


---

### **Modules and Deployment**

### 17. In Java concurrency, what is the effect of merely creating an instance of the Thread class?

- [ ] **A)** The JVM allocates a new operating-system thread and begins executing the associated task.
- [ ] **B)** A Thread object exists, but no execution begins until start() is called.
- [ ] **C)** The run() method is automatically invoked in the current thread.
- [ ] **D)** The thread immediately enters the TIMED_WAITING state.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Creating a Thread object only creates an instance; no execution begins until start() is invoked. Calling run() would execute synchronously in the calling thread, which is a common trap.
 
 
</details>

### 18. Which two statements are true about invoking run() directly on a Thread object instead of calling start()?

- [ ] **A)** The code inside run() executes on the current calling thread.
- [ ] **B)** The code inside run() executes synchronously, not on a new thread.
- [ ] **C)** A new thread is started and run() executes on that new thread.
- [ ] **D)** The thread automatically changes from NEW to TIMED_WAITING.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Directly calling run() executes it as an ordinary method in the current thread. To launch a new thread of execution, start() must be used instead.
 
 
</details>


---

### **Object-Oriented Concepts**

### 19. What happens when a Thread object is created?

- [ ] **A)** It only creates a Thread instance.
- [ ] **B)** It immediately starts a new thread.
- [ ] **C)** It automatically calls run() in parallel.
- [ ] **D)** It schedules the task on the main thread.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Creating a Thread object only creates an instance. The start() method must be called to create and run a new execution thread.
 
 
</details>

### 20. Which statements about Thread.run() are true? Select all that apply.

- [ ] **A)** Direct run() calls execute synchronously.
- [ ] **B)** Always call run() to launch a thread.
- [ ] **C)** run() can be overridden in a subclass.
- [ ] **D)** start() causes run() to run on another thread.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Calling run() directly executes it in the caller's thread. The start() method creates the new call stack and then invokes run() on the new thread.
 
 
</details>

### 21. Given the code block, what output is printed to the console?

```java
public class RunDemo {
    public static void main(String[] args) {
        Thread t = new Thread(() -> System.out.print("task "));
        t.run();
        System.out.print("main");
    }
}
```

- [ ] **A)** task main
- [ ] **B)** main task
- [ ] **C)** task task main
- [ ] **D)** No output

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code calls t.run() directly, so the Runnable executes synchronously in the main thread. Therefore, task prints before main.
 
 
</details>

### 22. Which statement about Future.get() is correct?

- [ ] **A)** It blocks until a result is available.
- [ ] **B)** It returns immediately with the task result.
- [ ] **C)** It never blocks the calling thread.
- [ ] **D)** It returns a null Future if the task succeeds.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Future.get() is not a non-blocking poll. It blocks the calling thread until the asynchronous task completes and the result is available.
 
 
</details>

### 23. Which statements about execute() and submit() are true? Select all that apply.

- [ ] **A)** submit() accepts Callable and returns Future.
- [ ] **B)** Future.get() exposes failures from submitted tasks.
- [ ] **C)** Task exceptions from execute() reach the uncaught handler.
- [ ] **D)** execute() returns a Future like submit().

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Unlike execute(), submit() accepts Callable and returns Future. Failures from submitted tasks are visible through Future.get(). Direct execute() routes exceptions to an uncaught handler.
 
 
</details>

### 24. Review the code block. Which statements are correct? Select all that apply.

```java
ExecutorService service = Executors.newFixedThreadPool(1);
try {
    Future<String> future = service.submit(() -> "ready");
    System.out.println(future.get());
} finally {
    service.shutdown();
}
```

- [ ] **A)** The text ready is printed before shutdown is called.
- [ ] **B)** get() blocks until the task is complete.
- [ ] **C)** submit() returns a Future for the task.
- [ ] **D)** newFixedThreadPool creates virtual thread tasks.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> submit() returns a Future, and get() blocks until the task finishes. After the value is printed, the finally block calls shutdown().
 
 
</details>

### 25. Which practice is essential when using an explicit Lock object?

- [ ] **A)** Call unlock() in a finally block.
- [ ] **B)** Use synchronized blocks with every explicit lock.
- [ ] **C)** Let the JVM release the Lock automatically.
- [ ] **D)** Release the Lock only at program shutdown.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An explicit Lock has no automatic release. Placing unlock() in a finally block guarantees that the lock is released even if an exception occurs.
 
 
</details>


---

### **Streams and Lambda Expressions**

### 26. When a Thread object is created, which invocation starts the separate execution of its task?

- [ ] **A)** Call start().
- [ ] **B)** Call run().
- [ ] **C)** Call join().
- [ ] **D)** Call yield().

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A new Thread object is not running. The start() method creates the new call stack and then invokes run() on that stack; calling run() directly executes it in the caller's thread.
 
 
</details>

### 27. While working with an ExecutorService, which statements correctly contrast execute() and submit() regarding return values and exceptions?

- [ ] **A)** submit() returns a Future.
- [ ] **B)** execute() returns a Future.
- [ ] **C)** execute() accepts Runnable only.
- [ ] **D)** submit() accepts Callable tasks.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> submit() accepts both Runnable and Callable and returns a Future for cancellation and result retrieval. execute() accepts Runnable, returns void, and does not expose a Future for that task.
 
 
</details>

### 28. The source shows a CompletableFuture chain. What static type is inferred for the result variable?

```java
var future = CompletableFuture.supplyAsync(() -> "data");
var result = future.thenAccept(System.out::println);
```

- [ ] **A)** Void
- [ ] **B)** Future<Void>
- [ ] **C)** CompletableFuture<String>
- [ ] **D)** CompletableFuture<Void>

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> thenAccept() takes a Consumer and returns CompletableFuture<Void>; it does not transform the value. Only a stage such as thenApply() would return CompletableFuture<String>.
 
 
</details>

### 29. Which Java inheritance rule prevents a class from extending both Thread and another parent class?

- [ ] **A)** It cannot extend another class.
- [ ] **B)** It cannot override run().
- [ ] **C)** It cannot be declared final.
- [ ] **D)** It cannot implement an interface.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Java supports single inheritance for classes. Once a class extends Thread, it cannot extend another class, although it may implement multiple interfaces and override run().
 
 
</details>


---

### **Supplementary Topics**

### 30. Which statement correctly describes how exception handling differs between execute(Runnable) and submit(Callable<T>) tasks?

- [ ] **A)** execute() returns a Future, but submit() does not return any handle to the task.
- [ ] **B)** Exceptions from execute() are not available to the caller; submit() captures failures in its returned Future.
- [ ] **C)** Both execute() and submit() throw ExecutionException synchronously at the call site.
- [ ] **D)** Both methods require InterruptedException to be handled at the call site.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> execute() is void, so task exceptions are not returned to the caller. submit() returns a Future, and the exception is revealed when Future.get() throws ExecutionException.
 
 
</details>

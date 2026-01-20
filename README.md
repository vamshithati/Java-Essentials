# 📚Java-Essentials

---

# ☕ Introduction to Java

## What is Java?
Java is a **high-level, object-oriented, platform-independent programming language** widely used for building enterprise applications, web services, mobile apps, and cloud-based systems.

Originally developed by **Sun Microsystems**, Java is now maintained by **Oracle**.

---

## Why Java is Popular?
Java has remained one of the most popular programming languages for decades because of:

- **Platform Independence** – Write Once, Run Anywhere
- **Object-Oriented Design**
- Strong community and ecosystem
- High performance with JVM optimizations
- Secure, robust, and scalable

---

## Where is Java Used?
Java powers many real-world applications such as:

- 🌐 Backend Web Applications
- ☁️ Cloud & Microservices
- 📱 Android Development
- 🏦 Banking & Financial Systems
- 🛒 E-commerce Platforms
- 📊 Big Data Technologies

---

## Key Features of Java
- Simple and easy to learn
- Object-Oriented
- Platform Independent
- Secure
- Multithreaded
- Robust and scalable

---

## How Java Works (High Level)
1. Java source code is written in `.java` files
2. Java Compiler converts it into **bytecode**
3. Bytecode runs on the **Java Virtual Machine (JVM)**
4. JVM enables Java programs to run on any operating system

---

## Java Editions
- **Java SE** – Core Java concepts
- **Java EE / Jakarta EE** – Enterprise applications
- **Java ME** – Embedded systems

---
## Who Should Learn Java?
This tutorial is ideal for:
- Beginners learning Java from scratch
- Students and fresh graduates
- Software Engineers preparing for interviews
- Backend and Full-Stack developers

---

## Prerequisites
- Basic computer knowledge
- No prior programming experience required

---

# 📚 Java Essentials – Learning Roadmap






## 🟢 Beginner Level

<details>
<summary>1.Java Installation & Environment Setup</summary>


### 📦 Java Development Kit (JDK) Overview

The **Java Development Kit (JDK)** is required to **develop, compile, and run Java applications**.

It includes:
- **Java Compiler (`javac`)** – converts source code into bytecode
- **Java Runtime (`java`)** – executes compiled bytecode
- **Core Java libraries** – standard APIs
- **Development tools** – debugging and monitoring utilities

Without the JDK, Java source code **cannot be compiled or executed**.



### ⚖️ OpenJDK vs Oracle JDK

**OpenJDK**
- Open-source and free
- Community-supported
- Widely used in development and production
- **Recommended choice**

**Oracle JDK**
- Commercial license
- Subscription required for long-term support
- Used mainly in enterprise environments

---

### 💻 Installation on Windows and macOS

**Windows**
1. Download the JDK `.exe` installer
2. Run the installer and follow setup instructions
3. Default installation directory:
```text
C:\Program Files\Java\
```
**MacOS**
1.Download the `.dmg` or `.pkg` installer
2.Follow installation steps
3.Installed under:
```text
/Library/Java/JavaVirtualMachines
```

### ⚙️ Environment Variables (JAVA_HOME & PATH)
Environment variables allow the operating system to locate Java tools globally.

`JAVA_HOME` → Path to the JDK installation directory

`PATH` → Enables running Java commands from any directory

Example (Linux/macOS)
```bash
export JAVA_HOME=/usr/lib/jvm/java-17-openjdk
export PATH=$JAVA_HOME/bin:$PATH
```
### ✅ Installation Verification
Verify the Java installation using the following commands:

```bash
java -version
javac -version
```
Expected output:
```text
openjdk version "17"
javac 17
```
### ⚠️ Common Setup Issues
java command not found → PATH is not configured correctly

Incorrect Java version → Multiple JDKs installed

Permission issues → Insufficient installation rights

---
</details>




<details>
<summary>2. First Java Program – Hello World</summary>
  
### 🧱 Java Program Structure 
A Java program is built using **classes and methods**. 
Every Java application must contain **at least one class**, and execution always begins from the main method. 
#### Basic structure of a Java program:
```java
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

### 🧩 class and main Method

**Class**

- A class is the basic building block of a Java program

- It acts as a blueprint for objects

- The class name must match the file name

**Example:**
```text
HelloWorld.java
```

**main** Method

- Entry point of every Java program

- Program execution starts from this method

- Required syntax:

```java 
public static void main(String[] args)
```

### 🔄 Compilation and Execution Flow

**1.Write the source code**

-Save the file as:
```text
HelloWorld.java
```

**2.Compile the program**

- Converts source code into bytecode
```bash
javac HelloWorld.java
```

**3.Execute the program**

- Runs the compiled bytecode using JVM
```bash
java HelloWorld
```
### 🖥️ Console Output

The output is printed using:
```java
System.out.println("Hello, World!");
```

Output on the console:
```java
Hello, World!
```
### 📌 Key Points
- Java programs start execution from the ```main``` method

- File name and class name must be the same

- Compilation and execution are two separate steps

-```System.out.println()``` displays output on the console

---
  
</details>


<details>
<summary>3. Variables & Data Types</summary>

### 📦 Variables in Java

A **variable** is a container used to store data values.  
Each variable in Java must be declared with a **data type** before it can be used.

Example:
```java
int number = 10;
```
### 🔢 Primitive Data Types

Primitive data types store **simple values directly in memory**.

| Data Type | Size    | Example |
|----------|---------|---------|
| `int`    | 4 bytes | `int a = 10;` |
| `float`  | 4 bytes | `float b = 5.5f;` |
| `double` | 8 bytes | `double d = 99.99;` |
| `char`   | 2 bytes | `char c = 'A';` |
| `boolean`| 1 bit   | `boolean flag = true;` |
| `byte`   | 1 byte  | `byte x = 100;` |
| `short`  | 2 bytes | `short s = 200;` |
| `long`   | 8 bytes | `long l = 100000L;` |

### 🧩 Non-Primitive Data Types

Non-primitive data types store **references to objects** rather than actual values.

#### Examples include:
- `String`
- Arrays
- Classes
- Interfaces

#### Example:

```java
String name = "Java";
int[] numbers = {1, 2, 3};
```
### ✍️ Variable Declaration and Initialization

#### Declaration

```java
int x;
```
#### Initialization
```java
x = 5;
```
#### Declaration + Initialization
```java
int y = 10;
```

### 🔁 Type Casting

Type casting is used to convert one data type into another.

#### Implicit Casting (Widening)
- Automatic conversion
- Smaller type → larger type

```java
int a = 10;
double b = a;
```
#### Explicit Casting (Narrowing)
- Manual conversion

- Larger type → smaller type

```java

double x = 10.5;
int y = (int) x;
```

### 📌 Key Points

- Variables must be declared before use
- Java is a **strongly typed language**
- Primitive types store values directly
- Non-primitive types store object references
- Casting allows type conversion between compatible data types

---
</details>

<details>
<summary>4.Operators</summary>

Operators are symbols used to perform operations on variables and values.
---

### ➕ Arithmetic Operators

Arithmetic operators are used to perform mathematical operations.

| Operator | Description | Example |
|--------|------------|---------|
| `+` | Addition | `a + b` |
| `-` | Subtraction | `a - b` |
| `*` | Multiplication | `a * b` |
| `/` | Division | `a / b` |
| `%` | Modulus | `a % b` |

---

### 🔍 Relational Operators

Relational operators are used to compare two values and return a boolean result.

| Operator | Description | Example |
|--------|------------|---------|
| `==` | Equal to | `a == b` |
| `!=` | Not equal to | `a != b` |
| `>` | Greater than | `a > b` |
| `<` | Less than | `a < b` |
| `>=` | Greater than or equal to | `a >= b` |
| `<=` | Less than or equal to | `a <= b` |

---

### 🔗 Logical Operators

Logical operators are used to combine boolean expressions.

| Operator | Description | Example |
|--------|------------|---------|
| `&&` | Logical AND | `a > 0 && b > 0` |
| `||` | Logical OR | `a > 0 || b > 0` |
| `!` | Logical NOT | `!flag` |

---

### 📝 Assignment Operators

Assignment operators are used to assign values to variables.

| Operator | Description | Example |
|--------|------------|---------|
| `=` | Assign | `a = 10` |
| `+=` | Add and assign | `a += 5` |
| `-=` | Subtract and assign | `a -= 5` |
| `*=` | Multiply and assign | `a *= 2` |
| `/=` | Divide and assign | `a /= 2` |
| `%=` | Modulus and assign | `a %= 2` |

---

### 🔄 Unary and Ternary Operators

#### Unary Operators
Operate on a single operand.

| Operator | Description | Example |
|--------|------------|---------|
| `+` | Unary plus | `+a` |
| `-` | Unary minus | `-a` |
| `++` | Increment | `a++` |
| `--` | Decrement | `a--` |
| `!` | Logical NOT | `!flag` |

#### Ternary Operator
A shorthand for `if-else` condition.

Syntax:
```java
condition ? expression1 : expression2;
```
Example:
```java
int max = (a > b) ? a : b;
```
---
</details>

<details>
<summary>5.Control Statements</summary>

Control statements are used to **control the flow of execution** of a program based on conditions.

---

### 🔀 `if` and `if-else` Statements

The `if` statement executes a block of code when a condition is true.

**Syntax (`if`)**
```java
if (condition) {
    // code to execute
}
```

**Syntax (if-else)**
```java
if (condition) {
    // code if condition is true
} else {
    // code if condition is false
}
```


**Example**
```java
int age = 18;

if (age >= 18) {
    System.out.println("Eligible to vote");
} else {
    System.out.println("Not eligible to vote");
}
```
### 🔁 switch Statement

The switch statement allows multiple conditions to be tested using a single variable.

#### Syntax
```java
switch (expression) {
    case value1:
        // code
        break;
    case value2:
        // code
        break;
    default:
        // default code
}
```

#### Example
```java

int day = 3;

switch (day) {
    case 1:
        System.out.println("Monday");
        break;
    case 2:
        System.out.println("Tuesday");
        break;
    case 3:
        System.out.println("Wednesday");
        break;
    default:
        System.out.println("Invalid day");
}
```

### 🔄 Decision-Making Flow

- Conditions are evaluated from top to bottom

- Based on the condition result (`true` or `false`), specific code blocks are executed

- `if-else` is used for **range-based conditions**

- `switch` is used for **fixed values**

### 📌 Key Points

- Control statements guide program execution

- `if-else` is suitable for conditional logic

- `switch` is useful for multiple fixed choices

- `break` prevents fall-through in switch cases

</details>



<details>
<summary>6.Loops</summary>

Loops are used to **execute a block of code repeatedly** based on a condition.

---

### 🔁 `for` Loop

The `for` loop is used when the number of iterations is known.

**Syntax**
```java
for (initialization; condition; increment/decrement) {
    // code to execute
}
```
#### Example

```java
Copy code
for (int i = 1; i <= 5; i++) {
    System.out.println(i);
}
```

### 🔄 while Loop
The `while` loop executes as long as the condition remains true.

#### Syntax

```java
Copy code
while (condition) {
    // code to execute
}
```
#### Example

```java
Copy code
int i = 1;

while (i <= 5) {
    System.out.println(i);
    i++;
}
```
### 🔃 do-while Loop
The `do-while` loop executes **at least once**, even if the condition is false.

#### Syntax

```java

do {
    // code to execute
} while (condition);
```

#### Example

```java

int i = 1;

do {
    System.out.println(i);
    i++;
} while (i <= 5);
```

#### ⛔ `break` and `continue`
`break`

- Terminates the loop immediately

```java
Copy code
for (int i = 1; i <= 5; i++) {
    if (i == 3) {
        break;
    }
    System.out.println(i);
}
```
`continue`

- Skips the current iteration and moves to the next one

```java

for (int i = 1; i <= 5; i++) {
    if (i == 3) {
        continue;
    }
    System.out.println(i);
}
```
### 📌 Key Points
- Loops reduce code repetition

- `for loop` is ideal when iteration count is known

- `while` loop is condition-based

- `do-while` loop executes at least once

- `break` exits the loop

- `continue` skips the current iteration
</details>


## 🟡 Intermediate Level

<details>
<summary>Object-Oriented Programming (OOP)</summary>

---

## What is Object-Oriented Programming?
Object-Oriented Programming (OOP) is a programming approach that organizes software design around **objects** rather than functions.

An object represents a real-world entity and contains:
- **Data** (variables)
- **Behavior** (methods)

---

## Principles of OOP

---

## 1. Encapsulation

Encapsulation means **binding data and methods together** and restricting direct access to data.

### Key Concepts
- Data hiding
- Controlled access using methods
- Improves security and maintainability

### Access Modifiers
- `private` – accessible only within the class
- `protected` – accessible within package and subclasses
- `public` – accessible everywhere
- `default` – package-level access

### Example
```java
class User {
    private String name;

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }
}
```

## 2. Inheritance

Inheritance allows a class to **acquire properties and behavior of another class**.

### Key Points
- Promotes **code reuse**
- Represents an **is-a relationship**

---

### Types of Inheritance
- **Single inheritance**
- **Multilevel inheritance**
- **Hierarchical inheritance**

> Java does **not** support multiple inheritance with classes.

---

### Example
```java
class Animal {
    void eat() {}
}

class Dog extends Animal {
    void bark() {}
}
```

In this example:

- `Dog` **is an** `Animal`
- `Dog` inherits the `eat()` method from `Animal`

### `super` Keyword

The `super` keyword is used to refer to the **parent class**.

#### Uses of `super`
- Access parent class methods
- Access parent class variables
- Call the parent class constructor

#### Example
```java
class Dog extends Animal {
    Dog() {
        super(); // Calls parent class constructor
    }
}
```

---

## 3. Polymorphism

Polymorphism means **one method behaving differently in different situations**.

---

### Types of Polymorphism

#### Compile-time Polymorphism (Method Overloading)
- Same method name
- Different parameter list
- Decision made at compile time

**Example:**
```java
int add(int a, int b) {
    return a + b;
}

double add(double a, double b) {
    return a + b;
}
```
In this example:

- The `sound()` method behaves differently based on the object type
- This demonstrates **runtime polymorphism**

### Runtime Polymorphism (Method Overriding)

Runtime polymorphism occurs when a **subclass provides a specific implementation** of a method that is already defined in its parent class.

#### Key Points
- Same method signature
- Different implementation in subclass
- Decision made at runtime

#### Example
```java
class Animal {
    void sound() {
        System.out.println("Animal sound");
    }
}

class Dog extends Animal {
    void sound() {
        System.out.println("Dog barks");
    }
}
```
### Overloading vs Overriding

| Feature        | Overloading        | Overriding        |
|---------------|-------------------|------------------|
| Method name   | Same              | Same             |
| Parameters    | Different         | Same             |
| Inheritance   | Not required      | Required         |
| Decision time | Compile-time      | Runtime          |

---

## 4. Abstraction

Abstraction focuses on **hiding implementation details** and exposing only the **essential behavior** of an object.

---

### Abstract Classes
- Can have abstract and non-abstract methods
- Cannot be instantiated

#### Example
```java
abstract class Shape {
    abstract void draw();
}
```
#### Interfaces
- Supports full abstraction

- All methods are abstract by default

- Java 8+ allows default methods

**Example**
```java

interface Flyable {
    void fly();
}
```
#### Functional Interfaces
A functional interface contains **only one abstract method**.

**Example**
```java
@FunctionalInterface
interface Calculator {
    int add(int a, int b);
}
```

Functional interfaces are used heavily in **lambda expressions.**

### Why Use Object-Oriented Programming (OOP)?
- Improves **code reusability**

- Makes code **easier to maintain**

- Supports **scalability**

- Closely models **real-world problems**

- Encourages **clean and structured design**


---

</details>




<details>
  <summary>2.Strings</summary>

In Java, a **String** is an object that represents a sequence of characters.  
Strings are widely used for storing and manipulating text data.

---

#### String Immutability

In Java, **String objects are immutable**, meaning **once a String is created, it cannot be changed**.

If you modify a String, Java actually creates a **new String object** instead of changing the existing one.

**Example:**
```java
String s = "Java";
s = s.concat(" Programming");
```
In this example:

- `"Java"` is **not modified**
- A new String `"Java Programming"` is created
- `s` now points to the **new object**

---

#### Why Immutability Matters

- Improves **security**
- Makes Strings **thread-safe**
- Enables **memory optimization** through the String pool

---

### `String` vs `StringBuilder` vs `StringBuffer`

| Feature        | String              | StringBuilder        | StringBuffer          |
|---------------|---------------------|----------------------|-----------------------|
| Mutability    | Immutable            | Mutable              | Mutable               |
| Thread-safe   | Yes                  | No                   | Yes                   |
| Performance   | Slow (modifications) | Fast                 | Slower than StringBuilder |
| Introduced in | Java 1.0             | Java 1.5             | Java 1.0              |

---

#### When to Use

- Use **String** when data should not change
- Use **StringBuilder** when modifying strings frequently (single-threaded)
- Use **StringBuffer** when thread safety is required

---

#### Example

```java
StringBuilder sb = new StringBuilder("Hello");
sb.append(" World");
System.out.println(sb);
```
### When to Use

- Use **String** when data should not change
- Use **StringBuilder** when modifying strings frequently (single-threaded)
- Use **StringBuffer** when thread safety is required

---

#### Example

```java
StringBuilder sb = new StringBuilder("Hello");
sb.append(" World");
System.out.println(sb);
```

### Common String Methods

Below are some commonly used `String` methods in Java:

- `length()` – returns the length of the string
- `charAt(int index)` – returns the character at a given index
- `substring(int beginIndex, int endIndex)` – extracts a substring
- `equals()` – compares string values
- `equalsIgnoreCase()` – compares strings ignoring case
- `toUpperCase()` – converts string to uppercase
- `toLowerCase()` – converts string to lowercase
- `trim()` – removes leading and trailing spaces
- `replace()` – replaces characters or substrings

---

#### Example

```java
String str = " Java Basics ";

System.out.println(str.length());
System.out.println(str.trim());
System.out.println(str.toUpperCase());
System.out.println(str.substring(1, 5));
```
### Key Takeaways

- Strings are **immutable** in Java
- Use **StringBuilder** for better performance when modifying strings
- Use **StringBuffer** when thread safety is required
- Java provides **rich built-in methods** for string manipulation

---
</details>

### Arrays
- One-dimensional arrays
- Multi-dimensional arrays
- Array utilities

---

### Collections Framework
- List (`ArrayList`, `LinkedList`)
- Set (`HashSet`, `TreeSet`)
- Map (`HashMap`, `TreeMap`)
- Iteration techniques

---

### Exception Handling
- Checked vs unchecked exceptions
- `try-catch-finally`
- `throw` vs `throws`
- Custom exceptions

</details>

---

<details>
<summary>🔵 Advanced Level</summary>

### Multithreading & Concurrency
- Thread lifecycle
- Creating threads
- Synchronization
- Executor framework
- Concurrency utilities

---

### Java 8+ Features
- Lambda expressions
- Streams API
- Functional interfaces
- Method references
- Optional class
- Date & Time API

---

### File Handling
- File class
- Reading and writing files
- Serialization and deserialization
- NIO overview

---

### JDBC
- JDBC architecture
- Database connectivity
- CRUD operations
- Prepared statements
- Connection pooling

---

### Design Patterns
- Singleton
- Factory
- Builder
- Observer
- Best practices

</details>

---

<details>
<summary>🔴 Interview & Real-World</summary>

### Java Interview Questions
- Core Java questions
- OOP interview questions
- Collections interview questions
- Multithreading interview questions

---

### Coding Problems
- String-based problems
- Array-based problems
- Logical problems
- Time & space complexity

---

### Best Practices
- Clean code principles
- Exception handling best practices
- Performance optimization
- Memory management

---

### Performance Optimization
- JVM memory model
- Garbage collection
- Profiling tools
- Common performance pitfalls

</details>

Happy Coding! 🚀



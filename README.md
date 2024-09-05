### **1. [Introduction to Java and OOP Concepts**](https://github.com/PROGHEIST/OOP-IN-JAVA/blob/main/README.md#chapter-1-introduction-to-java-and-oop-concepts)
   - What is Object-Oriented Programming?
   - History of Java and OOP
   - Key OOP principles (Encapsulation, Inheritance, Polymorphism, Abstraction)

### **2. Java Basics Refresher**
   - Java Syntax Overview
   - Data Types, Variables, and Operators
   - Control Structures (if-else, loops)
   - Functions and Methods in Java

### **3. Classes and Objects**
   - What are Classes and Objects?
   - Creating Objects from Classes
   - The `new` keyword
   - Fields and Methods
   - Constructors and Destructors

### **4. Encapsulation in Java**
   - Access Modifiers (public, private, protected)
   - Getters and Setters
   - The `this` Keyword
   - Benefits of Encapsulation

### **5. Inheritance in Java**
   - Basics of Inheritance
   - The `extends` Keyword
   - Method Overriding
   - The `super` Keyword
   - Types of Inheritance (Single, Multilevel, Hierarchical)
   - Abstract Classes and Methods

### **6. Polymorphism in Java**
   - Method Overloading
   - Method Overriding
   - Static vs Dynamic Binding
   - The `instanceof` Keyword

### **7. Abstraction in Java**
   - Abstract Classes vs Interfaces
   - Defining Abstract Classes
   - Implementing Interfaces
   - Multiple Inheritance using Interfaces

### **8. Packages and Access Control**
   - Creating and Using Packages
   - Importing Packages
   - Package-level Access

### **9. Exception Handling**
   - What are Exceptions?
   - Try, Catch, and Finally Blocks
   - Throwing Exceptions
   - Creating Custom Exceptions

### **10. OOP Design Principles and Patterns**
   - SOLID Principles
   - Design Patterns Overview (Factory, Singleton, etc.)
   - Practical Examples of OOP Design

### **11. File I/O and Serialization**
   - Working with Files in Java
   - Input and Output Streams
   - Serialization and Deserialization of Objects

### **12. Collections Framework**
   - Introduction to Collections
   - List, Set, and Map Interfaces
   - ArrayList, LinkedList, HashSet, TreeSet, HashMap
   - Iterators and Enhanced for Loop

### **13. Inner Classes and Lambda Expressions**
   - Types of Inner Classes
   - Local, Anonymous, Static, and Non-static Inner Classes
   - Lambda Expressions in Java

### **14. Java Memory Management**
   - Stack vs Heap Memory
   - Garbage Collection
   - Finalization in Java

### **15. OOP Case Studies and Real-world Examples**
   - Implementing OOP in Real-world Projects
   - Sample Applications (Banking System, E-Commerce)

This index offers a comprehensive guide through the key OOP concepts in Java, from the basics to advanced design principles.

### **Chapter 1: Introduction to Java and OOP Concepts**

#### **1.1 What is Object-Oriented Programming (OOP)?**
Object-Oriented Programming (OOP) is a programming paradigm that organizes software design around data, or objects, rather than functions and logic. OOP focuses on objects as the central entities that encapsulate both state (data) and behavior (functions or methods). This allows for modularity, reusability, and flexibility in building software systems.

##### Key Features of OOP:
- **Encapsulation:** Bundling data (variables) and methods (functions) together in a single unit or object.
- **Abstraction:** Hiding complex details and exposing only essential parts to reduce complexity.
- **Inheritance:** Creating new classes based on existing classes, allowing reuse of methods and properties.
- **Polymorphism:** The ability of a function, object, or method to take on multiple forms.

#### **1.2 History of Java and OOP**
Java is a high-level, class-based, object-oriented programming language developed by Sun Microsystems in 1995. It was designed to be platform-independent, meaning programs written in Java can run on any device that supports the Java Virtual Machine (JVM).

**Key Points in Java’s Development:**
- **1991:** Java was initially conceived by James Gosling and his team as a part of the Green Project to create software for embedded systems.
- **1995:** Java was officially launched with the tagline "Write Once, Run Anywhere" (WORA), highlighting its platform independence.
- **2006:** Sun Microsystems made Java open-source.
- **2010:** Oracle acquired Sun Microsystems, taking ownership of Java.

#### **1.3 Key OOP Principles**

1. **Encapsulation:**
   - **Definition:** Encapsulation is the concept of wrapping data (variables) and code (methods) together into a single unit known as an object. It helps protect the internal state of the object by restricting direct access to some of its components, making it easier to maintain and modify the code without affecting other parts.
   - **Example:**
     ```java
     public class Car {
         private String brand;
         private int speed;

         public void setBrand(String brand) {
             this.brand = brand;
         }

         public String getBrand() {
             return brand;
         }

         public void accelerate() {
             speed += 10;
         }
     }
     ```

2. **Abstraction:**
   - **Definition:** Abstraction allows programmers to focus on essential qualities of an object rather than dealing with its internal complexities. In Java, abstraction is achieved using abstract classes and interfaces.
   - **Example:** Consider a class `Vehicle` where you define the essential properties like `speed` and `fuel`. Specific details of different types of vehicles like cars or bikes are abstracted out.
     ```java
     abstract class Vehicle {
         abstract void start();
     }

     class Car extends Vehicle {
         @Override
         void start() {
             System.out.println("Car is starting");
         }
     }
     ```

3. **Inheritance:**
   - **Definition:** Inheritance allows one class (child or subclass) to inherit properties and methods from another class (parent or superclass). It promotes code reuse and establishes a parent-child relationship between classes.
   - **Example:**
     ```java
     class Animal {
         void sound() {
             System.out.println("This is an animal sound");
         }
     }

     class Dog extends Animal {
         @Override
         void sound() {
             System.out.println("Dog barks");
         }
     }
     ```

4. **Polymorphism:**
   - **Definition:** Polymorphism means "many forms" and allows methods or objects to be used in different ways based on context. It can be achieved via method overloading and overriding.
   - **Example:**
     ```java
     class Calculator {
         // Method Overloading: Same method name but different parameters
         int add(int a, int b) {
             return a + b;
         }

         double add(double a, double b) {
             return a + b;
         }
     }

     class Animal {
         void makeSound() {
             System.out.println("Some sound");
         }
     }

     class Cat extends Animal {
         @Override
         void makeSound() {
             System.out.println("Meow");
         }
     }
     ```

#### **1.4 Why OOP?**
OOP provides several advantages:
   - **Modularity:** OOP divides a program into small, manageable objects, making it easier to develop, maintain, and debug.
   - **Reusability:** Inheritance promotes code reuse.
   - **Flexibility:** Polymorphism and abstraction provide the ability to create flexible, scalable software.
   - **Data Security:** Encapsulation hides data and exposes only what is necessary, making the system more secure.

#### **1.5 Summary**
In this chapter, we introduced the core principles of Object-Oriented Programming (OOP), including Encapsulation, Abstraction, Inheritance, and Polymorphism. These principles guide the way we design and organize Java programs. We also explored Java's history and its importance in the OOP paradigm.

### Next Chapter: Java Basics Refresher
In the next chapter, we will dive into the basic building blocks of Java, including data types, control structures, and methods.

### **Chapter 2: Java Basics Refresher**

Before diving deeper into Object-Oriented Programming (OOP) in Java, it’s essential to revisit some basic concepts of the Java programming language. This will help solidify your understanding of how OOP fits within the broader context of Java development.

#### **2.1 Java Syntax Overview**

Java follows a simple and consistent syntax, which makes it easier to read and write. Here's a quick overview of Java's structure:

- **Java Program Structure:**
   - A Java program consists of classes, and within classes, we have methods and fields (variables).
   - A basic Java program starts with a `main` method, which acts as the entry point for execution.

   **Example:**
   ```java
   public class HelloWorld {
       public static void main(String[] args) {
           System.out.println("Hello, World!");
       }
   }
   ```

   - **Class Definition:** `public class HelloWorld` – defines a class.
   - **Method:** `public static void main(String[] args)` – the main method where the program starts.
   - **Statements:** Inside the `main` method, you define statements like `System.out.println("Hello, World!");` to print output to the console.

#### **2.2 Data Types in Java**

Data types specify the type of data that can be stored in variables. Java provides two categories of data types: **Primitive Types** and **Reference Types**.

##### **Primitive Data Types:**
These are predefined by Java and store simple values.

- **byte:** 1 byte, range -128 to 127.
- **short:** 2 bytes, range -32,768 to 32,767.
- **int:** 4 bytes, range -2^31 to 2^31-1 (commonly used for integers).
- **long:** 8 bytes, range -2^63 to 2^63-1 (use for large integer values).
- **float:** 4 bytes, single-precision floating point (e.g., 3.14f).
- **double:** 8 bytes, double-precision floating point (e.g., 3.14159).
- **char:** 2 bytes, stores a single character (e.g., 'a').
- **boolean:** 1 bit, stores `true` or `false`.

**Example:**
```java
int age = 25;
double salary = 50000.75;
boolean isJavaFun = true;
char grade = 'A';
```

##### **Reference Data Types:**
These are objects or arrays. Reference variables store memory addresses of objects.

- **String:** Represents sequences of characters.
- **Arrays:** Hold multiple values of the same type.

**Example:**
```java
String name = "John";
int[] numbers = {1, 2, 3, 4, 5};
```

#### **2.3 Variables in Java**

Variables store data values and must be declared before use. Java is a statically typed language, so you must specify the type of the variable.

**Example:**
```java
int age = 30; // Declaring an integer variable
double price = 19.99; // Declaring a double variable
```

##### **Types of Variables:**
1. **Local Variables:** Declared inside methods and used within that method only.
2. **Instance Variables:** Declared inside a class but outside methods; they represent the state of an object.
3. **Static Variables:** Declared with the `static` keyword and shared by all instances of a class.

**Example of Variables:**
```java
public class Person {
    String name;  // Instance variable
    static int population = 0; // Static variable

    public void setName(String name) {
        this.name = name;  // Local variable in method
    }
}
```

#### **2.4 Operators in Java**

Operators in Java are used to perform operations on variables and values. They include:

1. **Arithmetic Operators:**
   - Addition (`+`), Subtraction (`-`), Multiplication (`*`), Division (`/`), Modulus (`%`)

   **Example:**
   ```java
   int result = 10 + 5;  // result = 15
   ```

2. **Relational Operators:**
   - Greater than (`>`), Less than (`<`), Equal to (`==`), Not equal to (`!=`), Greater than or equal to (`>=`), Less than or equal to (`<=`)

   **Example:**
   ```java
   boolean isAdult = age >= 18;  // Checks if age is greater than or equal to 18
   ```

3. **Logical Operators:**
   - AND (`&&`), OR (`||`), NOT (`!`)

   **Example:**
   ```java
   boolean isEligible = (age >= 18 && isRegistered);  // Checks if age is greater than or equal to 18 and registered
   ```

4. **Assignment Operators:**
   - Assigns values using `=`, and other operators like `+=`, `-=`, `*=`, etc.

   **Example:**
   ```java
   int x = 10;
   x += 5;  // x = x + 5
   ```

#### **2.5 Control Structures**

Control structures guide the flow of a Java program based on conditions or loops.

##### **If-Else Statements:**
Used for decision-making.

**Example:**
```java
if (age >= 18) {
    System.out.println("Adult");
} else {
    System.out.println("Not an Adult");
}
```

##### **Switch Case:**
Used for multi-way branching based on the value of an expression.

**Example:**
```java
int day = 2;
switch(day) {
    case 1: System.out.println("Monday"); break;
    case 2: System.out.println("Tuesday"); break;
    default: System.out.println("Invalid Day");
}
```

##### **Loops:**
1. **For Loop:**
   Repeats a block of code a specific number of times.
   ```java
   for (int i = 0; i < 5; i++) {
       System.out.println(i);
   }
   ```

2. **While Loop:**
   Repeats a block of code as long as a condition is true.
   ```java
   int i = 0;
   while (i < 5) {
       System.out.println(i);
       i++;
   }
   ```

3. **Do-While Loop:**
   Similar to a `while` loop but guarantees at least one iteration.
   ```java
   int i = 0;
   do {
       System.out.println(i);
       i++;
   } while (i < 5);
   ```

#### **2.6 Methods in Java**

A method is a block of code that performs a specific task. Methods promote code reusability and modularity.

##### **Defining a Method:**
```java
public int addNumbers(int a, int b) {
    return a + b;
}
```

##### **Calling a Method:**
```java
int sum = addNumbers(5, 10);
System.out.println("Sum: " + sum);
```

##### **Method Parameters and Return Values:**
- Methods can take arguments (parameters) and return values. If a method doesn’t return a value, it is declared as `void`.

**Example:**
```java
public void printMessage() {
    System.out.println("Hello, Java");
}
```

#### **2.7 Summary**

In this chapter, we revisited the fundamental concepts of Java, such as data types, variables, operators, control structures, and methods. These are the basic building blocks that are crucial for understanding the more advanced OOP concepts in Java. In the next chapter, we will explore **Classes and Objects**, which form the foundation of OOP in Java.

---

### Next Chapter: Classes and Objects

### **Chapter 3: Classes and Objects**

In Object-Oriented Programming (OOP), classes and objects are the fundamental building blocks. Java uses classes to define the blueprint of an object, and objects are instances of classes. In this chapter, we will explore how to create and use classes and objects in Java.

#### **3.1 What are Classes and Objects?**

- **Class:** A class is a template or blueprint for creating objects. It defines the properties (fields or variables) and behaviors (methods) that objects created from the class can have.
- **Object:** An object is an instance of a class. When a class is instantiated (created), it forms an object. Each object has its own state, defined by its fields, and behavior, defined by its methods.

**Example:**
```java
public class Car {
    // Fields (attributes)
    String brand;
    int speed;

    // Methods (behaviors)
    void accelerate() {
        speed += 10;
        System.out.println("Accelerating... Speed is now: " + speed);
    }

    void brake() {
        speed -= 10;
        System.out.println("Braking... Speed is now: " + speed);
    }
}
```

In the above example, `Car` is a class, and it has two fields (`brand` and `speed`) and two methods (`accelerate` and `brake`).

#### **3.2 Creating Objects from Classes**

Once a class is defined, we can create objects from it using the `new` keyword. Each object created from a class will have its own state (values of fields).

**Example:**
```java
public class Main {
    public static void main(String[] args) {
        // Creating an object of the Car class
        Car myCar = new Car();
        
        // Setting the field values
        myCar.brand = "Toyota";
        myCar.speed = 0;
        
        // Using the object's methods
        myCar.accelerate();
        myCar.brake();
    }
}
```

- **`new Car()`**: This creates a new object of the `Car` class.
- **`myCar`**: This is the reference variable that holds the object.
- The object’s methods (`accelerate()` and `brake()`) can be called to perform actions on that object.

#### **3.3 Fields and Methods**

- **Fields (Attributes/Properties):** These are variables declared inside a class. Fields represent the state or data of an object.
- **Methods (Functions):** Methods define the behavior of an object. They are blocks of code designed to perform a specific task.

**Example:**
```java
public class Dog {
    String breed;
    int age;
    
    void bark() {
        System.out.println("Woof! Woof!");
    }
    
    void displayInfo() {
        System.out.println("Breed: " + breed + ", Age: " + age);
    }
}
```

In the `Dog` class:
- Fields: `breed` and `age` represent the state of a dog.
- Methods: `bark()` and `displayInfo()` define the actions a dog can perform.

#### **3.4 Constructors**

A constructor is a special type of method that is called when an object is instantiated. It is used to initialize the object’s fields with specific values.

- **Default Constructor:** If no constructor is provided, Java provides a default constructor.
- **Parameterized Constructor:** Allows passing values during object creation.

**Example of a Constructor:**
```java
public class Person {
    String name;
    int age;

    // Constructor
    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    void displayInfo() {
        System.out.println("Name: " + name + ", Age: " + age);
    }
}
```

**Creating an Object with a Constructor:**
```java
public class Main {
    public static void main(String[] args) {
        // Creating an object using the constructor
        Person person = new Person("John", 30);
        person.displayInfo();
    }
}
```

In this example, the `Person` class has a constructor that takes two arguments (`name` and `age`). The constructor initializes the fields when the object is created.

#### **3.5 The `this` Keyword**

The `this` keyword in Java is a reference to the current object. It is used to differentiate between instance variables (fields) and parameters that have the same name.

**Example:**
```java
public class Employee {
    String name;
    int id;

    public Employee(String name, int id) {
        this.name = name; // 'this.name' refers to the instance variable
        this.id = id;     // 'this.id' refers to the instance variable
    }

    void displayInfo() {
        System.out.println("Name: " + this.name + ", ID: " + this.id);
    }
}
```

In the constructor, `this.name` refers to the instance variable `name`, while `name` without `this` refers to the parameter.

#### **3.6 Accessing Fields and Methods**

Fields and methods of an object are accessed using the dot (`.`) operator. We use the reference variable followed by the field or method name.

**Example:**
```java
Car myCar = new Car();
myCar.brand = "Honda";  // Accessing field
myCar.accelerate();     // Accessing method
```

#### **3.7 Constructor Overloading**

Java allows you to define multiple constructors with different parameter lists in a class. This is known as **constructor overloading**.

**Example:**
```java
public class Student {
    String name;
    int grade;

    // Default constructor
    public Student() {
        this.name = "Unknown";
        this.grade = 0;
    }

    // Parameterized constructor
    public Student(String name, int grade) {
        this.name = name;
        this.grade = grade;
    }

    void displayInfo() {
        System.out.println("Name: " + name + ", Grade: " + grade);
    }
}
```

You can create objects using either the default or the parameterized constructor:
```java
Student student1 = new Student();               // Calls the default constructor
Student student2 = new Student("Alice", 90);    // Calls the parameterized constructor
```

#### **3.8 Destructors in Java**

Java does not have destructors like other programming languages (e.g., C++). Instead, Java has a garbage collector that automatically deallocates memory when objects are no longer needed. However, if you want to perform cleanup before an object is destroyed, you can use the `finalize()` method, although its usage is discouraged as it's not guaranteed when or if it will be executed.

**Example:**
```java
protected void finalize() {
    System.out.println("Object is being destroyed");
}
```

#### **3.9 Summary**

In this chapter, we explored the core concepts of **classes** and **objects** in Java. We learned how to define classes, create objects, and use fields and methods. Additionally, we covered constructors, the `this` keyword, and constructor overloading. Understanding these concepts is crucial for working with OOP principles in Java.

---

### Next Chapter: Encapsulation in Java
In the next chapter, we will dive deeper into one of the key OOP principles: **Encapsulation**, and learn how to protect data in Java using access modifiers, getters, and setters.

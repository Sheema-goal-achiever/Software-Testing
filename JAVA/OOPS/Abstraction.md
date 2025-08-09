# Abstraction

**Definition:**  
Abstraction is the process of hiding implementation details and showing only the essential features.

**Key Points:**
- Achieved using **abstract classes** or **interfaces**
- Helps reduce complexity
- Focuses on **what** an object does rather than **how** it does it

**Example in Java:**
```java
abstract class Vehicle {
    abstract void start();
}

class Car extends Vehicle {
    void start() {
        System.out.println("Car starts with a key.");
    }
}

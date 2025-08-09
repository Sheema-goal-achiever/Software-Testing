# Polymorphism

**Definition:**  
Polymorphism means **many forms** — the ability of an object to take different forms depending on the situation.

**Types:**
1. **Compile-time Polymorphism** (Method Overloading)
2. **Runtime Polymorphism** (Method Overriding)

**Example in Java:**
```java
// Compile-time polymorphism
class Calculator {
    int add(int a, int b) {
        return a + b;
    }
    double add(double a, double b) {
        return a + b;
    }
}

// Runtime polymorphism
class Animal {
    void sound() {
        System.out.println("Animal makes a sound");
    }
}
class Dog extends Animal {
    void sound() {
        System.out.println("Dog barks");
    }
}

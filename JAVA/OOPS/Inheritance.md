# Inheritance

**Definition:**  
Inheritance is the process where one class (child) can use the properties and methods of another class (parent).

**Key Points:**
- Promotes **code reusability**
- Achieved using the `extends` keyword
- Supports **single** and **multilevel** inheritance (but not multiple inheritance with classes)

**Example in Java:**
```java
class Animal {
    void eat() {
        System.out.println("This animal eats food.");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("Dog barks.");
    }
}

public class Main {
    public static void main(String[] args) {
        Dog d = new Dog();
        d.eat(); // from Animal
        d.bark(); // from Dog
    }
}

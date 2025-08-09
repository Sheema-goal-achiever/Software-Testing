# Encapsulation

**Definition:**  
Encapsulation is the process of hiding the internal details of a class and only exposing the necessary parts through methods.

**Key Points:**
- Achieved by making variables **private**
- Accessed and modified through **getter** and **setter** methods
- Protects the data from unwanted changes

**Example in Java:**
```java
class Person {
    private String name; // private variable

    public String getName() { // getter
        return name;
    }

    public void setName(String name) { // setter
        this.name = name;
    }
}

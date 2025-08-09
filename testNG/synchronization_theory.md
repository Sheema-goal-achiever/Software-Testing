# ⏳ Selenium Synchronization – Theory

Synchronization in Selenium ensures tests wait for elements or events before proceeding.

---

## Types of Wait
1. **Implicit Wait** – The driver waits for a specific duration to make sure all the elements are loaded within DOM. The default time is 0 sec  , if the element is not found it throws NoSuchElementException.
2. **Explicit Wait** – The driver waits for a specific DOM element for a specific duration under a given condition. Incased driver is not able to find the element the driver throws NoSuchElementException.
3. **Fluent Wait** – It is an explicit wait but more flexible . It has a polling rate(frequency) .It waits for a specific element for a specific duration under a specific condition

**Note** In industry Explicite wait is more commonly used than Fluent wait.

---

## 📄 Practical Example
See: [Synchronization Practical](./synchronization_practical.md)

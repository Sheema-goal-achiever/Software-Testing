# 📝 Test Scenarios

## **What is a Test Scenario?**
A **test scenario** is a high-level description of **what needs to be tested** in the software.  
It focuses on **real-world use cases** and helps testers ensure the software behaves as expected.

Think of it like a *to-do list* for testing, written in plain language.

---

## **Why are Test Scenarios Important?**
- They help **cover all possible functionalities**.
- They ensure the software is tested from a **user’s perspective**.
- They guide testers in creating **detailed test cases** later.

---

## **Example**

**Project:** Online Shopping Website  
**Feature:** Login Page

### Possible Test Scenarios:
1. Verify that a user can log in with a valid username and password.
2. Verify that login fails with an incorrect password.
3. Verify that the "Forgot Password" link works correctly.
4. Verify that the system shows an error when fields are left blank.
5. Verify that a logged-in user can log out successfully.

---

## 📌 Key Points:
- Test scenarios are **broad** and **do not include step-by-step details**.
- They are **derived from requirements**.
- They are helpful for **both manual and automation testing**.

---

## **Test Scenario vs Test Case**

| Feature            | Test Scenario                                  | Test Case                                      |
|--------------------|-----------------------------------------------|------------------------------------------------|
| **Definition**     | High-level idea of what to test               | Detailed steps on how to test                  |
| **Details**        | Minimal                                        | Very detailed (steps, data, expected results)  |
| **Purpose**        | Ensure coverage of features                   | Ensure correctness of features                 |
| **Example**        | "Check login functionality"                   | Steps: Enter username, enter password, click login, verify homepage |

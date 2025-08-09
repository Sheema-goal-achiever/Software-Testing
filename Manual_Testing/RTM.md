# 📌 Requirement Traceability Matrix (RTM)

## 🔍 What is RTM?
A **Requirement Traceability Matrix (RTM)** is a table that links each requirement to its corresponding **test cases** to ensure that **all requirements are covered by testing**.

It helps in:
- Making sure **no requirement is missed** during testing
- Tracking the status of each requirement
- Proving that testing is complete

---

## 📖 Example

| Requirement ID | Requirement Description               | Test Case ID(s)    | Status   |
|----------------|---------------------------------------|--------------------|----------|
| R1             | User should be able to login          | TC001, TC002       | Pass     |
| R2             | Password should reset via email link  | TC003, TC004       | Fail     |
| R3             | User can search products by name      | TC005              | Pass     |

---

## 🛠️ Benefits of RTM
1. Ensures **complete test coverage**
2. Easy to identify **missing test cases**
3. Tracks the progress of testing
4. Helps during **impact analysis** when requirements change

---

## 📌 Types of Traceability in RTM
1. **Forward Traceability** → Links requirements to test cases (ensures all requirements are tested)
2. **Backward Traceability** → Links test cases back to requirements (ensures test cases are relevant)
3. **Bi-Directional Traceability** → Combines both forward and backward traceability

---

✅ **In short:** RTM is like a checklist that maps **every requirement to at least one test case**, ensuring **nothing is left untested**.

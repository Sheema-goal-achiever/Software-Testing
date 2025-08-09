# ⚙ JDBC Architecture

The JDBC architecture consists of two main layers:

1. **JDBC API** – Defines interfaces and classes for connecting and interacting with databases.
2. **JDBC Driver API** – Communicates with the specific database via drivers.

### 🔹 Flow:
1. Java application calls JDBC API
2. JDBC API interacts with JDBC Driver
3. JDBC Driver sends SQL to the database
4. Database processes request and returns results

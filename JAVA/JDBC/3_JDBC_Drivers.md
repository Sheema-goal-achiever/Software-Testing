# 🔌 JDBC Drivers

JDBC uses **drivers** to connect to databases. There are 4 main types:

1. **Type 1: JDBC-ODBC Bridge Driver** – Uses ODBC for connection (outdated).
2. **Type 2: Native API Driver** – Uses database-specific native libraries.
3. **Type 3: Network Protocol Driver** – Uses middleware for database access.
4. **Type 4: Thin Driver** – Pure Java driver, directly connects to the database.

**✅ Most Common Today:** Type 4 (Thin Driver) for MySQL, PostgreSQL, Oracle, etc.

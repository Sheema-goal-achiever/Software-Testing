# 🛠 Steps to Connect Java with Database (JDBC)

1. **Import JDBC packages**  
   ```java
   import java.sql.*;

2. **Load and Register the driver**
   ```java
   Class.forName("com.mysql.cj.jdbc.Driver");

3. **Establish a connection**
   ```java
   Connection con = DriverManager.getConnection(
    "jdbc:mysql://localhost:3306/mydb", "username", "password");

4. **Create a Statement**
   ```java
   Statement stmt = con.createStatement();

5. **Execute a query**
   ```java
   ResultSet rs = stmt.executeQuery("SELECT * FROM users");

6. **Process the results**
   ```java
   while(rs.next()) {
    System.out.println(rs.getString("name"));
}

7. **Close the connection**
   ```java
   con.close();

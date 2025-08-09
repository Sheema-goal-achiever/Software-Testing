# Test Case vs Test Script

## 🧪 Test Case
- A **test case** is a written document that describes **what to test** and **the steps to follow**.
- It’s usually **manual** and focuses on checking one specific function or feature.
- Written in simple language so **any tester** can follow it.

**Example:**
**Test Case:** Verify login with valid credentials  
1. Open the login page.  
2. Enter a valid username.  
3. Enter a valid password.  
4. Click "Login".  
5. **Expected Result:** User should be redirected to the homepage.

---

## 💻 Test Script
- A **test script** is a **set of instructions written in code** to automate a test case.
- Used in **automation testing** with tools like Selenium, TestNG, etc.
- Runs automatically without manual steps.

**Example (Selenium Java Script):**
```java
driver.get("https://example.com/login");
driver.findElement(By.id("username")).sendKeys("validUser");
driver.findElement(By.id("password")).sendKeys("validPass");
driver.findElement(By.id("loginButton")).click();

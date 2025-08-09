# 🚗 Selenium WebDriver – Practical Example
```java
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class WebDriverExample {
    public static void main(String[] args) {
        // Set the path to chromedriver
        System.setProperty("webdriver.chrome.driver", "path/to/chromedriver");

        // Create instance of ChromeDriver
        WebDriver driver = new ChromeDriver();

        // Open Google
        driver.get("https://www.google.com");

        // Print page title
        System.out.println("Page title: " + driver.getTitle());

        // Close browser
        driver.quit();
    }
}

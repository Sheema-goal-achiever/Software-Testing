# 🎯 Selenium Locators – Practical Example
```java
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;

public class LocatorsExample {
    public static void main(String[] args) {
        System.setProperty("webdriver.chrome.driver", "path/to/chromedriver");
        WebDriver driver = new ChromeDriver();

        driver.get("https://www.example.com");

        // By ID
        WebElement elementById = driver.findElement(By.id("username"));

        // By Name
        WebElement elementByName = driver.findElement(By.name("password"));

        // By XPath
        WebElement elementByXPath = driver.findElement(By.xpath("//button[@type='submit']"));

        // By CSS Selector
        WebElement elementByCSS = driver.findElement(By.cssSelector(".btn-login"));

        driver.quit();
    }
}

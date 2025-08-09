```java
import org.openqa.selenium.*;
import org.openqa.selenium.chrome.ChromeDriver;
import org.testng.ITestResult;
import org.testng.annotations.*;

import java.io.File;
import java.io.IOException;
import java.nio.file.Files;

public class ReportsExample {
    WebDriver driver;

    @BeforeTest
    public void setup() {
        System.setProperty("webdriver.chrome.driver", "path/to/chromedriver");
        driver = new ChromeDriver();
    }

    @Test
    public void testExample() {
        driver.get("https://example.com");
        WebElement element = driver.findElement(By.id("nonExistentElement")); // Will fail
        element.click();
    }

    @AfterMethod
    public void takeScreenshotOnFailure(ITestResult result) throws IOException {
        if (result.getStatus() == ITestResult.FAILURE) {
            TakesScreenshot ts = (TakesScreenshot) driver;
            File src = ts.getScreenshotAs(OutputType.FILE);
            Files.copy(src.toPath(), new File("screenshot_" + result.getName() + ".png").toPath());
        }
    }

    @AfterTest
    public void tearDown() {
        driver.quit();
    }
}

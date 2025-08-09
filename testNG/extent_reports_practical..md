```java
import com.aventstack.extentreports.*;
import com.aventstack.extentreports.reporter.ExtentHtmlReporter;

public class ExtentReportsExample {
    public static void main(String[] args) {
        ExtentHtmlReporter htmlReporter = new ExtentHtmlReporter("extentReport.html");
        ExtentReports extent = new ExtentReports();
        extent.attachReporter(htmlReporter);

        ExtentTest test = extent.createTest("Sample Test", "Checking report generation");
        test.pass("Step 1 passed");
        test.fail("Step 2 failed");
        test.info("Execution completed");

        extent.flush();
    }
}

# TestNG attributes
```java
import org.testng.annotations.Test;

public class TestNGAttributesExample {

    @Test(priority = 1)
    public void testLogin() {
        System.out.println("Login Test");
    }

    @Test(priority = 2, dependsOnMethods = "testLogin")
    public void testSearch() {
        System.out.println("Search Test");
    }

    @Test(priority = 3, enabled = false)
    public void testDisabled() {
        System.out.println("This will not run");
    }
}

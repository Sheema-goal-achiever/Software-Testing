```java
import java.io.FileInputStream;
import java.io.IOException;
import java.util.Properties;

public class PropertiesFileExample {
    public static void main(String[] args) throws IOException {
        Properties props = new Properties();
        FileInputStream fis = new FileInputStream("config.properties");
        props.load(fis);

        System.out.println("URL: " + props.getProperty("url"));
        System.out.println("Username: " + props.getProperty("username"));
    }
}

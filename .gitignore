import java.util.concurrent.TimeUnit;
import org.openqa.selenium.*;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.firefox.FirefoxDriver;

public class webDriverdemo {
	public static void main(String[] args) {
		// WebDriver driver = new FirefoxDriver();

		System.setProperty("webdriver.chrome.driver",
				"C:\\Program Files (x86)\\Google\\Chrome\\Application\\chromedriver.exe");
		WebDriver driver = new ChromeDriver();

		// Puts a Implicit wait, Will wait for 10 seconds before throwing
		// exception
		driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);

		// Launch website
		driver.get("http://www.baidu.com/");

		// Maximize the browser
		driver.manage().window().maximize();
		//login in account
		WebElement element = driver.findElement(By.name("wd"));
		element.clear();
		element.sendKeys("google");
		driver.findElement(By.id("su")).click();;
		
		//login
		driver.findElement(By.name("tj_login")).click();
		
		WebElement elementUsername = driver.findElement(By.name("userName"));
		elementUsername.click();
		elementUsername.sendKeys("a420344");
		
		WebElement elementPwd = driver.findElement(By.name("password"));
		elementPwd.click();
		elementPwd.sendKeys("420344");
		
		driver.findElement(By.id("TANGRAM__PSP_8__submit")).click();

		// Close the Browser.
		driver.close();
	}
}

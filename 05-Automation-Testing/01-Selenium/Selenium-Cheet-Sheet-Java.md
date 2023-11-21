# Selenium with Java Cheat Sheet

## Driver Initialization

```java
// Firefox
WebDriver driver = new FirefoxDriver();
// Chrome
WebDriver driver = new ChromeDriver();
// Internet Explorer
WebDriver driver = new InternetExplorerDriver();
// Safari
WebDriver driver = new SafariDriver();
// HtmlUnit
WebDriver driver = new HtmlUnitDriver();
```

## Navigation

```java
// Open a web page
driver.navigate().to("http://www.google.com");
driver.get("http://www.google.com");
// Click the forward button
driver.navigate().forward();
// Click the back button
driver.navigate().back();
// Refresh the page
driver.navigate().refresh();
```

## Waits

```java
// Implicit wait 10 seconds
driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);
// Explicit wait 10 seconds
WebDriverWait wait = new WebDriverWait(driver, 10);
// Wait until element is visible
wait.until(ExpectedConditions.visibilityOfElementLocated(By.id("someid")));
```

## Find Elements

```java
// By.id
driver.findElement(By.id("someid"));
// By.name
driver.findElement(By.name("somename"));
// By.className
driver.findElement(By.className("someclass"));
// By.tagName
driver.findElement(By.tagName("sometag"));
// By.linkText
driver.findElement(By.linkText("some link"));
// By.partialLinkText
driver.findElement(By.partialLinkText("some partial link"));
// By.cssSelector
driver.findElement(By.cssSelector("input#email"));
// By.xpath
driver.findElement(By.xpath("//input[@id='email']"));
```

## Find Multiple Elements

```java
```

## Element Actions

```java
// Click
driver.findElement(By.id("someid")).click();
// Send keys
driver.findElement(By.id("someid")).sendKeys("some text");
// Clear
driver.findElement(By.id("someid")).clear();
// Get text
driver.findElement(By.id("someid")).getText();
// Get attribute
driver.findElement(By.id("someid")).getAttribute("someattribute");
// Get tag name
driver.findElement(By.id("someid")).getTagName();
// Get css value
driver.findElement(By.id("someid")).getCssValue("somecssvalue");
// Is displayed
driver.findElement(By.id("someid")).isDisplayed();
// Is enabled
driver.findElement(By.id("someid")).isEnabled();
// Is selected
driver.findElement(By.id("someid")).isSelected();
```

## Select

```java
// Select by visible text
Select select = new Select(driver.findElement(By.id("someid")));
select.selectByVisibleText("some text");
// Select by index
select.selectByIndex(1);
// Select by value
select.selectByValue("somevalue");
// Get all options
List<WebElement> options = select.getOptions();
```

## Alerts

```java
// Switch to alert
Alert alert = driver.switchTo().alert();
// Accept alert
alert.accept();
// Dismiss alert
alert.dismiss();
// Get alert text
alert.getText();
// Send keys to alert
alert.sendKeys("some text");
// Accept alert
driver.switchTo().alert().accept();
```

## Frames

```java
// Switch to frame by index
driver.switchTo().frame(0);
// Switch to frame by name
driver.switchTo().frame("somename");
// Switch to frame by id
driver.switchTo().frame("someid");
// Switch to frame by WebElement
driver.switchTo().frame(driver.findElement(By.id("someid")));
// Switch to default content
driver.switchTo().defaultContent();
```

## Windows

```java
// Switch to window by name
driver.switchTo().window("somename");
// Switch to window by handle
driver.switchTo().window("somehandle");
// Get current window handle
driver.getWindowHandle();
// Get all window handles
import java.util.Set;
driver.getWindowHandles();
// Switch to new window
driver.switchTo().newWindow(WindowType.WINDOW);
// Switch to new tab
driver.switchTo().newWindow(WindowType.TAB);
// Set window position
driver.manage().window().setPosition(new Point(0, 0));
// Set window size
driver.manage().window().setSize(new Dimension(1024, 768));
// Maximize window
driver.manage().window().maximize();
// Fullscreen window
driver.manage().window().fullscreen();
// Minimize window
driver.manage().window().minimize();
// Screenshot window
import org.apche.commons.io.FileUtils;
File screenshot = ((TakesScreenshot) driver).getScreenshotAs(OutputType.FILE);
FileUtils.copyFile(screenshot, new File("screenshot.png"));
```

## Cookies

```java
// Add cookie
Cookie cookie = new Cookie("somecookie", "somevalue");
driver.manage().addCookie(cookie);
// Get cookie
driver.manage().getCookieNamed("somecookie");
// Get all cookies
driver.manage().getCookies();
// Delete cookie
driver.manage().deleteCookie(cookie);
// Delete all cookies
driver.manage().deleteAllCookies();
```

## TestNG

```java
// Before suite
@BeforeSuite
public void beforeSuite() {
}
// After suite
@AfterSuite
public void afterSuite() {
}
// Before test
@BeforeTest
public void beforeTest() {
}
// After test
@AfterTest
public void afterTest() {
}
// Before class
@BeforeClass
public void beforeClass() {
}
// After class
@AfterClass
public void afterClass() {
}
// Before method
@BeforeMethod
public void beforeMethod() {
}
// After method
@AfterMethod
public void afterMethod() {
}
// Test
@Test
public void test() {
}
// Data provider
@DataProvider
public Object[][] dataProvider() {
}
// Factory
@Factory
public Object[] factory() {
}
// Listener
@Listeners({ TestListener.class })
public class TestClass {
}
// Test listener
public class TestListener implements ITestListener {
}
// Test suite
<suite name="Test Suite">
  <test name="Test">
    <classes>
      <class name="TestClass" />
    </classes>
  </test>
</suite>
```

## JUnit

```java
// Before class
@BeforeClass
public static void beforeClass() {
}
// After class
@AfterClass
public static void afterClass() {
}
// Before
@Before
public void before() {
}
// After
@After
public void after() {
}
// Test
@Test
public void test() {
}
// Test suite
@RunWith(Suite.class)
@SuiteClasses({ TestClass.class })
public class TestSuite {
}
```

## Logging

```java
// Log4j
import org.apache.log4j.Logger;
private static final Logger logger = Logger.getLogger(TestClass.class);
logger.info("some info");
logger.warn("some warning");
logger.error("some error");
logger.fatal("some fatal");
```

## Exceptions

```java
// Try catch
try {
} catch (Exception e) {
}
// Throw
throw new Exception("some exception");
// Throws
public void someMethod() throws Exception {
}
```

## Miscellaneous

```java
// Get current URL
driver.getCurrentUrl();
// Get page source
driver.getPageSource();
// Get title
driver.getTitle();
// Get window handle
driver.getWindowHandle();
// Get window handles
driver.getWindowHandles();
// Get screenshot
File screenshot = ((TakesScreenshot) driver).getScreenshotAs(OutputType.FILE);
// Get size
driver.manage().window().getSize();
// Get position
driver.manage().window().getPosition();
// Get orientation
driver.manage().window().getOrientation();
// Get timeouts
driver.manage().timeouts();
// Print page title
System.out.println(driver.getTitle());
// Sleep
Thread.sleep(1000);
```

## Working with files

```java
// Read file with BufferedReader
File file = new File("somefile.txt");
BufferedReader reader = new BufferedReader(new FileReader(file));
String line;
while ((line = reader.readLine()) != null) {
  System.out.println(line);
}
reader.close();
// Read file with InputStream
File file = new File("somefile.txt");
InputStream inputStream = new FileInputStream(file);
int data;
while ((data = inputStream.read()) != -1) {
  System.out.println(data);
}
inputStream.close();
// Read file with FileReader
File file = new File("somefile.txt");
FileReader fileReader = new FileReader(file);
int data;
while ((data = fileReader.read()) != -1) {
  System.out.println(data);
}
fileReader.close();
// Read file from a CSV file
import au.com/bytecode.opencsv.CSVReader;
CSVReader reader = new CSVReader(new FileReader("somefile.csv"));
String[] line;
while ((line = reader.readNext()) != null) {
  System.out.println(line[0] + " " + line[1] + " " + line[2]);
}
reader.close();
// Read file from an Excel file
import org.apache.poi.ss.usermodel.HSSFSheet;
import org.apache.poi.ss.usermodel.HSSFWorkbook;
import java.io.File;
import java.io.FileInputStream;
import java.io.IOException;
public class ReadExcel {
  public static void main(String[] args) throws IOException {
    File file = new File("somefile.xls");
    FileInputStream inputStream = new FileInputStream(file);
    HSSFWorkbook workbook = new HSSFWorkbook(inputStream);
    HSSFSheet sheet = workbook.getSheetAt(0);
    HSSFRow row = sheet.getRow(0);
    HSSFCell cell = row.getCell(0);
    for (int i = 0; i <= sheet.getLastRowNum(); i++) {
      System.out.println(sheet.getRow(i).getCell(0).getStringCellValue() + " " + sheet.getRow(i).getCell(1).getStringCellValue() + " " + sheet.getRow(i).getCell(2).getStringCellValue());
    }
    workbook.close();
    inputStream.close();
  }
}
// Write file
File file = new File("somefile.txt");
BufferedWriter writer = new BufferedWriter(new FileWriter(file));
writer.write("some text");
writer.close();
// Delete file
File file = new File("somefile.txt");
file.delete();
// Create directory
File dir = new File("somedir");
dir.mkdir();
// Delete directory
File dir = new File("somedir");
dir.delete();
// Get current directory
File dir = new File(".");
dir.getAbsolutePath();
// Get files in directory
File dir = new File(".");
File[] files = dir.listFiles();
for (File file : files) {
  System.out.println(file.getName());
}
// Upload file
WebElement element = driver.findElement(By.id("someid"));
element.sendKeys("/path/to/file");
element.submit();
// Download file
driver.get("http://www.example.com/somefile.txt");
File file = new File("somefile.txt");
FileUtils.copyURLToFile(driver.getCurrentUrl(), file);

```

## Working with databases

```java
// Connect to database
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;
public class Database {
  public static void main(String[] args) throws SQLException {
    Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/somedatabase", "someuser", "somepassword");
  }
}
// Execute query
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.ResultSet;
import java.sql.SQLException;
import java.sql.Statement;
public class Database {
  public static void main(String[] args) throws SQLException {
    Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/somedatabase", "someuser", "somepassword");
    Statement statement = connection.createStatement();
    ResultSet resultSet = statement.executeQuery("SELECT * FROM sometable");
    while (resultSet.next()) {
      System.out.println(resultSet.getString("somecolumn"));
    }
    resultSet.close();
    statement.close();
    connection.close();
  }
}
// Execute update
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;
import java.sql.Statement;
public class Database {
  public static void main(String[] args) throws SQLException {
    Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/somedatabase", "someuser", "somepassword");
    Statement statement = connection.createStatement();
    statement.executeUpdate("UPDATE sometable SET somecolumn = 'somevalue'");
    statement.close();
    connection.close();
  }
}
// Execute insert
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;
import java.sql.Statement;
public class Database {
  public static void main(String[] args) throws SQLException {
    Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/somedatabase", "someuser", "somepassword");
    Statement statement = connection.createStatement();
    statement.executeUpdate("INSERT INTO sometable (somecolumn) VALUES ('somevalue')");
    statement.close();
    connection.close();
  }
}
// Execute delete
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;
import java.sql.Statement;
public class Database {
  public static void main(String[] args) throws SQLException {
    Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/somedatabase", "someuser", "somepassword");
    Statement statement = connection.createStatement();
    statement.executeUpdate("DELETE FROM sometable WHERE somecolumn = 'somevalue'");
    statement.close();
    connection.close();
  }
}
// Execute stored procedure
import java.sql.CallableStatement;
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;
public class Database {
  public static void main(String[] args) throws SQLException {
    Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/somedatabase", "someuser", "somepassword");
    CallableStatement statement = connection.prepareCall("{call someprocedure(?, ?)}");
    statement.setString(1, "somevalue");
    statement.setString(2, "somevalue");
    statement.execute();
    statement.close();
    connection.close();
  }
}
// Execute batch
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;
import java.sql.Statement;
public class Database {
  public static void main(String[] args) throws SQLException {
    Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/somedatabase", "someuser", "somepassword");
    Statement statement = connection.createStatement();
    statement.addBatch("UPDATE sometable SET somecolumn = 'somevalue'");
    statement.addBatch("UPDATE sometable SET somecolumn = 'somevalue'");
    statement.addBatch("UPDATE sometable SET somecolumn = 'somevalue'");
    statement.executeBatch();
    statement.close();
    connection.close();
  }
}
// Execute transaction
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;
import java.sql.Statement;
public class Database {
  public static void main(String[] args) throws SQLException {
    Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/somedatabase", "someuser", "somepassword");
    connection.setAutoCommit(false);
    Statement statement = connection.createStatement();
    statement.executeUpdate("UPDATE sometable SET somecolumn = 'somevalue'");
    statement.executeUpdate("UPDATE sometable SET somecolumn = 'somevalue'");
    statement.executeUpdate("UPDATE sometable SET somecolumn = 'somevalue'");
    connection.commit();
    statement.close();
    connection.close();
  }
}
// Execute rollback
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;
import java.sql.Statement;
public class Database {
  public static void main(String[] args) throws SQLException {
    Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/somedatabase", "someuser", "somepassword");
    connection.setAutoCommit(false);
    Statement statement = connection.createStatement();
    statement.executeUpdate("UPDATE sometable SET somecolumn = 'somevalue'");
    statement.executeUpdate("UPDATE sometable SET somecolumn = 'somevalue'");
    statement.executeUpdate("UPDATE sometable SET somecolumn = 'somevalue'");
    connection.rollback();
    statement.close();
    connection.close();
  }
}
// Execute prepared statement
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.PreparedStatement;
import java.sql.SQLException;
public class Database {
  public static void main(String[] args) throws SQLException {
    Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/somedatabase", "someuser", "somepassword");
    PreparedStatement statement = connection.prepareStatement("UPDATE sometable SET somecolumn = ? WHERE somecolumn = ?");
    statement.setString(1, "somevalue");
    statement.setString(2, "somevalue");
    statement.executeUpdate();
    statement.close();
    connection.close();
  }
}
```

## Selenium Grid

```java
// Start hub
java -jar selenium-server-standalone-3.141.59.jar -role hub
// Start node
java -jar selenium-server-standalone-3.141.59.jar -role node -hub http://localhost:4444/grid/register
// Start node with Chrome
java -Dwebdriver.chrome.driver="chromedriver.exe" -jar selenium-server-standalone-3.141.59.jar -role node -hub http://localhost:4444/grid/register
// Start node with Chrome and Firefox
java -Dwebdriver.chrome.driver="chromedriver.exe" -Dwebdriver.gecko.driver="geckodriver.exe" -jar selenium-server-standalone-3.141.59.jar -role node -hub http://localhost:4444/grid/register
// Start node with Chrome and Firefox on Windows
java -Dwebdriver.chrome.driver="chromedriver.exe" -Dwebdriver.gecko.driver="geckodriver.exe" -jar selenium-server-standalone-3.141.59.jar -role node -hub http://localhost:4444/grid/register -browser "browserName=chrome,platform=WINDOWS" -browser "browserName=firefox,platform=WINDOWS"
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
// Click the forward button
driver.navigate().forward();
// Click the back button
driver.navigate().back();

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
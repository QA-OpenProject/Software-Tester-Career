# Questions include Software Testing Concepts + Automation (Web + API) + Core Java + SQL

1. What are the challenges with Selenium Automation?
   - No support for non-web based applications
   - Timeout or Sync issues
   - Slowness in IE
   - Limited Reporting
2. What's different between 'WebDriver.findElement()' and 'WebElement.findElement()'?
   - WebDriver.findElement() is used to find the element in the entire page
   - WebElement.findElement() is used to find the element within the webelement
3. What is the difference between Page Object Model (POM) and Page Factory?
   - Page Object Model (POM) is a design pattern to create Object Repository for web UI elements. Under this model, for each web page in the application, there should be corresponding page class. This Page class will find the WebElements of that web page and also contains Page methods which perform operations on those WebElements.
   - Page Factory is an inbuilt Page Object Model concept for Selenium WebDriver but it is enhanced by Page Object Model. It is used to initialize the elements of the Page Object or instantiate the Page Objects itself.
4. What are all the locators that support selenium?
   - ID
   - Name
   - Class Name
   - Tag Name
   - Link Text
   - Partial Link Text
   - CSS Selector
   - XPath
5. How to overcome 'StaleElementReferenceException'?
   - Use 'try-catch' block to handle the exception
   - Use 'PageFactory' to initialize the elements
   - Use 'Explicit Wait' to wait for the element to be present
6. What is the difference between 'Xpath' and 'CSS Selector'?
   - XPath is slower than CSS Selector
   - XPath supports text, but CSS Selector does not
   - XPath can move in both forward and backward direction, but CSS Selector can move only in the forward direction
7. What is the difference between 'findElement' and 'findElements'?
8. How to access the CSS selector using the nth element?
   Here is a syntax for using the CSS selector using the nth element: <type>: nth-child(n)
   Example: input:nth-child(2)
9. How to handle the alerts in Selenium?
   - Use 'Alert' interface to handle the alerts: 
  ```java
  Alert alert = driver.switchTo().alert();
  ```
   - Use 'accept()', 'dismiss()', 'getText()', 'sendKeys("String")' methods to handle the alerts
10. What are the different exceptions you faced in Selenium?
    - NoSuchElementException
    - NoSuchFrameException
    - NoAlertPresentException
    - NoSuchWindowException
    - StaleElementReferenceException
    - ElementNotVisibleException
    - ElementNotSelectableException
    - ElementNotInteractableException
    - TimeoutException
    - WebDriverException
    - SessionNotCreatedException
    - InvalidSelectorException
    - IllegalStateException
11. What is framework? What are the different types of frameworks?
    - A framework is a set of guidelines, coding standards, concepts, practices, processes, project hierarchies, modularity, reporting mechanism, test data injections, etc. to build a software application.
    - Types of frameworks:
      - Data-Driven Framework
      - Keyword-Driven Framework
      - Hybrid Framework
      - Behavior Driven Development (BDD) Framework
12. How ro run Tests in Headless Mode with Chrome?
    - Use 'ChromeOptions' to run the tests in headless mode:
  ```java
  ChromeOptions options = new ChromeOptions();
  options.addArguments("--headless");
  WebDriver driver = new ChromeDriver(options);
  ```
13. How to handle windows-based alerts/popups in Selenium?
    - Use 'Robot' class to handle the windows-based alerts/popups
    - Use 'AutoIT' tool to handle the windows-based alerts/popups
14. What are the Listeners in Selenium?
    - Listeners are used to generate logs and reports
    - Types of Listeners:
      - WebDriver Listeners
        - WebDriverEventListener
        - TestListener
        - IInvokedMethodListener
        - ITestListener
      - TestNG Listeners
        - IAnnotationTransformer
        - IAnnotationTransformer2
        - IConfigurable
        - IHookable
        - IInvokedMethodListener
        - IMethodInterceptor
        - IReporter
        - ISuiteListener
        - ITestListener
15. What are the differents between StringBuffer and StringBuilder?
    - StringBuffer is synchronized, but StringBuilder is not
    - StringBuffer is slower than StringBuilder
16. What are the advantages of Selenium in automation testing world?
    - Open Source
    - Support for multiple languages
    - Support for multiple browsers
    - Support for multiple OS
    - Support for parallel execution
    - Support for distributed testing
    - Support for headless testing
    - Support for cloud testing
    - Support for CI/CD
    - Support for multiple frameworks
    - Support for multiple testing types
    - Support for multiple testing tools
    - Support for multiple reporting tools
    - Support for multiple version control tools
    - Support for multiple build tools
    - Support for multiple project management tools
    - Support for multiple bug tracking tools
    - Support for multiple test management tools
    - Support for multiple test data management tools
    - Support for multiple test environment management tools
    - Support for multiple test execution management tools
    - Support for multiple test result management tools
    - Support for multiple test case management tools
    - Support for multiple test plan management tools
    - Support for multiple test suite management tools
    - Support for multiple test scenario management tools
    - Support for multiple test step management tools
    - Support for multiple test run management tools
    - Support for multiple test cycle management tools
    - Support for multiple test set management tools
    - Support for multiple test log management tools
    - Support for multiple test report management tools
    - Support for multiple test dashboard management tools
    - Support for multiple test chart management tools
    - Support for multiple test graph management tools
    - Support for multiple test metric management tools
    - Support for multiple test KPI management tools
    - Support for multiple test trend management tools
    - Support for multiple test analysis management tools
    - Support for multiple test improvement management tools
    - Support for multiple test automation management tools
    - Support for multiple test maintenance management tools
    - Support for multiple test monitoring management tools
    - Support for multiple test control management tools
    - Support for multiple test governance management tools
    - Support for multiple test compliance management tools
    - Support for multiple test risk management tools
    - Support for multiple test security management tools
    - Support for multiple test privacy management tools
    - Support for multiple test confidentiality management tools
    - Support for multiple test integrity management tools
    - Support for multiple test availability management tools
    - Support for multiple test resilience management tools
    - Support for multiple test performance management tools
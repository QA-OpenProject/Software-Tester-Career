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
      - This exception occurs when an element specified by the locator cannot be found in the DOM. It usually happens when trying to interact with an element that is not present or visible on the web page.
    - NoSuchFrameException
    - NoAlertPresentException
    - NoSuchWindowException
      - This exception occurs when attempting to switch to a window or frame that does not exist or is no longer available. It may happen if the window or frame is closed or changed after it was initially located.
    - StaleElementReferenceException
      - This exception occurs when a previously located element is no longer attached to the DOM. It typically happens when the DOM is refreshed or modified after an element is located but before an action is performed on it.
    - ElementNotVisibleException
      - This exception occurs when trying to interact with an element that is present in the DOM but not visible on the web page. It may happen if the element is hidden, overlapped by other elements, or outside the visible area of the page.
    - ElementNotSelectableException
    - ElementNotInteractableException
      - This exception is thrown when an element is present in the DOM but cannot be interacted with, such as clicking, typing, or selecting. It may happen due to element attributes, such as being disabled or hidden.
    - TimeoutException
      - This exception is thrown when a command in Selenium WebDriver does not complete within the specified timeout period. It can occur during page load, element visibility check, or other operations that require waiting.
    - WebDriverException
      - This is a general exception class for WebDriver-related errors. It can be thrown for various reasons, such as unexpected browser behavior, network issues, or internal WebDriver errors.
    - SessionNotCreatedException
    - InvalidSelectorException
      - This exception is thrown when an invalid or incorrect selector is used to locate elements. It may happen if the CSS selector, XPath, or other locators provided are not valid.
    - IllegalStateException
    - UnhandledAlertException
      - This exception occurs when trying to perform an action on a web page that has an unhandled alert dialog. It may happen if an alert, confirmation, or prompt dialog is displayed and not handled appropriately.
    - UnexpectedTagNameException
      - This exception is thrown when interacting with an element (e.g., input field, button) of an unexpected tag name. It may happen if the expected element type does not match the actual element type on the web page.
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
17. What are the disadvantages of Selenium in the automation testing world?
    - No support for non-web-based applications
    - Timeout or Sync issues
    - Slowness in IE
    - Limited Reporting
18. What kind of test cases are not suitable for automation?
    - Test cases that are executed only once
    - Test cases that are executed on an ad-hoc basis
    - Test cases that are executed on an unstable application
    - Test cases that are executed on an application that frequently changes
    - Documentation test cases
    - The 3rd party system which is always changing when making the API calls
    - Easy to test manually, but hard to automate (UI test cases that are always changing, especially when creating the UI interface at the initial stage)
19. How would you build the automation framework from scratch?
    - Understand the requirements
    - Choose the right tools
    - Design the framework
    - Implement the framework
    - Execute the tests
    - Generate the reports
20. Write down the Selenium script to launch the webpage and change the language from the dropdown list.
21. Write down the BDD feature file to test the login function.
22. How many types of inheritance?
23. How to simulate the mouse hover a section which should display the date and time?
24. Which language have you experienced and can you give a rate?
25. How do you do the API testing through Postman?
26. What kind of verification mechanism is used for API testing?
27. How do you make the Postman assertions?
28. Can you give me some common status codes and their meanings?
29. Can you explain your automation framework briefly?

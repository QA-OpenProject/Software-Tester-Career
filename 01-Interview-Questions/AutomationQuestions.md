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
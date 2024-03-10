1. Difference between get and navigate method in Selenium?
2. Difference between quit and close method in WebDriver?
3. What is implicit wait?
4. Difference between implicit and explicit wait?
5. How many ways to handle frames in WebDriver?
6. Code to handle multiple windows in WebDriver?
7. Code to handle multiple tabs in WebDriver?
8. How to handle https certificate in Selenium?
9. Different type of locators present in Selenium?
10. Write syntax for Xpath and CSS Selector if id and tag name is given?
11. How to use contains regular expression in Xpath?
12. How to use regular expression in CSS Selector?
13. What is the class available in Selenium to handle the dropdown?
14. What is the method to check if checkbox is selected?
15. How to validate if element is visible or hiden in webpage?
16. How to get the count of similar object list in the webpage?
17. Importance of desired capabilities in Selenium?
18. How to enter the text in capslock mode in Selenium?
19. How to mouse hover on an element in Selenium?
20. Methods to handle alerts in Selenium?
21. How to get links count in webpage?
22. How to validate if we are navigating to child window successfully?
23. Differences between relative and absolute Xpath?
24. Write down the sample Xpath syntax to handle parent from child object?
25. What driver is must to run tests in Firefox?
26. What driver is must to run tests in Chrome?
27. How to set driver in Firefox and Chrome through script?
28. Difference between findElement and findElements?
29. List out 2 methods available in explicit wait?
30. How to take screenshot in Selenium?
31. How to hit enter key from WebDriver?
32. what's the difference between driver.close() and driver.quit() in the selenium?
    1.  close: close the current window or tab
    2.  quit: close all the windows or tabs opened by the WebDriver instance
33. what's the difference between implicitylyWait and explicitylyWait in the selenium?
    1.  implicitylyWait: it is used to tell the WebDriver to wait for a certain amount of time when trying to find an element or elements if they are not immediately available
    2.  explicitylyWait: it is used to tell the WebDriver to wait for a certain condition to occur before proceeding further in the code
34. How many method to open the url in the selenium?
    1.  get():  it is used to open the url in the browser, it will wait for the page to load before returning control to your test.
    2.  navigate().to(): it is used to open the url in the browser, it will not wait for the page to load before returning control to your test.
35. How many types of locators in the selenium?
    1.  Normal Locators: id, name, class, tagname, linktext, partiallinktext
    2.  Dynamic Locators (Customized Locators): xpath (Absolute/Relative Xpath), CSS Selector
36. what's the difference between absolute xpath and relative xpath in the selenium?
    1.  Absolute XPath: starts from the root node of the document and includes the complete path to the element.
    2.  Relative XPath:  defining their relationship to other elements
37. Between the absolute and relative xpath, which one you are prefer and why?
    1. Relative is performing more efficiency, because it doesn't need to traverse from root node to the end element.
    2. If developer change any element in the absolute xpath chain, the path will be broken.
38. what's the difference between navigate().to(url) and driver.get(url)?
    1.  navigate().to(url): accept url is URL or String format.
    2.  driver.get(url): only accept String format
39. dd

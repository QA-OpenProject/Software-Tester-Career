# Scenario Questions

## Can you walk through your approach to testing a login page for a web application?
- Functional Testing
  - Positive Testing
    - Valid Username and Password
    - Check for case sensitivity in Username and Password.
    - Check for special characters in Username and Password.
  - Negative Testing
    - Invalid Username and Password
    - Empty Username and Password
- Usability Testing
  - UI
    - Text, Labels, Buttons, Links are as per the design.
    - Check for the alignment of the elements according to different screen sizes.
  - Messages
    - Error messages are displayed in case of invalid credentials.
    - Success message is displayed after successful login.
- Security Testing
  - SQL Injection
  - Cross-Site Scripting
  - Brute Force Attack
- Performance Testing
  - Load Testing
  - Stress Testing
  - Endurance Testing
- Compability Testing
  - Browser Compability
  - Device Compability
  - OS Compability
- Accessibility Testing
  - WCAG Guidelines
    - Screen Reader Testing
  - Interactive Elements
    - Keyboard Navigation
    - Focus Order
- Localization Testing
  - Elements are displayed in the correct language.
  - Date and Time formats are as per the country.

## Which area of testing do you invest more in automation UI or API and why?

## With reference to your current Test framework can you explain what the technologies are that you are using and how to achieve the scenario below:
- Test source code management.
- Build test solution
- How you integrate the build system with the test framework
- How do you trigger the test
- How you report

## What is the most challenging UI element that you have come across and how did you handle that?
- Dropdowns
  - Selecting an option from a dropdown.
  - Handling dynamic dropdowns.
- Date Picker
  - Selecting a date from a date picker.
  - Handling different date formats.
- File Upload
  - Uploading a file.
  - Handling different file types.
- Alerts
  - Handling alerts.
  - Handling multiple alerts.
- Iframes
  - Switching to an iframe.
  - Handling elements inside an iframe.
- Tables
  - Handling tables.
  - Handling dynamic tables.
- Popups
  - Handling popups.
  - Handling multiple popups.
- Captcha
  - Handling Captcha.
  - Bypassing Captcha.
- Drag and Drop
  - Dragging an element.
  - Dropping an element.
- Scrolling
  - Scrolling to an element.
  - Scrolling to the bottom of the page.
- Hover
  - Hovering over an element.
  - Handling hover menus.
- Tooltips
  - Handling tooltips.
  - Verifying the text in tooltips.

### How to handle those dynamic contents
- Use XPath or CSS Selectors to locate the element.
- Use Explicit Waits to wait for the element to be present.
- Use Actions class to perform actions like hover, drag and drop, etc.
- Use Retry Mechanism to handle StaleElementReferenceException.

## You are asked to automate the shopping API of Foodstuffs. What are the things you are requesting from the developer to start the project? (Technical aspect only)
- API Documentation
  - Endpoints
  - Request and Response format
  - Authentication details
- Sample Data
  - Sample Request and Response
  - Sample Data for testing
- Environment Details
  - URL of the API
  - Test Environment details
- Error Codes
  - List of Error Codes
  - Error Messages
- Security Details
  - Authentication details
  - Authorization details
- Performance Details
  - Expected Response Time
  - Expected Load
- Integration Details
  - Integration with other APIs
  - Integration with the Database
- Testing Details
  - Testing Scenarios
  - Testing Tools
- Monitoring Details
  - Monitoring Tools
  - Alerts and Notifications
- Version Control
  - API Version
  - Changes in the API
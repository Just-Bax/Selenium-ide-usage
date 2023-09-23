## Installing Selenium IDE
- Go to the official Selenium IDE website: https://www.selenium.dev/selenium-ide/
- Download the selenium IDE extension to your browser.

## Recording a test case
- Launch the Selenium IDE extension in your browser.
- Click "Record a new test in a new project" and enter a name in the `Project Name` input field.

![image](documents/1.png)

- Enter a name in the `Project Name` input field.

![image](documents/2.png)

- Enter a base url of website in the input field `Base url` and click `Start Recording` button.

![image](documents/3.png)

- After entering all the data, the base URL that you entered will open.
- Every action you will perform will be recorded in `Commands window`.

![image](documents/4.png)

Each record contains 4 components:
- The `Command` represents the action or operation you want Selenium IDE to perform. It is a keyword that tells Selenium what to do. Examples of common commands include `click`, `type`, `wait`, `assert` and many others.
- The `Target` specifies the web element(s) on which the command should be executed. It serves as a locator or identifier for the element. The Target can be expressed using various locators, such as `XPath`, `CSS selectors`, `IDs`, `class names`, or `link text`, depending on the specific command and the element you want to interact with.
- The `Value` field is used to provide additional information or data required for the execution of the command. The content of the Value field can vary depending on the command being used. For instance, if you're using the `type` command, the Value would contain the text you want to input into an input field.
- The `Description` field is an optional component. It allows you to add a human-readable description of the command.

![image](documents/5.png)

To manually record an action, right-click in recording view and select `Selenium IDE`. There are 4 basic actions which can do manually: `assert`, `store`, `verify` and `wait for`:
- The assert command is used to verify or assert a specific condition or property of a web element or the page itself. It is primarily used for validation purposes to ensure that the application under test behaves as expected. If the assertion fails, the test case will fail.
-- `Example: assertElementPresent, which verifies the presence of a specified element on the page.`
- The store command is used to capture and store values from web elements or the page into variables. These variables can then be used later in the test script for various purposes, such as input data or verification.
-- `Example: storeText, which stores the text value of a specified element into a variable for later use.`
- The verify command is similar to the assert command in that it is used for validation. However, unlike assert, verify commands do not cause the test case to fail if the verification fails. Instead, they log the result as a warning and allow the test to continue executing.
-- `Example: verifyTitle, which verifies if the page title matches the expected title but does not fail the test if it doesn't match.`
- The wait for command is used to pause the test execution until a certain condition or element state is met. It is particularly useful for handling asynchronous behavior in web applications or ensuring that an element becomes visible, clickable, or available before performing actions on it.
-- `Example: waitForElementVisible, which waits for a specified element to become visible before proceeding with further actions.`

![image](documents/6.png)

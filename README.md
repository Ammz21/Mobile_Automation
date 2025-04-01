# Mobile_Automation

## Overview
This project implements a Behavior-Driven Development (BDD) framework for mobile automation using Selenium, Appium, TestNG, and Cucumber. The goal is to automate a login and checkout scenario in an Android emulator for a mobile application.

## Project Structure
The project is structured as a Maven + TestNG project, with all necessary folders and framework methods created under `test->java`. The latest Java client is included in the `pom.xml`.

## Technologies Used
- **Selenium**: For web automation.
- **Appium**: For mobile application automation.
- **TestNG**: For test management and execution.
- **Cucumber**: For BDD implementation using Gherkin language.
- **Maven**: For project management and dependency management.

## Implementation Details

### BDD Framework
- Gherkin language is used for writing BDD scripts.
- A Runner Class is implemented that extends the `RunnerBase` class to handle data parameters.
- TestNG XML is utilized to call the Runner Class.

### Test Scenario
The following scenario is automated:

**Scenario 1: Login and Checkout**
1. Login to the app as `standard_user`.
2. Add the item **‘Sauce Labs Onesie’** to the cart on the PRODUCTS page.
3. Click on the Cart icon and verify navigation to the **‘YOUR CART’** page.
4. Click on the **‘CHECKOUT’** button.
5. Fill in the **First Name**, **Last Name**, and **Zip/Postal Code**.
6. Click on the **‘Continue’** button.
7. Click on the **‘FINISH’** button.
8. Validate that the user is navigated to the **‘CHECKOUT: COMPLETE PAGE’**.

### Assertions
All "Then" statements in the BDD scripts include assertions to validate the expected outcomes. Test evidence is captured using Selenium methods where applicable.

## Playback
Post-implementation, a playback session will be conducted to demonstrate the functionality of the automated tests.

## Getting Started
1. Clone the repository.
2. Navigate to the project directory.
3. Run `mvn clean install` to install dependencies.
4. Execute the tests using the TestNG XML file.

## Contributing
Feel free to fork the repository and submit pull requests for any improvements or enhancements.



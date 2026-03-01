# Playwright-BDD-Automation

## Overview

Welcome to the **Playwright-BDD-Automation** repository! This project leverages the power of [Playwright](https://playwright.dev/), [Playwright BDD](https://github.com/playwright-community/playwright-bdd), and the Showcasing BDD framework to create a robust, scalable automation suite. The framework follows the Page Object Model (POM) design pattern and utilizes fixtures to manage test data and state, ensuring clean and maintainable test code.

## Features

- **Playwright Integration**: Harness the capabilities of Playwright for high-performance browser automation.
- **BDD Framework**: Implement Behavior-Driven Development (BDD) with Playwright BDD for clear and human-readable test scenarios.
- **Page Object Model (POM)**: Maintainable and reusable code structure using the Page Object Model.
- **Fixtures Support**: Simplified setup and teardown with fixtures for better test isolation and reusability.
- **Parallel Test Execution**: Run tests in parallel to save time and get faster feedback.
- **Retry Mechanism**: Automatically retry failed tests to increase the reliability of the test suite.
- **Comprehensive Reporting**: Generate detailed HTML reports for test execution results.
- **Cross-Browser Testing**: Test on different browsers and devices to ensure cross-browser compatibility.
- **Environment Configuration**: Load environment-specific settings seamlessly using dotenv.

## Installation

To get started with this project, follow the steps below:

1. **Clone the repository**:
   ```sh
   git clone https://github.com/TestRoverAutomation/Playwright-BDD-Automation.git
   cd playwright-bdd-automation
2. **Install dependencies:**:
    ```sh
    npm install
3. **Set environment variables: Create .env files for different environments in the env directory.**

### Configuration

This repository is configured to handle different test setups and environments, supporting various browsers and devices. Below are some key configurations:

Playwright Configuration (playwright.config.ts)
The configuration supports parallel test execution, retries on CI, HTML reporting, trace, screenshot, and video recording on first retries. Environment-specific settings are managed using dotenv.

Project Setup
The configuration includes multiple projects for different testing needs:

- Admin Setup: Authentication setup for admin users.
- User Setup: Authentication setup for regular users.
- Test Setup: General authentication setup for test users.
- Admin Tests: Runs admin-specific tests using predefined storage state.
- User Tests: Executes user-specific tests with respective storage state.
- Test User Tests: Conducts tests for general users with appropriate storage state.

### Scripts
The following scripts are available in the package.json file:

- Run all tests: npm test
- Generate BDD steps: npm run bddgen
- Clean generated files: npm run clean
- Run Playwright tests: npm run playwright-test
- Run tests in QA environment: npm run qa-env
- Run tests in development environment: npm run dev-env

- Run tests in production environment: npm run prod-env

# npm install -i
# npm install playwright playwright-bdd cross-env dotenv
# npm init playwright
# npm run test

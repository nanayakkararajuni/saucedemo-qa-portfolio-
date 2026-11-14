# Manual Test Plan — SauceDemo E-Commerce Application

## 1. Project Information

| Field | Details |
|---|---|
| Project Name | SauceDemo QA Testing Portfolio |
| Test Plan ID | TP-001 |
| Application Under Test | SauceDemo (Swag Labs) |
| Application URL | https://www.saucedemo.com/ |
| Testing Type | Manual Functional Testing |
| Prepared By | QA Portfolio Project Owner |
| Prepared Date | 14 November 2026 |
| Document Version | 1.0 |
| Status | Draft — Pending Test Execution |

## 2. Introduction

This test plan describes the manual testing activities planned for the SauceDemo e-commerce web application.

The purpose of this project is to practise real-world software quality assurance activities, including test planning, test case design, execution, defect reporting, and test result documentation.

The project focuses on the key user workflows of an e-commerce application, including authentication, product browsing, shopping cart operations, and checkout.

## 3. Test Objectives

The main objectives of this testing project are:

1. Verify that the application's main features behave as expected.
2. Validate successful and unsuccessful user interactions.
3. Identify unexpected behavior and potential software defects.
4. Document clear and reproducible manual test cases.
5. Record actual results and compare them with expected results.
6. Prepare defect reports with supporting evidence where applicable.
7. Produce a test execution summary showing the testing outcomes.

## 4. Test Scope

### 4.1 In Scope

The following features are planned for manual testing.

| Feature ID | Feature | Testing Focus | Priority |
|---|---|---|---|
| F-01 | Login | Valid, invalid, empty, and locked-out account scenarios | High |
| F-02 | Product Listing | Product visibility, details, and sorting | Medium |
| F-03 | Shopping Cart | Add items, remove items, verify cart contents | High |
| F-04 | Checkout | Required-field validation and successful checkout | High |
| F-05 | Logout | Session logout and protected page access | Medium |

### 4.2 Out of Scope

The following areas will not be included in the initial manual testing phase:

- Real payment transactions
- Advanced performance and load testing
- Penetration testing
- Backend database validation
- Mobile application testing
- Comprehensive cross-browser compatibility testing

## 5. Test Strategy and Approach

### 5.1 Testing Level

**System Testing**

The application will be tested from the end-user perspective, focusing on its visible functionality.

### 5.2 Testing Types

**Functional Testing**

Verify that features operate according to expected behavior.

**Positive Testing**

Test the application with valid inputs and permitted user actions.

**Negative Testing**

Test the application's handling of invalid or missing information.

**Exploratory Testing**

Explore the application to discover unexpected behavior beyond predefined test cases.

**Regression Testing**

Re-execute selected tests when changes or fixes justify regression checks.

### 5.3 Test Design Techniques

The following techniques will be used where appropriate:

- Equivalence Partitioning
- Boundary Value Analysis
- Experience-Based Testing
- Error Guessing

### 5.4 Test Execution Process

1. Review the selected feature and its expected behavior.
2. Identify test scenarios.
3. Design test cases with clear steps and expected results.
4. Prepare the test environment and test data.
5. Execute the test cases.
6. Record actual results and execution status.
7. Investigate unexpected behavior.
8. Report confirmed defects with reproduction steps.
9. Prepare the test execution summary.

Expected results will be based on observable application behavior, available application instructions, and clearly documented assumptions when formal requirements are unavailable.

## 6. Test Environment

| Component | Test Environment |
|---|---|
| Application | SauceDemo |
| Website | https://www.saucedemo.com/ |
| Test Platform | Desktop web browser |
| Operating System | To be recorded before execution |
| Browser and Version | To be recorded before execution |
| Test Management | GitHub and Markdown/CSV files |
| Automation | Not part of this manual test phase |

The exact browser, version, operating system, and execution date will be documented before running tests.

## 7. Test Data

Testing will use the sample accounts and credentials provided by the SauceDemo application.

Test data will cover:

- A valid test user
- Invalid login credentials
- A locked-out test account
- Empty username and password fields
- Sample checkout customer information
- Different shopping cart item selections

Only demo or fictitious information will be used. Passwords and sensitive information will not be committed to the public repository.

## 8. Entry and Exit Criteria

### 8.1 Entry Criteria

Manual test execution can begin when:

- The SauceDemo application is accessible.
- The required testing environment is available.
- Test data is prepared.
- Test scenarios and expected outcomes are documented.
- The selected manual test cases have been reviewed.

### 8.2 Exit Criteria

The initial manual testing phase will be considered complete when:

- At least 15 planned manual test cases have been executed or their blockers clearly documented.
- Actual results and test statuses have been recorded.
- Unexpected behavior has been investigated.
- Confirmed defects, if any, have been documented.
- Test execution evidence has been organized.
- A test execution summary has been prepared.

Completing this portfolio testing phase does not mean the application is defect-free or approved for production release.

## 9. Test Deliverables

The following artifacts will be prepared:

| Deliverable | Description |
|---|---|
| Test Plan | Defines testing objectives, scope, approach, and schedule |
| Test Scenarios | Identifies conditions and workflows to be tested |
| Test Cases | Includes test steps, expected results, and execution results |
| Defect Reports | Documents confirmed defects, if discovered |
| Test Evidence | Stores relevant screenshots and supporting information |
| Test Execution Summary | Summarizes coverage, results, and limitations |

## 10. Test Schedule

| Date | Planned Activity |
|---|---|
| November 14 | Project setup and documentation |
| November 15 | Complete and review the test plan |
| November 16 | Design manual test cases |
| November 17 | Execute manual test cases |
| November 18 | Exploratory testing and defect reporting |
| November 19 | Complete test execution summary |

**Planned Completion Date:** 19 November 2026

**Career Fair Portfolio Deadline:** 29 November 2026

This schedule may be adjusted if testing is blocked or additional investigation is required.

## 11. Risks, Assumptions, and Limitations

| Risk or Limitation | Potential Impact | Mitigation |
|---|---|---|
| Limited time | Reduced test coverage | Prioritize critical user workflows |
| Demo application changes | Test cases may become outdated | Review behavior before executing tests |
| Limited requirements documentation | Uncertain expected outcomes | Record assumptions and investigate discrepancies |
| Environment or network problems | Tests may be blocked | Record blockers and retry when possible |
| Limited browser coverage | Browser-specific issues may be missed | Clearly state the tested environment |

### Assumptions

- Testing will be performed against the publicly available demo application.
- Only intended demo accounts and fictitious checkout data will be used.
- All testing activities will remain within normal, authorized application usage.
- The initial testing phase will be performed by one tester for learning and portfolio purposes.

---

**Document Status:** Draft

**Next Step:** Design manual test cases for login, product listing, shopping cart, and checkout functionality.

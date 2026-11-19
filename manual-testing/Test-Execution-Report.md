# SauceDemo — Manual Test Execution Report

## 1. Report Information

| Field | Details |
|---|---|
| Project | SauceDemo QA Testing Portfolio |
| Report ID | TER-001 |
| Application Under Test | SauceDemo (Swag Labs) |
| Application URL | https://www.saucedemo.com/ |
| Testing Type | Manual Functional Testing and Exploratory Testing |
| Tester | QA Portfolio Project Owner |
| Report Prepared | 19 November 2026 |
| Test Execution Date(s) | Not provided in the finalized execution records |
| Browser / Version | Not provided |
| Operating System | Not provided |
| Report Status | Completed — based on recorded manual test execution results |
| Related Test Plan | [Test-Plan.md](Test-Plan.md) |

> **Evidence note:** Results in this report are based on the tester's supplied execution statuses and exploratory observations. Browser details, precise execution dates, and screenshot filenames were not supplied for this report; no values have been assumed.

## 2. Executive Summary

This report summarizes the results of manual functional testing for the SauceDemo e-commerce demonstration application. Testing covered four modules: **Login, Product Listing, Shopping Cart, and Checkout**.

A total of **15 test cases** were designed and executed. **All 15 passed**, with **0 failures, 0 blocked tests, and 0 tests not run**. The **pass rate was 100%** among executed cases, and **execution coverage was 100%** of planned cases.

Separately, exploratory testing investigated cart add/remove/re-add behavior, checkout with an empty cart, and cart persistence after logout and login. The tester observed that checkout could be completed with an empty cart; this was documented as **BUG-001**, a **potential business-logic defect** whose expected requirement is **not confirmed**. Cart persistence after relogin also needs requirement clarification. Neither finding is counted as a failed predefined test case.

## 3. Test Scope and Approach

### 3.1 In Scope

- **Login:** Valid credentials, invalid password, empty username, empty password, locked-out account.
- **Product Listing:** Product display, price sorting (low to high), name sorting (A to Z), product details.
- **Shopping Cart:** Add product, remove product, add two different products.
- **Checkout:** Complete checkout with valid details; required-field validation for first name and postal code.
- **Exploratory Testing:** Cart state changes, empty-cart checkout, and cart persistence across logout/login.

### 3.2 Test Approach

The predefined tests were executed manually, using positive and negative functional scenarios. Each result was assessed against the test case's expected behavior and recorded as Pass, Fail, Blocked, or Not Run. Exploratory testing was documented separately to investigate behavior beyond the predefined suite.

### 3.3 Out of Scope

Real payment processing, advanced performance/load testing, penetration testing, backend database validation, mobile-app testing, and comprehensive cross-browser compatibility testing were not included in this phase.

## 4. Test Execution Results

### 4.1 Overall Summary

| Metric | Result |
|---|---:|
| Total planned test cases | 15 |
| Executed test cases (Pass + Fail) | 15 |
| Passed | 15 |
| Failed | 0 |
| Blocked | 0 |
| Not Run | 0 |
| **Pass rate (Passed / Executed)** | **100%** |
| **Execution coverage (Executed / Planned)** | **100%** |

### 4.2 Module-Wise Results

| Module | Planned | Passed | Failed | Blocked | Not Run | Pass Rate |
|---|---:|---:|---:|---:|---:|---:|
| Login | 5 | 5 | 0 | 0 | 0 | 100% |
| Product Listing | 4 | 4 | 0 | 0 | 0 | 100% |
| Shopping Cart | 3 | 3 | 0 | 0 | 0 | 100% |
| Checkout | 3 | 3 | 0 | 0 | 0 | 100% |
| **Total** | **15** | **15** | **0** | **0** | **0** | **100%** |

### 4.3 Detailed Test Case Results

| Test Case ID | Scenario | Status |
|---|---|---|
| TC-LOGIN-001 | Login with valid credentials | Pass |
| TC-LOGIN-002 | Login with incorrect password | Pass |
| TC-LOGIN-003 | Login with empty username | Pass |
| TC-LOGIN-004 | Login with empty password | Pass |
| TC-LOGIN-005 | Login with locked-out user | Pass |
| TC-PROD-001 | Products displayed after login | Pass |
| TC-PROD-002 | Sort products by price, low to high | Pass |
| TC-PROD-003 | Sort products by name, A to Z | Pass |
| TC-PROD-004 | Open correct product details | Pass |
| TC-CART-001 | Add a product to the cart | Pass |
| TC-CART-002 | Remove a product from the cart | Pass |
| TC-CART-003 | Add two different products to the cart | Pass |
| TC-CHK-001 | Checkout with valid customer information | Pass |
| TC-CHK-002 | Checkout with empty first name | Pass |
| TC-CHK-003 | Checkout with empty postal code | Pass |

### 4.4 Interpretation

All **15 predefined functional test cases** met their recorded expected outcomes. This result applies only to the tested scenarios and does **not** establish that every workflow or business rule in the application behaves correctly.

## 5. Exploratory Testing Summary

The tester performed exploratory testing beyond the planned functional cases. Three observations were documented:

| ID | Area / Action | Reported Observation | Assessment |
|---|---|---|---|
| ET-001 / Observation 1 | Add, remove, and re-add an item | The item could be added, removed, and added again. Quantity was shown as 1, with no visible control for adjusting it. | Add/remove/re-add behavior as expected; quantity control not available, but no requirement violation confirmed. |
| ET-001 / Observation 2 | Checkout with an empty cart | With all products removed, the tester could proceed through customer information, checkout overview, and order completion. | **Potential defect — BUG-001; requires requirement verification.** |
| ET-001 / Observation 3 | Cart contents after logout and login | Two selected products remained in the cart after logging out and then logging back into the same account. | Needs requirement verification; persistence may be intentional. |

**Exploratory report:** [Exploratory-Testing.md](Exploratory-Testing.md)

The observations are **not additional formal test cases** and are not added to the 15-case Pass/Fail totals.

## 6. Defect / Investigation Summary

### BUG-001 — Checkout Can Be Completed with an Empty Shopping Cart

| Field | Assessment |
|---|---|
| Bug ID | BUG-001 |
| Affected Module | Checkout |
| Classification | Potential functional / business-logic defect |
| Severity | Medium — provisional |
| Priority | Medium — provisional |
| Status | **Needs Triage / Requirement Verification** |
| Reported Behavior | An empty cart did not prevent progressing through checkout and reaching order completion. |
| Expected Behavior | Under an **assumed** e-commerce rule, checkout should require at least one item. |
| Requirement Evidence | No official SauceDemo requirement confirming this restriction was supplied. |

**Investigation:** The tester reported the behavior during exploratory testing and captured screenshot evidence. Exact evidence filenames and the number of reproducibility attempts were not supplied to this report. The observed behavior is documented, but a defect **against a confirmed requirement** has not been established.

**Detailed report:** [BUG-001.md](bug-reports/BUG-001.md)

**Count summary:** 1 potential defect report requiring triage; 0 confirmed requirement violations established by the information available for this report.

> BUG-001 does **not** change the recorded result of TC-CHK-001: that predefined case covers successful checkout *with valid information and a selected product*, not checkout with an empty cart.

## 7. Evidence and Supporting Documentation

- [Manual Test Plan](Test-Plan.md)
- [Login test cases](test-cases/Login-Test-Cases.md)
- [Product Listing test cases](test-cases/Product-Test-Cases.md)
- [Shopping Cart test cases](test-cases/Cart-Test-Cases.md)
- [Checkout test cases](test-cases/Checkout-Test-Cases.md)
- [Exploratory Testing Report](Exploratory-Testing.md)
- [BUG-001 investigation](bug-reports/BUG-001.md)
- [Evidence folder](evidence/)

Screenshot references, where present, should be inspected in their respective test case or bug report documents. This report does not assert any unverified screenshot filenames.

## 8. Risks and Limitations

1. **Unconfirmed business requirements:** SauceDemo's intended behavior for empty-cart checkout and cart persistence was not established from an authoritative requirement document.
2. **Limited scenario coverage:** The 15 tests focus on selected user journeys, not every application state or input combination.
3. **Environment details not supplied:** Browser/version, operating system, and exact test execution dates are not recorded in the data used to prepare this report. Add them from test records if available.
4. **Exploratory results separate from formal results:** The potential checkout issue was observed outside the 15 predefined tests and must be evaluated separately.
5. **No production release assessment:** This is a QA portfolio exercise on a demo application, not a certification that the application is free of defects or ready for production.

## 9. Conclusion and Recommended Next Actions

**Conclusion:** The tester executed all **15** planned manual functional test cases across Login, Product Listing, Shopping Cart, and Checkout; all **15 passed**, resulting in **100% pass rate** and **100% execution coverage** for the planned suite. Exploratory testing additionally identified a potential empty-cart checkout issue (**BUG-001**) and cart persistence behavior that merit clarification. There is currently insufficient confirmed requirement information to treat either exploratory observation as a proven defect.

**Recommended next actions:**

1. Verify the expected empty-cart checkout business rule and then triage BUG-001 appropriately.
2. Clarify whether cart persistence across logout/login is intended.
3. Add actual execution environment details and ensure all evidence links work.
4. Use the manual test cases as the basis for a small Playwright automation suite.

---

*Report prepared for the SauceDemo QA Internship Portfolio. All stated test counts come from the tester's finalized execution records.*

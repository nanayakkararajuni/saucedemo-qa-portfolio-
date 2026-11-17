# SauceDemo — Checkout Manual Test Cases

## Test Information
- **Application:** SauceDemo
- **Module:** Checkout
- **Testing Type:** Manual Functional Testing
- **Execution Status:** Not Started

---

## TC-CHK-001: Verify Checkout with Valid Information

**Test Type:** Positive  
**Priority:** High  
**Module:** Checkout

### Preconditions
- SauceDemo website is accessible.
- A valid user account is available.
- The user is logged out.
- The shopping cart is initially empty.

### Test Data
- Username: `standard_user`
- Password: `secret_sauce`
- Product: `Sauce Labs Backpack`
- First Name: `Test`
- Last Name: `User`
- Postal Code: `12345`

### Test Steps
1. Open https://www.saucedemo.com/.
2. Enter username as standard_user and password as secret_sauce .
3. Click the Login button and log in to items page.
4. Add the Sauce Labs Backpack to the cart.
5. Open the shopping cart.
6. Enter Proceed to checkout.
7. Enter first name as Test last name as User and Postel code as 12345 customer information.
8. Continue to the checkout overview.
9. Complete the order.
10. Verify the confirmation message.

### Expected Result
After Successfully submit the  customer information get the comfirmation massage.

### Actual Result
Not executed yet.

### Status
Not Run

### Evidence
Not collected yet.

---

## TC-CHK-002: Verify Checkout with an Empty First Name

**Test Type:** Negative  
**Priority:** High  
**Module:** Checkout

### Preconditions
- SauceDemo website is accessible.
- A valid user account is available.
- The user is logged out.
- The shopping cart is initially empty.

### Test Data
- Username: `standard_user`
- Password: `secret_sauce`
- Product: `Sauce Labs Backpack`
- First Name: Empty
- Last Name: `User`
- Postal Code: `12345`

### Test Steps
1. Open https://www.saucedemo.com/.
2. Enter username as standard_user and password as secret_sauce .
3. Click the Login button and log in to items page.
4. Add the Sauce Labs Backpack to the cart.
5. Click the Login button and log in to items page.
6. Add the Sauce Labs Backpack to the cart.
7. Open the shopping cart.
8. Enter Proceed to checkout.
9. Enter first name empty, last name as User and Postel code as 12345 customer information.
10. Continue to the checkout overview.

### Expected Result
System need to give validation massage as first name is required, and stay in checkout page


### Actual Result
Not executed yet.

### Status
Not Run

### Evidence
Not collected yet.

---

## TC-CHK-003: Verify Checkout with an Empty Postal Code

**Test Type:** Negative  
**Priority:** High  
**Module:** Checkout

### Preconditions
- SauceDemo website is accessible.
- A valid user account is available.
- The user is logged out.
- The shopping cart is initially empty.

### Test Data
- Username: `standard_user`
- Password: `secret_sauce`
- Product: `Sauce Labs Backpack`
- First Name: `Test`
- Last Name: `User`
- Postal Code: Empty

### Test Steps
1. Open https://www.saucedemo.com/.
2. Enter username as standard_user and password as secret_sauce .
3. Click the Login button and log in to items page.
4. Add the Sauce Labs Backpack to the cart.
5. Click the Login button and log in to items page.
6. Add the Sauce Labs Backpack to the cart.
7. Open the shopping cart.
8. Enter Proceed to checkout.
9. Enter first name Test, last name as User and Postel code empty in customer information.
10. Continue to the checkout overview.

### Expected Result
System need to give validation massage as postel code is required, and stay in checkout page

### Actual Result
Not executed yet.

### Status
Not Run

### Evidence
Not collected yet.


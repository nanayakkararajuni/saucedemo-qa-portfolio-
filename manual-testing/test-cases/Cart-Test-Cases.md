# SauceDemo — Shopping cart Manual Test Cases

## Test Information
- **Application:** SauceDemo
- **Module:** Shopping Cart
- **Testing Type:** Manual Functional Testing
- **Execution Status:** Not Started

---

### TC-CART-001: Verify adding a product to the cart

**Test Type:** Positive  
**Priority:** High  
**Module:** shopping cart

### Preconditions
- SauceDemo website is accessible.
- A valid user account is available.
- The user is logged out.
- The user is on the Products page
- The shopping cart is empty

### Test Data
- Username: standard_user
- Password: secret_sauce
- Product: Sauce Labs Backpack
- Quantity: 1

### Test Steps
1. Open https://www.saucedemo.com/
2. Enter standard_user in the Username field.
3. Enter secret_sauce in the Password field.
4. Click the Login button.
5. Verify that the user is redirected to the Products page.
6. Observe the product listing.
7. Locate the Sauce Labs Backpack product.
8. Click the Add to cart button for that product
9. Verify that the shopping cart badge displays 1.
10. Click the shopping cart icon.
11. Verify that Sauce Labs Backpack appears in the shopping cart with a quantity of 1.


### Expected Result
The system should successfully add Sauce Labs Backpack to the shopping cart. The shopping cart badge should display 1, and the selected product should appear on the Cart page with the correct product name and quantity.

### Actual Result
Not executed yet.

### Status
Not Run

### Evidence
Not collected yet.

---


### TC-CART-002: Verify removing a product from the cart

**Test Type:** Positive  
**Priority:** High  
**Module:** shopping cart

### Preconditions
- SauceDemo website is accessible.
- A valid user account is available.
- The user is logged out.
- The shopping cart is initially empty.

### Test Data
- Username: standard_user
- Password: secret_sauce
- Product: Sauce Labs Backpack
- Quantity: 1

### Test Steps
1.Verify that the user is redirected to the Products page.
2.Locate the Sauce Labs Backpack product.
3.Click the Add to cart button for that product.
4.Verify that the shopping cart badge displays 1.
5.Click the shopping cart icon to open the Cart page.
6.Verify that Sauce Labs Backpack is displayed in the cart.
7.Click the Remove button for Sauce Labs Backpack.
8.Verify that the product is removed from the cart.
9.Verify that the shopping cart badge no longer displays an item count.

### Expected Result
The system should successfully remove Sauce Labs Backpack from the shopping cart. The removed product should no longer appear on the Cart page, and the shopping cart badge should disappear because the cart is empty

### Actual Result
Not executed yet.

### Status
Not Run

### Evidence
Not collected yet.

---



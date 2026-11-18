
# SauceDemo — Products Manual Test Cases

## Test Information
- **Application:** SauceDemo
- **Module:** Products
- **Testing Type:** Manual Functional Testing
- **Execution Status:** Not Started

---

### TC-PROD-001: Verify Products Are Displayed After Successful Login

**Test Type:** Positive  
**Priority:** High  
**Module:** Product Listing

### Preconditions
- SauceDemo website is accessible.
- A valid user account is available.
- The user is logged out.

### Test Data
- Username: standard_user
- Password: secret_sauce

### Test Steps
1. Open https://www.saucedemo.com/
2. Enter standard_user in the Username field.
3. Enter secret_sauce in the Password field.
4. Click the Login button.
5. Verify that the user is redirected to the Products page.
6. Observe the product listing.
7. Check whether each displayed product has a name, description, price, image, and Add to cart button.

### Expected Result
The system should successfully log in and redirect the user to the Products page. The available products should be displayed with their names, descriptions, prices, images, and Add to cart buttons.

### Actual Result
The system  successfully log in and redirect the user to the Products page. The available products displayed with their names, descriptions, prices, images, and Add to cart buttons.

### Status
Run

### Evidence
[View Screenshot](../evidence/TC-PROD-001.png)

---

### TC-PROD-002: Verify Product Sorting by Price (Low to High)

**Test Type:** Positive  
**Priority:** High  
**Module:** Product Listing

### Preconditions
- The user has successfully logged in and is on the Products page.

### Test Data
- Sorting option: Price (low to high).

### Test Steps
1. Locate the product sorting dropdown at the top-right of the Products page.
2. Click the sorting dropdown.
3. Select Price (low to high).
4. Observe the prices of the displayed products.
5. Verify that the products are arranged in ascending order of price, from lowest to highest.

### Expected Result
The system should display the products in ascending order of price (lowest to highest) without missing or duplicating products.

### Actual Result
system display the products in ascending order of price (lowest to highest) without missing or duplicating products.

### Status
 Run

### Evidence
[View Screenshot](../evidence/TC-PROD-002.png)

---

### TC-PROD-003: Verify Product Sorting by Price (High to Low)

**Test Type:** Positive  
**Priority:** High  
**Module:** Product Listing

### Preconditions
- The user has successfully logged in and is on the Products page.

### Test Data
- Sorting option: Price (high to low).

### Test Steps
1. Locate the product sorting dropdown at the top-right of the Products page.
2. Click the sorting dropdown.
3. Select Price (high to low).
4. Observe the prices of the displayed products.
5. Verify that the products are arranged in descending order of price, from highest to lowest.

### Expected Result
The system should display the products in descending order of price (highest to lowest) without missing or duplicating products.

### Actual Result
system display the products in descending order of price (highest to lowest) without missing or duplicating products.

### Status
Run

### Evidence
[View Screenshot](../evidence/TC-PROD-003.png)

---

### TC-PROD-004: Verify Product Details Open Correctly

**Test Type:** Positive  
**Priority:** High  
**Module:** Product Listing

### Preconditions
- The user has successfully logged in and is on the Products page.

### Test Data
- Product: Sauce Labs Backpack

### Test Steps
1. Locate the Sauce Labs Backpack product on the Products page.
2. Click the product name.
3. Verify that the product details page opens.
4. Check whether the product name, description, price, and image are displayed correctly.

### Expected Result
The system should open the selected product's details page and correctly display its name, description, price, and image.

### Actual Result
The system  open the selected product's details page and correctly display its name, description, price, and image.

### Status
 Run

### Evidence
[View Screenshot](../evidence/TC-PROD-004.png)
---

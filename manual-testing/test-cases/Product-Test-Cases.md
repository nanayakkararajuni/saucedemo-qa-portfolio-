
# SauceDemo — Products Manual Test Cases

## Test Information
- Application: SauceDemo
- Module: Products 
- Testing Type: Manual Functional Testing
- Execution Status: Not Started

---

###TC-PROD-001: Verify Products Are Displayed After Successful Login

**Test Type:** Positive
**Priority:** High 
**Module:** Product Listing

### Preconditions
- SauceDemo website is accessible.
- valid user account is available.
- The user is logged out.

### Test Data
- Username       - standard_user
- product        - secret_sauce

### Test Steps
1. Open https://www.saucedemo.com/
2. Enter standard_user in the Username field.
3. Enter secret_sauce in the Password field.
4. Click the Login button.
5. Verify that the user is redirected to the Products page.
6. Observe the product listing.
7. Check whether each displayed product has a name, description, price, image, and Add to cart button.

### Expected Result
[Describe the correct system behavior.]

### Actual Result
The system should successfully log in and redirect the user to the Products page. The available products should be displayed with their names, descriptions, prices, images, and Add to cart buttons.

### Status
Not Run

### Evidence
Not collected yet.


###TC-PROD-002: Verify Product Sorting by Price (Low to High)

**Test Type:** Positive
**Priority:** High 
**Module:** Product Listing

### Preconditions
-User has successfully logged in and is on the Products page.

### Test Data
- Sorting option — Price (low to high).

### Test Steps
1. Open https://www.saucedemo.com/
2. Enter standard_user in the Username field.
3. Enter secret_sauce in the Password field.
4. Click the Login button.
5. Verify that the user is redirected to the Products page.
6. Locate the product sorting dropdown at the top-right of the Products page.
7. Click the sorting dropdown.
8. Select Price (low to high).
9. Observe the prices of the displayed products.
10. Verify that the products are arranged in ascending order of price, from lowest to highest.

### Expected Result
The system should display the products in ascending order of price (lowest to highest) without missing or duplicating products.

### Actual Result


### Status
Not Run

### Evidence
Not collected yet.

###TC-PROD-003: Verify Product Sorting by Price (Low to High)

**Test Type:** Positive
**Priority:** High 
**Module:** Product Listing

### Preconditions
-User has successfully logged in and is on the Products page.

### Test Data
- Sorting option — Price (low to high).

### Test Steps
1. Open https://www.saucedemo.com/
2. Enter standard_user in the Username field.
3. Enter secret_sauce in the Password field.
4. Click the Login button.
5. Verify that the user is redirected to the Products page.
6. Locate the product sorting dropdown at the top-right of the Products page.
7. Click the sorting dropdown.
8. Select Price (low to high).
9. Observe the prices of the displayed products.
10. Verify that the products are arranged in ascending order of price, from lowest to highest.

### Expected Result
The system should display the products in ascending order of price (lowest to highest) without missing or duplicating products.

### Actual Result


### Status
Not Run

### Evidence
Not collected yet.



###TC-PROD-004: Verify product details open correctly

**Test Type:** Positive
**Priority:** High 
**Module:** Product Listing

### Preconditions
-User has successfully logged in and is on the Products page.

### Test Data


### Test Steps
1. Open https://www.saucedemo.com/
2. Enter standard_user in the Username field.
3. Enter secret_sauce in the Password field.
4. Click the Login button.
5. Verify that the user is redirected to the Products page.
6.  Click the product name
7.  Verify that the products details are open and shown correctly.


### Expected Result
The system should open display the product details
### Actual Result

### Status
 Run

### Evidence
Not collected yet.




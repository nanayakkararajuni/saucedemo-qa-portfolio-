
# SauceDemo — Products Manual Test Cases

## Test Information
- Application: SauceDemo
- Module: Products 
- Testing Type: Manual Functional Testing
- Execution Status: Not Started

---

##TC-PROD-001: Verify Products Are Displayed After Successful Login

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


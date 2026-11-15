

# SauceDemo — Manual Login Test Cases

## Test Information

- Application: SauceDemo
- Module: Login
- Testing Type: Manual Functional Testing
- Execution Status: Not Started

---

## TC-LOGIN-001: Verify Login With Valid Credentials

**Test Type:** Positive Testing  
**Priority:** High  
**Module:** Login

### Preconditions
- SauceDemo login page is accessible.
- A valid test account is available.
- User is logged out.

### Test Data
- Username: `standard_user`
- Password: `secret_sauce`

### Test Steps
1. Open https://www.saucedemo.com/
2. Enter `standard_user` in the Username field.
3. Enter `secret_sauce` in the Password field.
4. Click the Login button.

### Expected Result
The user should be successfully logged in and redirected
to the Products page.

### Actual Result
Successfully log in and redirect to the landing page.

### Status
 Run

### Evidence

[View Screenshot](../evidence/TC-LOGIN-001.png)



## TC-LOGIN-002:Verify login with incorrect password

**Test Type:** Negative  
**Priority:** High  
**Module:** Login

### Preconditions
- SauceDemo login page is accessible.
- A valid test account is available.
- User is logged out.

### Test Data
- Username: `standard_user`
- Password: `incorrect123`

### Test Steps
1. Open https://www.saucedemo.com/
2. Enter  `standard_user` in login username feild
3. Enter `incorrect123` in login password feild
4. Click the login buttom

### Expected Result
The system should reject the login attempt, display an appropriate error message indicating invalid credentials, and keep the user on the login page.

### Actual Result
display Username and password do not match any user in this service error massage and keep the user on the login page.

### Status
 Run

### Evidence

[View Screenshot](../evidence/TC-LOGIN-002.png)



## TC-LOGIN-003:Verify login with empty username

**Test Type:** Negative  
**Priority:** High  
**Module:** Login

### Preconditions
- SauceDemo login page is accessible.
- A valid test account is available.
- User is logged out.

### Test Data
- Username:empty
- Password: `secret_sauce`

### Test Steps
1. Open https://www.saucedemo.com/
2. set empty in login username feild
3. Enter `secret_sauce` in login password feild
4. Click the login buttom

### Expected Result
The system should reject the login attempt, display an appropriate error message indicating username is required , and keep the user on the login page.

### Actual Result
system reject the login, display username is required,  and keep the user on the login page.

### Status
 Run

### Evidence
[View Screenshot](../evidence/TC-LOGIN-003.png)


## TC-LOGIN-004:Verify login with empty password

**Test Type:** Negative  
**Priority:** High  
**Module:** Login

### Preconditions
- SauceDemo login page is accessible.
- A valid test account is available.
- User is logged out.

### Test Data
- Username: `standard_user`
- Password: empty

### Test Steps
1. Open https://www.saucedemo.com/
2. Enter  `standard_user` in login username feild
3. set empty in login password feild
4. Click the login buttom

### Expected Result
The system should reject the login attempt, display an appropriate error message indicating Password is required , and keep the user on the login page.

### Actual Result
system reject the login, display password is required,  and keep the user on the login page.

### Status
Run

### Evidence
[View Screenshot](../evidence/TC-LOGIN-004.png)


## TC-LOGIN-005:Verify login with locked-out user

**Test Type:** Negative  
**Priority:** High  
**Module:** Login

### Preconditions
- SauceDemo login page is accessible.
- locked_out_user test account is available.
- User is logged out.

### Test Data
- Username: `locked_out_user`
- Password: `secret_sauce`

### Test Steps
1. Open https://www.saucedemo.com/
2. Enter  `locked_out_user` in login username feild
3. Enter `secret_sauce` in login password feild
4. Click the login buttom

### Expected Result
The system should prevent the user from logging in and display an error message indicating that the account is locked out.

### Actual Result
system reject the login, display sorry user has been locked out ,  and keep the user on the login page.

### Status
 Run

### Evidence
[View Screenshot](../evidence/TC-LOGIN-005.png)


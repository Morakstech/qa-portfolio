# Login Functionality - Manual Test Cases

## Test Case 1
**Test Case ID:** TC_LOGIN_001  
**Title:** Verify login with valid credentials  
**Preconditions:** User is registered and on the login page  

**Steps:**
1. Enter a valid username
2. Enter a valid password
3. Click the Login button

**Expected Result:**
- User is successfully logged in
- User is redirected to the dashboard

---

## Test Case 2
**Test Case ID:** TC_LOGIN_002  
**Title:** Verify login with invalid password  
**Preconditions:** User is registered and on the login page  

**Steps:**
1. Enter a valid username
2. Enter an invalid password
3. Click the Login button

**Expected Result:**
- Login fails
- Error message is displayed

---

## Test Case 3
**Test Case ID:** TC_LOGIN_003  
**Title:** Verify login with empty fields  

**Steps:**
1. Leave username field empty
2. Leave password field empty
3. Click the Login button

**Expected Result:**
- Login is not allowed
- Validation message is displayed

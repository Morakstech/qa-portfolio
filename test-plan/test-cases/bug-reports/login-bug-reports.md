# Login Module - Bug Reports

## Bug 1
**Bug ID:** BUG_LOGIN_001  
**Title:** Login button allows submission with empty fields  

**Environment:** Chrome on Windows  

**Steps to Reproduce:**
1. Navigate to the login page
2. Leave username and password fields empty
3. Click the Login button

**Expected Result:**
- Login should be blocked
- Validation message should be displayed

**Actual Result:**
- Login request is submitted without validation

**Severity:** Major  
**Priority:** High  

---

## Bug 2
**Bug ID:** BUG_LOGIN_002  
**Title:** Incorrect error message displayed for invalid password  

**Environment:** Chrome on Windows  

**Steps to Reproduce:**
1. Enter a valid username
2. Enter an invalid password
3. Click the Login button

**Expected Result:**
- Clear error message indicating invalid credentials

**Actual Result:**
- Generic system error message is displayed

**Severity:** Minor  
**Priority:** Medium

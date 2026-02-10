# SQL Validation for Login Functionality

## Purpose
These SQL queries are used to validate backend data related to user login functionality and authentication behavior.

---

## Validation Scenario 1
**Objective:** Verify user record exists in the database  

**Query:**
SELECT * 
FROM users
WHERE username = 'validUser';

**Expected Result:**
- User record exists
- Username matches the input provided during login

---

## Validation Scenario 2
**Objective:** Verify failed login attempts are recorded  

**Query:**
SELECT failed_login_attempts
FROM users
WHERE username = 'validUser';

**Expected Result:**
- Failed login count increases after an invalid login attempt

---

## Validation Scenario 3
**Objective:** Verify last login timestamp is updated after successful login  

**Query:**
SELECT last_login
FROM users
WHERE username = 'validUser';

**Expected Result:**
- last_login timestamp reflects the most recent successful login

---

## Validation Scenario 4
**Objective:** Ensure inactive users cannot log in  

**Query:**
SELECT status
FROM users
WHERE username = 'inactiveUser';

**Expected Result:**
- User status is inactive
- Login attempt should be rejected

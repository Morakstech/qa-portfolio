# Login API - Test Cases

## API Overview
Endpoint used to authenticate users and return login status.

**Endpoint:** POST /api/login  
**Request Format:** JSON  
**Response Format:** JSON  

---

## Test Case 1
**Test Case ID:** API_LOGIN_001  
**Title:** Verify login API with valid credentials  

**Request Body:**
{
  "username": "validUser",
  "password": "validPassword"
}

**Expected Result:**
- Status code 200
- Successful login response returned

---

## Test Case 2
**Test Case ID:** API_LOGIN_002  
**Title:** Verify login API with invalid password  

**Request Body:**
{
  "username": "validUser",
  "password": "invalidPassword"
}

**Expected Result:**
- Status code 401
- Error message indicating invalid credentials

---

## Test Case 3
**Test Case ID:** API_LOGIN_003  
**Title:** Verify login API with missing fields  

**Request Body:**
{
  "username": "",
  "password": ""
}

**Expected Result:**
- Status code 400
- Validation error message returned

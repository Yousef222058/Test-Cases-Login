# Test Cases – Login Page

## Task 1: Login Page Test Cases

| Test Case ID | Description   | Steps | Expected Result | Status |
|--------------|--------------|-------|-----------------|--------|
| TC_01 | Valid login | 1. Open login page <br> 2. Enter valid username <br> 3. Enter valid password <br> 4. Click login | User successfully logged in and redirected to dashboard | Not Executed |
| TC_02 | Invalid login | 1. Open login page <br> 2. Enter invalid username/password <br> 3. Click login | Error message displayed: "Invalid credentials" | Not Executed |
| TC_03 | Empty fields | 1. Open login page <br> 2. Leave username and password empty <br> 3. Click login | Validation message displayed: "Fields cannot be empty" | Not Executed |
| TC_04 | SQL Injection | 1. Open login page <br> 2. Enter ' OR '1'='1 in username field <br> 3. Enter any password <br> 4. Click login | Login should fail; system must prevent SQL injection and show error | Not Executed |

---

## Task 2: Boundary Value Testing – Password Length (8–12 characters)

| Test Case ID | Input (Password Length) | Description | Expected Result |
|--------------|------------------------|------------|-----------------|
| TC_BV_01 | 7 characters | Below minimum boundary | Rejected; error message displayed |
| TC_BV_02 | 8 characters | Minimum boundary | Accepted |
| TC_BV_03 | 12 characters | Maximum boundary | Accepted |
| TC_BV_04 | 13 characters | Above maximum boundary | Rejected; error message displayed |

---

## Notes
- All test cases are written for a standard login system.
- Status is set to **Not Executed**.
- Covers validation, functionality, and basic security testing.

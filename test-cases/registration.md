# Registration — Test Cases

## Test Environment
- **Application:** PetStore
- **Environment:** Production
- **Browser:** Chrome (latest)
- **Operating System:** Windows 11

---

## PS-TC-001 — User ID field should not accept an already registered User ID

**Preconditions:**  
An existing User ID is already registered in the system.

Example test data:
- User ID: `existingUser`

**Priority:** High  
**Status:** Passed

### Steps to Perform
1. Open the main page.
2. Click the [Sign In] link.
3. Click the [Register Now!] link.
4. Enter an already registered User ID in the User ID field.
5. Fill in all other required fields with valid data.
6. Click the [Save Account Information] button.

### Expected Result
An error message is displayed indicating that the User ID must be unique.

---

## PS-TC-002 — User ID field should not accept special characters

**Preconditions:** None

Example test data:
- User ID: `user@123`

**Priority:** High  
**Status:** Passed

### Steps to Perform
1. Open the main page.
2. Click the [Sign In] link.
3. Click the [Register Now!] link.
4. Enter a value containing a special character in the User ID field.
5. Fill in all other required fields with valid data.
6. Click the [Save Account Information] button.

### Expected Result
An error message is displayed indicating that the User ID accepts only alphanumeric characters.

---

## PS-TC-003 — User ID field should accept letters and numbers

**Preconditions:** None

Example test data:
- User ID: `user123`
- Email: `user123@test.com`
- Password: `Qwerty1!`

**Priority:** High  
**Status:** Passed

### Steps to Perform
1. Open the main page.
2. Click the [Sign In] link.
3. Click the [Register Now!] link.
4. Enter a value containing letters and numbers in the User ID field.
5. Fill in all other required fields with valid data.
6. Click the [Save Account Information] button.

### Expected Result
The user is registered successfully and redirected to the main page.

---

## PS-TC-004 — New Password field should not accept a value without a number

**Preconditions:** None

Example test data:
- Password: `Qwerty`

**Priority:** High  
**Status:** Passed

### Steps to Perform
1. Open the main page.
2. Click the [Sign In] link.
3. Click the [Register Now!] link.
4. Enter `Qwerty` in the New Password field.
5. Fill in all other required fields with valid data.
6. Click the [Save Account Information] button.

### Expected Result
An error message is displayed indicating that the password must contain at least one number.

---

## PS-TC-005 — New Password field should not accept a value without a special character

**Preconditions:** None

Example test data:
- Password: `Petstore1`

**Priority:** High  
**Status:** Passed

### Steps to Perform
1. Open the main page.
2. Click the [Sign In] link.
3. Click the [Register Now!] link.
4. Enter `Petstore1` in the New Password field.
5. Fill in all other required fields with valid data.
6. Click the [Save Account Information] button.

### Expected Result
An error message is displayed indicating that the password must contain at least one special character.

---

## PS-TC-006 — Repeat Password field should not accept a value different from the New Password field

**Preconditions:** None

Example test data:
- New Password: `Petstore1@`
- Repeat Password: `Petstore11@`

**Priority:** High  
**Status:** Passed

### Steps to Perform
1. Open the main page.
2. Click the [Sign In] link.
3. Click the [Register Now!] link.
4. Enter `Petstore1@` in the New Password field.
5. Enter `Petstore11@` in the Repeat Password field.
6. Fill in all other required fields with valid data.
7. Click the [Save Account Information] button.

### Expected Result
An error message is displayed indicating that the Repeat Password value must match the New Password value.

---

## PS-TC-007 — Email field should not accept an already registered email address

**Preconditions:**  
The email address is already registered in the system.

Example test data:
- Email: `petboy@store.com`

**Priority:** High  
**Status:** Passed

### Steps to Perform
1. Open the main page.
2. Click the [Sign In] link.
3. Click the [Register Now!] link.
4. Enter an already registered email address in the Email field.
5. Fill in all other required fields with valid data.
6. Click the [Save Account Information] button.

### Expected Result
An error message is displayed indicating that the email address is already registered.

---

## PS-TC-008 — Email field should not accept an invalid email format

**Preconditions:** None

Example test data:
- Email: `petboystore,com`

**Priority:** High  
**Status:** Passed

### Steps to Perform
1. Open the main page.
2. Click the [Sign In] link.
3. Click the [Register Now!] link.
4. Enter an invalid email format in the Email field.
5. Fill in all other required fields with valid data.
6. Click the [Save Account Information] button.

### Expected Result
An error message is displayed indicating that the email format is invalid.

### Related Bug
- [PS-0002 — The system accepts an invalid email address format in Account Information](../bug-reports/PS-0002-invalid-email-format.md)

---

## PS-TC-009 — User should be able to register using only required fields

**Preconditions:** None

Example test data:
- User ID: `userQA`
- Email: `test@qa.team`
- Password: `12345Qwert!`

**Priority:** High  
**Status:** Passed

### Steps to Perform
1. Open the main page.
2. Click the [Sign In] link.
3. Click the [Register Now!] link.
4. Fill in only the required fields: User ID, Email, New Password, and Repeat Password.
5. Click the [Save Account Information] button.

### Expected Result
The user is registered successfully, redirected to the main page, and the user name is visible in the header.

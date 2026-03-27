# Login — Test Cases

## Test Environment
- **Application:** PetStore
- **Environment:** Production
- **Browser:** Chrome (latest)
- **Operating System:** Windows 11

---

## PS-TC-010 — User should be able to log in with valid credentials

**Preconditions:**  
User account is already registered.

Example test data:
- Username: `userQA`
- Password: `12345Qwert!`

**Priority:** High  
**Status:** Passed

### Steps to Perform
1. Open the main page.
2. Click the [Sign In] link.
3. Enter a valid Username.
4. Enter a valid Password.
5. Click the [Login] button.

### Expected Result
The user is successfully logged in and redirected to the main page. The user name is displayed in the header.

---

## PS-TC-011 — Login should not be possible with empty Username and Password fields

**Preconditions:** None  

**Priority:** High  
**Status:** Failed

### Steps to Perform
1. Open the main page.
2. Click the [Sign In] link.
3. Leave the Username field empty.
4. Leave the Password field empty.
5. Click the [Login] button.

### Expected Result
Validation messages are displayed indicating that both Username and Password fields are required.

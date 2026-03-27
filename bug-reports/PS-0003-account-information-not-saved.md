## PS-0003 — Updated account information is not saved after clicking [Save Account Information]

**Module:** Account Information  
**Severity:** Critical  
**Priority:** High  
**Environment:** PetStore web application, Desktop (Chrome)

### Preconditions
User is logged in and is on the Account Information page.

### Steps to Reproduce
1. Open the Account Information page.
2. Modify any user data (e.g. first name, last name, email).
3. Click the [Save Account Information] button.
4. Refresh the page or reopen the Account Information section.

### Expected Result
The updated user data should be saved and displayed correctly after refreshing the page.

### Actual Result
The changes are not saved. The previously stored data is still displayed.

### Attachment
[PS-0003.png](../attachments/bug-screenshots/PS-0003.png)

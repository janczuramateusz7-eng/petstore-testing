## PS-0002 — The system accepts an invalid email address format in Account Information

**Module:** Account Information  
**Severity:** Major  
**Priority:** High  
**Environment:** PetStore web application, Desktop (Chrome)

### Preconditions
User is logged in and is on the Account Information page.

### Steps to Reproduce
1. Open the Account Information page.
2. Enter an invalid email address (e.g. `test@`, `test.com`, `@mail.com`) in the Email field.
3. Click the [Save Account Information] button.

### Expected Result
The system should display a validation error message and prevent saving incorrect email format.

### Actual Result
The system accepts the invalid email address and saves the data without any validation error.

### Attachment
[[PS-0002.png](../attachments/bug-screenshots/PS-0002.png)](https://drive.google.com/file/d/1y07th4Ncml_ojUkHJjjLsCsEocBYLnxO/view)

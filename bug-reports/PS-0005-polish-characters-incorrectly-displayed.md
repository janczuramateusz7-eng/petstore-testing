## PS-0005 — Polish characters are displayed incorrectly in User Information

**Module:** User Information  
**Severity:** Major  
**Priority:** Medium  
**Environment:** PetStore web application, Desktop (Chrome)

### Preconditions
User is logged in and is on the User Information page.

### Steps to Reproduce
1. Open the User Information page.
2. Enter text containing Polish characters (e.g. `ą, ę, ł, ó, ś, ć, ż, ź`) in any text field.
3. Save the data (if applicable) or observe the displayed values.

### Expected Result
Polish characters should be displayed correctly according to UTF-8 encoding.

### Actual Result
Polish characters are displayed incorrectly (e.g. as unreadable or corrupted symbols).

### Attachment
[PS-0005.png](../attachments/bug-screenshots/PS-0005.png)

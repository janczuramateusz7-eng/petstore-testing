
## PS-0014 — No warning message is displayed when adding more items than available in stock

**Module:** Cart / Validation  
**Severity:** Critical  
**Priority:** High  
**Environment:** Windows 11, Chrome (latest), PetStore Demo

### Preconditions
User is logged in.

### Steps to Reproduce
1. Open the website.
2. Log in.
3. Attempt to add a large quantity of a product exceeding stock.

### Expected Result
A warning message about limited stock availability is displayed.

### Actual Result
The system allows adding large quantities without any warning.

### Attachment
![PS-0014](../attachments/bug-screenshots/PS-0014.png)

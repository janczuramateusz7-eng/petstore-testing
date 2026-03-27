# Search — Test Cases

## Test Environment
- **Application:** PetStore
- **Environment:** Production
- **Browser:** Chrome (latest)
- **Operating System:** Windows 11

---

## PS-TC-015 — Search should allow users to find products by category

**Preconditions:** None

Example test data:
- Category: `Reptiles`

**Priority:** Medium  
**Status:** Failed

### Steps to Perform
1. Open the main page.
2. Enter `Reptiles` in the Search field.
3. Click the [Search] button.

### Expected Result
Products related to the `Reptiles` category are displayed in the search results.

---

## PS-TC-016 — Search should allow users to find products by product name

**Preconditions:** None

Example test data:
- Product name: `Bulldog`

**Priority:** Medium  
**Status:** Passed

### Steps to Perform
1. Open the main page.
2. Enter `Bulldog` in the Search field.
3. Click the [Search] button.

### Expected Result
Products related to `Bulldog` are displayed in the search results.

---

## PS-TC-017 — Search should allow users to find products by Product ID

**Preconditions:** None

Example test data:
- Product ID: `K9-BD-01`

**Priority:** Medium  
**Status:** Failed

### Steps to Perform
1. Open the main page.
2. Enter `K9-BD-01` in the Search field.
3. Click the [Search] button.

### Expected Result
The product with Product ID `K9-BD-01` is displayed in the search results.

---

## PS-TC-018 — Search should not display duplicate results for a two-word query

**Preconditions:** None

Example test data:
- Search query: `Golden Retriever`

**Priority:** Medium  
**Status:** Failed

### Steps to Perform
1. Open the main page.
2. Enter `Golden Retriever` in the Search field.
3. Click the [Search] button.

### Expected Result
Each search result is displayed only once.

### Related Bug
- [PS-0008 — Duplicate results are displayed when searching using a two-word query](../bug-reports/PS-0008-duplicate-search-results.md)

---

## PS-TC-019 — Search should display only one validation message when submitted with an empty field

**Preconditions:** None

**Priority:** Medium  
**Status:** Failed

### Steps to Perform
1. Open the main page.
2. Leave the Search field empty.
3. Click the [Search] button.

### Expected Result
Only one validation message is displayed informing the user that the Search field is required.

### Related Bug
- [PS-0001 — Duplicate validation messages are displayed after clicking the empty Search field](../bug-reports/PS-0001-duplicate-validation-message.md)

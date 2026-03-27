# Cart — Test Cases

## Test Environment
- **Application:** PetStore
- **Environment:** Production
- **Browser:** Chrome (latest)
- **Operating System:** Windows 11

---

## PS-TC-012 — User should be able to add a product to the cart from the Product Details Page

**Preconditions:** None

Example test data:
- Category: `Fish`
- Product name: `Goldfish`
- Product ID: `FI-FW-02`

**Priority:** Medium  
**Status:** Passed

### Steps to Perform
1. Open the main page.
2. Click the `Fish` category.
3. Open the product with Product ID `FI-FW-02`.
4. Click the [Add to Cart] button.

### Expected Result
The selected product is added to the cart successfully and is visible in the Shopping Cart.

---

## PS-TC-013 — User should be able to add a product to the cart from search results

**Preconditions:** None

Example test data:
- Search query: `Goldfish`
- Product name: `Goldfish`
- Product ID: `FI-FW-02`

**Priority:** Medium  
**Status:** Passed

### Steps to Perform
1. Open the main page.
2. Enter `Goldfish` in the Search field.
3. Click the [Search] button.
4. Open the product with Product ID `FI-FW-02`.
5. Click the [Add to Cart] button.

### Expected Result
The selected product is added to the cart successfully and is visible in the Shopping Cart.

---

## PS-TC-014 — User should be able to update product quantity in the cart

**Preconditions:**  
At least one product is already added to the cart.

Example test data:
- Product: `Goldfish`
- Updated quantity: `2`

**Priority:** High  
**Status:** Failed

### Steps to Perform
1. Open the main page.
2. Add any product to the cart.
3. Open the Shopping Cart page.
4. Change the quantity of the product to `2`.
5. Click the [Update Cart] button.

### Expected Result
The cart is updated successfully. The new quantity and total price are displayed correctly.

### Related Bug
- [PS-0004 — Shopping cart is not updated after clicking [Update Cart]](../bug-reports/PS-0004-cart-not-updated.md)

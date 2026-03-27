# Cart Requirements — PetStore

## Overview
This document describes functional and validation requirements for the Cart module in the PetStore application.

---

## General Requirements

### CART-001 — Cart Access
Users should be able to access the Cart from any page in the application.

---

### CART-002 — Cart Tooltip
The Cart icon should display a tooltip labeled "Cart".

---

### CART-003 — Cart Table Structure
The cart should display added products in a table with the following columns:
- Item ID
- Product ID
- Name
- Description
- In Stock
- Quantity
- List Price
- Total Cost

---

### CART-004 — Cart Summary Row
The last row of the cart table should contain:
- Sub Total
- [Update Cart] button

---

### CART-005 — Empty Cart
If no products are added, the cart should display the message:
"Your cart is empty."

---

### CART-006 — Checkout Button Visibility
The [Proceed to Checkout] button should be visible when at least one product is added to the cart.

---

### CART-007 — Checkout Redirection
- Logged-in users → Checkout page  
- Not logged-in users → Login page  

---

### CART-008 — Return Navigation
Users should be able to leave the Cart page using the [Return to Main Menu] link.

---

## Adding and Removing Products

### CART-009 — Add to Cart
Users should be able to add products to the cart:
- from Product Details Page (PDP)
- from product list

---

### CART-010 — Cart Badge
After adding a product, the Cart icon should display a badge with the number of items in the cart.

---

### CART-011 — Clickable Links
The following fields in the cart should be clickable:
- Item ID
- Product Name

---

### CART-012 — Quantity Input
The Quantity field:
- should accept only numeric values

---

### CART-013 — Quantity Limit
Users should not be able to add more than 5 units of the same product per order.

---

### CART-014 — Quantity Validation Trigger
Validation should be triggered:
- after pressing Enter
- after clicking the [Update Cart] button

---

### CART-015 — Quantity Limit Message
If quantity exceeds 5 items, the system should display:
"We are sorry, but you can’t buy more than 5 items of the product."

---

### CART-016 — Stock Limit Message
If quantity exceeds available stock, the system should display:
"We are sorry, but we have only N items of this product for now. Would you like to subscribe to notifications when this product will be available?"

---

### CART-017 — Remove Product
Users should be able to remove a product using the [Remove] button.

---

### CART-018 — Remove by Quantity = 0
If the quantity is set to 0 and the cart is updated, the product should be removed.

---

### CART-019 — Out-of-Stock Restriction
Users should not be able to add products that are out of stock.

---

## Cross-Session Behavior

### CART-020 — Cart Persistence Across Sessions
If a logged-in user adds a product to the cart, it should be visible across all sessions.

---

### CART-021 — Cart Reset on Logout
After logout, the cart should be cleared for the current session.

---

### CART-022 — Cross-Session Removal
If a product is removed from the cart, it should be removed across all sessions.

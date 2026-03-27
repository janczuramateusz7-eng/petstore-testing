# Cart Checklist — PetStore

## References
- PetStore Cart requirements
- PetStore application

## Test Run Information
- **Module:** Cart
- **Run date:** `29/07/2025`
- **Environment:** Production
- **Browser:** Chrome (latest)
- **Operating System:** Windows 11

## Preconditions
- User can open the PetStore application.
- Products are available in the catalog.
- Both logged-in and not logged-in scenarios can be tested.

---

## Checklist Execution Results

| # | Checklist Item | Priority | Result | Bug ID | Comment |
|---|---|---|---|---|---|
| 1 | User can access the Cart from any page in the application. | High | Passed |  |  |
| 2 | The Cart icon displays the `Cart` tooltip. | Critical | Failed | PS-001 |  |
| 3 | The cart table displays the `Item ID` column. | High | Passed |  |  |
| 4 | The cart table displays the `Product ID` column. | High | Passed |  |  |
| 5 | The cart table displays the `Name` column. | High | Failed | PS-002 |  |
| 6 | The cart table displays the `Description` column. | High | Passed |  |  |
| 7 | The cart table displays the `In Stock?` column. | High | Passed |  |  |
| 8 | The cart table displays the `Quantity` column. | High | Passed |  |  |
| 9 | The cart table displays the `List Price` column. | High | Passed |  |  |
| 10 | The cart table displays the `Total Cost` column. | High | Passed |  |  |
| 11 | The last row of the cart table displays `Sub Total` and the [Update Cart] button. | High | Passed |  |  |
| 12 | An empty cart displays the message `Your cart is empty.` by default. | High | Passed |  |  |
| 13 | The [Proceed to Checkout] button is displayed when at least one product is added to the cart. | High | Passed |  |  |
| 14 | The [Proceed to Checkout] button redirects logged-in users to Checkout and not logged-in users to Login. | High | Passed |  |  |
| 15 | User can leave the Cart page using the [Return to Main Menu] link. | High | Passed |  |  |
| 16 | User can add products to the cart from the Product Details Page. | High | Passed |  |  |
| 17 | User can add products to the cart from the product list. | High | Passed |  |  |
| 18 | After adding a product, the Cart icon displays a badge with the number of added items. | High | Failed | PS-003 |  |
| 19 | The `Item ID` value in the cart is a clickable link. | High | Passed |  |  |
| 20 | The `Quantity` field in the cart accepts only numeric values. | High | Passed |  |  |
| 21 | User cannot add more than 5 units of the same product per order. | High | Failed | PS-004 |  |
| 22 | Quantity validation is triggered after entering a new quantity and pressing Enter. | High | Passed |  |  |
| 23 | Quantity validation is triggered after entering a new quantity and clicking [Update Cart]. | High | Passed |  |  |
| 24 | If quantity exceeds the allowed limit, the message `We are sorry, but you can’t buy more than 5 items of the product.` is displayed under the table. | Critical | Failed | PS-005 |  |
| 25 | If requested quantity exceeds stock, the message about limited stock availability and subscription to notifications is displayed under the table. | Critical | Failed | PS-006 |  |
| 26 | User can remove a product from the cart using the [Remove] button next to the product price. | High | Passed |  |  |
| 27 | If the quantity is changed to `0` and the cart is updated, the product is removed from the cart. | High | Passed |  |  |
| 28 | User cannot add an out-of-stock product to the cart. | High | Failed | PS-007 |  |
| 29 | For a logged-in user, added cart products are visible across other sessions. | High | Passed |  |  |
| 30 | After logout, the cart becomes empty for the current session. | High | Passed |  |  |
| 31 | If a logged-in user removes a product from the cart, the change is reflected across other sessions. | High | Passed |  |  |
| 32 | The product `Name` value in the cart is a clickable link. | High | Failed | PS-008 |  |

---

## Summary
- **Total checklist items:** 32
- **Passed:** 24
- **Failed:** 8
- **Blocked / Not Run:** 0

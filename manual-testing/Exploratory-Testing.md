# SauceDemo — Exploratory Testing Observations

## Observation 1 — Add, Remove, and Re-add a Product

**Action Performed:**

1. Logged into SauceDemo.
2. Added one product to the shopping cart.
3. Opened the Cart page.
4. Removed the selected product.
5. Returned to the Products page.
6. Added the same product again.
7. Observed the product quantity.

**Expected Behavior:**

The system should successfully add and remove the selected product. The user should be able to add the same product again after removing it.

**Observed Behavior:**

The product was successfully added to the cart, removed, and added again without any issues. The product quantity was displayed as 1, and no option was available to increase or decrease the quantity.

**Result:** As Expected

**Additional Note:** The cart interface does not provide a quantity adjustment feature. This is a feature limitation, not a confirmed defect.

---

## Observation 2 — Checkout with an Empty Shopping Cart

**Action Performed:**

1. Logged into SauceDemo.
2. Removed all products from the shopping cart.
3. Opened the empty Cart page.
4. Clicked the Checkout button.
5. Entered valid customer information.
6. Continued to the checkout overview.
7. Completed the checkout process.

**Expected Behavior:**

For a typical e-commerce application, the system should prevent order completion when the shopping cart is empty and inform the user that at least one product must be added.



**Observed Behavior:**

The system allowed checkout to proceed even though the shopping cart was empty. After entering valid customer information, the system displayed the checkout overview and allowed the user to finish the order without any products.

**Result:** Potential Defect — Requires Verification

**Possible Issue:** Empty shopping cart checkout is allowed.

---

## Observation 3 — Cart Contents After Logout and Login

**Action Performed:**

1. Logged into SauceDemo.
2. Added two different products to the shopping cart.
3. Logged out of the application.
4. Logged in again using the same account.
5. Opened the shopping cart.

**Expected Behavior:**

Cart persistence after logout should follow the application's requirements. Some e-commerce applications intentionally preserve cart items between login sessions.

**Observed Behavior:**

After logging out and logging in again, both previously selected products were still available in the shopping cart.

**Result:** Needs Requirement Verification

**Additional Note:** Cart persistence is not necessarily a defect. Further requirement verification is needed to determine whether the observed behavior is intended.

---

## Session Summary

Three behaviors were investigated:

- **Observation 1:** Add, remove, and re-add product — As Expected
- **Observation 2:** Checkout with an empty cart — Potential Defect
- **Observation 3:** Cart persistence after logout — Needs Requirement Verification

**Conclusion:**

The basic add-and-remove cart functionality behaved as expected. However, the application allowed checkout to be completed with an empty shopping cart, which may represent a business logic defect. Cart persistence after logout also requires clarification of the expected behavior.

Further investigation is recommended for the empty-cart checkout scenario before finalizing a defect report.

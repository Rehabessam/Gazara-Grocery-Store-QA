# High-Level Test Scenarios  
## Gazara Grocery Store – Website

---

## Overview
This document lists the high-level test scenarios derived directly from the
designed manual test cases for the Gazara Grocery Store website.

Each scenario is mapped to at least one test case and linked to Jira User Stories
to ensure full requirement coverage and traceability.

The project is requirement-based and does not include live execution.

---

# EPIC: User Authentication & Registration  
**Jira Epic ID:** GGS-1

### Scenario AUTH-01: Successful user registration using valid email and password
**Related Test Cases:** GGS-T1  
**Related Story:** GGS-3  
User signs up successfully when all required fields contain valid data.

---

### Scenario AUTH-02: Successful login after registration
**Related Test Cases:** GGS-T2  
**Related Story:** GGS-4  
Registered user logs in successfully using valid credentials.

---

### Scenario AUTH-03: Signup fails when First Name is missing
**Related Test Cases:** GGS-T3  
**Related Story:** GGS-3  
System prevents signup and displays validation error when First Name is empty.

---

### Scenario AUTH-04: Signup fails when Email is missing
**Related Test Cases:** GGS-T4  
**Related Story:** GGS-3  
System enforces Email as a mandatory field during signup.

---

### Scenario AUTH-05: Signup fails when Password does not meet minimum length
**Related Test Cases:** GGS-T5  
**Related Story:** GGS-3  
System validates password length and blocks submission if less than 8 characters.

---

# EPIC: Navigation & Website Structure  
**Jira Epic ID:** GGS-5

### Scenario NAV-01: User navigates to Vegetables category
**Related Test Cases:** GGS-T6  
**Related Story:** GGS-6  
User clicks Vegetables link and views all vegetable products.

---

### Scenario NAV-02: User navigates to Shop All page
**Related Test Cases:** GGS-T7  
**Related Story:** GGS-6  
User accesses Shop All page displaying products from all categories.

---

### Scenario NAV-03: User starts shopping using Shop Now CTA
**Related Test Cases:** GGS-T8  
**Related Story:** GGS-7  
Shop Now button redirects the user to Shop All page.

---

# EPIC: Shopping Cart Management  
**Jira Epic ID:** GGS-8

### Scenario CART-01: Logged-in user adds item to cart
**Related Test Cases:** GGS-T9  
**Related Story:** GGS-10  
Authenticated user successfully adds an item to the cart and receives confirmation.

---

### Scenario CART-02: User views cart from add-to-cart notification
**Related Test Cases:** GGS-T10  
**Related Story:** GGS-11  
User navigates to the cart using the side pop-up notification.

---

### Scenario CART-03: Logged-in user accesses cart directly
**Related Test Cases:** GGS-T11  
**Related Story:** GGS-9  
Authenticated user accesses the cart via navigation icon.

---

### Scenario CART-04: Non-logged-in user cannot add item to cart
**Related Test Cases:** GGS-T12  
**Related Story:** GGS-9  
System blocks unauthenticated users from adding items to cart.

---

### Scenario CART-05: Non-logged-in user cannot view cart
**Related Test Cases:** GGS-T13  
**Related Story:** GGS-9  
System prevents unauthenticated users from accessing the cart page.

---

# EPIC: Checkout & Delivery  
**Jira Epic ID:** GGS-12

### Scenario CHECKOUT-01: User enters valid delivery details
**Related Test Cases:** GGS-T14  
**Related Story:** GGS-13  
User fills in all required delivery fields successfully during checkout.

---

### Scenario CHECKOUT-02: Delivery details summary is displayed correctly
**Related Test Cases:** GGS-T15  
**Related Story:** GGS-14  
System displays saved delivery details for review and editing.

---

# EPIC: Payment Processing  
**Jira Epic ID:** GGS-15

### Scenario PAY-01: User selects card payment method
**Related Test Cases:** GGS-T16  
**Related Story:** GGS-16  
User selects Pay by Card and views card payment form.

---

### Scenario PAY-02: User completes payment using valid Visa card
**Related Test Cases:** GGS-T17  
**Related Story:** GGS-18  
System processes payment successfully with valid Visa card details.

---

### Scenario PAY-03: User completes end-to-end payment flow successfully
**Related Test Cases:** GGS-T18  
**Related Story:** GGS-19  
User completes checkout, payment, and order placement successfully.

---

### Scenario PAY-04: First-time user is restricted from Cash on Delivery
**Related Test Cases:** GGS-19  
**Related Story:** GGS-17  
System restricts Cash on Delivery option for first-time users.

---

## Notes
- Every high-level scenario is mapped to at least one test case.
- All scenarios maintain Jira ID consistency for Epics, Stories, and Test Cases.

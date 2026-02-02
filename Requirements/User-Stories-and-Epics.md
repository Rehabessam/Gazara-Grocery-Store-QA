# User Stories & Epics  
## Gazara Grocery Store – Website

---

## Project Overview
This document contains all Epics and User Stories created in **Jira Scrum** for the Gazara Grocery Store website.
These requirements were used as the foundation for designing high-level test scenarios and detailed manual test cases as part of a **requirement-based QA project**.

---

# EPIC: User Authentication & Registration  
**Jira Epic ID:** GGS-1  

**Summary:** Implement user registration and login functionality  
**Description:**  
Enable users to register and log in using multiple methods (Email, Google, Facebook)
with proper validation and security measures.

**Business Value:** Critical for user account management and personalized shopping experience  
**Priority:** Highest  

---

## STORY: Multi-Option User Registration  
**Jira Story ID:** GSS-3  
**Epic Link:** GGS-1  

**As a:** new user  
**I want to:** register using email, Google, or Facebook  
**So that:** I can create an account with my preferred method  

### Acceptance Criteria:
- User can sign up via email with first name, last name, email, and password
- User can sign up via Google OAuth
- User can sign up via Facebook OAuth
- First name accepts alphabets only
- Last name accepts alphabets only
- Email must be in valid format
- Password must be minimum 8 characters with numbers and letters

**Priority:** High  
**Sprint:** Sprint 1  

---

## STORY: User Login  
**Jira Story ID:** GSS-4  
**Epic Link:** GGS-1  

**As a:** registered user  
**I want to:** log in to my account  
**So that:** I can access personalized features and my shopping cart  

### Acceptance Criteria:
- User can log in with registered email and password
- Invalid credentials show appropriate error message
- Successful login redirects to home page
- User session is maintained
- Logout ends the user session

**Priority:** High  
**Sprint:** Sprint 1  

---

# EPIC: Navigation & Website Structure  
**Jira Epic ID:** GGS-5  

**Summary:** Implement main navigation and website structure  
**Description:**  
Create an intuitive navigation system allowing users to browse
different product categories and access key website sections.

**Business Value:** Essential for user experience and product discovery  
**Priority:** High  

---

## STORY: Main Navigation Menu  
**Jira Story ID:** GSS-6  
**Epic Link:** GGS-5  

**As a:** user  
**I want to:** navigate between Home, Vegetables, Fruits, Meat, and Shop All sections  
**So that:** I can browse different product categories  

### Acceptance Criteria:
- Navigation bar contains Home, Vegetables, Fruits, Meat, and Shop All
- Current page is indicated in bold
- All links are functional and redirect correctly

**Priority:** High  
**Sprint:** Sprint 1  

---

## STORY: Shop Now Call-to-Action  
**Jira Story ID:** GSS-7  
**Epic Link:** GGS-5  

**As a:** visitor  
**I want to:** click a "Shop Now" button  
**So that:** I can quickly start shopping  

### Acceptance Criteria:
- "Shop Now" button is displayed on the home page
- Button redirects to "Shop All" page
- Redirect is immediate

**Priority:** Medium  
**Sprint:** Sprint 1  

---

# EPIC: Shopping Cart Management  
**Jira Epic ID:** GGS-8  

**Summary:** Implement shopping cart functionality  
**Description:**  
Enable users to add items to cart, view cart contents,
and proceed to checkout with proper authentication.

**Business Value:** Core e-commerce functionality  
**Priority:** Critical  

---

## STORY: Authentication Requirement for Cart  
**Jira Story ID:** GSS-9  
**Epic Link:** GGS-8  

**As a:** business owner  
**I want to:** require users to log in before using cart features  
**So that:** we can track orders and provide personalized service  

### Acceptance Criteria:
- Non-logged-in users cannot add items to cart
- Non-logged-in users cannot view cart
- Non-logged-in users cannot proceed to payment
- Attempting these actions redirects to login page

**Priority:** Critical  
**Sprint:** Sprint 1  

---

## STORY: Add Items to Cart with Notification  
**Jira Story ID:** GSS-10  
**Epic Link:** GGS-8  

**As a:** logged-in customer  
**I want to:** add items to my cart and see confirmation  
**So that:** I know my items have been added successfully  

### Acceptance Criteria:
- Logged-in users can add items to cart
- Side pop-up notification appears upon adding
- Pop-up shows item name, price, and size
- Confirmation message is clear

**Priority:** High  
**Sprint:** Sprint 1  

---

## STORY: View Cart from Notification  
**Jira Story ID:** GSS-11  
**Epic Link:** GGS-8  

**As a:** customer  
**I want to:** navigate to cart from the add-to-cart notification  
**So that:** I can quickly review my selections  

### Acceptance Criteria:
- "View Cart" button appears in side pop-up
- Clicking button opens cart page
- All added items are displayed
- Order summary is visible
- The cart total price is calculated correctly

**Priority:** Medium  
**Sprint:** Sprint 1  

---

# EPIC: Checkout & Delivery  
**Jira Epic ID:** GGS-12  

**Summary:** Implement the checkout process and delivery details collection 
**Description:** Enable users to provide delivery information and review order details before proceeding to payment
**Business Value:** Essential for order fulfillment  
**Priority:** Critical  

---

## STORY: Enter Delivery Details  
**Jira Story ID:** GSS-13  
**Epic Link:** GGS-12  

**As a:** customer  
**I want to:** provide my delivery information during checkout  
**So that:** my order can be shipped to the correct address  

### Acceptance Criteria:
- Checkout form includes first name, last name, phone, address, region, postal code
- All fields are validated
- Required fields are enforced
- Users can save and continue
- Users can return to browsing

**Priority:** Critical  
**Sprint:** Sprint 1  

---

## STORY: Review and Edit Delivery Details  
**Jira Story ID:** GSS-14  
**Epic Link:** GGS-12  

**As a:** customer  
**I want to:** review and edit my delivery information  
**So that:** I can ensure accuracy before payment  

### Acceptance Criteria:
- A summary of the delivery details is displayed after saving
- The change option is available
- Clicking “change”  reopens the form with saved data
- Changes can be saved
- Summary updates with new information

**Priority:** High  
**Sprint:** Sprint 1  

---

# EPIC: Payment Processing  
**Jira Epic ID:** GGS-15  

**Summary:** Implement payment processing functionality 
**Description:** 
Enable Users to complete purchases using card payment or cash on delivery with proper validation and security 
**Business Value:** Critical for revenue generation  
**Priority:** Critical  

---

## STORY: Select Payment Method  
**Jira Story ID:** GSS-16  
**Epic Link:** GGS-15  

**As a:** customer  
**I want to:** choose between cash on delivery and card payment 
**So that:** I can pay using my preferred method 

### Acceptance Criteria:
- The payment selection screen shows both options
- Users can select one payment method
- Selection determines the next steps
- The payment method is recorded with the order

**Priority:** Critical  
**Sprint:** Sprint 1  

---

## STORY: Cash on Delivery Restriction  
**Jira Story ID:** GSS-17  
**Epic Link:** GGS-15  

**As a:** business owner  
**I want to:** restrict cash on delivery to users with prior card payments  
**So that:** we can establish payment credibility

### Acceptance Criteria:
- First-time users cannot select cash on delivery
- The option is disabled or shows an error message
- Users with at least one card payment order can use Cash on Delivery
- Clear messaging explains the restriction

**Priority:** High  
**Sprint:** Sprint 1  

---

## STORY: Card Payment Processing  
**Jira Story ID:** GSS-18  
**Epic Link:** GGS-15  

**As a:** customer  
**I want to:** pay by credit/debit card  
**So that:** I can complete my purchase securely

### Acceptance Criteria:
- Card payment form includes: card number, name, expiry, CVV
- Card Number must be a numeric string with 16 digits
- Card Types (Visa, Mastercard, etc.) should be detected and displayed dynamically based on the first 4 digits
- The card number should pass Luhn’s Algorithm for credit card number validation
- Name on Card must be a non-empty string, accepts alphabets (A-Z, a-z), spaces, and hyphens
- Name on Card Minimum length: 2 characters, Maximum length: 50 characters
- Expiry Date must be a valid future date in MM/YY format, Month (MM) should range from 01 to 12, Year (YY) should not be in the past
- CVV must be a numeric string with 3 or 4 digits (depending on the card type). Only numbers are allowed
- All fields are validated
- Payment processes upon valid submission

**Priority:** Critical  
**Sprint:** Sprint 1  

---

## STORY: Complete Order Placement  
**Jira Story ID:** GSS-19  
**Epic Link:** GGS-15  

**As a:** customer  
**I want to:** place my order after entering payment details  
**So that:** my purchase can be processed and delivered

### Acceptance Criteria:
- Valid payment details allow order placement
- The order is submitted for processing
- Confirmation page/message is displayed
- Order details are saved
- Customer receives order confirmation
- The customer can track the order

**Priority:** Critical  
**Sprint:** Sprint 1  

---

## Notes
All Jira issue IDs were preserved to maintain full traceability
between Epics, User Stories, and Test Cases.
This project is requirement-based and does not include live test execution.

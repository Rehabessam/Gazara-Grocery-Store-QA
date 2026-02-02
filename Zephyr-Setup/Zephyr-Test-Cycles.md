# Zephyr Test Cycle – Gazara Grocery Store Website

## Test Cycle Name
GGS_Regression_Cycle_01 (GGS-R1)

---

## Tool Used
- Jira Software (Scrum Project)
- Zephyr Scale for Jira

---

## Test Cycle Objective
The objective of this test cycle is to validate the core functional
flows of the Gazara Grocery Store website based on the approved
requirements and user stories.

This cycle focuses on ensuring that critical business processes
such as authentication, navigation, shopping cart, checkout,
and payment workflows are logically correct and testable.

---

## Test Cycle Type
Regression Test Cycle (Requirement-Based)

---

## Website Status
- The Website is **not live**.
- Test cases were **designed and organized** based on documented
  requirements and user stories.
- No real execution was performed due to the absence of a deployed
  website under test.

---

## Scope of Testing

### In Scope
- User Authentication (Signup & Login)
- Main Navigation
- Shopping Cart functionality
- Checkout flow
- Payment methods and restrictions

### Out of Scope
- Performance testing
- Security testing
- API testing
- Cross-browser compatibility testing
- Production data validation

---

## Linked Epics (Jira IDs)
- GGS-1:  User Authentication & Registration
- GGS-6:  Main Navigation Menu
- GGS-9:  Authentication Requirement for Cart
- GGS-10: Add Items to Cart with Notification
- GGS-13: Delivery Details
- GGS-16: Select Payment Method
- GGS-17: Cash on Delivery Restriction
- GGS-18: Card Payment Processing
- GGS-19: Complete Order Placement

---

## Test Cases Coverage

| Module         | Test Case IDs                | Count  |
|----------------|----------------------------- |------- |
| Authentication | GGS-T1   – GGS-T5            |   5    |
| Navigation     | GGS-T6   – GGS-T8            |   3    |
| Shopping Cart  | GGS-T9   – GGS-T13           |   5    |
| Checkout       | GGS-T14  – GGS-T15           |   2    |
| Payment        | GGS-T16  – GGS-T19           |   4    |
| **Total**      | **GGS-T1 – GGS-T19**         | **19** |

---

## Test Cycle Execution Status

| Status        | Count |
|---------------|-------|
| Not Executed  | 19    |
| Executed      | 0     |
| Passed        | 0     |
| Failed        | 0     |

---

## Reason for Non-Execution
The test cycle was not executed because the project is based on
requirements documentation only and no live or test environment
was available.

---

## Data Sets
- Test data sets were created in Zephyr Scale to support
  parameterized test cases.
- Data sets include valid and invalid user inputs for:
  - Authentication
  - Checkout
  - Payment scenarios

---

## Traceability
- All test cases are linked to corresponding Jira User Stories.
- Full traceability is maintained between:
  - Epics
  - User Stories
  - Test Cases
  - Test Cycle

---

## Notes
This test cycle was designed to be executed as a full regression
cycle once the application becomes available for testing.

The structure reflects real-world usage of Zephyr Scale in
requirement-based testing projects.

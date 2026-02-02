# Zephyr Data Sets Documentation

## Overview
This document outlines the **data sets** created in **Zephyr Scale**
to support data-driven testing for the Gazara Grocery Store project.

The data sets were designed to validate multiple input combinations
without duplicating test cases.

---

## Data Set Usage
- Data sets were linked to test cases in Zephyr Scale
- Parameters were used inside test steps
- Supports positive and negative testing scenarios

---

## Defined Data Sets

### 🔹 Data Set 1: User Registration Data
**Related Stories:** GSS-3  

**Parameters:**
- First Name
- Last Name
- Email
- Password

**Test Data Examples:**
- Valid user data
- Empty email
- Invalid email format
- Short password
- Empty First Name
- Numeric characters in name fields

---

### 🔹 Data Set 2: Login Credentials
**Related Stories:** GSS-4  

**Parameters:**
- Email
- Password

**Test Data Examples:**
- Valid credentials
- Invalid password
- Unregistered email

---

### 🔹 Data Set 3: Delivery Information
**Related Stories:** GSS-13, GSS-14  

**Parameters:**
- First Name
- Last Name
- Phone Number
- Address
- Region
- Postal Code

**Test Data Examples:**
- Valid delivery details
- Missing required fields
- Invalid phone number

---

### 🔹 Data Set 4: Card Payment Details
**Related Stories:** GSS-18  

**Parameters:**
- Card Number
- Name on Card
- Expiry Date
- CVV

**Test Data Examples:**
- Valid Visa / Mastercard
- Invalid card number
- Expired card
- Invalid CVV length

---

## Conclusion
The use of data sets demonstrates:
- Knowledge of data-driven testing concepts
- Efficient test design practices
- Proper usage of Zephyr Scale advanced features

# Registration Requirements — PetStore

## Overview
This document describes functional and validation requirements for the Registration module in the PetStore application.

---

## Navigation

### REG-001 — Access to Registration Page
User should be able to access the Registration page from the [Sign In] page by clicking the [Register Now] button.

---

## Registration Flow

### REG-002 — Registration Submission
User should be able to submit the registration form by:
- clicking the [Save Account Information] button
- pressing the Enter key

---

### REG-003 — Successful Registration
If all fields are valid and no conflicts exist:
- a new user account is created
- user is redirected to the main page
- user gains access to the product ordering section
- user is NOT automatically logged in

---

## Page Structure

### REG-004 — Registration Sections
The Registration page should contain the following sections:
- User Information
- Account Information
- Profile Information

---

## User Information

### REG-005 — Required Fields
The User Information section should contain required fields:
- User ID
- New Password
- Repeat Password

All required fields must be marked with an asterisk (*).

---

### REG-006 — User ID Rules
User ID:
- must be unique
- must contain 4–40 characters
- may include Latin letters and digits
- must not contain special or non-printing characters
- is NOT case-sensitive

---

### REG-007 — New Password Rules
New Password:
- is required
- input must be masked
- must contain 8–30 characters
- must include:
  - at least one uppercase letter
  - at least one digit
  - at least one special character
- must not contain non-printing characters
- copy, cut, and paste must be disabled

---

### REG-008 — Repeat Password Rules
Repeat Password:
- is required
- must contain 8–30 characters
- must exactly match New Password
- copy and cut must be disabled

---

## Account Information

### REG-009 — Optional Account Data
Account Information:
- is optional during registration
- can be updated later in user profile settings

---

### REG-010 — Email Rules
Email:
- must follow pattern: `[name]@[domain].com`
- must contain 14–72 characters
- must be unique

[name] may contain:
- Latin letters
- digits
- special characters: + - _ .

---

### REG-011 — Phone Rules
Phone:
- must start with "+"
- must contain only digits and "+"
- must not contain letters
- must not contain special characters (except "+")
- must not contain non-printing characters
- should include placeholder: `+38 098 765 43 21`

---

## Profile Information

### REG-012 — Optional Profile Data
Profile Information:
- is optional
- contains user preferences

---

### REG-013 — Language Selection
User should be able to select one language from:
- EN
- ES
- UK
- JP

---

### REG-014 — Categories Selection
User should be able to:
- select one primary favorite category
- select multiple interest categories

---

### REG-015 — MyBanner Checkbox
- "Enable MyBanner" checkbox must be present
- checkbox should be enabled by default

---

## Validation

### REG-016 — Duplicate User ID Validation
If a User ID is already registered, the system should display a validation message.

---

### REG-017 — Required Fields Validation
If required fields are empty:
- fields should be highlighted in red

---

### REG-018 — General Validation Error
If validation fails:
- message should be displayed:

"Validation failed! Check that all required fields are filled with valid data."

# Test Report — PetStore Application

## Overview
This document summarizes the results of manual testing conducted on the PetStore application.  
The testing covered core functionalities including Registration, Login, Search, and Cart modules.

---

## Scope of Testing

The following modules were tested:

- Registration
- Login
- Search
- Cart

---

## Test Environment

- **Application:** PetStore (Demo)
- **Environment:** Production
- **Browser:** Chrome (latest)
- **Operating System:** Windows 11

---

## Test Execution Summary

| Metric | Value |
|------|------|
| Total Test Cases | 19 |
| Passed | 14 |
| Failed | 5 |
| Blocked | 0 |
| Not Run | 0 |

---

## Defect Summary

| Severity | Count |
|--------|------|
| Critical | 2 |
| Major | 6 |
| Minor | 4 |

**Total Defects:** 12

---

## Defect Distribution by Module

| Module | Defects |
|--------|--------|
| Cart | 8 |
| Search | 2 |
| Registration | 1 |
| UI / General | 1 |

---

## Key Findings

- Several validation issues were identified in Registration and Cart modules.
- Critical defects were found in Cart functionality related to product quantity and stock validation.
- Search functionality has issues with duplicate results and validation messages.
- UI inconsistencies were identified (missing tooltip, inconsistent category order).

---

## Risks

- Users can add more items than allowed, which may lead to incorrect orders.
- Lack of validation messages may confuse users and reduce usability.
- Ability to add out-of-stock products may affect system integrity.
- Missing product information in the cart affects user experience.

---

## Conclusion

The PetStore application contains several functional and validation defects.  
Some of them (especially in the Cart module) have a significant impact on business logic and user experience.

The application requires further improvements before it can be considered stable for production use.

---

## Recommendations

- Fix critical issues in Cart module as a top priority.
- Improve validation mechanisms across the application.
- Ensure consistency between UI components.
- Add proper user feedback (validation messages, tooltips).

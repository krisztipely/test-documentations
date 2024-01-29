# Traceability Matrix

## Project Information
- **Project Name:** Online Shopping Platform
- **Version:** 1.0
- **Date:** 2024-03-15

## Purpose
The purpose of this traceability matrix is to establish a link between the requirements and their associated test cases for the Online Shopping Platform.

## Legend
- R: Requirement
- TC: Test Case

## Traceability Matrix Table

| Requirement/User Story | Test Case(s) |
|------------------------|--------------|
| R001: User Registration | TC001, TC002 |
| R002: Product Search    | TC003, TC004 |

## Notes
- Please update this matrix as requirements or test cases are added, modified, or removed.
- Ensure that each requirement has at least one corresponding test case, and vice versa.
- If a test case covers multiple requirements, list them accordingly.

## Test Case Details

### TC001: User Registration - Positive Case
- **Objective:** To verify that a user can successfully register on the platform.
- **Preconditions:** The user is on the registration page.
- **Steps:**
  1. Enter valid user details.
  2. Click the "Register" button.
- **Expected Result:** User is registered successfully, and a confirmation message is displayed.

### TC002: User Registration - Invalid Input
- **Objective:** To verify that the system handles invalid input during user registration.
- **Preconditions:** The user is on the registration page.
- **Steps:**
  1. Enter invalid user details (e.g., missing email).
  2. Click the "Register" button.
- **Expected Result:** Proper error message is displayed, and user registration fails.

### TC003: Product Search - Basic Search
- **Objective:** To verify that users can perform a basic search for products.
- **Preconditions:** The user is logged into the platform.
- **Steps:**
  1. Enter a product name in the search bar.
  2. Press "Enter" or click the search icon.
- **Expected Result:** Relevant products matching the search criteria are displayed.

### TC004: Product Search - Advanced Search
- **Objective:** To verify that users can perform an advanced search for products.
- **Preconditions:** The user is logged into the platform.
- **Steps:**
  1. Use filters such as category and price range in the search.
  2. Click the "Search" button.
- **Expected Result:** Products matching the advanced search criteria are displayed.

## Changes
| Version | Date       | Changes Made                     | Author       |
|---------|------------|----------------------------------|--------------|
| 1.0     | 2024-03-15 | Initial version created          | John Tester  |
| 1.1     | 2024-03-20 | Added new requirement R003        | John Tester  |

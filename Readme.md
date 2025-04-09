# TEST CASES - To-Do List Application with Keycloak Authentication

## Submitted By
Manish Kumar Chaudhary  

## Submitted To
Mr. Vipin Tripathi

## Test Case Version
1.0

## Reviewer Name
Ms. Manmeet Narang

---

## Goal
The goal of this project is to develop a To-Do List Application with authentication and authorization using Keycloak. The application should securely authenticate users, authorize API requests, and manage user sessions efficiently. The backend, built with FastAPI, should validate access tokens with Keycloak, interact with MongoDB for data storage, and return appropriate responses to the Angular frontend.

---

## Table of Contents
1. [TC1: User Login Redirection](#tc1-user-login-redirection)
2. [TC2: Token Validation in FastAPI](#tc2-token-validation-in-fastapi)
3. [TC3: Creating a To-Do Item](#tc3-creating-a-to-do-item)
4. [TC4: Retrieving To-Do Items](#tc4-retrieving-to-do-items)
5. [TC5: Unauthorized API Access](#tc5-unauthorized-api-access)

---

## TC1: User Login Redirection
### Scenario
A user opens the Angular application and is redirected to the Keycloak login page.

### Remarks
Ensures that unauthenticated users are redirected to Keycloak for authentication.

### Given
- The user accesses the Angular application (`http://localhost:4200`).

### When
- The user is not logged in.

### Then
- The user is successfully redirected to the Keycloak login page for authentication.

### Test Run
- **Date:** <Date>
- **Result:** Pending/Pass/Fail


---

## TC2: Token Validation in FastAPI
### Scenario
The FastAPI backend should validate the token received from Keycloak before processing requests.

### Remarks
Ensures that only valid tokens are accepted.

### Given
- The user has successfully logged in and received an access token.

### When
- The Angular app sends an API request to FastAPI with the token.

### Then
- The user is successfully authorized to access the requested resource.
- The user receives a "401 Unauthorized" error message when the token is invalid.

### Test Run
- **Date:** <Date>
- **Result:** Pending/Pass/Fail


---

## TC3: Creating a To-Do Item
### Scenario
A logged-in user creates a new to-do item via the API.

### Remarks
Ensures authenticated users can add tasks.

### Given
- The user is authenticated with a valid token.

### When
- The user submits a POST request to `/api/todo` with task details.

### Then
- The new to-do item is created successfully and a "201 Created" success message is returned.

### Test Run
- **Date:** <Date>
- **Result:** Pending/Pass/Fail


---

## TC4: Retrieving To-Do Items
### Scenario
A logged-in user fetches their to-do list from the backend.

### Remarks
Ensures that only authenticated users can retrieve tasks.

### Given
- The user has logged in and has tasks stored in MongoDB.

### When
- The user sends a GET request to `/api/todo` with a valid token.

### Then
- The user's to-do list is successfully retrieved and displayed with a "200 OK" success response.

### Test Run
- **Date:** <Date>
- **Result:** Pending/Pass/Fail


---

## TC5: Unauthorized API Access
### Scenario
A user tries to access API endpoints without a valid token.

### Remarks
Ensures unauthorized requests are rejected.

### Given
- The user does not have a valid token.

### When
- The user sends an API request to the FastAPI backend.

### Then
- The user is shown a "401 Unauthorized" error message indicating access is denied.

### Test Run
- **Date:** <Date>
- **Result:** Pending/Pass/Fail



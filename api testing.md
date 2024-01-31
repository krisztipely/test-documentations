# API testing 

Test the functionality of an API that retrieves information about users from a user management system.

Base URL of the API is https://api.example.com.

API Endpoint: /users/{userId}

HTTP Method: GET

Sample Request:

```GET https://api.example.com/users/123```

Sample Response (Success):

```
{
  "userId": 123,
  "firstName": "John",
  "lastName": "Doe",
  "email": "john.doe@example.com",
  "status": "active"
}
```

Sample Response (User Not Found):
```
{
  "error": "User not found"
}
```
Some test scenarios for this API:

**Positive Test Case - Retrieve User:**

Test Case: Verify that the API returns the correct user information when a valid user ID is provided.

Steps:
1. Send a GET request to /users/123.
2. Verify that the response status code is 200 (OK).
3. Validate the response JSON to ensure it contains the correct user information.

**Negative Test Case - User Not Found:**

Test Case: Verify that the API returns an appropriate error message when an invalid user ID is provided.

Steps:
1. Send a GET request to /users/999 (assuming user with ID 999 does not exist).
2. Verify that the response status code is 404 (Not Found).
3. Validate the response JSON to ensure it contains the "User not found" error message.

**Boundary Test Case - Invalid User ID Format:**

Test Case: Verify that the API handles requests with invalid user ID formats gracefully.

Steps:
1. Send a GET request to /users/abc (non-numeric user ID).
2. Verify that the response status code is 400 (Bad Request).
3. Validate the response JSON to ensure it contains an appropriate error message.
   
**Performance Test Case - Response Time:**

Test Case: Verify the API's response time under normal conditions.

Steps:
1. Send multiple consecutive GET requests to /users/123.
2. Measure the response time for each request.
3. Ensure that the average response time is within acceptable limits.

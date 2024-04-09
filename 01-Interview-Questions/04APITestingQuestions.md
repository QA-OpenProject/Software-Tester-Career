1. What's the most important when we make the API testing?
- API Documentation
  - API endpoints
  - Request and Response format
  - Authentication details
  - Error codes
  
2. What must be checked when performing API testing?
- Accuracy of data
- Schema validation
- HTTP status codes
- Data type, validations, order, and completeness
- Authorization checks
- Implementation of response timeout
- Error codes in case API returns, and
- Non-functional testing like performance and security testing

3. Status Codes
- 200 OK: The request was successful.
- 201 Created: The request was successful and a resource was created.
- 204 No Content: The request was successful but no content was returned.
- 400 Bad Request: The request was malformed.
- 401 Unauthorized: The request did not include an authentication token or the authentication token was expired.
- 403 Forbidden: The client did not have permission to access the requested resource.
- 404 Not Found: The requested resource was not found.
- 405 Method Not Allowed: The HTTP method in the request was not supported by the resource.
- 500 Internal Server Error: The request was not completed. The server met an unexpected condition.
- 502 Bad Gateway: The server was acting as a gateway or proxy and received an invalid response from the upstream server.
- 503 Service Unavailable: The server is currently unavailable (overloaded or down).
- 504 Gateway Timeout: The server was acting as a gateway or proxy and did not receive a timely response from the upstream server.
- 505 HTTP Version Not Supported: The server does not support the HTTP protocol version used in the request.
- 511 Network Authentication Required: The client needs to authenticate to gain network access.

4. API Methods
- GET: Retrieve information from the server.
- POST: Send new information to the server.
- PUT: Update existing information on the server.
- DELETE: Remove information from the server.
- PATCH: Update existing information on the server.
- OPTIONS: Get information about the communication options available for the target resource.
- HEAD: Retrieve the headers of a resource without the body.

5. what 's the difference between put and patch method in the API testing?
- PUT: The PUT method is used to update an existing resource or create a new resource if it doesn't exist. It replaces the entire resource with the new data provided in the request.
- PATCH: The PATCH method is used to update an existing resource with partial data. It only updates the specified fields in the resource, leaving the rest of the resource unchanged.

6. What are the major challenges faced in API testing?
- Understanding the API documentation
- Handling authentication and authorization
- Testing for different data types and formats
- Handling different request and response formats
- Testing for error codes and error handling
- Testing for performance and security
- Parameter combinations and boundary value testing
  - Testing with valid and invalid input data
  - Testing with different data types and formats
  - Testing with different parameter combinations

1. dd



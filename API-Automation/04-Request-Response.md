# 🚀 API Automation → Request & Response

This is one of the core API testing topics.

Interviewers ask this to check:
- API structure understanding
- Validation knowledge
- Real-world testing capability

--------------------------------------------------

Topics Covered:

1. What is Request
2. What is Response
3. Request Components
4. Response Components
5. Request Body
6. Response Body
7. Query Parameters
8. Path Parameters
9. Real-Time Flow
10. Best Practices

--------------------------------------------------

# 🧠 1. What is Request

## What is it

A request is data sent from client to server asking for some operation or information.

---

## Key Components

- Endpoint
- Method
- Headers
- Body
- Parameters

---

## How to Answer (Interview Style)

API request is sent by the client to server containing operation details such as endpoint, HTTP method, headers, and request data.

---

## Practical Example

```text
POST /users
```

---

## Common Mistakes

- Missing mandatory headers
- Invalid payload structure
- Wrong endpoint usage

---

## Expected Interview Questions

- What is API request?
- What are request components?
- Difference between request and response?

--------------------------------------------------

# 🧠 2. What is Response

## What is it

A response is data returned by server after processing the client request.

---

## Key Components

- Status code
- Response body
- Headers
- Response time

---

## How to Answer (Interview Style)

API response contains server output after processing a request, including status code, response body, and headers.

---

## Practical Example

```json
{
  "id": 1,
  "name": "Kalpesh"
}
```

---

## Common Mistakes

- Validating only status code
- Ignoring response body validation

---

## Expected Interview Questions

- What is API response?
- What validations do you perform on response?
- What does response contain?

--------------------------------------------------

# 🧠 3. Request Components ⭐

## What is it

Important elements included in API requests.

---

## Key Components

- URL
- HTTP Method
- Headers
- Body
- Authentication
- Parameters

---

## How to Answer (Interview Style)

API requests contain endpoint URL, HTTP method, headers, authentication details, parameters, and optional request body.

---

## Practical Example

```text
POST /users
Authorization: Bearer token
Content-Type: application/json
```

---

## Common Mistakes

- Missing authentication
- Wrong content type
- Invalid parameters

---

## Expected Interview Questions

- Explain request structure.
- What are request headers?
- What is request payload?

--------------------------------------------------

# 🧠 4. Response Components ⭐

## What is it

Important data returned in API responses.

---

## Key Components

- Status code
- Response body
- Headers
- Cookies
- Response time

---

## How to Answer (Interview Style)

API responses contain status code, response body, headers, and performance information used for validations.

---

## Practical Example

```text
200 OK
Content-Type: application/json
```

---

## Common Mistakes

- Ignoring headers validation
- Not validating response time

---

## Expected Interview Questions

- Explain response structure.
- What validations do you perform?
- Why validate headers?

--------------------------------------------------

# 🧠 5. Request Body ⭐

## What is it

Request body contains data sent to server during API operations.

---

## Key Components

- JSON payload
- Input data
- Objects
- Arrays

---

## How to Answer (Interview Style)

Request body contains input data sent to API for operations like create or update actions.

---

## Practical Example

```json
{
  "name": "Kalpesh",
  "role": "SDET"
}
```

---

## Common Mistakes

- Invalid JSON format
- Missing mandatory fields
- Wrong data types

---

## Expected Interview Questions

- What is request payload?
- When request body is used?
- Can GET have request body?

--------------------------------------------------

# 🧠 6. Response Body ⭐

## What is it

Response body contains data returned from server.

---

## Key Components

- JSON response
- API output
- Business data
- Error message

---

## How to Answer (Interview Style)

Response body contains API output data returned from server after request processing.

---

## Practical Example

```json
{
  "status": "success",
  "userId": 101
}
```

---

## Common Mistakes

- Weak field validations
- Ignoring error messages

---

## Expected Interview Questions

- How do you validate response body?
- What validations do you perform?
- Difference between response body and headers?

--------------------------------------------------

# 🧠 7. Query Parameters

## What is it

Query parameters are optional key-value pairs passed in URL for filtering or searching data.

---

## Key Components

- Filtering
- Searching
- Pagination

---

## How to Answer (Interview Style)

Query parameters are used for filtering or customizing API responses without changing endpoint structure.

---

## Practical Example

```text
GET /users?page=1
GET /products?category=mobile
```

---

## Common Mistakes

- Invalid query format
- Hardcoded query values

---

## Expected Interview Questions

- What are query parameters?
- Difference between path and query parameters?
- Real-time example?

--------------------------------------------------

# 🧠 8. Path Parameters ⭐

## What is it

Path parameters identify specific resources directly in URL path.

---

## Key Components

- Resource identification
- Dynamic values
- URL path

---

## How to Answer (Interview Style)

Path parameters are dynamic values in API URLs used to identify specific resources.

---

## Practical Example

```text
GET /users/101
```

---

## Common Mistakes

- Confusing path and query params
- Hardcoding resource IDs

---

## Expected Interview Questions

- What are path parameters?
- Difference between query and path params?
- Real-time path param example?

--------------------------------------------------

# 🧠 9. Real-Time API Flow ⭐

## 1. User Login Flow

```text
Client → Login Request → Server
Server → Token Response → Client
```

---

## 2. Product Search

```text
GET /products?category=mobile
```

---

## 3. Fetch User Profile

```text
GET /users/101
```

--------------------------------------------------

# 🧠 10. Best Practices

## What is it

Guidelines for validating requests and responses effectively.

---

## Key Components

- Proper validations
- Secure headers
- Validate body and status
- Negative testing

---

## How to Answer (Interview Style)

I validate request structure, response body, headers, status codes, and error messages to ensure reliable API behavior.

---

## Practical Example

```text
Validate:
- Status Code
- Headers
- Body
- Response Time
```

---

## Common Mistakes

- Validating only response code
- Ignoring headers and body
- No negative testing

---

## Expected Interview Questions

- What validations do you perform?
- What is request payload?
- Difference between path and query parameters?

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## MOST IMPORTANT TOPICS

1. Request vs Response ⭐
2. Path vs Query Parameters ⭐
3. Request Body vs Response Body ⭐
4. Real-Time API Flow ⭐

--------------------------------------------------

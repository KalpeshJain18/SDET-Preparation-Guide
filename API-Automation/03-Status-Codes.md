# 🚀 API Automation → Status Codes

This is one of the most frequently asked API interview topics.

Interviewers use this topic to check:
- API understanding
- Error handling knowledge
- Real-world debugging capability

--------------------------------------------------

Topics Covered:

1. What are Status Codes
2. 2xx Success Codes
3. 4xx Client Error Codes
4. 5xx Server Error Codes
5. Most Important Status Codes
6. Real-Time Scenarios
7. Negative Testing
8. Best Practices

--------------------------------------------------

# 🧠 1. What are Status Codes

## What is it

HTTP status codes are server responses that indicate whether an API request was successful or failed.

---

## Key Components

- Response status
- Success codes
- Error codes
- Client/server communication

---

## How to Answer (Interview Style)

Status codes are HTTP response indicators that tell whether an API request succeeded, failed, or encountered an error.

---

## Practical Example

```text
200 → Success
404 → Not Found
500 → Server Error
```

---

## Common Mistakes

- Ignoring status code validation
- Validating only response body
- Confusing client and server errors

---

## Expected Interview Questions

- What are HTTP status codes?
- Why validate status codes?
- Commonly used status codes?

--------------------------------------------------

# 🧠 2. 2xx Success Codes ⭐

## What is it

2xx codes indicate successful API operations.

---

## Key Components

- 200 OK
- 201 Created
- 204 No Content

---

## How to Answer (Interview Style)

2xx status codes indicate successful request processing. 200 means success, 201 means resource created, and 204 means success with no response body.

---

## Practical Example

```text
200 OK → Fetch successful
201 Created → User created
204 No Content → Delete successful
```

---

## Common Mistakes

- Expecting 200 for every API
- Ignoring 201 for create operations

---

## Expected Interview Questions

- Difference between 200 and 201?
- When do you get 204?
- Which success codes have you used?

--------------------------------------------------

# 🧠 3. 4xx Client Error Codes ⭐

## What is it

4xx codes indicate client-side/request-related issues.

---

## Key Components

- 400 Bad Request
- 401 Unauthorized
- 403 Forbidden
- 404 Not Found

---

## How to Answer (Interview Style)

4xx status codes occur when the request sent by client is invalid, unauthorized, or requests unavailable resources.

---

## Practical Example

```text
400 → Invalid request
401 → Authentication missing
403 → Access denied
404 → Resource not found
```

---

## Common Mistakes

- Confusing 401 and 403
- Ignoring negative testing

---

## Expected Interview Questions

- Difference between 401 and 403?
- What causes 400 Bad Request?
- Real-time 404 scenario?

--------------------------------------------------

# 🧠 4. 5xx Server Error Codes ⭐

## What is it

5xx codes indicate server-side failures.

---

## Key Components

- 500 Internal Server Error
- 502 Bad Gateway
- 503 Service Unavailable

---

## How to Answer (Interview Style)

5xx status codes indicate backend or server-side issues where the request reached server successfully but processing failed.

---

## Practical Example

```text
500 → Internal server failure
503 → Service unavailable
```

---

## Common Mistakes

- Assuming all failures are frontend issues
- Not reporting server logs properly

---

## Expected Interview Questions

- What is 500 Internal Server Error?
- Difference between 4xx and 5xx?
- How do you debug server failures?

--------------------------------------------------

# 🧠 5. Most Important Status Codes ⭐

## Commonly Used Codes

| Code | Meaning |
|------|----------|
| 200 | OK |
| 201 | Created |
| 204 | No Content |
| 400 | Bad Request |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |
| 500 | Internal Server Error |

---

## How to Answer (Interview Style)

The most commonly used status codes in API testing are 200, 201, 400, 401, 403, 404, and 500.

---

## Expected Interview Questions

- Most common status codes?
- Which codes do you validate most?
- Difference between success and error codes?

--------------------------------------------------

# 🧠 6. Real-Time Scenarios ⭐

## 1. Login Failure

```text
401 Unauthorized
```

---

## 2. Invalid API Payload

```text
400 Bad Request
```

---

## 3. Resource Not Found

```text
404 Not Found
```

---

## 4. Backend Crash

```text
500 Internal Server Error
```

--------------------------------------------------

# 🧠 7. Negative Testing ⭐

## What is it

Testing APIs with invalid or unexpected data.

---

## Key Components

- Invalid payload
- Missing headers
- Unauthorized access
- Boundary testing

---

## How to Answer (Interview Style)

Negative testing validates how APIs behave with invalid inputs, unauthorized access, or incorrect requests to ensure proper error handling.

---

## Practical Example

```text
Missing token → 401
Invalid endpoint → 404
```

---

## Common Mistakes

- Testing only positive scenarios
- Ignoring invalid data testing

---

## Expected Interview Questions

- What is negative testing?
- Why is negative testing important?
- Examples of API negative scenarios?

--------------------------------------------------

# 🧠 8. Best Practices

## What is it

Guidelines for validating and handling API status codes effectively.

---

## Key Components

- Validate all responses
- Include negative testing
- Log failures properly
- Verify error messages

---

## How to Answer (Interview Style)

I validate both success and failure status codes, perform negative testing, and verify meaningful error responses for reliable API validation.

---

## Practical Example

```text
Validate:
- Status Code
- Error Message
- Response Body
```

---

## Common Mistakes

- Validating only success cases
- Ignoring error response body
- Weak assertions

---

## Expected Interview Questions

- How do you validate APIs?
- What negative scenarios do you test?
- Why are status codes important?

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## MOST IMPORTANT TOPICS

1. 401 vs 403 ⭐
2. 4xx vs 5xx ⭐
3. Negative Testing ⭐
4. 200 vs 201 ⭐

--------------------------------------------------

# 🚀 Playwright → API Testing with Playwright

This section covers API testing capabilities in Playwright required for modern SDET and product-company interviews.

--------------------------------------------------

Topics Covered:

1. APIRequestContext
2. HTTP Methods (GET, POST, PUT, DELETE)
3. Request Headers
4. Authentication (Bearer Token)
5. Response Validation
6. Status Code Validation
7. API Chaining
8. UI + API Combined Flow
9. Best Practices

--------------------------------------------------

# 🧠 1. APIRequestContext ⭐

## What is it

APIRequestContext is Playwright’s built-in API testing utility used to send HTTP requests directly without browser interaction.

---

## Key Components

- request
- API context
- HTTP requests
- Base URL

---

## How to Answer (Interview Style)

APIRequestContext in Playwright is used for backend/API testing without launching the browser. It helps perform direct HTTP operations like GET, POST, PUT, and DELETE efficiently.

---

## Practical Example

```javascript
const response = await request.get('/users');
```

---

## Common Mistakes

- Confusing browser page and API request
- Hardcoding endpoints
- Not validating responses

---

## Expected Interview Questions

- What is APIRequestContext?
- Why use API testing in Playwright?
- Difference between UI and API testing?

--------------------------------------------------

# 🧠 2. HTTP Methods (GET, POST, PUT, DELETE)

## What is it

HTTP methods are operations used to interact with APIs.

---

## Key Components

- GET → Fetch data
- POST → Create data
- PUT → Update data
- DELETE → Remove data

---

## How to Answer (Interview Style)

HTTP methods define the type of API operation. GET retrieves data, POST creates data, PUT updates resources, and DELETE removes resources.

---

## Practical Example

```javascript
await request.get('/users');

await request.post('/users', {
  data: {
    name: 'Kalpesh'
  }
});
```

---

## Common Mistakes

- Using wrong HTTP methods
- Not validating response codes
- Sending incorrect payloads

---

## Expected Interview Questions

- Difference between PUT and POST?
- Which HTTP methods have you used?
- What is idempotency?

--------------------------------------------------

# 🧠 3. Request Headers

## What is it

Headers provide additional information in API requests such as authentication and content type.

---

## Key Components

- Authorization
- Content-Type
- Accept
- Custom headers

---

## How to Answer (Interview Style)

Request headers are used to pass metadata such as authentication tokens and content type information during API communication.

---

## Practical Example

```javascript
await request.get('/users', {
  headers: {
    Authorization: 'Bearer token'
  }
});
```

---

## Common Mistakes

- Missing authentication headers
- Incorrect content types
- Hardcoding sensitive tokens

---

## Expected Interview Questions

- What are request headers?
- Why use Authorization header?
- Difference between headers and body?

--------------------------------------------------

# 🧠 4. Authentication (Bearer Token) ⭐

## What is it

Authentication verifies user identity before accessing protected APIs.

---

## Key Components

- Bearer token
- JWT token
- Authorization header
- Session handling

---

## How to Answer (Interview Style)

Bearer token authentication is commonly used in APIs where a token is passed in the Authorization header to access secured endpoints.

---

## Practical Example

```javascript
headers: {
  Authorization: `Bearer ${token}`
}
```

---

## Common Mistakes

- Exposing tokens in code
- Expired tokens
- Incorrect token format

---

## Expected Interview Questions

- What is bearer token authentication?
- How do you handle tokens securely?
- Difference between session and token auth?

--------------------------------------------------

# 🧠 5. Response Validation

## What is it

Validating API response body and returned data.

---

## Key Components

- JSON validation
- Response body
- Field validation
- Schema checks

---

## How to Answer (Interview Style)

Response validation ensures the API returns correct and expected data. I validate fields, response structure, and important business values.

---

## Practical Example

```javascript
const body = await response.json();

expect(body.name).toBe('Kalpesh');
```

---

## Common Mistakes

- Validating only status codes
- Ignoring response body
- Weak assertions

---

## Expected Interview Questions

- How do you validate API responses?
- What validations do you perform?
- Difference between schema and field validation?

--------------------------------------------------

# 🧠 6. Status Code Validation

## What is it

Validating API response status codes.

---

## Key Components

- 200 OK
- 201 Created
- 400 Bad Request
- 401 Unauthorized
- 500 Server Error

---

## How to Answer (Interview Style)

Status code validation confirms whether API operations are successful or failed as expected.

---

## Practical Example

```javascript
expect(response.status()).toBe(200);
```

---

## Common Mistakes

- Ignoring failure codes
- Hardcoding wrong expectations
- Not validating negative scenarios

---

## Expected Interview Questions

- Common HTTP status codes?
- Difference between 401 and 403?
- Why validate status codes?

--------------------------------------------------

# 🧠 7. API Chaining ⭐

## What is it

Using data from one API response in another API request.

---

## Key Components

- Dynamic IDs
- Sequential requests
- Dependency handling

---

## How to Answer (Interview Style)

API chaining is used when one API response provides data required for another API request, such as user IDs or authentication tokens.

---

## Practical Example

```javascript
const createUser = await request.post('/users');

const body = await createUser.json();

await request.get(`/users/${body.id}`);
```

---

## Common Mistakes

- Hardcoding IDs
- Ignoring dependency failures
- Poor response handling

---

## Expected Interview Questions

- What is API chaining?
- Real-time example of chaining?
- Why is chaining important?

--------------------------------------------------

# 🧠 8. UI + API Combined Flow ⭐

## What is it

Combining API and UI testing together for faster and more efficient automation.

---

## Key Components

- Backend setup
- UI validation
- Faster execution
- Reduced UI dependency

---

## How to Answer (Interview Style)

In real-time projects, I use APIs to create or prepare test data and then validate functionality through UI. This improves execution speed and reduces UI dependency.

---

## Practical Example

```javascript
await request.post('/users', {
  data: {
    name: 'Kalpesh'
  }
});

await page.reload();
```

---

## Common Mistakes

- Creating all data through UI
- Ignoring backend validation
- Slow test setup

---

## Expected Interview Questions

- Why combine API and UI testing?
- Real-time use case?
- Benefits of API-driven setup?

--------------------------------------------------

# 🧠 9. Best Practices ⭐

## What is it

Guidelines for writing stable and maintainable API tests.

---

## Key Components

- Reusable request methods
- Proper validations
- Secure token handling
- Avoid hardcoded data

---

## How to Answer (Interview Style)

I focus on reusable API utilities, proper response validations, secure token management, and meaningful assertions to maintain reliable API automation.

---

## Practical Example

```javascript
expect(response.ok()).toBeTruthy();
```

---

## Common Mistakes

- Hardcoded test data
- No negative testing
- Weak assertions

---

## Expected Interview Questions

- API automation best practices?
- How do you secure API tests?
- How do you manage reusable APIs?

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## Most Important API Topics

1. API Chaining ⭐
2. Authentication ⭐
3. Response Validation ⭐
4. UI + API Combined Flow ⭐

---

## Important Validations

| Validation | Purpose |
|------------|----------|
| Status Code | Operation success |
| Response Body | Data correctness |
| Headers | Metadata validation |
| Schema | Structure validation |

--------------------------------------------------

# 🚀 API Automation → Headers & Authentication

This is one of the highest-value API interview topics.

Interviewers ask this to check:
- Security understanding
- Real-time API experience
- Authentication knowledge

--------------------------------------------------

Topics Covered:

1. What are Headers
2. Types of Headers
3. Authentication Basics
4. Bearer Token Authentication
5. Basic Authentication
6. API Keys
7. OAuth Basics
8. Real-Time Scenarios
9. Security Best Practices
10. Common Interview Questions

--------------------------------------------------

# 🧠 1. What are Headers

## What is it

Headers are key-value pairs sent between client and server containing metadata about the request or response.

---

## Key Components

- Authorization
- Content-Type
- Accept
- Cookies
- Custom headers

---

## How to Answer (Interview Style)

Headers provide additional information about API requests and responses such as authentication, content type, and communication preferences.

---

## Practical Example

```text
Content-Type: application/json
Authorization: Bearer token
```

---

## Common Mistakes

- Missing mandatory headers
- Wrong content type
- Exposing sensitive data

---

## Expected Interview Questions

- What are headers?
- Why are headers important?
- Common headers used in APIs?

--------------------------------------------------

# 🧠 2. Types of Headers

## What is it

Different categories of headers used during API communication.

---

## Key Components

- Request headers
- Response headers
- General headers
- Security headers

---

## How to Answer (Interview Style)

Request headers are sent from client to server, while response headers are returned by server to provide metadata about the response.

---

## Practical Example

```text
Request Header:
Authorization: Bearer token

Response Header:
Content-Type: application/json
```

---

## Common Mistakes

- Confusing request and response headers
- Ignoring response header validations

---

## Expected Interview Questions

- Difference between request and response headers?
- Which headers have you validated?
- Why validate Content-Type?

--------------------------------------------------

# 🧠 3. Authentication Basics ⭐

## What is it

Authentication verifies user or system identity before granting API access.

---

## Key Components

- Username/password
- Tokens
- API keys
- OAuth

---

## How to Answer (Interview Style)

Authentication ensures only authorized users or systems can access secured APIs using credentials, tokens, or authentication mechanisms.

---

## Practical Example

```text
Login API → Token Generated → Access Secured APIs
```

---

## Common Mistakes

- Exposing credentials in code
- Ignoring token expiration
- Weak security practices

---

## Expected Interview Questions

- What is API authentication?
- Why authentication is important?
- Types of API authentication?

--------------------------------------------------

# 🧠 4. Bearer Token Authentication ⭐

## What is it

Bearer token authentication uses tokens passed in Authorization header to access protected APIs.

---

## Key Components

- JWT token
- Authorization header
- Token expiration
- Secure access

---

## How to Answer (Interview Style)

Bearer token authentication is widely used in REST APIs where tokens are passed in Authorization headers for secure API access.

---

## Practical Example

```text
Authorization: Bearer eyJhbGci...
```

---

## Common Mistakes

- Hardcoding tokens
- Using expired tokens
- Incorrect token format

---

## Expected Interview Questions

- What is bearer token?
- How do you handle token authentication?
- Difference between session and token auth?

--------------------------------------------------

# 🧠 5. Basic Authentication

## What is it

Basic authentication uses username and password encoded in request headers.

---

## Key Components

- Username
- Password
- Base64 encoding

---

## How to Answer (Interview Style)

Basic authentication sends encoded username and password in headers for authentication, but it is less secure compared to token-based authentication.

---

## Practical Example

```text
Authorization: Basic dXNlcjpwYXNz
```

---

## Common Mistakes

- Sending credentials without HTTPS
- Confusing encoding with encryption

---

## Expected Interview Questions

- What is basic authentication?
- Why bearer token is preferred?
- Difference between encoding and encryption?

--------------------------------------------------

# 🧠 6. API Keys

## What is it

API keys are unique identifiers used to authenticate API consumers.

---

## Key Components

- API key
- Access control
- Usage tracking

---

## How to Answer (Interview Style)

API keys are unique identifiers used for authentication and tracking API usage by applications or users.

---

## Practical Example

```text
x-api-key: abc123xyz
```

---

## Common Mistakes

- Exposing API keys publicly
- Hardcoding keys in repository

---

## Expected Interview Questions

- What are API keys?
- Difference between API key and token?
- Why secure API keys?

--------------------------------------------------

# 🧠 7. OAuth Basics ⭐

## What is it

OAuth is an authorization framework that allows secure third-party access without exposing passwords.

---

## Key Components

- Access token
- Authorization server
- Client application
- Resource owner

---

## How to Answer (Interview Style)

OAuth allows secure authorization between applications using tokens instead of sharing user credentials directly.

---

## Practical Example

```text
Login with Google
```

---

## Common Mistakes

- Confusing OAuth with authentication only
- Not understanding token flow

---

## Expected Interview Questions

- What is OAuth?
- Why OAuth is used?
- Difference between OAuth and basic auth?

--------------------------------------------------

# 🧠 8. Real-Time Scenarios ⭐

## 1. Login Flow

```text
Login API → Generate JWT Token
```

---

## 2. Secured API Access

```text
Authorization: Bearer token
```

---

## 3. Third-Party Login

```text
OAuth → Login with Google
```

--------------------------------------------------

# 🧠 9. Security Best Practices ⭐

## What is it

Guidelines for secure API communication and authentication handling.

---

## Key Components

- Avoid hardcoding credentials
- Use HTTPS
- Secure token handling
- Token expiration management

---

## How to Answer (Interview Style)

I follow secure authentication practices such as using HTTPS, avoiding hardcoded credentials, and managing tokens securely.

---

## Practical Example

```text
Store tokens securely
Use environment variables
```

---

## Common Mistakes

- Hardcoded passwords
- Exposed tokens in logs
- Weak security validation

---

## Expected Interview Questions

- How do you secure API tests?
- Why use HTTPS?
- Best practices for token handling?

--------------------------------------------------

# 🧠 10. Common Interview Questions ⭐

- What are request headers?
- Difference between authentication and authorization?
- What is bearer token?
- Difference between API key and token?
- Why OAuth is used?
- Difference between Basic Auth and Bearer Token?

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## MOST IMPORTANT TOPICS

1. Bearer Token ⭐
2. Authentication vs Authorization ⭐
3. API Keys vs OAuth ⭐
4. Security Best Practices ⭐

--------------------------------------------------

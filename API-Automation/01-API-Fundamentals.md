# 🚀 API Automation → API Fundamentals

This is the foundation of all API testing and backend automation.

--------------------------------------------------

Topics Covered:

1. What is API
2. Types of APIs
3. API Architecture
4. Client-Server Communication
5. REST API Basics
6. JSON Basics
7. Real-Time Flow
8. Best Practices

--------------------------------------------------

# 🧠 1. What is API

## What is it

API (Application Programming Interface) is a medium that allows two applications or systems to communicate with each other.

---

## Key Components

- Request
- Response
- Endpoint
- Client
- Server

---

## How to Answer (Interview Style)

API acts as a bridge between client and server. It allows applications to exchange data using requests and responses without directly accessing internal implementation.

---

## Practical Example

```text
Mobile App → API → Database
```

Example:

```text
PhonePe app sends payment request to backend API.
```

---

## Common Mistakes

- Saying API is only for testing
- Confusing API with database
- Ignoring request-response flow

---

## Expected Interview Questions

- What is API?
- Why are APIs used?
- Real-time API example?

--------------------------------------------------

# 🧠 2. Types of APIs

## What is it

Different API categories based on accessibility and architecture.

---

## Key Components

- REST API
- SOAP API
- GraphQL API
- Internal API
- Public API

---

## How to Answer (Interview Style)

REST APIs are most commonly used in modern applications because they are lightweight and use JSON for communication. SOAP APIs are XML-based and more strict.

---

## Practical Example

```text
REST API → JSON
SOAP API → XML
```

---

## Common Mistakes

- Not knowing REST vs SOAP
- Saying SOAP is modern standard
- Ignoring GraphQL basics

---

## Expected Interview Questions

- Difference between REST and SOAP?
- What APIs have you worked on?
- Why REST is popular?

--------------------------------------------------

# 🧠 3. API Architecture

## What is it

API architecture defines how APIs are designed and communicate.

---

## Key Components

- Client
- Server
- Endpoint
- HTTP Protocol
- Request/Response

---

## How to Answer (Interview Style)

API architecture follows a client-server model where the client sends requests and the server processes and returns responses over HTTP protocol.

---

## Practical Example

```text
Client → HTTP Request → Server
Server → HTTP Response → Client
```

---

## Common Mistakes

- Confusing frontend and backend roles
- Not understanding stateless communication

---

## Expected Interview Questions

- Explain API architecture.
- What is client-server communication?
- What protocol APIs use?

--------------------------------------------------

# 🧠 4. Client-Server Communication

## What is it

Communication model where client sends requests and server returns responses.

---

## Key Components

- Request
- Response
- HTTP
- Status Code
- Data Exchange

---

## How to Answer (Interview Style)

In client-server communication, the client sends HTTP requests to the server, and the server processes the request and returns a response with status code and data.

---

## Practical Example

```text
Browser → Login Request → Server
Server → Authentication Response → Browser
```

---

## Common Mistakes

- Ignoring status codes
- Confusing request and response

---

## Expected Interview Questions

- Explain request-response cycle.
- What happens when API is called?
- What is stateless communication?

--------------------------------------------------

# 🧠 5. REST API Basics ⭐

## What is it

REST (Representational State Transfer) is a lightweight architecture used for API communication over HTTP.

---

## Key Components

- HTTP methods
- Stateless
- JSON
- Resource-based URLs

---

## How to Answer (Interview Style)

REST APIs use HTTP methods like GET, POST, PUT, and DELETE for communication. They are lightweight, stateless, and mostly use JSON data format.

---

## Practical Example

```text
GET /users
POST /users
PUT /users/1
DELETE /users/1
```

---

## Common Mistakes

- Not understanding statelessness
- Confusing REST with HTTP
- Ignoring resource-based design

---

## Expected Interview Questions

- What is REST API?
- Why REST is widely used?
- What is stateless API?

--------------------------------------------------

# 🧠 6. JSON Basics

## What is it

JSON (JavaScript Object Notation) is a lightweight data format used in APIs.

---

## Key Components

- Key-value pairs
- Objects
- Arrays
- Nested JSON

---

## How to Answer (Interview Style)

JSON is a lightweight and readable data format used for request and response communication in REST APIs.

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

- Invalid JSON syntax
- Confusing object and array

---

## Expected Interview Questions

- What is JSON?
- Why JSON is preferred?
- Difference between JSON object and array?

--------------------------------------------------

# 🧠 7. Real-Time API Flow ⭐

## What is it

Understanding how APIs work in real applications.

---

## Key Components

- Frontend
- Backend
- Database
- API layer

---

## How to Answer (Interview Style)

In real-time applications, frontend sends requests to backend APIs, APIs process business logic, interact with database, and return responses to frontend.

---

## Practical Example

```text
Mobile App
   ↓
API Layer
   ↓
Database
```

---

## Common Mistakes

- Thinking frontend directly accesses database
- Ignoring backend processing

---

## Expected Interview Questions

- Explain real-time API flow.
- How frontend communicates with backend?
- Where APIs fit in architecture?

--------------------------------------------------

# 🧠 8. Best Practices

## What is it

Guidelines for understanding and testing APIs effectively.

---

## Key Components

- Proper validations
- Understanding architecture
- Response verification
- Error handling

---

## How to Answer (Interview Style)

I focus on understanding request-response flow, validating responses correctly, and using proper API structures for maintainable testing.

---

## Practical Example

```text
Validate:
- Status Code
- Response Body
- Headers
- Response Time
```

---

## Common Mistakes

- Only validating status codes
- Ignoring negative testing
- Weak validations

---

## Expected Interview Questions

- API testing best practices?
- What validations do you perform?
- How do you test APIs effectively?

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## MOST IMPORTANT TOPICS

1. REST API ⭐
2. Request-Response Flow ⭐
3. JSON Basics ⭐
4. Real-Time Architecture ⭐

--------------------------------------------------

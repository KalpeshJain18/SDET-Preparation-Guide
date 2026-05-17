# 🚀 API Automation → HTTP Methods

This is one of the most important API interview topics.

Almost every API interview starts from here.

--------------------------------------------------

Topics Covered:

1. GET Method
2. POST Method
3. PUT Method
4. DELETE Method
5. PATCH Method
6. Idempotency
7. Real-Time Scenarios
8. Best Practices

--------------------------------------------------

# 🧠 1. GET Method

## What is it

GET method is used to retrieve/fetch data from the server.

---

## Key Components

- Read operation
- No request body
- Query parameters
- Safe operation

---

## How to Answer (Interview Style)

GET method is used to fetch data from the server without modifying resources. It is commonly used for retrieving user details, reports, or records.

---

## Practical Example

```text
GET /users
GET /orders/101
```

---

## Common Mistakes

- Sending body in GET request
- Using GET for update operations
- Ignoring query parameters

---

## Expected Interview Questions

- What is GET method?
- Can GET modify data?
- Difference between GET and POST?

--------------------------------------------------

# 🧠 2. POST Method ⭐

## What is it

POST method is used to create new resources/data on the server.

---

## Key Components

- Create operation
- Request body
- JSON payload
- Data submission

---

## How to Answer (Interview Style)

POST method is used to send data to the server for creating resources such as users, orders, or transactions.

---

## Practical Example

```text
POST /users
```

Request Body:

```json
{
  "name": "Kalpesh",
  "role": "SDET"
}
```

---

## Common Mistakes

- Missing request body
- Invalid JSON format
- Not validating response

---

## Expected Interview Questions

- What is POST method?
- Why POST is not idempotent?
- Difference between POST and PUT?

--------------------------------------------------

# 🧠 3. PUT Method ⭐

## What is it

PUT method is used to update existing resources completely.

---

## Key Components

- Update operation
- Full resource update
- Idempotent operation

---

## How to Answer (Interview Style)

PUT method updates an existing resource completely. Sending the same PUT request multiple times produces the same result.

---

## Practical Example

```text
PUT /users/1
```

---

## Common Mistakes

- Using PUT for partial updates
- Confusing PUT and PATCH

---

## Expected Interview Questions

- Difference between PUT and POST?
- Why PUT is idempotent?
- Real-time PUT example?

--------------------------------------------------

# 🧠 4. DELETE Method

## What is it

DELETE method removes resources/data from the server.

---

## Key Components

- Delete operation
- Resource removal
- Permanent deletion

---

## How to Answer (Interview Style)

DELETE method removes existing resources from the server such as deleting users, records, or transactions.

---

## Practical Example

```text
DELETE /users/1
```

---

## Common Mistakes

- Deleting wrong resources
- Ignoring authorization validation

---

## Expected Interview Questions

- What is DELETE method?
- How do you validate delete operations?
- Real-time delete scenario?

--------------------------------------------------

# 🧠 5. PATCH Method

## What is it

PATCH method is used for partial updates of resources.

---

## Key Components

- Partial update
- Lightweight update
- Specific field modification

---

## How to Answer (Interview Style)

PATCH method updates only specific fields of a resource instead of replacing the entire object.

---

## Practical Example

```text
PATCH /users/1
```

---

## Common Mistakes

- Confusing PATCH with PUT
- Sending full payload unnecessarily

---

## Expected Interview Questions

- Difference between PUT and PATCH?
- Why PATCH is useful?
- Real-time PATCH example?

--------------------------------------------------

# 🧠 6. Idempotency ⭐

## What is it

Idempotency means performing the same operation multiple times gives the same result.

---

## Key Components

- Repeatable operation
- Same result
- Resource consistency

---

## How to Answer (Interview Style)

Idempotent APIs return the same result even if the same request is executed multiple times. GET, PUT, and DELETE are generally idempotent, while POST is not.

---

## Practical Example

```text
PUT /users/1
```

Sending same request multiple times:
→ Same final state

---

## Common Mistakes

- Saying POST is idempotent
- Confusing response and state

---

## Expected Interview Questions

- What is idempotency?
- Which HTTP methods are idempotent?
- Why POST is not idempotent?

--------------------------------------------------

# 🧠 7. Real-Time Scenarios ⭐

## 1. User Registration

```text
POST /users
```

---

## 2. Fetch User Details

```text
GET /users/1
```

---

## 3. Update Profile

```text
PUT /users/1
```

---

## 4. Delete Account

```text
DELETE /users/1
```

--------------------------------------------------

# 🧠 8. Best Practices

## What is it

Guidelines for using HTTP methods properly in APIs.

---

## Key Components

- Correct method usage
- Proper validations
- Resource-based APIs
- Secure operations

---

## How to Answer (Interview Style)

I ensure correct HTTP method usage, proper validations, and meaningful assertions to maintain API reliability and clarity.

---

## Practical Example

```text
GET → Fetch
POST → Create
PUT → Update
DELETE → Remove
```

---

## Common Mistakes

- Wrong HTTP method usage
- Ignoring status code validations
- Weak API design understanding

---

## Expected Interview Questions

- Explain all HTTP methods.
- Which methods are idempotent?
- Difference between PUT and PATCH?

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## MOST IMPORTANT TOPICS

1. POST vs PUT ⭐
2. Idempotency ⭐
3. PUT vs PATCH ⭐
4. Real-time CRUD operations ⭐

--------------------------------------------------

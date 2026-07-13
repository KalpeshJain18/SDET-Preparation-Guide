# 🚀 Automation Framework for SDET → Screenshots on Failure ⭐

Screenshots on Failure is one of the MOST IMPORTANT topics for:
- SDET Interviews
- Playwright Framework Design
- Selenium Framework Design
- Enterprise Automation Projects
- Debugging Failed Test Cases

Interviewers frequently ask:
- How do you capture screenshots on failure?
- Why are screenshots important?
- Where are screenshots stored?
- How do screenshots integrate with reports?
- How do you capture screenshots in Playwright?

--------------------------------------------------

# 🎯 Topics Covered

1. What are Screenshots on Failure?
2. Why Screenshots are Important
3. Types of Screenshots
4. Screenshot Capture Flow
5. Screenshot Naming Strategy
6. Integration with Reports
7. Real-Time Enterprise Screenshot Handling
8. Common Mistakes
9. Common Interview Questions
10. Best Practices

--------------------------------------------------

# 🧠 1. What are Screenshots on Failure?

## What is it

Screenshots on Failure is an automation framework feature that automatically captures the application screen whenever a test case fails.

The captured screenshot shows the exact state of the application at the moment of failure, making it easier to identify UI issues, unexpected behaviors, missing elements, or incorrect data.

In enterprise frameworks, screenshots are usually attached to HTML or Allure reports for easier debugging.

---

## Key Components

- Automatic Screenshot Capture
- Failure Detection
- Screenshot Storage
- Screenshot Attachment
- Timestamp-based Naming
- Report Integration

---

## How to Answer (Interview Style)

Screenshots on Failure is a framework feature that automatically captures the browser screen whenever a test fails. It provides visual evidence of the application's state and significantly reduces debugging time by helping engineers identify the root cause of failures.

---

## Practical Example

```text
Login Test

↓

Enter Username

↓

Click Login

↓

Dashboard Not Loaded

↓

Capture Screenshot

↓

Attach to HTML Report
```

---

## Common Mistakes

- Capturing screenshots after the browser closes
- Capturing screenshots for every test step
- Overwriting screenshots with the same filename

---

## Expected Interview Questions

- What are Screenshots on Failure?
- Why do we capture screenshots?
- How are screenshots useful during debugging?

--------------------------------------------------

# 🧠 2. Why Screenshots are Important ⭐

## What is it

Screenshots provide visual proof of application failures, helping QA engineers and developers understand exactly what happened without reproducing the issue.

---

## Key Components

- Faster Debugging
- Visual Evidence
- Easier Defect Reporting
- Better Communication
- Historical Reference
- Faster Root Cause Analysis

---

## How to Answer (Interview Style)

Screenshots help engineers understand the exact UI state when a test fails. They reduce debugging time, improve defect reporting, and make communication between QA and developers more efficient.

---

## Practical Example

```text
Checkout Button Missing

↓

Screenshot Captured

↓

Developer Opens Screenshot

↓

UI Issue Identified
```

---

## Benefits

- Reduces debugging effort
- Improves defect quality
- Useful for remote teams
- Helps analyze intermittent failures
- Supports audit and historical analysis

---

## Common Mistakes

- Not capturing screenshots for failed tests
- Capturing low-quality screenshots

---

## Expected Interview Questions

- Why are screenshots important?
- What are the advantages of screenshots?

--------------------------------------------------

# 🧠 3. Types of Screenshots ⭐

## Common Types

### Full Page Screenshot

Captures the complete webpage, including content outside the visible viewport.

Example

```text
Entire Checkout Page Captured
```

---

### Viewport Screenshot

Captures only the currently visible browser window.

Example

```text
Visible Login Screen Captured
```

---

### Element Screenshot

Captures only a specific UI element.

Example

```text
Login Button Screenshot
```

---

### Failure Screenshot

Automatically captured whenever a test fails.

Example

```text
Dashboard Validation Failed

↓

Failure Screenshot Saved
```

---

### Manual Screenshot

Captured intentionally during execution for verification or documentation.

---

## How to Answer (Interview Style)

Depending on the scenario, automation frameworks can capture full-page, viewport, element-level, or failure screenshots. Failure screenshots are the most commonly used in enterprise automation.

---

## Common Mistakes

- Always taking full-page screenshots when not required
- Capturing screenshots without context

---

## Expected Interview Questions

- Which screenshot types have you used?
- Difference between full-page and viewport screenshots?

--------------------------------------------------

# 🧠 4. Screenshot Capture Flow ⭐

## Framework Execution Flow

```text
Start Test

↓

Execute Test Steps

↓

Validation Fails

↓

Capture Screenshot

↓

Save Screenshot

↓

Attach to Report

↓

Generate Report
```

---

## How to Answer (Interview Style)

Whenever a validation fails or an exception occurs, the framework automatically captures a screenshot before browser cleanup and attaches it to the execution report.

---

## Practical Example

```text
Login Test

↓

Dashboard Validation Failed

↓

Capture Screenshot

↓

Generate HTML Report

↓

Close Browser
```

---

## Common Mistakes

- Capturing screenshots after browser closure
- Missing exception handling during screenshot capture

---

## Expected Interview Questions

- Explain screenshot capture flow.
- When should screenshots be captured?

--------------------------------------------------

# 🧠 5. Screenshot Naming Strategy ⭐

## What is it

A proper naming convention prevents screenshots from being overwritten and makes them easy to identify.

---

## Recommended Naming Convention

```text
<TestName>_<Browser>_<Environment>_<Timestamp>.png
```

---

## Example

```text
LoginTest_Chrome_QA_2026-07-13_10-45-22.png
```

---

## Why Naming Matters

- Prevents overwriting
- Easy identification
- Better organization
- Faster debugging
- Easy report integration

---

## Folder Structure Example

```text
screenshots/

Login/

Checkout/

Dashboard/

API/
```

---

## Common Mistakes

- Generic names like screenshot.png
- Missing timestamps

---

## Expected Interview Questions

- How do you name screenshots?
- Why should screenshots have timestamps?

--------------------------------------------------

# 🧠 6. Integration with Reports ⭐

## What is it

Modern reporting tools automatically attach screenshots to failed test cases.

This allows anyone reviewing the report to click and view the screenshot immediately.

---

## Integration Flow

```text
Test Failure

↓

Capture Screenshot

↓

Save Screenshot

↓

Attach to HTML / Allure Report

↓

Report Published
```

---

## Practical Example

```text
Login Failed

↓

Screenshot Attached

↓

HTML Report

↓

Click Screenshot

↓

View Failure
```

---

## Reporting Tools Supporting Screenshots

- Playwright HTML Reporter
- Allure Report
- Extent Reports
- ReportNG

---

## Common Mistakes

- Saving screenshots without attaching them
- Broken screenshot links in reports

---

## Expected Interview Questions

- How do screenshots integrate with reports?
- Which reporting tools support screenshots?

--------------------------------------------------

# 🧠 7. Real-Time Enterprise Screenshot Handling ⭐

## Enterprise Folder Structure

```text
framework/

├── screenshots/
│   ├── Login/
│   ├── Checkout/
│   ├── Dashboard/
│   ├── API/
│   └── Failed/
│
├── reports/
│
└── logs/
```

---

## Enterprise CI/CD Flow

```text
Developer Pushes Code

↓

GitHub Actions / Jenkins

↓

Execute Tests

↓

Capture Failure Screenshot

↓

Generate HTML Report

↓

Upload Report & Screenshots

↓

Slack / Email Notification
```

---

## Enterprise Example

```text
Nightly Regression

↓

300 Test Cases

↓

5 Failed

↓

5 Screenshots Captured

↓

Published in Allure Report
```

---

## Common Mistakes

- Storing screenshots inside source code
- Never deleting old screenshots
- No screenshot organization

---

## Expected Interview Questions

- How are screenshots managed in enterprise frameworks?
- Where are screenshots stored?

--------------------------------------------------

# 🧠 8. Common Mistakes ⭐

- Capturing screenshots after browser closure
- Overwriting screenshots
- Generic screenshot names
- Capturing every step unnecessarily
- Storing screenshots in Git repository
- Missing report integration
- No cleanup strategy

--------------------------------------------------

# 🧠 9. Common Interview Questions ⭐

- How do you capture screenshots on failure?
- Why are screenshots important?
- Where are screenshots stored?
- How do screenshots integrate with reports?
- Difference between Full Page and Viewport screenshots?
- Which Playwright method is used for screenshots?
- How are screenshots handled in CI/CD?

--------------------------------------------------

# 🧠 10. Best Practices ⭐

- Capture screenshots automatically on failures.
- Capture screenshots before closing the browser.
- Use timestamp-based naming conventions.
- Store screenshots outside source code folders.
- Attach screenshots to reports automatically.
- Archive screenshots in CI/CD pipelines.
- Organize screenshots by module or execution.
- Clean old screenshots periodically.
- Avoid capturing unnecessary screenshots.
- Never store screenshots containing sensitive information.

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## MOST IMPORTANT TOPICS

1. Screenshots on Failure ⭐
2. Types of Screenshots ⭐
3. Screenshot Capture Flow ⭐
4. Screenshot Naming Strategy ⭐
5. Report Integration ⭐
6. Enterprise Screenshot Handling ⭐
7. Screenshot Best Practices ⭐

--------------------------------------------------

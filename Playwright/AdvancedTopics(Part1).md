# 🚀 Playwright → Advanced Topics (Part 1)

This section covers advanced real-time scenarios asked in SDET and product-company interviews.

--------------------------------------------------

Topics Covered:

1. Handling Frames
2. Handling Multiple Tabs / Windows
3. File Upload & Download

--------------------------------------------------

# 🧠 1. Handling Frames

## What is it

Frames (iframes) are embedded HTML documents inside a web page. Playwright provides specific methods to interact with elements inside frames.

---

## Key Components

- iframe
- frameLocator()
- Nested frames
- Frame isolation

---

## How to Answer (Interview Style)

Frames are embedded web documents inside a page. In Playwright, I use frameLocator() to interact with elements inside iframes because normal locators cannot directly access frame elements.

---

## Practical Example

```javascript
await page.frameLocator('#login-frame')
  .locator('#username')
  .fill('Kalpesh');
```

---

## Common Mistakes

- Trying to access iframe elements directly
- Using normal locators without frameLocator()
- Ignoring nested frames

---

## Expected Interview Questions

- What is iframe?
- How do you handle frames in Playwright?
- Difference between page locator and frame locator?

--------------------------------------------------

# 🧠 2. Handling Multiple Tabs / Windows ⭐

## What is it

Handling scenarios where clicking an element opens a new browser tab or window.

---

## Key Components

- context.waitForEvent()
- New page event
- Switching tabs
- Browser context

---

## How to Answer (Interview Style)

In Playwright, multiple tabs are handled using browser context and page events. I use context.waitForEvent('page') to capture and switch to newly opened tabs.

---

## Practical Example

```javascript
const [newPage] = await Promise.all([
  context.waitForEvent('page'),
  page.click('#open-tab')
]);

await newPage.waitForLoadState();
```

---

## Common Mistakes

- Not waiting for new page event
- Confusing browser context and page
- Hardcoding tab switching logic

---

## Expected Interview Questions

- How do you handle multiple tabs in Playwright?
- Difference between context and page?
- How do you switch between tabs?

--------------------------------------------------

# 🧠 3. File Upload & Download

## What is it

Handling file upload and file download scenarios in automation testing.

---

## Key Components

- setInputFiles()
- Download event
- File path handling
- Upload validation

---

## How to Answer (Interview Style)

Playwright provides built-in support for file upload and download handling. I use setInputFiles() for uploads and download event listeners for validating downloaded files.

---

## Practical Example

### File Upload

```javascript
await page.locator('input[type="file"]')
  .setInputFiles('test-data/sample.pdf');
```

---

### File Download

```javascript
const downloadPromise = page.waitForEvent('download');

await page.click('#download-btn');

const download = await downloadPromise;
```

---

## Common Mistakes

- Using OS-level automation unnecessarily
- Hardcoding file paths
- Not validating downloaded file

---

## Expected Interview Questions

- How do you upload files in Playwright?
- How do you validate downloads?
- Difference between Selenium and Playwright file handling?

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## Advanced Scenario Priority

1. Multiple Tabs ⭐
2. Frames
3. File Upload/Download

---

## Important Concepts to Remember

| Concept | Key Point |
|----------|------------|
| frameLocator() | Used for iframe handling |
| context.waitForEvent('page') | Used for new tabs |
| setInputFiles() | Used for uploads |

--------------------------------------------------

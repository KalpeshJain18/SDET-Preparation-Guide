# 🚀 Playwright → Core Concepts (Complete Guide)

This section covers the fundamental building blocks of Playwright required for SDET interviews.

--------------------------------------------------

Topics Covered:

1. Architecture  
2. Installation & Project Setup  
3. Test Runner (test, expect)  
4. Browser Context & Page  

--------------------------------------------------

1. Playwright Architecture

What is it:
Playwright architecture defines how tests interact with browsers using a Node.js layer and browser engines like Chromium, Firefox, and WebKit.

Key Components:
- Test Script  
- Playwright API  
- Browser Server  
- Browser Engines (Chromium, Firefox, WebKit)  
- Browser Context  
- Page  

How to Answer (Interview):
Playwright follows a client-server architecture where test scripts communicate with browser engines using Playwright APIs. It supports multiple browsers and uses browser contexts for isolated execution.

Practical Example:

```javascript
import { test } from '@playwright/test';

test('basic test', async ({ page }) => {
  await page.goto('https://example.com');
});
```

Flow:
Test Script → Playwright API → Browser → Execution  

Common Mistakes:
- Saying Playwright works only on Chrome  
- Not mentioning browser context  
- Over-explaining internals  

Expected Interview Questions:
- What is Playwright architecture?  
- How is it different from Selenium?  
- What is browser context?  

--------------------------------------------------

2. Installation & Project Setup

What is it:
Setting up Playwright using Node.js and installing required dependencies.

Key Components:
- Node.js  
- npm  
- @playwright/test  
- Browser installation  
- Project structure  

How to Answer (Interview):
I set up Playwright using Node.js by installing @playwright/test via npm, then install browser binaries and create a test structure.

Practical Example:

```bash
npm init -y
npm install -D @playwright/test
npx playwright install
```

Project Structure:

```text
project-root/
├── tests/
├── node_modules/
├── package.json
├── playwright.config.js
```

Common Mistakes:
- Thinking Playwright needs Selenium  
- Not knowing commands  
- Not understanding structure  

Expected Interview Questions:
- How do you install Playwright?  
- What is project structure?  

--------------------------------------------------

3. Test Runner (test, expect)

What is it:
Playwright provides a built-in test runner to execute tests and perform assertions.

Key Components:
- test()  
- expect()  
- hooks (beforeEach, afterEach)  
- fixtures  

How to Answer (Interview):
Playwright test runner allows defining test cases using test() and validating using expect(). It also supports hooks and fixtures.

Practical Example:

```javascript
import { test, expect } from '@playwright/test';

test('title validation', async ({ page }) => {
  await page.goto('https://example.com');
  await expect(page).toHaveTitle(/Example/);
});
```

Common Mistakes:
- Confusing test() with function  
- Not understanding expect()  
- Ignoring hooks  

Expected Interview Questions:
- What is test()?  
- What is expect()?  
- What are hooks?  

--------------------------------------------------

4. Browser Context & Page

What is it:
Browser context is an isolated session, and page represents a browser tab.

Key Components:
- Browser  
- Context  
- Page  

How to Answer (Interview):
Browser context is like an incognito session, and page represents a tab. It helps in running tests independently.

Practical Example:

```javascript
const context = await browser.newContext();
const page = await context.newPage();
```

Common Mistakes:
- Confusing browser and context  
- Not understanding isolation  
- Mixing page and context  

Expected Interview Questions:
- What is browser context?  
- Difference between browser and context?  
- Why context is important?  

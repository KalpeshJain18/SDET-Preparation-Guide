****🚀 Playwright → Core Concepts (Complete)

We will cover:

1. Architecture  
2. Installation & Project Setup  
3. Test Runner (test, expect)  
4. Browser Context & Page  

---

🧠 1. Playwright Architecture

What is it
Playwright architecture defines how tests interact with browsers using a Node.js layer and browser engines like Chromium, Firefox, and WebKit.

Key Components
- Test Script
- Playwright API
- Browser Server
- Browser Engines
- Browser Context
- Page

How to Answer (Interview)
Playwright follows a client-server architecture where test scripts communicate with browser engines using Playwright APIs. It supports multiple browsers and uses browser contexts for isolated execution.

Practical Example
```javascript**
test('example', async ({ page }) => {
  await page.goto('https://example.com');
});
Common Mistakes
Saying Playwright works only on Chrome
Not mentioning browser context
Over-explaining internals
Interview Questions
What is Playwright architecture?
How is it different from Selenium?
What is browser context?

⚙️ 2. Installation & Project Setup
What is it

Setting up Playwright using Node.js and installing dependencies.

Key Components
Node.js
npm
@playwright/test
Browser installation
Project structure
How to Answer (Interview)

I install Playwright using npm, set up the project structure, and install browser binaries using Playwright commands.

Practical Example
npm init -y
npm install -D @playwright/test
npx playwright install
Common Mistakes
Thinking Playwright needs Selenium
Not knowing commands
Not understanding project structure
Interview Questions
How do you install Playwright?
What are prerequisites?
What is project structure?

🧪 3. Test Runner (test, expect)
What is it

Playwright provides a built-in test runner to execute tests and perform assertions.

Key Components
test()
expect()
hooks (beforeEach, afterEach)
fixtures
How to Answer (Interview)

Playwright test runner allows us to define test cases using test() and validate using expect(). It also supports hooks and fixtures for better structure.

Practical Example
test('title check', async ({ page }) => {
  await page.goto('https://example.com');
  await expect(page).toHaveTitle(/Example/);
});
Common Mistakes
Confusing test() with function
Not understanding expect()
Ignoring hooks
Interview Questions
What is test()?
What is expect()?
What are hooks?

🌐 4. Browser Context & Page
What is it

Browser context is an isolated session, and page represents a browser tab.

Key Components
Browser
Context
Page
How to Answer (Interview)

Browser context is like an incognito session, and page represents a single tab. It helps in running tests independently without affecting each other.

Practical Example
const context = await browser.newContext();
const page = await context.newPage();
Common Mistakes
Confusing browser and context
Not understanding isolation
Mixing page and context
Interview Questions
What is browser context?
Difference between browser and context?
Why context is important?

**

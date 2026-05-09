# 🚀 Playwright → Locators (Complete Guide)

This section covers all locator strategies in Playwright required for SDET interviews.

--------------------------------------------------

Topics Covered:

1. locator()  
2. getByRole() ⭐  
3. getByText()  
4. CSS & XPath  
5. Best Practices  

--------------------------------------------------

1. locator()

What is it:
locator() is a Playwright method used to locate elements using selectors like CSS, XPath, id, class, etc.

Key Components:
- CSS selectors (#id, .class)
- XPath
- Chaining (locator().locator())
- Auto-waiting

How to Answer (Interview):
locator() is a flexible method in Playwright used to identify elements using CSS or XPath selectors. It supports auto-waiting and allows chaining for precise element selection.

Practical Example:

```javascript
await page.locator('#username').fill('Kalpesh');
await page.locator('.login-btn').click();
```

Common Mistakes:
- Using long XPath unnecessarily
- Not using chaining
- Over-relying on CSS when better locators exist

Expected Interview Questions:
- What is locator() in Playwright?
- Difference between locator() and Selenium findElement?
- What are advantages of locator()?

--------------------------------------------------

2. getByRole() ⭐ (MOST IMPORTANT)

What is it:
getByRole() is used to locate elements based on accessibility roles (ARIA roles), making tests more stable and user-centric.

Key Components:
- Role (button, textbox, link)
- Name (visible label)
- Accessibility tree

How to Answer (Interview):
getByRole() is the most recommended locator in Playwright because it uses accessibility roles, making tests more reliable, readable, and aligned with real user behavior.

Practical Example:

```javascript
await page.getByRole('button', { name: 'Login' }).click();
await page.getByRole('textbox', { name: 'Username' }).fill('Kalpesh');
```

Common Mistakes:
- Ignoring role-based locators
- Using XPath instead of semantic locators
- Not understanding accessibility

Expected Interview Questions:
- Why is getByRole preferred over locator()?
- What is ARIA role?
- How does Playwright use accessibility?

--------------------------------------------------

3. getByText()

What is it:
getByText() is used to locate elements using visible text on the page.

Key Components:
- Exact text match
- Partial text match
- Case sensitivity

How to Answer (Interview):
getByText() is useful for locating elements based on visible text. It is simple to use but should be used carefully as UI text can change frequently.

Practical Example:

```javascript
await page.getByText('Login').click();
await page.getByText('Submit').click();
```

Common Mistakes:
- Overusing text locators
- Not handling dynamic text
- Using when role-based locator is better

Expected Interview Questions:
- When to use getByText()?
- What are limitations of text-based locators?

--------------------------------------------------

4. CSS & XPath

What is it:
CSS and XPath are traditional selector strategies used to locate elements in DOM.

Key Components:
- CSS (#id, .class, tag)
- XPath (//, contains(), text())

How to Answer (Interview):
CSS and XPath are fallback locator strategies. CSS is faster and preferred over XPath, but XPath is useful for complex DOM traversal when other locators are not sufficient.

Practical Example:

```javascript
await page.locator('#username').fill('test'); // CSS
await page.locator('//button[text()="Login"]').click(); // XPath
```

Common Mistakes:
- Writing long and complex XPath
- Using XPath when better locators exist
- Not optimizing selectors

Expected Interview Questions:
- CSS vs XPath?
- Which is faster and why?
- When to use XPath?

--------------------------------------------------

5. Best Practices ⭐ (INTERVIEW GOLD)

What is it:
Guidelines to write stable, maintainable, and reliable locators.

Key Points:
- Prefer getByRole() first
- Use data-testid if available
- Avoid XPath unless necessary
- Keep selectors short and readable
- Use chaining for precision

How to Answer (Interview):
I prefer role-based locators like getByRole() for stability. If not available, I use data-testid or CSS selectors. I avoid XPath unless required and ensure locators are maintainable.

Practical Example:

```javascript
await page.getByRole('button', { name: 'Submit' }).click();
await page.locator('[data-testid="login-btn"]').click();
```

Common Mistakes:
- Using absolute XPath
- Writing brittle selectors
- Ignoring readability

Expected Interview Questions:
- What is your locator strategy?
- Which locator do you prefer and why?
- How do you write stable locators?

--------------------------------------------------

Final Strategy (VERY IMPORTANT)

Locator Priority Order:

1. getByRole() ⭐  
2. getByTestId()  
3. getByText()  
4. CSS  
5. XPath (last option)

--------------------------------------------------

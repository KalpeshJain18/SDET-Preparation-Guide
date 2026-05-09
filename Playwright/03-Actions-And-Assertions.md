# 🚀 Playwright → Actions & Assertions (Complete Guide)

This section covers all major actions, assertions, and auto-waiting concepts in Playwright required for SDET interviews.

--------------------------------------------------

Topics Covered:

1. Actions  
2. Assertions  
3. Auto-Waiting  
4. Best Practices  

--------------------------------------------------

# 🧠 1. Actions

## What is it

Actions are methods used to interact with web elements like clicking, typing, selecting, hovering, etc.

---

## Key Components

- click()
- fill()
- type()
- check()
- uncheck()
- hover()
- selectOption()
- press()

---

## How to Answer (Interview Style)

Actions in Playwright are used to simulate real user interactions such as clicking buttons, entering text, selecting dropdown values, and hovering over elements. Playwright automatically waits for elements before performing actions.

---

## Practical Example

```javascript
await page.locator('#username').fill('Kalpesh');
await page.getByRole('button', { name: 'Login' }).click();
await page.locator('#country').selectOption('India');
```

---

## Common Mistakes

- Using unnecessary waits before actions
- Using force click without reason
- Confusing fill() and type()

---

## Expected Interview Questions

- Difference between fill() and type()?
- What actions have you used in Playwright?
- How does Playwright handle waits during actions?

--------------------------------------------------

# 🧠 2. Assertions

## What is it

Assertions are validations used to verify expected behavior or UI state.

---

## Key Components

- toHaveText()
- toBeVisible()
- toHaveURL()
- toHaveTitle()
- toBeChecked()

---

## How to Answer (Interview Style)

Assertions in Playwright are used to validate application behavior. Playwright provides built-in auto-retrying assertions which improve test stability and reduce flaky tests.

---

## Practical Example

```javascript
await expect(page).toHaveTitle(/Dashboard/);

await expect(page.locator('.success-msg')).toBeVisible();

await expect(page.locator('#name')).toHaveValue('Kalpesh');
```

---

## Common Mistakes

- Using manual validations instead of expect()
- Not understanding auto-retry behavior
- Writing weak assertions

---

## Expected Interview Questions

- What is assertion in Playwright?
- Difference between hard and soft assertion?
- Why are Playwright assertions stable?

--------------------------------------------------

# 🧠 3. Auto-Waiting ⭐

## What is it

Playwright automatically waits for elements to become ready before performing actions or assertions.

---

## Key Components

- Visibility check
- Element enabled state
- Stability check
- Auto-retrying assertions

---

## How to Answer (Interview Style)

One major advantage of Playwright is built-in auto-waiting. Before performing actions, Playwright ensures elements are visible, stable, and actionable, reducing flaky tests and minimizing explicit waits.

---

## Practical Example

```javascript
await page.getByRole('button', { name: 'Submit' }).click();
```

No explicit wait required.

---

## Common Mistakes

- Adding unnecessary waitForTimeout()
- Using hard waits everywhere
- Not trusting Playwright auto-wait

---

## Expected Interview Questions

- What is auto-waiting in Playwright?
- Difference between Playwright and Selenium waits?
- Why does Playwright reduce flaky tests?

--------------------------------------------------

# 🧠 4. Best Practices ⭐

## What is it

Guidelines for writing reliable actions and assertions.

---

## Key Components

- Prefer built-in assertions
- Avoid hard waits
- Use stable locators
- Validate meaningful UI behavior

---

## How to Answer (Interview Style)

I avoid hard waits and rely on Playwright’s built-in auto-waiting and assertions. I also use stable locators and meaningful validations to improve test reliability.

---

## Practical Example

```javascript
await expect(page.getByRole('heading')).toHaveText('Dashboard');
```

---

## Common Mistakes

- Using waitForTimeout() frequently
- Weak validations
- Over-validating unnecessary UI elements

---

## Expected Interview Questions

- What are best practices for assertions?
- How do you avoid flaky tests?
- Why avoid hard waits?

--------------------------------------------------

# 🎯 FINAL INTERVIEW GOLD

## Difference Between fill() and type()

| Method | Purpose |
|--------|----------|
| fill() | Replaces existing text instantly |
| type() | Types character by character |

---

## Assertion Priority

1. toBeVisible()
2. toHaveText()
3. toHaveURL()
4. toHaveTitle()

--------------------------------------------------

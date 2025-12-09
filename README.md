# ⚡ Locator Labs Desktop

<p align="center">
<a align="center" href="https://www.locator-labs.com">LocatorLabs</a>
</p>

<p align="center">
  <b>The Ultimate Element Locator Generator for Test Automation Engineers</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-macOS%20%7C%20Windows%20%7C%20Linux-blue?style=for-the-badge" alt="Platform">
  <img src="https://img.shields.io/badge/Playwright-45ba4b?style=for-the-badge&logo=playwright&logoColor=white" alt="Playwright">
  <img src="https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white" alt="Selenium">
  <img src="https://img.shields.io/badge/Cypress-17202C?style=for-the-badge&logo=cypress&logoColor=white" alt="Cypress">
</p>

<p align="center">
  A powerful desktop application that generates reliable, maintainable locators for Playwright, Selenium, and Cypress test automation frameworks. No browser extension needed - works in enterprise/restricted environments!
</p>

---

## ✨ Features

### 🎯 Smart Locator Generation
- **Semantic Locators** - Accessibility-first locators (`getByRole`, `getByLabel`, `getByText`)
- **Quality Ratings** - Each locator rated as BEST, GOOD, OK, or FRAGILE
- **Multiple Strategies** - ID, Name, CSS Selector, XPath, Link Text, and more

### 🔧 Multi-Framework Support

| Framework | Languages |
|-----------|-----------|
| **Playwright** | JavaScript/TypeScript, Python |
| **Selenium** | Java, Python |
| **Cypress** | JavaScript/TypeScript |

### 🚀 Powerful Capabilities

| Feature | Description |
|---------|-------------|
| **Live Element Inspector** | Point and click to select elements |
| **Built-in Browser** | No need to switch between apps |
| **Multi-Tab Support** | Work with multiple pages simultaneously |
| **Shadow DOM Support** | Works with web components |
| **iFrame Support** | Handles nested frames automatically with `frameLocator()` |
| **SVG Element Support** | Special handling for SVG elements |
| **Test Locator** | Validate locators before using them |
| **Action Autocomplete** | `.click()`, `.fill()`, `.type()`, `.should()` and more |
| **Dark/Light Theme** | Easy on the eyes |

### 📦 Page Object Model Generator

Generate production-ready Page Object classes for:
- Playwright (TypeScript, JavaScript, Python)
- Selenium (Java, Python)
- Cypress
- WebdriverIO
- Robot Framework

---

## 📥 Download

### Latest Release: v1.1.5

| Platform | Download |
|----------|----------|
| 🍎 **macOS** (Universal - Intel & Apple Silicon) | [LocatorLabs-1.1.5-universal.dmg](https://github.com/naveenanimation20/Locator-Labs-App-Releases/releases/download/1.1.5/LocatorLabs-1.1.5-universal.dmg) |
| 🪟 **Windows** | [LocatorLabs Setup 1.1.5.exe](https://github.com/naveenanimation20/Locator-Labs-App-Releases/releases/download/1.1.5/LocatorLabs.Setup.1.1.5.exe) |
| 🐧 **Linux** | [LocatorLabs-1.1.5.AppImage](https://github.com/naveenanimation20/Locator-Labs-App-Releases/releases/download/1.1.5/LocatorLabs-1.1.5.AppImage) |

---

👉 **[View all releases](https://github.com/naveenanimation20/Locator-Labs-App-Releases/releases)**

> 💡 **Note**: macOS users may need to right-click and select "Open" for the first launch due to Gatekeeper.

---

## 🚀 Getting Started

### Installation

1. **Download** the installer for your platform from [Releases](https://github.com/naveenanimation20/Locator-Labs-App-Releases/releases)
2. **macOS**: Open the `.dmg` and drag Locator Labs to Applications
3. **Windows**: Run the `.exe` installer
4. **Linux**: Make the `.AppImage` executable: `chmod +x LocatorLabs-1.1.0.AppImage` and run it

### Quick Start Guide

1. **Launch** Locator Labs Desktop
2. **Enter a URL** in the address bar and press Go
3. **Click "Start Inspecting"** to enable element selection
4. **Click any element** on the page to generate locators
5. **Choose your framework** (Playwright/Selenium/Cypress) using the tabs
6. **Copy the locator** using the 📋 button

---

## 📖 How to Use

### Generating Locators

```
1. Navigate to your target website
2. Click "Start Inspecting" button (turns green when active)
3. Hover over elements - they get highlighted
4. Click an element to capture it
5. View all generated locators with quality ratings
6. Click 📋 to copy or ➕ to add to Page Object cart
```

### Testing Locators

```
1. Enter any locator in the "Test Locator" field
2. Click ▶ to execute
3. See how many elements match
4. Use ◀ ▶ arrows to navigate through matches
5. Supports Playwright, Selenium, and Cypress syntax
```

### Building Page Objects

```
1. While inspecting, click ➕ on locators you want to save
2. Click the 📦 cart icon in the header
3. Enter a page name (e.g., "LoginPage")
4. Select your framework and language
5. Click "Download File" or "Copy to Clipboard"
```

---

## 🎯 Locator Quality Guide

| Rating | Meaning | Stability |
|--------|---------|-----------|
| 🟢 **BEST** | Semantic, accessible locators | Very Stable |
| 🔵 **GOOD** | Reliable with good specificity | Stable |
| 🟡 **OK** | Works but may need updates | Moderate |
| 🔴 **FRAGILE** | Likely to break with UI changes | Unstable |

### Examples by Framework

**Playwright (BEST)**
```javascript
page.getByRole('button', { name: 'Submit' })
page.getByLabel('Email')
page.getByTestId('login-form')
page.frameLocator('iframe#main').getByRole('button')
```

**Selenium (BEST → GOOD)**
```java
driver.findElement(By.id("submit-btn"))
driver.findElement(By.name("email"))
driver.findElement(By.cssSelector("[data-testid='login']"))
```

**Cypress (BEST → GOOD)**
```javascript
cy.get('[data-testid="submit"]')
cy.contains('button', 'Submit')
cy.get('#email').shadow().find('input')
cy.xpath('//button[@id="login"]')
```

---

## ⚙️ System Requirements

| Platform | Minimum Version |
|----------|-----------------|
| **macOS** | 10.13 High Sierra or later |
| **Windows** | Windows 10 or later |
| **Linux** | Ubuntu 18.04+ or equivalent |

---



## ❓ FAQ

<details>
<summary><b>Why use this instead of browser DevTools?</b></summary>

- Generates semantic locators automatically (getByRole, getByLabel)
- Provides quality ratings to help you choose the best locator
- Works in enterprise environments where extensions are blocked
- Built-in Page Object Model generator
- Supports Playwright, Selenium, and Cypress in one tool
- Test and validate locators before using them in your tests
</details>

<details>
<summary><b>macOS says the app is from an unidentified developer</b></summary>

Right-click the app and select "Open", then click "Open" in the dialog. You only need to do this once.
</details>

<details>
<summary><b>Can I use this for websites that require login?</b></summary>

Yes! The built-in browser maintains your session, so you can log in and inspect authenticated pages. Your session persists across page navigations.
</details>

<details>
<summary><b>Does it support Cypress?</b></summary>

Yes! As of v1.1.0, full Cypress support is included with `cy.get()`, `cy.contains()`, `cy.xpath()`, Shadow DOM chains, and action autocomplete.
</details>

<details>
<summary><b>How do I handle elements inside iframes?</b></summary>

LocatorLabs automatically detects elements inside iframes and generates the appropriate locators:
- **Playwright**: Adds `frameLocator()` prefix automatically (e.g., `page.frameLocator('iframe#main').getByRole('button')`)
- **Selenium**: Shows "Switch to Frame First" instructions with the frame switching code
- **Cypress**: Generates iframe-aware locators

Nested iframes are also supported!
</details>

<details>
<summary><b>Does it work with Shadow DOM?</b></summary>

Yes! LocatorLabs fully supports Shadow DOM elements:
- **Playwright**: Uses pierce selectors or JS path to reach shadow elements
- **Selenium**: Generates JavaScript executor code for shadow DOM traversal
- **Cypress**: Creates `.shadow()` chain locators (e.g., `cy.get('#host').shadow().find('button')`)
</details>

<details>
<summary><b>What does the Test Locator feature do?</b></summary>

The Test Locator lets you validate any locator before using it in your tests:
- Enter any Playwright, Selenium, or Cypress locator
- Click ▶ to execute and see how many elements match
- Elements are highlighted on the page
- Navigate through multiple matches using ◀ ▶ arrows
- Autocomplete suggests actions like `.click()`, `.fill()`, `.type()`
</details>

<details>
<summary><b>How do I generate a Page Object Model class?</b></summary>

1. While inspecting elements, click ➕ on locators you want to include
2. Click the 📦 cart icon in the header
3. Enter a page name (e.g., "LoginPage")
4. Select your framework (Playwright, Selenium, Cypress, WebdriverIO, Robot Framework)
5. Choose your language
6. Click "Download File" or "Copy to Clipboard"
</details>

<details>
<summary><b>What's the difference between locator quality ratings?</b></summary>

| Rating | Example | Why |
|--------|---------|-----|
| 🟢 **BEST** | `getByRole('button', { name: 'Submit' })` | Semantic, accessibility-based, resilient to UI changes |
| 🔵 **GOOD** | `By.id("submit-btn")` | Stable identifiers, unlikely to change |
| 🟡 **OK** | `By.cssSelector(".btn-primary")` | Class-based, may change with styling updates |
| 🔴 **FRAGILE** | `By.xpath("//div[3]/button[1]")` | Position-based, breaks easily with DOM changes |
</details>

<details>
<summary><b>Can I use XPath locators?</b></summary>

Yes! XPath is supported for all frameworks:
- **Playwright**: `page.locator('xpath=//button[@id="submit"]')`
- **Selenium**: `driver.findElement(By.xpath("//button[@id='submit']"))`
- **Cypress**: `cy.xpath('//button[@id="submit"]')` (requires cypress-xpath plugin)

LocatorLabs handles quote escaping automatically for complex XPath expressions.
</details>

<details>
<summary><b>Does the autocomplete support actions?</b></summary>

Yes! After typing a complete locator and adding a `.`, you'll see action suggestions:
- **Playwright**: `.click()`, `.fill()`, `.textContent()`, `.isVisible()`, `.hover()`, and more
- **Selenium**: `.click()`, `.sendKeys()`, `.getText()`, `.isDisplayed()`, and more
- **Cypress**: `.click()`, `.type()`, `.should()`, `.invoke()`, `.trigger()`, and more
</details>

<details>
<summary><b>What if multiple elements match my locator?</b></summary>

The Test Locator shows you the count of matching elements. Use the ◀ ▶ navigation arrows to cycle through each match - each element gets highlighted in turn. This helps you verify your locator is specific enough or identify if you need to add more specificity.
</details>

<details>
<summary><b>Does it work offline?</b></summary>

The application itself works offline, but you need an internet connection to browse websites. All locator generation, testing, and Page Object creation happen locally on your machine.
</details>

<details>
<summary><b>Can I use keyboard shortcuts?</b></summary>

Yes! Common shortcuts include:
- **Ctrl/Cmd + R**: Refresh page
- **Ctrl/Cmd + L**: Focus URL bar
- **Escape**: Stop inspecting
- **Arrow keys**: Navigate through autocomplete suggestions
</details>

<details>
<summary><b>How do I handle dynamic elements or elements with changing IDs?</b></summary>

LocatorLabs prioritizes stable locators:
1. Use semantic locators like `getByRole`, `getByLabel`, `getByText` (rated BEST)
2. Look for `data-testid` attributes if available
3. Use partial matches with `contains()` for text that remains stable
4. Avoid position-based XPath (rated FRAGILE)

The quality ratings help you identify which locators are most resilient.
</details>

<details>
<summary><b>Is there an interactive tutorial for new users?</b></summary>

Yes! Version 1.1.0 includes an interactive Tour Guide that walks you through all the features step-by-step. It starts automatically for first-time users, or you can restart it anytime from the Help menu.
</details>

<details>
<summary><b>Why isn't my element being detected?</b></summary>

Common reasons and solutions:
- **Element is in an iframe**: LocatorLabs should detect this automatically, but ensure the iframe is same-origin
- **Element is in Shadow DOM**: Supported - check if the shadow root is open
- **Page is still loading**: Wait for the page to fully load before inspecting
- **Element is dynamically rendered**: Interact with the page to make the element appear first
</details>

<details>
<summary><b>Can I use this in corporate/enterprise environments?</b></summary>

Yes! LocatorLabs Desktop is designed for enterprise use:
- No browser extension required (works where extensions are blocked)
- Runs locally on your machine (no data sent to external servers)
- Works with internal/intranet applications
- Supports authentication and maintains sessions
</details>

---

## 🤝 Support & Feedback

- **Issues**: [GitHub Issues](https://github.com/naveenanimation20/Locator-Labs-Desktop-App/issues)
- **Website**: [locator-labs.com](https://www.locator-labs.com)
- **YouTube**: [Naveen AutomationLabs](https://youtube.com/naveenautomationlabs)

---

## 📄 License

Proprietary Software - All Rights Reserved
© 2025 Naveen Automation Labs

---

<p align="center">
  <b>Built with ❤️ by Naveen Automation Labs</b>
  <br><br>
  <a href="https://www.locator-labs.com">Website</a> •
  <a href="https://youtube.com/naveenautomationlabs">YouTube</a> •
  <a href="https://naveenautomationlabs.com">Blog</a>
</p>

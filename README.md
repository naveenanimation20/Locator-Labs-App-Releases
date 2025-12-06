# ⚡ Locator Labs Desktop

<p align="center">
  <img src="assets/icon.png" alt="Locator Labs" width="128" height="128">
</p>

<p align="center">
  <b>The Ultimate Element Locator Generator for Test Automation Engineers</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-macOS%20%7C%20Windows%20%7C%20Linux-blue?style=for-the-badge" alt="Platform">
  <img src="https://img.shields.io/badge/Playwright-45ba4b?style=for-the-badge&logo=playwright&logoColor=white" alt="Playwright">
  <img src="https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white" alt="Selenium">
</p>

<p align="center">
  A powerful desktop application that generates reliable, maintainable locators for Playwright and Selenium test automation frameworks. No browser extension needed - works in enterprise/restricted environments!
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

### 🚀 Powerful Capabilities

| Feature | Description |
|---------|-------------|
| **Live Element Inspector** | Point and click to select elements |
| **Built-in Browser** | No need to switch between apps |
| **Multi-Tab Support** | Work with multiple pages simultaneously |
| **Shadow DOM Support** | Works with web components |
| **iFrame Support** | Handles nested frames automatically |
| **SVG Element Support** | Special handling for SVG elements |
| **Test Locator** | Validate locators before using them |
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

### Latest Release: v1.0.0

| Platform | Architecture | Download |
|----------|--------------|----------|
| **macOS** | Apple Silicon (M1/M2/M3) | [Download .dmg](#) |
| **macOS** | Intel | [Download .dmg](#) |
| **Windows** | x64 | [Download .exe](#) |
| **Linux** | x64 | [Download .AppImage](#) |

> 💡 **Note**: macOS users may need to right-click and select "Open" for the first launch due to Gatekeeper.

---

## 🚀 Getting Started

### Installation

1. **Download** the installer for your platform from [Releases](#)
2. **macOS**: Open the `.dmg` and drag Locator Labs to Applications
3. **Windows**: Run the `.exe` installer
4. **Linux**: Make the `.AppImage` executable: `chmod +x LocatorLabs.AppImage`

### Quick Start Guide

1. **Launch** Locator Labs Desktop
2. **Enter a URL** in the address bar and press Go
3. **Click "Start Inspecting"** to enable element selection
4. **Click any element** on the page to generate locators
5. **Choose your framework** (Playwright/Selenium) using the tabs
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
```

**Selenium (BEST → GOOD)**
```java
driver.findElement(By.id("submit-btn"))
driver.findElement(By.name("email"))
driver.findElement(By.cssSelector("[data-testid='login']"))
```

---

## ⚙️ System Requirements

| Platform | Minimum Version |
|----------|-----------------|
| **macOS** | 10.13 High Sierra or later |
| **Windows** | Windows 10 or later |
| **Linux** | Ubuntu 18.04+ or equivalent |

---

## 🆕 What's New

### v1.0.0
- ✅ Initial Release
- ✅ Playwright & Selenium support
- ✅ Page Object Model generator (8 frameworks)
- ✅ Shadow DOM & iFrame handling
- ✅ Multi-tab browsing
- ✅ Dark/Light theme
- ✅ URL history with suggestions
- ✅ Test locator with element navigation

---

## ❓ FAQ

<details>
<summary><b>Why use this instead of browser DevTools?</b></summary>

- Generates semantic locators automatically (getByRole, getByLabel)
- Provides quality ratings to help you choose the best locator
- Works in enterprise environments where extensions are blocked
- Built-in Page Object Model generator
</details>

<details>
<summary><b>macOS says the app is from an unidentified developer</b></summary>

Right-click the app and select "Open", then click "Open" in the dialog. You only need to do this once.
</details>

<details>
<summary><b>Can I use this for websites that require login?</b></summary>

Yes! The built-in browser maintains your session, so you can log in and inspect authenticated pages.
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

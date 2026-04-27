# Swag Labs Playwright Testing

A Playwright end-to-end test suite for [Sauce Demo](https://www.saucedemo.com), built inside a React app workspace. This repository validates Sauce Demo login, cart, and checkout flows with Playwright using Chromium and generates HTML test reports.

## What this project covers

- Sauce Demo login page validation
- invalid credentials and form validation checks
- add-to-cart / remove-from-cart behavior
- checkout flow and order completion verification
- Playwright HTML reporting for easy result review

## Key files

- `playwright.config.ts` — Playwright configuration for the test suite
- `tests/login.spec.ts` — login and authentication scenarios
- `tests/cart.spec.ts` — cart add/remove assertions
- `tests/checkout.spec.ts` — checkout and order completion flows

## Scripts

From the project root, run:

```bash
npm run playwright:test
```

Runs the full Playwright test suite.

```bash
npm run playwright:report
```

Opens the latest Playwright HTML report.

```bash
npx playwright install
```

Installs Playwright browser dependencies.

## Setup

Install dependencies first:

```bash
npm install
```

If Playwright browsers are not installed, run:

```bash
npx playwright install
```

## How to run tests

Run the suite with:

```bash
npm run playwright:test
```

This uses the configured Chromium project and test directory defined in `playwright.config.ts`.

## How to view reports

After test execution, open the latest HTML report with:

```bash
npm run playwright:report
```

If the default port is in use, use a free port manually:

```bash
npx playwright show-report --port=0
```

## Notes

- The suite uses `data-test` selectors from Sauce Demo for stability.
- Tests are intentionally scoped to example end-to-end flows rather than exhaustive coverage.
- This repo is a demo of Playwright automation against a public demo web app.

## Recommended workflow

1. `npm install`
2. `npx playwright install`
3. `npm run playwright:test`
4. `npm run playwright:report`

---

Built for Sauce Demo automation practice and GitHub-ready Playwright testing.

A Playwright-based automation suite for https://www.saucedemo.com built inside a React app workspace. This repository captures Sauce Demo’s core e2e flows and makes it easy to run stable browser tests and generate HTML reports.

What it does

validates Sauce Demo login behavior
verifies cart add/remove functionality
completes checkout flow and verifies final confirmation
keeps tests isolated with reusable login logic
uses Playwright’s Chromium runner for reliable results
generates HTML reports for test results
Why it exists
This repo is designed to demonstrate:

real user journeys on Sauce Demo
Playwright best practices for selector usage and wait logic
test automation that is easy to run locally and review via reports
Key scripts
npm run playwright:test — run the full Playwright suite
npm run playwright:report — open the latest HTML report
npx playwright install — install Playwright browser dependencies

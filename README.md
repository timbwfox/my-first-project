# My First Project

A calculator web app built with Vite and tested end-to-end with Playwright.

The main purpose of this project is to demonstrate behavior-driven testing of a UI app using BDD Feature files (Gherkin) plus Playwright step definitions and a Page Object Model.

All application code and all tests in this repository were written 100% by GitHub Copilot.

## Prerequisites

- Node.js 24+
- npm 11+

## Install

```bash
npm install
```

## Run Locally

```bash
npm run dev
```

## Build

```bash
npm run build
```

## Test Commands

Run unit tests:

```bash
npm test
```

Generate BDD tests from feature files:

```bash
npm run bddgen
```

Run E2E tests (BDD + Playwright):

```bash
npm run test:e2e
```

Run E2E tests in headed mode:

```bash
npm run test:e2e:headed
```

## CI/CD

GitHub Actions workflow:

- Builds the app
- Runs all unit tests
- Runs all BDD E2E tests
- Uploads the build artifact (`dist`)

Workflow file: `.github/workflows/ci-cd.yml`

## Project Structure

```text
my-first-project/
	.github/
		workflows/
			ci-cd.yml
	public/
	src/
		styles/
			main.css
		bootstrap.js
		calculator.js
		calculator-app.js
		calculator-engine.js
		calculator.test.js
		calculator.unit.test.js
		calculator.buttons.test.js
		main.js
		run-tests.js
	tests/
		e2e/
			features/
				calculator.feature
			steps/
				calculator.steps.js
			pages/
				calculator.page.js
			calculator.spec.js
	index.html
	playwright.config.js
	package.json
	package-lock.json
	.gitignore
	README.md
```

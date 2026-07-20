# Playwright-Automation
Playwright and Typescript test automation framework.

## Tech Stack
- Playwright
- Typescript
- Husky + lint-staged - pre-commit hooks (Prettier -> ESLint -> tsc)

## Getting started
Node.js (check package.json for version)

### Install

```bash
npm install
```

## Running Tests

```bash
# Run all tests
npx playwright test

# Run regression-taggeed tests only
npm run regression:tests

# Run a single test file
npx playwright test
features/ui/tests/example.spec.ts

# Debug mode
npx playwright test --debug

# Interactive UI mode
npx playwright test --ui

# View HTML report
npx playwright show-report
```

## Linting and Type Checking

```bash
# Lint
npm run lint

# Type check
npx tsc --noEmit
```
Pre-commit hooks automatically run Prettier, ESLint and `tsc` on staged `.ts` files.

## Project Structure

```
features/ui/
|━ constants/ 
|━ fixtures/ 
|━ helpers/   
|━ pages/       
|━ services/   
|━ tests/    
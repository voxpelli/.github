# Contributing

Thanks for your interest in contributing to my projects! Contributions are very welcome – whether it's filing an issue, suggesting an improvement, or sending a pull request.

This document provides a high-level guide to contributing.

For project-specific details like Node.js versions, testing specifics, or scripts, please refer to the `README.md` or `package.json` of the respective repository.

## Quick Start

The general workflow for getting started is:

1.  **Fork & Clone:** Fork the repository and clone it locally.
2.  **Install Dependencies:** Run `npm install` in your terminal
3.  **Run Checks & Tests:** Most projects use a single command to run all quality checks (linting, type-checking) and the full test suite: `npm test`

If `npm test` passes, you're ready to make changes!

## Development Philosophy

My projects generally follow these principles:

- **Minimal & Focused:** Prefer small and clear changes, preferably well-tested.
- **High Standards:** Code is desired to be clean and strongly typed (usually via JSDoc and TypeScript).
- **Minimal Dependencies:** Avoid adding new runtime dependencies unless there is a strong justification.
- **Modern JavaScript:** Use modern language features, but stay compatible with the Node.js versions listed in the project's `package.json`.

## Making Changes

1.  **Branch:** Create a new feature branch for your work (e.g., `feat/add-new-feature` or `fix/correct-a-bug`).
2.  **Code:** Make your changes, adhering to the existing code style.
3.  **Test:** Add or update tests to cover your changes. Ensure all tests pass by running `npm test`.
4.  **Commit:** Write a clear and descriptive commit message. I encourage using the [Conventional Commits](https://www.conventionalcommits.org/) format.
    - `feat:` for new features.
    - `fix:` for bug fixes.
    - `docs:` for documentation changes.
    - `test:` for test-only changes.
    - `chore:` for maintenance tasks.

## Submitting a Pull Request

When you're ready to submit your work:

- Fill in the pull request template with a clear description of the "what" and "why" of your changes.
- Ensure the PR is focused on a single change. Avoid unrelated formatting or refactoring.
- Reference any related issues in your PR description (e.g., `Closes #123`).
- (Make sure `npm test` passes, they will have to pass before any PR is merged)

## Tips & Tricks

### Automated running of tests

In most of my projects `husky` is installed to automatically run tests on `push` (and sometimes to automatically verify structure of git commit messages).

In the newer of my projects `husky` is not automatically activated, instead you do:

*  To activate: `npm run husky-activate`
*  To deactivate: `npm run husky-deactivate`

### Running quality checks

To run just quality checks (ESLint, type checking, Knip etc) and not the unit tests, in most of my projects you can do: `npm run check`

## Security Vulnerabilities

Please do **not** open a public issue for security vulnerabilities. Instead, follow the security guidelines of the project.

## Code of Conduct

Please be respectful and constructive in all interactions. Lets focus on fostering a positive and inclusive community.

---

Thanks again for your contribution

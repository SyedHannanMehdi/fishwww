# Contributing Guide

Thank you for your interest in contributing to this project! This guide outlines the process for proposing changes, reporting issues, and opening pull requests.

---

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [Reporting Issues](#reporting-issues)
- [Branching Strategy](#branching-strategy)
- [Commit Messages](#commit-messages)
- [Code Style](#code-style)
- [Pull Request Process](#pull-request-process)
- [Review Expectations](#review-expectations)

---

## Code of Conduct

By participating in this project, you agree to maintain a respectful and inclusive environment for all contributors. Please be constructive and kind in all interactions.

---

## Getting Started

1. **Fork** the repository to your own GitHub account.
2. **Clone** your fork locally:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```
3. **Install dependencies** (if applicable):
   ```bash
   npm install
   # or
   pip install -r requirements.txt
   ```
4. **Create a new branch** for your changes (see [Branching Strategy](#branching-strategy)).

---

## Reporting Issues

Before opening a new issue, please search existing issues to avoid duplicates.

When filing a bug report, include:
- A clear and descriptive title.
- Steps to reproduce the problem.
- Expected vs. actual behaviour.
- Environment details (OS, language/runtime version, etc.).
- Any relevant logs or screenshots.

For feature requests, describe:
- The problem you are trying to solve.
- Your proposed solution or approach.
- Any alternatives you have considered.

---

## Branching Strategy

Use short, descriptive branch names that reference the type of work being done:

| Prefix | Purpose |
|--------|---------|
| `feat/` | New features |
| `fix/` | Bug fixes |
| `docs/` | Documentation updates |
| `refactor/` | Code refactoring (no functional change) |
| `test/` | Adding or improving tests |
| `chore/` | Build process, tooling, or dependency updates |

**Examples:**
```
feat/add-user-auth
fix/null-pointer-on-login
docs/update-readme
```

Always branch off the latest `main` (or `master`) branch:
```bash
git checkout main
git pull upstream main
git checkout -b feat/my-new-feature
```

---

## Commit Messages

Follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

```
<type>(<scope>): <short summary>

[optional body]

[optional footer(s)]
```

**Types:** `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`

**Rules:**
- Use the **imperative mood** in the summary line ("add feature" not "added feature").
- Keep the summary line under **72 characters**.
- Reference related issues in the footer: `Closes #42` or `Refs #15`.

**Examples:**
```
feat(auth): add JWT-based login endpoint

Implements token generation and validation using jsonwebtoken.
Closes #10
```

```
fix(api): handle null response from upstream service

Previously the app crashed when the upstream returned null.
Added a guard clause and fallback value.
Refs #22
```

---

## Code Style

- Follow the existing code style of the repository.
- Run linters and formatters before committing:
  ```bash
  npm run lint
  npm run format
  ```
- Ensure all existing tests pass:
  ```bash
  npm test
  ```
- Add or update tests for any new or changed behaviour.
- Keep functions small and focused on a single responsibility.
- Write clear, self-documenting code and add comments where the intent is not immediately obvious.

---

## Pull Request Process

1. **Push** your branch to your fork:
   ```bash
   git push origin feat/my-new-feature
   ```
2. **Open a Pull Request** against the `main` branch of the upstream repository.
3. Fill in the PR template (if provided), including:
   - A clear description of *what* changed and *why*.
   - Reference to the related issue (e.g., `Closes #15`).
   - Screenshots or recordings for UI changes.
4. Ensure your branch is **up to date** with `main` before requesting review:
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```
5. Mark the PR as a **Draft** if it is still a work-in-progress.

---

## Review Expectations

- A maintainer will review your PR as soon as possible.
- Be responsive to feedback and update your branch accordingly.
- All CI checks must pass before a PR can be merged.
- At least **one approving review** from a maintainer is required.
- Maintainers may request changes, ask clarifying questions, or close PRs that are out of scope.
- Once approved, a maintainer will merge your PR.

---

Thank you for helping improve this project! 🎉

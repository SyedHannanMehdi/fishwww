# Contributing Guide

Thank you for your interest in contributing to this project! This guide explains how to propose changes, report issues, and open pull requests effectively.

---

## Table of Contents

- [Getting Started](#getting-started)
- [Reporting Issues](#reporting-issues)
- [Branching Strategy](#branching-strategy)
- [Commit Messages](#commit-messages)
- [Code Style](#code-style)
- [Opening a Pull Request](#opening-a-pull-request)
- [Code of Conduct](#code-of-conduct)

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
4. Create a new branch for your change (see [Branching Strategy](#branching-strategy)).

---

## Reporting Issues

- Search [existing issues](../../issues) before opening a new one to avoid duplicates.
- Use a clear, descriptive title.
- Include:
  - A summary of the problem or feature request.
  - Steps to reproduce (for bugs).
  - Expected vs. actual behaviour.
  - Relevant logs, screenshots, or code snippets.
- Apply the appropriate label (`bug`, `enhancement`, `question`, etc.) if you have permission.

---

## Branching Strategy

| Branch type    | Naming convention              | Purpose                              |
|----------------|-------------------------------|--------------------------------------|
| Feature        | `feat/<short-description>`    | New features or enhancements         |
| Bug fix        | `fix/<short-description>`     | Correcting existing behaviour        |
| Documentation  | `docs/<short-description>`    | Documentation-only changes           |
| Chore / Misc   | `chore/<short-description>`   | Tooling, deps, CI, refactoring, etc. |

**Rules:**
- Always branch off the latest `main` (or `develop` if the project uses one).
- Keep branches focused — one logical change per branch.
- Delete your branch after the PR is merged.

---

## Commit Messages

Follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

```
<type>(<scope>): <short summary>

[optional body]

[optional footer(s)]
```

**Common types:** `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`

**Examples:**
```
feat(auth): add OAuth2 login flow
fix(api): handle null response from /users endpoint
docs: add contributing guide
```

**Guidelines:**
- Use the imperative mood in the summary line ("add feature" not "added feature").
- Keep the summary under 72 characters.
- Reference relevant issue numbers in the footer: `Closes #42` or `Refs #15`.

---

## Code Style

- Follow the style conventions already present in the codebase.
- Run any existing linters/formatters before committing:
  ```bash
  npm run lint
  npm run format
  # or
  black . && flake8 .
  ```
- Do not introduce unnecessary whitespace changes or re-format unrelated code.
- Write or update tests for any code you add or modify.
- Keep functions small and focused; add comments where the intent is not immediately clear.

---

## Opening a Pull Request

1. Push your branch to your fork:
   ```bash
   git push origin feat/my-feature
   ```
2. Open a PR against the `main` branch of the upstream repository.
3. Fill in the PR template (if provided) or include:
   - **What** was changed and **why**.
   - A reference to the related issue: `Closes #<issue-number>`.
   - Screenshots or recordings for UI changes.
   - Notes on testing performed.
4. Ensure all CI checks pass before requesting a review.
5. Respond promptly to review feedback and push fixes to the same branch — the PR will update automatically.
6. Do **not** force-push to a branch once a review is in progress unless specifically asked to rebase.

### PR Checklist

- [ ] Branch is up to date with `main`
- [ ] Code follows project style guidelines
- [ ] All tests pass locally
- [ ] New tests added for new functionality
- [ ] Documentation updated (if applicable)
- [ ] PR description references the related issue

---

## Code of Conduct

Please be respectful and constructive in all interactions. We follow the [Contributor Covenant](https://www.contributor-covenant.org/) code of conduct. Harassment or hostile behaviour of any kind will not be tolerated.

---

Thank you for helping improve this project! 🎉

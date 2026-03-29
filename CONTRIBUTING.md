# Contributing to fishwww

Thank you for your interest in contributing! We welcome contributions of all kinds — bug fixes, new features, documentation improvements, and more.

## Table of Contents

- [Getting Started](#getting-started)
- [How to Contribute](#how-to-contribute)
- [Code Style](#code-style)
- [Commit Messages](#commit-messages)
- [Pull Request Process](#pull-request-process)
- [Reporting Issues](#reporting-issues)
- [Code of Conduct](#code-of-conduct)

---

## Getting Started

1. **Fork** the repository on GitHub.
2. **Clone** your fork locally:
   ```bash
   git clone https://github.com/YOUR_USERNAME/fishwww.git
   cd fishwww
   ```
3. **Install dependencies** (if applicable):
   ```bash
   npm install
   # or
   pip install -r requirements.txt
   ```
4. **Create a branch** for your changes:
   ```bash
   git checkout -b feature/your-feature-name
   ```

---

## How to Contribute

### Bug Fixes
- Check the [issue tracker](https://github.com/192600/fishwww/issues) for existing bug reports.
- If your bug isn't listed, open a new issue before submitting a fix so it can be discussed.

### New Features
- Open an issue to propose your feature before implementing it.
- This helps avoid duplicate work and ensures the feature aligns with the project direction.

### Documentation
- Improvements to docs, README, or inline comments are always welcome.
- No issue is required for minor documentation changes.

---

## Code Style

- Follow the existing code style and conventions used throughout the project.
- Use meaningful variable and function names.
- Keep functions small and focused — one responsibility per function.
- Add comments for non-obvious logic.
- Remove unused imports and dead code before submitting.

---

## Commit Messages

Write clear, descriptive commit messages:

- Use the imperative mood: `Add feature`, `Fix bug`, `Update docs`
- Keep the subject line under 72 characters
- Reference related issues where applicable: `Fix #42 — handle null input`

---

## Pull Request Process

1. Ensure your branch is up to date with `main` before opening a PR:
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```
2. Push your branch to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```
3. Open a pull request against the `main` branch of this repository.
4. Fill in the PR template (if provided) — describe what changed and why.
5. Reference the relevant issue in your PR description (e.g., `Closes #17`).
6. Be responsive to review feedback — address all comments before the PR can be merged.

---

## Reporting Issues

When filing a bug report or feature request, please include:

- **A clear title** summarising the problem or request.
- **Steps to reproduce** (for bugs) — the more detail, the better.
- **Expected behaviour** vs **actual behaviour**.
- **Environment details** — OS, language/runtime version, relevant dependencies.
- **Screenshots or logs** if applicable.

Open issues here: [https://github.com/192600/fishwww/issues](https://github.com/192600/fishwww/issues)

---

## Code of Conduct

Please be respectful and constructive in all interactions. We are committed to providing a welcoming and inclusive environment for everyone.

---

Thank you for helping make this project better! 🙌

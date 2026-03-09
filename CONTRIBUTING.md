# Contributing to test-ai-pipeline

Thank you for your interest in contributing to the **test-ai-pipeline** project! We welcome contributions from everyone and are grateful for your help in making this project better.

## Table of Contents

- [Getting Started](#getting-started)
- [Branch Naming Conventions](#branch-naming-conventions)
- [Commit Message Style Guide](#commit-message-style-guide)
- [Pull Request Process](#pull-request-process)
- [Code Review Expectations](#code-review-expectations)
- [Reporting Bugs and Suggesting Features](#reporting-bugs-and-suggesting-features)
- [Code of Conduct](#code-of-conduct)

## Getting Started

### Fork and Clone the Repository

1. **Fork the repository** by clicking the "Fork" button on the GitHub repository page
2. **Clone your fork** to your local machine:
   ```bash
   git clone https://github.com/YOUR-USERNAME/test-ai-pipeline.git
   cd test-ai-pipeline
   ```
3. **Add the upstream remote** to keep your fork synchronized with the original repository:
   ```bash
   git remote add upstream https://github.com/volodymyr-1/test-ai-pipeline.git
   ```
4. **Create a new branch** for your changes (see [Branch Naming Conventions](#branch-naming-conventions) below)
5. **Make your changes** and commit them following the [Commit Message Style Guide](#commit-message-style-guide)
6. **Push your changes** to your fork and create a Pull Request

### Setting Up Your Local Environment

No special setup is required for this project. Simply ensure you have:
- **Git** installed and configured
- A GitHub account
- A text editor of your choice

## Branch Naming Conventions

Please use the following branch naming conventions to keep our repository organized:

### Branch Types

- **`feature/`** - New features or enhancements
  - Example: `feature/add-ci-workflow`
  - Example: `feature/improve-documentation`

- **`fix/`** - Bug fixes
  - Example: `fix/github-api-error`
  - Example: `fix/incorrect-formatting`

- **`docs/`** - Documentation updates
  - Example: `docs/update-readme`
  - Example: `docs/add-troubleshooting-guide`

- **`chore/`** - Maintenance tasks, dependencies, or configuration changes
  - Example: `chore/update-dependencies`
  - Example: `chore/configure-git-hooks`

- **`refactor/`** - Code refactoring without functional changes
  - Example: `refactor/simplify-logic`
  - Example: `refactor/improve-code-structure`

### Example Branch Names

✅ Good:
- `feature/contributing-guidelines`
- `fix/readme-typo`
- `docs/add-faq-section`
- `chore/update-github-workflows`

❌ Bad:
- `my-changes`
- `update`
- `fix_bug`
- `NewFeature123`

## Commit Message Style Guide

Write clear and descriptive commit messages to help others understand your changes. Follow these guidelines:

### Commit Message Format

```
<type>: <subject>

<body>

<footer>
```

### Rules

1. **Separate subject from body with a blank line**
2. **Limit the subject line to 50 characters**
3. **Capitalize the subject line**
4. **Do not end the subject line with a period**
5. **Use the imperative mood in the subject line** (e.g., "Add feature" not "Added feature")
6. **Wrap the body at 72 characters**
7. **Use the body to explain what and why, not how**
8. **Reference issues in the footer** (e.g., "Closes #123")

### Commit Types

- **feat**: A new feature
- **fix**: A bug fix
- **docs**: Documentation changes
- **style**: Code style changes (formatting, missing semicolons, etc.)
- **refactor**: Code refactoring without functional changes
- **perf**: Performance improvements
- **test**: Adding or updating tests
- **chore**: Maintenance, dependencies, or build-related changes

### Example Commit Messages

✅ Good:
```
feat: Add contribution guidelines to CONTRIBUTING.md

This adds a comprehensive guide for contributors including branch naming
conventions, commit message style, and pull request process.

Closes #5
```

```
fix: Correct typo in README.md

Changed "README" to "README.md" in the project description.
```

❌ Bad:
- `fixed stuff` - Too vague
- `Update` - No context
- `Add feature` - Doesn't reference issue
- `I added a new feature to the project` - Not imperative mood

## Pull Request Process

### Before Submitting a Pull Request

1. **Ensure your branch is up to date** with the main branch:
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```
2. **Test your changes** locally to ensure they work as expected
3. **Review your own changes** before submitting (check for typos, formatting, etc.)
4. **Run a final check** to ensure your commit messages follow the style guide

### Submitting a Pull Request

1. **Push your branch** to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```
2. **Create a Pull Request** on GitHub with a descriptive title and body:
   - Use a clear, descriptive title that explains the changes
   - Reference the related issue number (e.g., "Closes #5")
   - Provide a summary of your changes
   - Explain why these changes are necessary
   - List any related issues or pull requests

### Pull Request Template

When creating a PR, please include:

```markdown
## Description
Brief description of the changes made.

## Related Issue
Closes #<issue-number>

## Type of Change
- [ ] New feature
- [ ] Bug fix
- [ ] Documentation update
- [ ] Other (please specify)

## Changes Made
- Bullet point 1
- Bullet point 2
- Bullet point 3

## Testing
Describe any testing you've done to verify the changes.

## Checklist
- [ ] I have followed the contribution guidelines
- [ ] I have updated documentation as needed
- [ ] My commit messages follow the style guide
- [ ] I have reviewed my own changes
```

## Code Review Expectations

### What to Expect

1. **Reviewers will** examine your code for:
   - Correctness and functionality
   - Adherence to project guidelines
   - Code clarity and maintainability
   - Alignment with the project's goals

2. **Feedback will be** constructive and respectful
3. **Review time** may vary depending on reviewer availability
4. **Changes may be requested** before approval

### How to Respond to Feedback

1. **Address all comments** and feedback from reviewers
2. **Reply to comments** explaining your changes or asking clarifying questions
3. **Make requested changes** and push new commits to your branch
4. **Request re-review** when you've addressed all feedback
5. **Be open to discussion** and willing to compromise on implementation details

### Approved and Merging

Once a PR is approved:
1. A maintainer will merge your changes into the main branch
2. Your branch will be deleted
3. Your contribution will be reflected in the project

## Reporting Bugs and Suggesting Features

### Reporting Bugs

If you discover a bug, please create an issue with:

1. **A clear title** describing the bug
2. **Steps to reproduce** the issue
3. **Expected behavior** - what should happen
4. **Actual behavior** - what actually happens
5. **Environment details** - OS, Git version, etc.
6. **Screenshots or error messages** (if applicable)

### Suggesting Features

To suggest a new feature, create an issue with:

1. **A clear title** describing the feature
2. **A detailed description** of the feature and why it would be useful
3. **Use cases** - how would this feature be used?
4. **Possible implementation** (optional) - any ideas on how to implement it
5. **Related issues** (optional) - links to similar requests

### Issue Labels

When creating an issue, please use appropriate labels:
- **bug** - Reports of bugs
- **enhancement** - Feature requests
- **documentation** - Documentation improvements
- **good first issue** - Good for newcomers

## Code of Conduct

### Our Pledge

We are committed to providing a welcoming and inspiring community for all. Please read and respect our code of conduct:

- **Be respectful** - Treat all community members with respect and courtesy
- **Be inclusive** - Welcome people of all backgrounds and experiences
- **Be constructive** - Provide constructive feedback and suggestions
- **No harassment** - Do not engage in harassment, discrimination, or personal attacks
- **Assume good intent** - Assume the best in others and give them the benefit of the doubt

### Reporting Violations

If you witness or experience behavior that violates our Code of Conduct, please report it by:
1. Creating a private issue on GitHub (if available)
2. Contacting the project maintainers directly

All reports will be taken seriously and handled confidentially.

---

## Questions?

If you have any questions about the contribution process, feel free to:
1. Open an issue labeled "question"
2. Check existing issues for similar questions
3. Reach out to the project maintainers

Thank you for contributing to test-ai-pipeline! 🎉

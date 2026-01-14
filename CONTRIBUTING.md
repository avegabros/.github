# Contributing to Avega Bros Projects ⚓

Welcome! We are excited that you are contributing to the Avega Bros Integrated Shipping Corp. codebase. To maintain the reliability of our logistics systems, we follow a strict set of standards for all our repositories.

## 🚀 Getting Started

Before you begin, ensure you have:
1. Been granted access to the relevant repository by the Admin team.
2. Set up your local environment according to the specific project's `README.md`.
3. Configured your Git identity with your corporate email.

## 🌿 Branching Strategy

We follow a simplified **GitFlow** model. Please name your branches using the following prefixes:

- `feature/` : New features or enhancements (e.g., `feature/gps-tracking-api`)
- `bugfix/` : Fixing issues in the code (e.g., `bugfix/login-latency`)
- `hotfix/` : Urgent fixes for production issues.
- `docs/`   : Documentation updates only.

**Note:** Direct commits to `main` or `develop` branches are restricted.

## 📝 Commit Message Standards

We use **Conventional Commits** to keep our history readable and to automate changelogs.
Format: `<type>(<scope>): <description>`

- **feat**: A new feature for the user.
- **fix**: A bug fix.
- **chore**: Updating build tasks, package manager configs, etc.
- **refactor**: A code change that neither fixes a bug nor adds a feature.

*Example:* `feat(vessel-sched): add real-time ETA calculation logic`

## 🛠️ Development Workflow

1. **Fork/Branch**: Create a new branch from `develop`.
2. **Code**: Follow the project's linting and styling rules (Prettier/ESLint).
3. **Test**: Ensure all unit tests pass locally before pushing.
4. **Push**: Push your branch to the origin.
5. **Pull Request (PR)**: Open a PR against the `develop` branch.

## 🔍 Pull Request Process

### 1. Linking Issues
When opening a PR, use specific keywords in the description to link it to an issue. This helps maintain a clear audit trail for our logistics software.

**To automatically close an issue when the PR is merged:**
* `fixes #123`
* `resolves #123`
* `closes #123`
* `fixed #123` (used for past tense/completed work)

**To link an issue without closing it (e.g., related tasks or context):**
* `addresses #123` (indicates the PR deals with part of an issue)
* `relates to #123`
* `see also #123`
* `refs #123`

### 2. PR Guidelines
* Every PR requires at least **one peer review** before merging.
* **Description:** Clearly explain *what* was changed and *why*.
* **Screenshots:** For UI/Frontend changes, include "Before" and "After" screenshots.
* **CI/CD:** All automated tests and linting checks must pass before the "Merge" button is enabled.
## 🔒 Security First

As a logistics company, data security is paramount:
- **Never** commit API keys, passwords, or shipping credentials to the repository.
- Use `.env` files and secret management tools (AWS Secrets Manager / Vault).
- If you find a security vulnerability, do not open a public issue; report it directly to the IT Security lead.

---

*Moving the nation with code.*

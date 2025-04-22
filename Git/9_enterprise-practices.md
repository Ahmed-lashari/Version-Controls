# 🏢 Enterprise Git Practices

## 📁 Branch Naming Convention


|Type   	|Example|
--------------------------------
|Feature	|feature/login-form|
|Bugfix	       |bugfix/crash-on-submit|
|Hotfix 	|hotfix/payment-fix|
|Release	|release/v1.2.0|

## 🔄 Commit Message Format (Conventional Commits)

```bash
<type>(scope): message
# example:
feat(auth): add login with OTP
fix(navbar): hide button on scroll
refactor(ui): update theme colors
```

- Types: "*feat, fix, refactor, chore, docs, test*"


## 🧪 Code Review Rules
- No direct push to `main`.

- Secondary brance's pull request must be approved by 1–2 project members.

- Code must be tested before merging into `main`.

## 🚫 Protecting Main Branch
**Use GitHub settings to:**

- Require pull-requests for merging.

- Enforce code review approvals.

- Block merge if build/test fails.

## 🔁 GitFlow (Optional Advanced) 
### Branches:
- `main`: bug-free and ready-to-use code

- `develop`: integration branch

- `feature/feature-name`: new features

- `release/relese-version`: prep releases

- `hotfix/fix-name-time`: urgent fixes

GitFlow keeps things organized at scale.

## 🧼 Clean Repos
- Use `.gitignore` properly.

- Squash commits before merging PRs if needed.

- Avoid committing `.env`, `node_modules`, `build/`, etc...

## Afvance Security Practices
- Use ***SSH*** keys for pushing code securely.

- Apply `role-based` access (e.g., Admin, Developer1, ...).

- Rotate secrets and API keys often (and never commit them).
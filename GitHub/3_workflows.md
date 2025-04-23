# 🔄 GitHub Collaboration Workflows

## ⚙️ What is a Workflow?

A **workflow** is a set of conventions and practices that teams follow to:
- Collaborate on code
- Submit and review changes
- Merge safely into the main codebase

---

## 🌱 GitHub Flow (Best for Continuous Deployment)

A lightweight workflow perfect for startups, solo developers, or CI/CD environments.

### 🔁 Steps:
1. **Create a new branch** from `main`
2. **Commit changes** to your feature branch
3. **Push** the branch to GitHub
4. **Open a Pull Request**
5. **Review and approve** changes
6. **Merge** into `main`
7. **Deploy** automatically (optional)

```bash
git branch Github/workflow-file
git switch Github/workflow-file
# Make your changes
git add .
git commit -m "workflow file added"
git push origin Github/workflow-file
```
## 🧱 GitLab Flow (More Structure)
A more advanced flow that mixes GitHub Flow and Git Flow:

- Best for larger teams

- Works with environments (staging, production)

Common Branches:
- `main` – Production-ready code

- `develop` – Integration branch for features

- `feature/feature-name` – Individual feature branches

- `release/version-here` – Code ready for final QA

- `hotfix/fix-name` – Critical fixes to production

## 🧬 Feature Branch Workflow
Each feature gets its own branch from main or develop.

Benefits:
- Isolated workspaces

- Easier to track who did what

- Safe experimentation

```bash
git branch feature/chat-module develop
git switch feature/chat-module develop
# Add commits
git push origin feature/chat-module
```

## 🔐 Protecting the main Branch
To avoid accidental commits or bad merges, protect the main branch:

- Require pull request before merging

- Require status checks to pass (tests)

- Limit who can push to main

You can configure this in `Repo Settings` > `Branch Protection Rules`.

## 👤 Roles & Permissions

|Role         |	GitHub Access|
|-------------|-------------------|
|Owner        |	Full control|
|Maintainer   |	High-level repo access|
|Contributor  |	PR-based contributions only|
|Collaborator |	Can be invited to push directly|

***🔒 For private repositories, only allow collaborators and team members to push.***


## 🧼 Merge Strategies
GitHub supports several merge methods:

- Merge Commit (default)
Keeps full history. Useful for large projects.

- Squash and Merge
Combines all commits into one. Cleaner history.

- Rebase and Merge
Rewrites commit history. Best for linear history.

- Set this under Settings > Merge Button Options.

## 🧠 Best Practices
- Keep branches short-lived

- Use clear names: feature/login, bugfix/signup-error

- Commit often, push regularly

- Use pull requests, even in solo projects

- Add reviewers and request feedback

- Merge only after approval + all checks pass

## ✅ Summary
### Workflow

|Type	              |Use Case	                     |Branches|
|--------------------|----------------------------------|---------|
|GitHub Flow	       |Simpler projects, CI/CD	       |main, feature/*      |
|GitLab Flow  	|Teams, environments, structure    |main, develop, feature/*, release/*|
|Feature Branch	|All types of collaboration	       |Any base branch|
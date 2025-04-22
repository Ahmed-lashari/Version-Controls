# Git: Revert vs Merge

Understanding the difference between `git revert` and `git merge` is essential for managing code history and collaboration effectively.

---

## 🔁 `git revert`

### ✅ What is it?

- `git revert` is used to **undo** a specific commit.
- It **does not remove** the commit from history — instead, it creates a **new commit** that "reverses" the changes of a previous commit.

### 📘 Use Case:

> You made a mistake in a previous commit (e.g., broke a feature) and want to undo it *without rewriting history*.

### 🛠️ Command:

```bash
git revert <commit-hash>
```

## 💡 Example:

1. Check your commit history:
```bash
git log --oneline
```
Let's say this is the log:
> hassam@192 Verrsion-Controls % git log
commit ea27ea2cb12c4080f71ca273bd25fa9797d61268 (HEAD -> main, origin/main)
Merge: e28ab3f 0718c6b
Author: Ahmed-lashari <ahmedlashari.official@gmail.com>
Date:   Tue Apr 22 16:12:11 2025 +0500
```bash
    folder flow adjusted
```
> commit 0718c6bd8c266e84326012ae51d8df853972fc50 (origin/custom-merging-branch, custom-merging-branch)
Author: Ahmed-lashari <ahmedlashari.official@gmail.com>
Date:   Tue Apr 22 16:04:38 2025 +0500
```bash
    branch-merging file adjusted into the folder
```

#### 2. Revert the commit that adjusted folder flow:

```bash
git revert e28ab3f
```

#### 3. This will open an editor to confirm the revert message.

#### 4. After saving, a new commit will appear that undoes the changes from e28ab3f.

---
# 🔀 git merge

## ✅ What is it?
git merge is used to combine changes from one branch into another.

It helps bring together development lines in a project.

### 📘 Use Case:
You created a new feature (*"custom-merging-branch"* in our case) branch and want to merge its work into the main branch once it's done.

🛠️ Command:

```bash
git checkout main
git merge custom-merging-branch
```

## 💡 Example:
1. You have two branches:
```bash
 custom-merging-branch
* main
```

## 2. To merge the *"custom-merging-branch"* into main:
```bash
git checkout main
git merge custom-merging-branch
```

- If there are no conflicts, Git will create a new merge commit.

- If there are conflicts, you will be prompted to resolve them before completing the merge.


# 📌 Key Differences

- `git revert` is about undoing commits safely.

- `git merge` is about combining branches.

- Both commands create new commits to preserve history.


# 🧠 Tips for Beginners
- Use `git revert` if you've pushed a mistake and want to undo it without breaking team collaboration.

- Use `git merge` to integrate features from different branches in a safe and trackable way.


---
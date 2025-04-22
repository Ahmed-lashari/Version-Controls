# 🔄 Undoing Things in Git is a very Important Concept

## 1️⃣ Unstaging Files

### 🧠 You added a file using `git add <file name>`, but you want to unstage it.

```bash
git restore --staged <file>
```

## 🧪 Example:
```bash
git add 6_undoings-in-git.md
git restore --staged 6_undoings-in-git.md
```
## 2️⃣ Discarding Local Changes
### 🧠 You modified a file but want to discard all your local changes.

```bash
git restore <file>
```

## 🧪 Example:
```bash
git restore 6_undoings-in-git.md
```

## 3️⃣ Amending a Commit
### 🧠 You committed but forgot to include a file or want to change the message.
```bash
git add missed_file.dart
git commit --amend
```
Rewrites the last commit *"⚠️ only safe if not pushed yet."*

## 4️⃣ Reset to a Previous Commit
### 🧠 Undo all commits after a certain commit (⚠️ use with care!).

```bash
git reset --hard <commit-hash>
```
This will rewrite the GitHub history.

## 5️⃣ Soft Reset (Keep changes in staging)

```bash
git reset --soft <commit-hash>
```
---

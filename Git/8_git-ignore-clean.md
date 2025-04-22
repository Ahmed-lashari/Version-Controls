# 🧼 .gitignore & git clean

## 📁 `.gitignore`
## 🧠 Tells Git to ignore certain files or folders.

## 📘 Use Case:
Ignore files like:
- .env (secrets)
- node_modules/
- *.log

## 🛠️ How to Use
### Create a `.gitignore` file:

```bash
# Ignores all log files
*.log

# Ignores secrets
.env

# Ignores build folders
/build
```
Git will stop tracking these files if not already committed.




## 🧼 `git clean`
## 🧠 Deletes untracked files (not staged or committed).
## ⚠️ Using with caution!

```bash
git clean -n    # dry run (shows what will be deleted)
git clean -f    # actually deletes files
```

## 🧪 Example:

```bash

git clean -n
# will remove:
# untracked_file.txt

git clean -f
# now its deleted
```
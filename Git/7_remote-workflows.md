# 🔁 Remote Workflows

## 🔄 Cloning a Repository
```bash 
git clone https://github.com/user-name/repository-link.git
```

## 🔼 Pushing Changes
```bash
git push origin main
```


## 🔽 Pulling Latest Changes
```bash
git pull origin main
```


## 🧪 Working in a Feature Branch

```bash
git branch feature/homepage
git switch feature/homepage
# changes made in the codebase
git add .
git commit -m "adding homepage"
git push origin feature/homepage
```


## 🔀 Merging a PR *"In GitHub"*

- Open a Pull Request (PR)

- Review and merge

Then, locally:

```bash
git switch main
git pull origin main
git push origin main
```



## 📌 Common Individual's Remote Workflow

```bash
git checkout -b feature/name
git add .
git commit -m "feat: add something"
git push origin feature/name
# create pull-request

# merge it with main
git switch main
git pull origin main
git push origin main
```

---



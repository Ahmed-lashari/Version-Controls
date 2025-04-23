# 🌐 Introduction to GitHub

## 📌 What is GitHub?

GitHub is a **web-based platform** that provides hosting for Git repositories. It adds a layer of collaboration tools, making it easier for developers to work together on code, track issues, review changes, and manage projects.

- Git: The version control system.
- GitHub: A platform **built on top of Git**, offering cloud storage and powerful team collaboration features.

> ✅ Git tracks code. GitHub helps you collaborate on that code with others.

---

## 🆚 Git vs GitHub

| Feature             | Git                                   | GitHub                                           |
|--------------------|----------------------------------------|--------------------------------------------------|
| Type               | CLI Tool                              | Web Platform                                     |
| Purpose            | Local version control                 | Remote collaboration & project management       |
| Works Without Net? | Yes                                   | No (requires internet for collaboration)        |
| UI Available?      | No (CLI only)                         | Yes (User-friendly interface)                   |

---

## 🧑‍💻 Why Use GitHub?

- 🧠 **Backup your code** to the cloud
- 👥 **Collaborate** with others in real time
- 🐛 **Track bugs and issues**
- 📂 **Review and discuss code changes**
- 🌎 **Open-source contribution**
- 🚀 **Host portfolio projects and documentation**

---

## 🪪 Setting Up GitHub

1. Go to [https://github.com](https://github.com)
2. Sign up and create a new account
3. Set your GitHub username and email same as Git config (recommended)
4. Optionally, set up your profile, add bio and profile picture

---

## 🧱 Creating Your First Repository

1. Click on the **+** icon > `New repository`
2. Set repository name (e.g., `GitHub-Intro`)
3. Choose:
   - **Public** (will be visible to everyone)  
   - **Private** (will be only visible to you/partners)
4. Initialize with:
   - `README.md` (recommended)
   - `.gitignore` (optional but recommended)
   - Choose a license if open source (MIT, APACHE)
5. Click **Create repository**

---

## 💻 Cloning a Repository (From GitHub to Local)

```bash
git clone https://github.com/your-username/your-repository-name.git
```
After cloning:
```bash
cd your-repo-name
```

## 🔁 Pushing Local Code to GitHub

```bash
git add .
git commit -m "Initial commit"
git push origin main
```


## 🔐 Security Tip
If you're pushing code to GitHub:
- Never include .env or credentials in your code.

- Use .gitignore to exclude sensitive files.

- Use GitHub Secrets or .env.local files if using in CI/CD.
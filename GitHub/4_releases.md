# 🚀 Releases & Tagging on GitHub

Releases help developers deliver stable versions of their code to users. They are based on **tags** and can include **release notes**, **changelogs**, and **downloadable assets**.

---

## 🏷️ What is a Tag?

A **tag** is a snapshot of your codebase at a specific point in time, often used to mark:
- Releases (v1.0.0, v2.1.4)
- Milestones (beta, stable)
- Deployments

### Creating a Tag:

```bash
git tag v1.0.0
git push origin v1.0.0
```

## 📦 What is a Release?
A release builds on a tag and allows you to:

- Write release notes (changes, fixes, features)

- Attach compiled files or binaries

- Notify users of new updates

## ✍️ How to Create a Release on GitHub
1. Go to your repo

2. Click "Releases"

3. Click "Draft a new release"

4. Select or create a tag (e.g., v1.0.0)

5. Fill in:

- Release title

- Description / Changelog

 - Attach any build assets (ZIPs, APKs, etc.)

6. Click "Publish release"

## 🔢 Semantic Versioning (SemVer)
Format: MAJOR.MINOR.PATCH

|Part|	Description|
|----|------------|
|MAJOR|	Breaking changes (e.g., v2.0.0)|
|MINOR|	New features (backward compatible, developer focused)|
|PATCH|	Bug fixes or small updates|

## Example:

`v1.0.0` => Initial release

`v1.1.0` => Added new feature

`v1.1.1` => Fixed a bug

## 🗒️ Changelog Example
```bash
## [v1.2.0] - 2025-04-23

### Added
- Github/releases-file

### Fixed
- Managed - Version-Control-Repo Structure
```
Keeping a changelogs in a CHANGELOG.md file at the root of your repo is also a most recommended approach.

## 🧪 Pre-release vs Draft
- **Draft**: Saved but unpublished. Only visible to collaborators.

- **Pre-release**: Marked as experimental or not production-ready.

Use these flags when testing beta builds or internal versions.

## 🧲 Downloading Assets from a Release
Users can download:

- Source code (.zip / .tar.gz)

- Any attached files (binaries, installers, PDFs)

## 🧠 Best Practices
- Always tag stable versions

- Use consistent semantic versioning

- Include a detailed changelog

- Use GitHub Releases for distribution

- Attach compiled assets for easier download

---
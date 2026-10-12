# GitHub Profile README Deployment Guide

This guide details how to publish and maintain your professional GitHub developer profile dashboard for the account **[@Haridh432](https://github.com/Haridh432)**.

---

## 📌 Prerequisites & Overview

GitHub allows you to display a custom profile dashboard by creating a repository with the exact same name as your username (`Haridh432/Haridh432`). Any content inside `README.md` of that repository is automatically rendered on your public profile overview page.

---

## 🚀 Step 1: Create the Special Profile Repository

1. Log into your GitHub account: [https://github.com](https://github.com).
2. Go to [https://github.com/new](https://github.com/new) to create a new repository.
3. Enter the repository details:
   - **Repository name:** `Haridh432` *(A special banner will appear: "You found a secret! Haridh432/Haridh432 is a special repository that you can use to add a README.md to your GitHub profile.")*
   - **Visibility:** Select **Public** *(The profile README will only appear if the repository is Public)*.
   - **Initialize this repository with:** Leave "Add a README file" **unchecked** (since you already have your prepared `README.md`).
4. Click **Create repository**.

---

## 💻 Step 2: Push the Profile README to GitHub

From your local project folder (`d:\New folder\Git`), open your terminal (PowerShell or Git Bash) and run:

```bash
# 1. Initialize git repository if not already initialized
git init

# 2. Add the README.md file
git add README.md

# 3. Create your first commit
git commit -m "feat: launch professional developer profile dashboard"

# 4. Set the default branch to main
git branch -M main

# 5. Add your new GitHub repository as the remote
git remote add origin https://github.com/Haridh432/Haridh432.git

# 6. Push your profile to GitHub
git push -u origin main
```

*(Alternatively, if you prefer using the GitHub web UI, you can simply create the `Haridh432` repository, click **Add file** -> **Upload files**, drag and drop `README.md`, and click **Commit changes**).*

---

## 👁️ Step 3: Verify Your Profile

1. Navigate to your public GitHub profile: [https://github.com/Haridh432](https://github.com/Haridh432).
2. You will immediately see your newly rendered profile dashboard featuring:
   - Animated typing banner.
   - Profile view counter and category tags.
   - "About Me" summary.
   - Categorized technical skills with dark-themed shields.
   - 5 Featured repositories (Network-Triage, phishing-email-analyzer, Sign-language-recognition, IoT, My-Trickster).
   - Dynamic GitHub stats & streak tracker.
   - Current focus and collaborative contact links.

---

## ⚙️ Maintenance & Customization

### 1. Updating Featured Projects
To add or modify featured repositories in the future:
- Open `README.md`.
- Locate the `<table width="100%">` block under `### 🚀 Featured Repositories`.
- Each project card is wrapped in a `<td>` element. Simply edit the repository links, descriptions, or badges as desired.

### 2. External Statistics Services & Caching
The dashboard uses three reliable external services:
- **Profile Views:** [komarev.com](https://komarev.com/ghpvc/) — Automatically increments when visitors view your profile.
- **GitHub Readme Stats:** [github-readme-stats.vercel.app](https://github-readme-stats.vercel.app/) — Computes stars, commits, PRs, and top languages.
- **GitHub Streak Stats:** [streak-stats.demolab.com](https://streak-stats.demolab.com/) — Tracks your daily contribution streak.

*Note:* External statistics services cache data for 2 to 4 hours to avoid GitHub API rate limits. New commits or contributions might not reflect instantly on the card images; this is expected behavior.

### 3. Adding LinkedIn or Email
When you are ready to link your LinkedIn profile or contact email:
- Find the `### 🤝 Connect & Collaborate` section in `README.md`.
- Add badges such as:
  ```html
  <a href="https://linkedin.com/in/YOUR_USERNAME" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:your.email@example.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  ```
- Commit and push the updates.

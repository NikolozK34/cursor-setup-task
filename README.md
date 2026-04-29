# Cursor Setup Task

## Tools Installed

* Cursor IDE
* Claude Code extension (installed via Cursor Extensions)
* Codex extension (installed via Cursor Extensions)
* Git (already installed on system)
* GitHub account

---

## Steps Completed

1. Installed and opened Cursor IDE
2. Installed **Claude Code** extension and logged in
3. Installed **Codex** extension and logged in
4. Created a public GitHub repository named `cursor-setup-task`
5. Cloned the repository into Cursor using Git
6. Created and edited the `README.md` file
7. Committed changes using terminal
8. Attempted to push changes to GitHub

---

## Issues Faced & Solutions

### 1. GitHub Authentication Failed

**Problem:**
When trying to push changes using:

```
git push
```

I received this error:

```
remote: Invalid username or token. Password authentication is not supported
```

**Cause:**
GitHub no longer supports password authentication for Git operations.

**Solution:**

* Created a **Personal Access Token (PAT)** in GitHub
* Used the token instead of password when prompted during `git push`

---

### 2. Git User Identity Warning

**Problem:**
Git showed this message during commit:

```
Your name and email address were configured automatically...
```

**Cause:**
Git was using system-generated credentials instead of my actual identity.

**Solution:**
Configured Git manually:

```
git config --global user.name "Mariam Pirosmanashvili"
git config --global user.email "my-email@example.com"
```

---

### 3. First Push Confusion

**Problem:**
Even after committing successfully, changes were not visible on GitHub.

**Cause:**
Push failed due to authentication issue.

**Solution:**
After fixing authentication (using PAT), re-ran:

```
git push
```

and changes appeared in the repository.

---

## Result

* Successfully set up Cursor with required extensions
* Created and connected GitHub repository
* Added and pushed README file
* Resolved authentication and Git configuration issues

---

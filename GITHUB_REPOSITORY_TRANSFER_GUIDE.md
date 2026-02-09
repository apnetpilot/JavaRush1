# How to Copy a GitHub Repository to Your Account

There are several ways to copy a repository from GitHub to your own account. Here are the most common methods:

## Method 1: Fork the Repository (Recommended for Contributing Back)

**Forking** creates a copy of the repository under your GitHub account while maintaining a connection to the original repository.

### Steps:
1. Go to your lecturer's GitHub repository page
2. Click the **"Fork"** button in the top-right corner
3. Select your account as the destination
4. GitHub will create a copy in your account (e.g., `your-username/repository-name`)

### Advantages:
- Easy to sync updates from the original repository
- Maintains attribution to the original author
- Ideal if you want to contribute back via pull requests

### To clone your forked repository locally:
```bash
git clone https://github.com/YOUR-USERNAME/repository-name.git
cd repository-name
```

### To keep your fork updated with the original:
```bash
# Add the original repository as "upstream"
git remote add upstream https://github.com/LECTURER-USERNAME/repository-name.git

# Fetch updates from the original repository
git fetch upstream

# Merge updates into your local branch
git merge upstream/main
# or: git merge upstream/master (depending on the default branch name)

# Push updates to your fork
git push origin main
```

---

## Method 2: Import the Repository (Clean Copy)

**Importing** creates a completely independent copy without any connection to the original repository.

### Steps:
1. Go to https://github.com/new/import
2. Paste the URL of your lecturer's repository
3. Choose a name for your new repository
4. Select public or private
5. Click **"Begin import"**

### Advantages:
- Creates a completely independent repository
- No connection to the original (clean slate)
- All commit history is preserved

---

## Method 3: Clone and Push to New Repository (Manual Method)

This method gives you full control over the process.

### Steps:

#### 1. Clone the original repository:
```bash
git clone https://github.com/LECTURER-USERNAME/repository-name.git
cd repository-name
```

#### 2. Create a new repository on GitHub:
- Go to https://github.com/new
- Create a new repository (don't initialize with README, .gitignore, or license)

#### 3. Change the remote URL to your new repository:
```bash
# Remove the original remote
git remote remove origin

# Add your new repository as the remote
git remote add origin https://github.com/YOUR-USERNAME/your-new-repo-name.git

# Push all branches and tags
git push -u origin --all
git push -u origin --tags
```

### Advantages:
- Full control over the process
- Can rename the repository
- Can choose which branches to push

---

## Method 4: Download and Upload (No Git History)

If you only want the code without the git history:

### Steps:
1. Go to the repository page
2. Click the green **"Code"** button
3. Select **"Download ZIP"**
4. Extract the ZIP file
5. Create a new repository on GitHub
6. Upload the files to your new repository

### Advantages:
- Simplest method
- No git history (fresh start)

### Disadvantages:
- Loses all commit history
- Loses all branches and tags

---

## Which Method Should You Use?

| Scenario | Recommended Method |
|----------|-------------------|
| You want to work on assignments and submit your own version | **Fork** or **Import** |
| You want to contribute improvements back to the lecturer | **Fork** |
| You want a completely independent copy | **Import** or **Clone & Push** |
| You only want the current code without history | **Download ZIP** |
| You're learning and want to experiment | **Fork** (easiest) |

---

## Best Practices for Students

1. **Always give credit**: If you use someone else's code, mention it in your README
2. **Check the license**: Make sure the repository has a license that allows copying
3. **Don't claim it as your own**: Academic integrity is important
4. **Keep your fork updated**: If the lecturer updates the repository, sync your fork
5. **Use branches**: Create branches for different assignments or experiments

---

## Example Workflow for a Student

```bash
# 1. Fork the repository on GitHub (click Fork button)

# 2. Clone YOUR fork to your computer
git clone https://github.com/YOUR-USERNAME/repository-name.git
cd repository-name

# 3. Add the lecturer's repository as upstream (to get updates)
git remote add upstream https://github.com/LECTURER-USERNAME/repository-name.git

# 4. Create a branch for your work
git checkout -b my-assignment-1

# 5. Make your changes
# ... edit files ...

# 6. Commit your changes
git add .
git commit -m "Complete assignment 1"

# 7. Push to YOUR repository
git push origin my-assignment-1

# 8. Later, to get updates from the lecturer:
git checkout main
git fetch upstream
git merge upstream/main
git push origin main
```

---

## Troubleshooting

### "Permission denied" when pushing
- Make sure you're pushing to YOUR repository, not the lecturer's
- Check that you've set up SSH keys or are using the correct credentials

### "Repository not found"
- Verify the repository URL is correct
- Make sure the repository is public or you have access

### "Already up to date" when trying to sync
- The repositories are already in sync
- No new changes from the original repository

---

## Additional Resources

- [GitHub Docs: Fork a repo](https://docs.github.com/en/get-started/quickstart/fork-a-repo)
- [GitHub Docs: Syncing a fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork)
- [GitHub Docs: Importing a repository](https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/importing-a-repository-with-github-importer)

---

## Quick Reference Commands

```bash
# Fork on GitHub, then clone your fork
git clone https://github.com/YOUR-USERNAME/repo-name.git

# Add original as upstream
git remote add upstream https://github.com/ORIGINAL-OWNER/repo-name.git

# Get updates from original
git fetch upstream
git merge upstream/main

# Push to your fork
git push origin main

# Create a new branch for your work
git checkout -b feature-branch-name

# Push your branch
git push origin feature-branch-name
```

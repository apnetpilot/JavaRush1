# How to Make Sure Your Lecturer Can See Your Repository

There are several ways to share your GitHub repository with your lecturer. Here's a comprehensive guide:

---

## Method 1: Make Your Repository Public (Easiest)

If your repository is **public**, anyone with the link can see it, including your lecturer.

### Steps to Make Repository Public:

1. Go to your repository on GitHub
2. Click **"Settings"** (top menu)
3. Scroll down to the **"Danger Zone"** section (bottom of the page)
4. Click **"Change visibility"**
5. Select **"Make public"**
6. Confirm by typing the repository name
7. Click **"I understand, change repository visibility"**

### How to Share:
Simply send your lecturer the repository URL:
```
https://github.com/YOUR-USERNAME/repository-name
```

### Advantages:
- ✅ Anyone can view it
- ✅ No additional setup needed
- ✅ Lecturer doesn't need a GitHub account to view

### Disadvantages:
- ⚠️ Everyone on the internet can see your code
- ⚠️ May violate academic integrity policies if assignments should be private

---

## Method 2: Add Lecturer as a Collaborator (Private Repository)

If you want to keep your repository **private** but give your lecturer access:

### Steps:

1. Go to your repository on GitHub
2. Click **"Settings"** (top menu)
3. Click **"Collaborators"** in the left sidebar
   - You may need to confirm your password
4. Click **"Add people"**
5. Enter your lecturer's GitHub username or email
6. Select the correct person from the dropdown
7. Choose permission level:
   - **Read** - Can only view (recommended for lecturers)
   - **Write** - Can view and make changes
   - **Admin** - Full control (not recommended)
8. Click **"Add [username] to this repository"**

### What Happens Next:
- Your lecturer will receive an email invitation
- They must **accept the invitation** to access your repository
- Once accepted, they can view your private repository

### Advantages:
- ✅ Repository stays private
- ✅ Only invited people can see it
- ✅ You control who has access

### Disadvantages:
- ⚠️ Lecturer must have a GitHub account
- ⚠️ Lecturer must accept the invitation

---

## Method 3: Share via GitHub Organization (Class/Course Setup)

Some lecturers create a GitHub Organization for their class.

### If Your Lecturer Has a GitHub Organization:

1. Wait for an invitation to join the organization
2. Accept the invitation (check your email)
3. Create your repository **inside the organization**
4. The lecturer (as organization owner) automatically has access

### Advantages:
- ✅ Organized structure for all students
- ✅ Lecturer can see all student repositories
- ✅ Can be private but accessible to the organization

---

## Method 4: Share Repository Link (Public Repos Only)

### For Public Repositories:

Simply share the URL with your lecturer via:
- Email
- Learning management system (Moodle, Canvas, etc.)
- Chat/messaging platform
- Assignment submission form

**Repository URL format:**
```
https://github.com/YOUR-USERNAME/repository-name
```

---

## How to Verify Your Lecturer Can See Your Repository

### For Public Repositories:

1. **Open an incognito/private browser window** (not logged into GitHub)
2. Paste your repository URL
3. If you can see the repository content → Your lecturer can see it ✅
4. If you see "404 Not Found" → Your lecturer cannot see it ❌

### For Private Repositories:

1. Go to your repository **Settings → Collaborators**
2. Check if your lecturer's username appears in the list
3. Check the status:
   - **"Pending invitation"** - Lecturer hasn't accepted yet
   - **"Active"** - Lecturer has access ✅

### Alternative Check:
Ask a friend (who is NOT a collaborator) to try accessing your repository URL:
- If they can see it → It's public ✅
- If they get "404 Not Found" → It's private ✅

---

## Best Practices for Sharing with Lecturers

### 1. **Ask Your Lecturer's Preference**
Different lecturers have different requirements:
- Some want public repositories
- Some require private repositories
- Some use GitHub Classroom
- Some use organization repositories

### 2. **Include a README**
Make sure your repository has a clear README.md with:
```markdown
# Assignment/Project Name

**Student Name:** Your Name
**Student ID:** Your ID
**Course:** Course Name
**Lecturer:** Lecturer Name

## Description
Brief description of the project

## How to Run
Instructions on how to run your code

## Assignment Requirements
- [x] Requirement 1
- [x] Requirement 2
- [ ] Requirement 3 (in progress)
```

### 3. **Organize Your Repository**
```
repository-name/
├── README.md
├── assignment-1/
│   ├── solution.py
│   └── README.md
├── assignment-2/
│   ├── solution.py
│   └── README.md
└── final-project/
    ├── src/
    └── README.md
```

### 4. **Use Clear Commit Messages**
```bash
# Good commit messages
git commit -m "Complete assignment 1: implement sorting algorithm"
git commit -m "Fix bug in assignment 2: handle edge case for empty input"
git commit -m "Add documentation for final project"

# Bad commit messages
git commit -m "update"
git commit -m "fix"
git commit -m "asdf"
```

### 5. **Don't Commit Sensitive Information**
Never commit:
- Passwords
- API keys
- Personal information
- Database credentials

---

## Common Scenarios and Solutions

### Scenario 1: "My lecturer says they can't see my repository"

**Solutions:**
1. Check if repository is public (Settings → Danger Zone → Visibility)
2. If private, check if lecturer is added as collaborator
3. Verify you shared the correct URL
4. Make sure lecturer accepted the invitation (if private)

### Scenario 2: "I want to keep my code private but share with lecturer"

**Solution:**
- Add lecturer as collaborator with "Read" permission
- Ask lecturer to accept the invitation

### Scenario 3: "I'm using GitHub Classroom"

**Solution:**
- Accept the assignment invitation from your lecturer
- GitHub Classroom automatically gives lecturer access
- No additional steps needed

### Scenario 4: "I forked lecturer's repository, can they see my fork?"

**Answer:**
- No, your fork is separate from the original
- If your fork is private, lecturer cannot see it unless you add them
- If your fork is public, anyone can see it

---

## Step-by-Step: Complete Workflow for Students

### Option A: Public Repository (Simple)

```bash
# 1. Make sure your repository is public (check on GitHub)

# 2. Get your repository URL
# It looks like: https://github.com/YOUR-USERNAME/repository-name

# 3. Share the URL with your lecturer via email or LMS
```

### Option B: Private Repository (More Secure)

```bash
# 1. Keep your repository private

# 2. Add lecturer as collaborator:
#    - Go to Settings → Collaborators
#    - Click "Add people"
#    - Enter lecturer's GitHub username
#    - Select "Read" permission
#    - Click "Add"

# 3. Notify your lecturer that you sent an invitation

# 4. Wait for lecturer to accept

# 5. Share your repository URL
```

---

## Verification Checklist

Before submitting your repository to your lecturer, verify:

- [ ] Repository is accessible (public OR lecturer is added as collaborator)
- [ ] README.md exists with your name and assignment details
- [ ] All required files are committed and pushed
- [ ] Code is properly organized in folders
- [ ] No sensitive information is committed
- [ ] Latest changes are pushed to GitHub (not just on your computer)
- [ ] Repository URL is correct and working
- [ ] If private, lecturer has accepted the invitation

---

## How to Get Your Repository URL

### Method 1: From GitHub Website
1. Go to your repository on GitHub
2. Copy the URL from your browser's address bar
3. Example: `https://github.com/username/repository-name`

### Method 2: From Git Command Line
```bash
# Show remote URL
git remote get-url origin

# Example output:
# https://github.com/username/repository-name.git
# Remove the .git at the end when sharing
```

---

## Troubleshooting

### "I added my lecturer but they still can't see the repository"

**Check:**
1. Did lecturer accept the invitation? (Check Settings → Collaborators)
2. Did you share the correct URL?
3. Is the repository actually private? (Settings → Danger Zone)
4. Did you push your latest changes? (`git push`)

### "I can't add my lecturer as a collaborator"

**Possible reasons:**
1. You're using GitHub Free and reached collaborator limit
2. You don't have admin access to the repository
3. The repository is in an organization (ask organization owner)

### "My lecturer wants to see my commit history"

**Solution:**
- Make sure you're pushing regularly: `git push`
- Don't delete and re-create the repository
- Don't force push: avoid `git push --force`
- Keep meaningful commit messages

---

## Quick Command Reference

```bash
# Check if you have uncommitted changes
git status

# Commit your changes
git add .
git commit -m "Descriptive message"

# Push to GitHub
git push

# Verify remote URL
git remote get-url origin

# Check which branch you're on
git branch

# Make sure you're on the main/master branch
git checkout main
# or: git checkout master
```

---

## Contact Your Lecturer

When sharing your repository, send a message like:

**Example Email:**

```
Subject: Assignment Submission - [Your Name] - [Course Name]

Dear [Lecturer Name],

I have completed [Assignment Name] and uploaded it to my GitHub repository.

Repository URL: https://github.com/YOUR-USERNAME/repository-name

[If private repository:]
I have added you as a collaborator with read access. Please check your 
email for the invitation and accept it to view my repository.

[If public repository:]
The repository is public, so you can view it directly using the link above.

The assignment files are located in the [folder-name] directory.

Thank you,
[Your Name]
[Student ID]
```

---

## Additional Resources

- [GitHub Docs: Inviting collaborators](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository)
- [GitHub Docs: Repository visibility](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/setting-repository-visibility)
- [GitHub Classroom Documentation](https://classroom.github.com/help)

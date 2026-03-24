# Git and VSCode Guide

This guide provides a comprehensive reference for Git commands on Linux and using Git within Visual Studio Code (VSCode) for project management.

---

## 1. Installing Git on Linux

**Ubuntu / Debian:**
```bash
sudo apt update
sudo apt install git
```

**Verify installation:**
```bash
git --version
```

**Configure Git (first-time setup):**
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Check configuration:
```bash
git config --list
```

---

## 2. Common Git Commands

### 2.1 Repository Management
```bash
# Initialize a new Git repository
git init

# Clone an existing repository
git clone <repository_url>
```

### 2.2 Staging and Committing
```bash
# Check status of files
git status

# Stage files for commit
git add <file_name>
git add .  # Add all files

# Commit changes
git commit -m "Commit message"
```

### 2.3 Branching
```bash
# List branches
git branch

# Create a new branch
git branch <branch_name>

# Switch branches
git checkout <branch_name>

# Create and switch to a new branch in one step
git checkout -b <branch_name>

# Merge a branch into current branch
git merge <branch_name>
```

### 2.4 Remote Repository Management
```bash
# Add a remote repository
git remote add origin <repository_url>

# View remotes
git remote -v
```

### 2.5 Push and Pull
```bash
# Push changes to remote repository
git push origin <branch_name>

# Pull changes from remote repository
git pull origin <branch_name>
```

### 2.6 Undo and Reset
```bash
# Undo unstaged changes
git checkout -- <file_name>

# Unstage a file
git reset <file_name>

# Reset last commit but keep changes
git reset --soft HEAD~1

# Reset last commit and discard changes
git reset --hard HEAD~1
```

### 2.7 Viewing History
```bash
# View commit history
git log

# Condensed log
git log --oneline

# Show differences
git diff
```

### 2.8 Tags
```bash
# Create a tag
git tag v1.0

# Push tags to remote
git push origin --tags
```

---

## 3. Using Git in VSCode

### 3.1 Loading a Project
1. Open VSCode.
2. Go to `File -> Open Folder` and select your project folder.
3. VSCode will automatically detect if it's a Git repository.

### 3.2 Git Panel
- Click the **Source Control** icon on the left sidebar (or `Ctrl+Shift+G`).
- You can see modified files, staged files, and commit history.

### 3.3 Basic Operations in VSCode
- **Stage Changes:** Click `+` next to files or `Stage All Changes`.
- **Commit Changes:** Enter a commit message and click the checkmark `✔`.
- **Push/Pull:**
  - Click the `...` menu in the Source Control panel.
  - Select `Push` to upload commits to remote.
  - Select `Pull` to fetch changes from remote.
- **Switch Branches:** Click the branch name in the bottom left corner and select or create a branch.
- **View History:** Right-click a file → `Open Timeline` or use extensions like `GitLens` for enhanced tracking.

### 3.4 Cloning a Repository in VSCode
1. Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on macOS) to open the command palette.
2. Type `Git: Clone` and select it.
3. Enter the repository URL.
4. Select a local folder for the cloned project.
5. Open the folder once cloning is complete.

### 3.5 Extensions for Git
- **GitLens** – advanced Git insights and history tracking.
- **Git Graph** – visual representation of branches and commits.

---

This guide provides all essential Git commands for Linux CLI and integrates Git workflows into VSCode efficiently.


# 🧭 Git & GitHub Workflow Guide

A concise guide for uploading, cloning, and managing Git repositories using the **terminal** and **VS Code**.

---

## 1️⃣ Uploading a Local Project to GitHub

- Setup Git (first time):
  
  `git config --global user.name "Your Name"`
  
  `git config --global user.email "you@example.com"`

- (Optional – set up SSH for passwordless access):
  
  `ssh-keygen -t ed25519 -C "you@example.com"`
  
  `cat ~/.ssh/id_ed25519.pub`

Copy the printed key into your GitHub account under, Settings → SSH and GPG keys → New SSH key

- Initialize & Push to a New Repo:
  
 ` cd ~/Projects/my-project`
  
  `git init`   => make it a git repo
  
  `git add .`  => stage all files
  
  `git commit -m "Initial commit"` => comment for commits

## 2️⃣ Loading (Cloning) a Repo from GitHub

cd ~/Projects
git clone git@github.com:username/repo-name.git   # SSH
# or
git clone https://github.com/username/repo-name.git  # HTTPS




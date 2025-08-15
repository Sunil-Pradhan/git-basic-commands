# 📚 Git Basic Commands

A simple guide to essential Git commands with practical examples. ✨

### 🛠 Practice Setup

We’ll create a demo project called `my-git-practice` and use it for all commands.


## 🐑 git clone – Clone a repository

**Use:** Download a copy of a remote repository to your local machine.


```bash
git clone https://github.com/username/repository.git
```

📌 Example: You find a project on GitHub and want it on your computer. It’s like **downloading a folder**, but with Git history.


## 📥 git add – Stage changes for commit

**Use:** Tell Git which files to track and include in the next commit.

```bash
git add file.txt

# OR add all changes(root directory)

git add .

# OR add all changes(root and other directory)

git add --all
```

📌 Example: You edit `index.html` and want to save it in Git’s memory for commit.

## 📦 git commit – Save staged changes

**Use:** Save a snapshot of your changes in the repository.

```bash
git commit -m "Added homepage content"
```

📌 Example: You finished adding homepage text and now commit it with a message.


## 🚀 git push – Upload commits to remote

**Use:** Send your commits from local to GitHub.

```bash
git push origin main
```

📌 Example: After committing, run `git push` to update GitHub with your changes.


## 🔄 git pull – Fetch & merge from remote

**Use:** Get the latest changes from GitHub and merge them into your local branch.

```bash
git pull origin main
```

📌 Example: Before starting work, run `git pull` to get the latest changes from your team.


## 🌿 git branch – Manage branches

**Use:** Create, list, or delete branches.

```bash
# List all branches
git branch

# Create new branch
git branch new-feature

# Delete branch
git branch -d old-feature
```

📌 Example: You create `new-feature` branch to work without affecting main.


## 🔀 git checkout – Switch branches or restore files

**Use:** Move between branches or restore files.

```bash
# Switch to a branch
git checkout new-feature

# Create and switch to new branch
git checkout -b new-feature
```

📌 Example: You switch to `new-feature` branch to continue your work.


## 🤝 git merge – Merge branches

**Use:** Combine changes from another branch into the current one.

```bash
git checkout main
git merge new-feature
```

📌 Example: After completing the `new-feature`, merge it into `main` with these commands.


## 🗂 git stash – Save work for later

**Use:** Temporarily store changes without committing.

```bash
# Stash changes
git stash

# Reapply stashed changes
git stash pop
```

📌 Example: You’re in the middle of work but need to switch branches — stash it first.


## 📋 git status – Check repository status

**Use:** See what’s changed, staged, or untracked.

```bash
git status
```

📌 Example: Before committing, check what files are ready.


## 📜 git log – View commit history

**Use:** Show a list of past commits.

```bash
git log
```

📌 Example: See who made changes and when.

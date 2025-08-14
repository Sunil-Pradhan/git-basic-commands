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


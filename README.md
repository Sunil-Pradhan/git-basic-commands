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


## 🕵️ git diff – See changes

**Use:** Compare changes between commits or working directory.

```bash
# See unstaged changes
git diff

# See staged changes
git diff --cached
```

📌 Example: Check what’s changed before committing.


**Recommended Visual Diff Tools:**


<table>
  <tr>
    <th>Tool</th>
    <th>Windows</th>
    <th>Linux</th>
    <th>Mac</th>
    <th>Link</th>
  </tr>
  <tr>
    <td><strong>Meld</strong></td>
    <td>✔️</td>
    <td>✔️</td>
    <td>✔️</td>
    <td><a href="https://meldmerge.org/">Link</a></td>
  </tr>
  <tr>
    <td><strong>Beyond Compare</strong></td>
    <td>✔️</td>
    <td>✔️</td>
    <td>✔️</td>
    <td><a href="https://www.scootersoftware.com/home">Link</a></td>
  </tr>
	<tr>
    <td><strong>DiffMerge</strong></td>
    <td>✔️</td>
    <td>✔️</td>
    <td>✔️</td>
    <td><a href="https://www.sourcegear.com/diffmerge/">Link</a></td>
  </tr>
	<tr>
    <td><strong>Diffuse</strong></td>
    <td>✔️</td>
    <td>✔️</td>
    <td>❌</td>
    <td><a href="https://diffuse.sourceforge.net/index.html">Link</a></td>
  </tr>
	<tr>
    <td><strong>Kaleidoscope</strong></td>
    <td>❌</td>
    <td>❌</td>
    <td>✔️</td>
    <td><a href="https://kaleidoscope.app/">Link</a></td>
  </tr>
	<tr>
    <td><strong>SemanticDiff</strong></td>
    <td>✔️</td>
    <td>✔️</td>
    <td>✔️</td>
    <td><a href="https://semanticdiff.com/">Link</a></td>
  </tr>
</table>


## 📐 git rebase – Reapply commits on top of another branch

**Use:** Alternative to merge for integrating changes.

```bash
git checkout new-feature
git rebase main
```

📌 Example: Use rebase to keep a clean linear history when updating your `new-feature` branch.


## 💡 Easy practice flow

Here’s a simple **practice scenario** using all commands:


```bash
# 1. Clone a test repo
git clone https://github.com/username/my-git-practice.git
cd my-git-practice

# 2. Create & switch to a new branch
git branch new-feature
git checkout new-feature

# 3. Add changes
echo "Hello Git!" > hello.txt
git add hello.txt
git commit -m "Added hello.txt"

# 4. Push branch to GitHub
git push origin new-feature


# 5. Merge branch into main
git checkout main
git pull origin main
git merge new-feature

# 6. Stash changes example
echo "Work in progress" > temp.txt
git stash
git stash pop

# 7. View logs, diffs
git log
git diff

# 8. Rebase example
git checkout new-feature
git rebase main
```

## 🎯 Final tip

Practice these commands daily with a dummy repo. Once you get used to them, Git will feel like magic.

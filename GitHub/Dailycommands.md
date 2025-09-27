Here’s a handy list of **commonly used Git commands**, grouped by purpose, with short explanations and example usage. You can copy these into a personal cheat sheet for quick reference.

---

## 1️⃣ Setup & Configuration

| Command                                            | Purpose             | Example                                             |
| -------------------------------------------------- | ------------------- | --------------------------------------------------- |
| `git config --global user.name "Your Name"`        | Set global username | `git config --global user.name "Gopi D"`            |
| `git config --global user.email "you@example.com"` | Set global email    | `git config --global user.email "gopi@example.com"` |
| `git config --list`                                | View all configs    | –                                                   |

---

## 2️⃣ Starting & Cloning Repos

| Command           | Purpose                                    | Example                                         |
| ----------------- | ------------------------------------------ | ----------------------------------------------- |
| `git init`        | Initialize a new repo in current directory | `git init`                                      |
| `git clone <url>` | Copy a remote repo locally                 | `git clone https://github.com/user/project.git` |

---

## 3️⃣ Basic Workflow

| Command                   | Purpose                   | Example                         |
| ------------------------- | ------------------------- | ------------------------------- |
| `git status`              | See changes & branch info | `git status`                    |
| `git add <file>`          | Stage a file              | `git add app.py`                |
| `git add .`               | Stage all changes         | –                               |
| `git commit -m "message"` | Save changes with message | `git commit -m "Fix login bug"` |
| `git log`                 | View commit history       | `git log --oneline` (compact)   |

---

## 4️⃣ Branching & Merging

| Command                    | Purpose                   | Example          |
| -------------------------- | ------------------------- | ---------------- |
| `git branch`               | List branches             | –                |
| `git branch new-feature`   | Create a branch           | –                |
| `git checkout new-feature` | Switch to a branch        | –                |
| `git checkout -b hotfix`   | Create & switch           | –                |
| `git merge main`           | Merge into current branch | `git merge main` |
| `git branch -d branchname` | Delete branch             | –                |

---

## 5️⃣ Remote Operations

| Command                       | Purpose                      | Example                                              |
| ----------------------------- | ---------------------------- | ---------------------------------------------------- |
| `git remote -v`               | View remote URLs             | –                                                    |
| `git remote add origin <url>` | Add a remote                 | `git remote add origin git@github.com:user/repo.git` |
| `git push origin main`        | Push branch to remote        | –                                                    |
| `git pull`                    | Fetch & merge latest changes | –                                                    |
| `git fetch`                   | Fetch without merge          | –                                                    |

---

## 6️⃣ Stashing & Cleaning

| Command         | Purpose                              | Example |
| --------------- | ------------------------------------ | ------- |
| `git stash`     | Save uncommitted changes temporarily | –       |
| `git stash pop` | Apply stashed changes                | –       |
| `git clean -fd` | Remove untracked files/dirs          | –       |

---

## 7️⃣ Undo & Reset

| Command                     | Purpose                                  | Example |
| --------------------------- | ---------------------------------------- | ------- |
| `git checkout -- <file>`    | Discard local changes                    | –       |
| `git reset HEAD <file>`     | Unstage a file                           | –       |
| `git revert <commit>`       | Create new commit to undo a specific one | –       |
| `git reset --hard <commit>` | Reset branch to a commit (destructive)   | –       |

---

## 8️⃣ Useful Logs & Diffs

| Command                                | Purpose               | Example |
| -------------------------------------- | --------------------- | ------- |
| `git diff`                             | Show unstaged changes | –       |
| `git diff --staged`                    | Show staged changes   | –       |
| `git log --graph --oneline --decorate` | Pretty branch graph   | –       |

---

### Quick Daily Flow

```bash
git pull origin main
git checkout -b feature/my-task
# ...code changes...
git add .
git commit -m "Implement my feature"
git push origin feature/my-task
```

This cheat sheet covers the **most common Git operations** you’ll use as a DevOps engineer or developer.

<img width="1200" height="674" alt="image" src="https://github.com/user-attachments/assets/f134cd03-fc1f-4bef-a076-03d1632ada26" />


# Git & GitHub Tutorials 

This repository contains my personal **Git & GitHub tutorials**, complete command references, and workflows.  
It covers everything from **beginner basics** to **advanced GitHub workflows**.

---

## 📌 Topics Covered

### **Git Basics**
- Initializing a repository
- Staging and committing changes
- Viewing commit history
- Resetting and discarding changes
- Restoring previous versions
- Using `.gitignore`
- Creating Git aliases

### **GitHub Integration**
- Linking local repositories to GitHub
- Pushing and pulling code
- Cloning repositories
- Fetching updates
- Force pushing changes

### **Branching & Merging**
- Creating and switching branches
- Merging branches into main
- Resolving merge conflicts

### **Feature Branch Workflow**
- Working on new features safely
- Creating pull requests
- Merging via GitHub interface
- Keeping local repositories updated

---

## Git Basics

| **Command**                 | **Description**                          |
|----------------------------|----------------------------------------|
| `git init`                 | Initialize a new repository            |
| `git status`               | Show changes in the working directory |
| `git add <file>`           | Stage a single file                   |
| `git add .`                | Stage all files                       |
| `git commit -m "msg"`      | Commit staged changes                 |
| `git commit --amend`       | Update the previous commit            |
| `git log --all --graph`    | View commit history visually          |
| `git reset <file>`         | Unstage a file                        |
| `git checkout -- <file>`   | Discard changes in a file             |
| `git checkout <hash>`      | Move to a specific commit             |
| `git config --global user.name "Name"` | Set username globally |
| `git config --global user.email "Email"` | Set email globally  |
| `git config --global alias.s "status"` | Create shortcut (`git s`) |
| `rm -rf .git`              | Remove Git from the project          |

---

## GitHub Integration

| **Command**                              | **Description** |
|----------------------------------------|-----------------|
| `git remote add <name> <url>`          | Link a local repo to GitHub |
| `git remote -v`                        | Show linked remotes |
| `git remote remove <name>`             | Remove remote link |
| `git config --global credential.username <username>` | Configure GitHub username |
| `git push <remote> <branch>`           | Push code to GitHub |
| `git push <remote> <branch> --set-upstream` | Set default remote push |
| `git push <remote> <branch> -f`        | Force push changes |
| `git clone <url>`                      | Clone a repository |
| `git clone <url> <folder>`             | Clone into a custom folder |
| `git fetch`                            | Fetch updates from remote |
| `git pull <remote> <branch>`           | Pull changes from GitHub |

---


## 🌿 Branching

| **Command**             | **Description** |
|------------------------|------------------|
| `git branch <name>`    | Create a new branch |
| `git branch`           | List all branches |
| `git checkout <name>`  | Switch to another branch |
| `git branch -D <name>` | Delete a branch |
| `git log --all --graph` | Visualize branches |

---

## Merging

| **Command**                           | **Description** |
|-------------------------------------|-----------------|
| `git checkout main`                 | Switch to the main branch |
| `git merge <branch>`                | Merge another branch into the current one |
| `git merge <branch> -m "message"`   | Merge with a commit message |

---

## Merge Conflicts

| **Steps**       | **Description** |
|---------------|------------------|
| **1. Conflict** | When two branches modify the same code, Git shows conflict markers like: <br> `<<<<<<< HEAD` <br> `=======` <br> `>>>>>>> branch` |
| **2. Resolve** | Edit the file → keep the correct code and delete conflict markers |
| **3. Stage**   | `git add .` |
| **4. Commit**  | `git commit -m "Resolved merge conflict"` |

---

##  Feature Branch Workflow

| **Step** | **Command**                                | **Description** |
|---------|--------------------------------------------|------------------|
| 1       | `git branch new-feature`                   | Create a new feature branch |
|         | `git checkout new-feature`                 | Switch to the feature branch |
| 2       | `git add .`                                | Stage changes |
|         | `git commit -m "Added new feature"`        | Commit changes |
| 3       | `git push origin new-feature`             | Push feature branch to GitHub |
| 4       | **Open Pull Request**                      | Go to GitHub → Create PR → Ask for review |
| 5       | **Merge Pull Request**                     | Merge PR into **main** on GitHub |
| 6       | `git checkout main`                        | Switch to main branch locally |
|         | `git pull origin main`                     | Update local main branch |

---

## 📘 References

- [Git Docs](https://git-scm.com/docs)
- [GitHub Guides](https://guides.github.com/)
- [Learn Git Branching](https://learngitbranching.js.org/)

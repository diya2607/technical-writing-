
# 🐙 GIT & GITHUB — VERSION CONTROL AND COLLABORATION

<p align="center">
  <b>TECHNICAL WRITING | MODULE 05</b>
</p>

> Git is a distributed version control system, while GitHub is an online platform for hosting Git repositories and collaborating on projects.

---

## 📑 TABLE OF CONTENTS

1. Introduction to Git
2. Introduction to GitHub
3. Git vs GitHub
4. Installation
5. Git Configuration
6. Repository Creation
7. Git Workflow
8. Essential Git Commands
9. Staging and Committing
10. Branching
11. Merging
12. Remote Repositories
13. Cloning
14. Push and Pull
15. Pull Requests
16. Forking
17. Merge Conflicts
18. .gitignore
19. GitHub Repository Management
20. Best Practices

## 01. INTRODUCTION TO GIT

Git is a distributed version control system.

It helps developers:
- Track changes in files.
- Maintain project history.
- Restore earlier versions.
- Work on separate branches.
- Collaborate with other developers.

## 02. INTRODUCTION TO GITHUB

GitHub is a cloud-based platform for hosting Git repositories.

It provides:
- Online code storage.
- Collaboration.
- Pull requests.
- Issues.
- Project management.
- Repository management.
- Code review.

Website:

https://github.com/

## 03. GIT VS GITHUB

| Git | GitHub |
|---|---|
| Version control system | Online hosting platform |
| Works locally | Works online |
| Tracks file changes | Hosts repositories |
| Uses Git commands | Provides graphical interface |
| Can work offline | Requires internet for online features |

## 04. INSTALLATION

Check Git:

```bash
git --version
```

On macOS, Git can be installed using Apple's Command Line Tools or other supported installation methods.

## 05. GIT CONFIGURATION

Set your username:

```bash
git config --global user.name "Your Name"
```

Set your email:

```bash
git config --global user.email "your-email@example.com"
```

Check configuration:

```bash
git config --global --list
```

## 06. REPOSITORY CREATION

A repository stores project files and Git history.

Initialise a repository:

```bash
git init
```

This creates a local Git repository.

## 07. UNDERSTANDING THE GIT WORKFLOW

Git has three important areas:

1. Working Directory
2. Staging Area
3. Local Repository

Workflow:

```text
Working Directory
       |
       | git add
       v
Staging Area
       |
       | git commit
       v
Local Repository
       |
       | git push
       v
Remote Repository
```

## 08. ESSENTIAL GIT COMMANDS

| Command | Purpose |
|---|---|
| `git init` | Initialise repository |
| `git status` | Check file status |
| `git add .` | Stage all changes |
| `git add file.md` | Stage a specific file |
| `git commit -m "message"` | Save a commit |
| `git log` | View commit history |
| `git log --oneline` | Compact history |
| `git diff` | View unstaged differences |
| `git diff --staged` | View staged differences |
| `git show` | Inspect a commit |
| `git rm file` | Remove tracked file |
| `git mv old new` | Rename or move tracked file |

## 09. STAGING AND COMMITTING

**Step 1: Check status**

```bash
git status
```

**Step 2: Stage changes**

```bash
git add .
```

**Step 3: Commit changes**

```bash
git commit -m "Added documentation"
```

A commit records a snapshot of the staged changes.

## 10. BRANCHING

Branches allow developers to work on different features independently.

List branches:

```bash
git branch
```

Create a branch:

```bash
git branch feature
```

Create and switch:

```bash
git switch -c feature
```

Switch branches:

```bash
git switch main
```

Delete a merged branch:

```bash
git branch -d feature
```

## 11. MERGING

Merging combines changes from one branch into another.

Example:

```bash
git switch main

git merge feature
```

This merges the feature branch into main.

## 12. REMOTE REPOSITORIES

A remote repository is a version of your project hosted online.

Connect a remote:

```bash
git remote add origin REPOSITORY_URL
```

View remote connections:

```bash
git remote -v
```

Change a remote URL:

```bash
git remote set-url origin REPOSITORY_URL
```

## 13. CLONING

Cloning creates a local copy of an existing remote repository.

```bash
git clone REPOSITORY_URL
```

It downloads the repository and its available history.

## 14. PUSH AND PULL

**Push:**

Uploads local commits to a remote repository.

```bash
git push
```

First push of a new branch:

```bash
git push -u origin main
```

**Pull:**

Fetches remote changes and integrates them into the current branch.

```bash
git pull
```

## 15. FETCH

Fetch downloads information from a remote repository without automatically integrating the changes.

```bash
git fetch origin
```

Difference:

- `git fetch`: Downloads remote updates.
- `git pull`: Fetches and integrates updates.

## 16. PULL REQUESTS

A Pull Request (PR) proposes merging changes from one branch into another on GitHub.

Steps:

1. Create a branch.
2. Make changes.
3. Commit changes.
4. Push the branch.
5. Open GitHub.
6. Create a Pull Request.
7. Review changes.
8. Merge the Pull Request.

## 17. FORKING

Forking creates your own GitHub copy of another user's repository.

It is commonly used for:
- Open-source contributions.
- Independent experimentation.
- Proposing changes to another project.

## 18. MERGE CONFLICTS

A merge conflict occurs when Git cannot automatically combine changes.

How to resolve:

1. Open the conflicting file.
2. Identify the conflicting sections.
3. Decide which changes to retain.
4. Remove conflict markers.
5. Save the file.
6. Stage the resolved file.
7. Commit the resolution.

## 19. .gitignore

The `.gitignore` file specifies files and directories Git should ignore when they are untracked.

Example:

```gitignore
.DS_Store
*.log
*.o
*.out
build/
```

This prevents unnecessary generated files from being added.

## 20. UNDOING CHANGES

Discard unstaged changes in a file:

```bash
git restore filename
```

Unstage a file:

```bash
git restore --staged filename
```

Create a new commit that reverses an earlier commit:

```bash
git revert COMMIT_ID
```

Reset to an earlier commit:

```bash
git reset --soft HEAD~1
```

**Note:** `git reset --hard` can permanently discard local work. Use it carefully.

## 21. GITHUB REPOSITORY MANAGEMENT

A GitHub repository can contain:

- README.md
- Source code
- Documentation
- Images
- Folders
- Issues
- Pull Requests
- Release information

The README introduces the project and helps visitors understand its purpose.

## 22. IMPORTANT GIT CONCEPTS

| Concept | Meaning |
|---|---|
| Repository | Project tracked by Git |
| Commit | Recorded snapshot |
| Branch | Independent development line |
| Merge | Combining branch histories |
| Remote | Linked repository |
| Clone | Copy a remote repository |
| Fork | Personal GitHub copy |
| Pull Request | Proposal to merge changes |
| Conflict | Changes that need manual resolution |
| HEAD | Reference to current checkout |

## 23. BEST PRACTICES

- Use meaningful commit messages.
- Commit changes regularly.
- Create branches for separate features.
- Keep README files updated.
- Never upload passwords or secret keys.
- Check status before committing.
- Review changes before pushing.
- Use `.gitignore` appropriately.

## 🎯 LEARNING OUTCOME

Through Git and GitHub, I learned how to initialise repositories, track changes, stage and commit files, create branches, merge changes, connect remote repositories, push and pull updates, and manage projects collaboratively.

---

**END OF MODULE 05 | GIT & GITHUB**

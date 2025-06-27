# Git Basics

This cheat sheet covers the most common Git commands for initializing repositories, tracking changes, and collaborating with others.

---

## Getting Started

| Command                                            | Description                          |
|----------------------------------------------------|--------------------------------------|
| `git --version`                                    | Checks the installed version of Git  |
| `git config --global user.name "Your Name"`        | Sets your Git username (global)      |
| `git config --global user.email "you@example.com"` | Sets your Git email address (global) |

---

## Repository Setup

| Command           | Description                                            |
|-------------------|--------------------------------------------------------|
| `git init`        | Initializes a new Git repository in the current folder |
| `git clone [url]` | Creates a local copy of a remote repository            |

---

## Staging and Committing

| Command                   | Description                                    |
|---------------------------|------------------------------------------------|
| `git status`              | Shows file changes (untracked, modified, etc.) |
| `git add filename`        | Adds a specific file to the staging area       |
| `git add .`               | Adds all current changes to staging            |
| `git commit -m "message"` | Records changes with a short description       |

---

## Viewing History

| Command             | Description                        |
|---------------------|------------------------------------|
| `git log`           | Shows a list of previous commits   |
| `git log --oneline` | Shows a simplified one-line log    |

---

## Working with Branches

| Command                  | Description                                  |
|--------------------------|----------------------------------------------|
| `git branch`             | Lists all branches                           |
| `git branch branchname`  | Creates a new branch                         |
| `git checkout branchname`| Switches to the specified branch             |
| `git switch branchname`  | Alternative to checkout (modern usage)       |
| `git merge branchname`   | Merges the given branch into the current one |

---

## Pushing and Pulling

| Command                   | Description                                  |
|---------------------------|----------------------------------------------|
| `git remote -v`           | Shows the remote repository connection(s)    |
| `git push`                | Uploads local commits to a remote repository |
| `git pull`                | Retrieves and merges changes from the remote |
| `git push -u origin main` | Pushes a local branch and sets upstream      |

---

## Undoing Changes (Caution)

| Command                         | Description                          |
|---------------------------------|--------------------------------------|
| `git restore filename`          | Reverts a file to last commit        |
| `git reset HEAD filename`       | Unstages a file                      |
| `git checkout -- filename`      | Discards local changes (legacy)      |

---

## Notes

- Use `.gitignore` to tell Git which files/folders to ignore.
- Always commit with a clear, meaningful message.
- Use branches to isolate features and avoid conflicts.

---

For full documentation, visit: https://git-scm.com/doc
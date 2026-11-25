# Mission 6 - Git and GitHub

## 1. Task / objective
Practice the core Git workflow, create a feature branch to update the root README, open a Pull Request on GitHub, and document essential Git commands and collaboration concepts.

## 2. Work completed
* Practiced checking repository status, staging files, committing snapshots, and viewing commit history.
* Created a new branch named `update-about`, added a `"My Learning"` section to the root `README.md`, and pushed the branch to GitHub.
* Opened a Pull Request comparing `update-about` into `main` on GitHub (PR Status: **Open / Unmerged**, awaiting instructor review).
* Switched back to the `main` branch locally and documented a complete Git command glossary.

## 3. Commands / tools used
* `git status` — Inspects modified, untracked, and staged files in the repository.
* `git add <file>` — Stages specific file changes in preparation for a commit.
* `git commit -m "..."` — Records a permanent snapshot of staged changes with a descriptive message.
* `git log` — Displays the commit history of the repository.
* `git checkout -b update-about` — Creates and switches to a new branch named `update-about`.
* `git push -u origin update-about` — Publishes the new branch to GitHub.
* `git checkout main` & `git pull` — Switches back to the `main` branch and retrieves any remote updates.

## 4. My understanding

### Task 6.1 - Basic Git Workflow

| Git Operation | What it does in your own words |
| :--- | :--- |
| **Check repository status (`git status`)** | Shows which files have been created, modified, or staged since the last commit, and tells me which branch I am currently on. |
| **Stage selected changes (`git add`)** | Moves specific modified files into the staging area so I can control exactly what goes into the next commit. |
| **Create a commit (`git commit`)** | Saves a permanent snapshot of all currently staged changes into Git's history along with a descriptive message. |
| **View commit history (`git log`)** | Displays a chronological list of previous commits, showing each commit's unique hash ID, author, date, and message. |

**Difference between staging a change and committing it:**
Staging (`git add`) is like putting items into a box before sealing it—it lets you select and review which specific changes you want to include. Committing (`git commit`) seals that box and permanently saves that snapshot into your repository's version history.

---

### Task 6.2 & 6.3 - Branches and Pull Requests
* **Branch & PR Status:** Created the `update-about` branch, added the `"My Learning"` section to the root `README.md`, pushed `update-about` to GitHub, and opened a Pull Request into `main`. The Pull Request is currently **Open (not merged)** on GitHub as instructed.
* **What a Branch and a Pull Request are:** A **branch** is an independent line of development that lets you make edits or build features without affecting the stable `main` branch. A **Pull Request (PR)** is a GitHub feature that proposes merging changes from one branch into another, allowing teammates or reviewers to inspect the differences and discuss changes before they become part of `main`.
* **Why they are useful in team projects:** When multiple people work on the same project, branches prevent teammates from overwriting each other's unfinished work, and Pull Requests provide a safety checkpoint to review code and catch bugs before merging into the main project.

---

### Task 6.4 - Git Command Glossary

| Git Operation | Command | One-Line Explanation |
| :--- | :--- | :--- |
| **Initialise a repository** | `git init` | Creates a new hidden `.git` folder to start tracking a project with Git version control. |
| **Check status** | `git status` | Displays the current branch along with modified, untracked, and staged files. |
| **Stage changes** | `git add` | Adds file modifications to the staging area so they are ready to be committed. |
| **Commit changes** | `git commit` | Permanently saves a snapshot of staged changes into the local repository history. |
| **View history** | `git log` | Lists past commits with their commit IDs, authors, timestamps, and messages. |
| **Create or list branches** | `git branch` | Lists all local branches or creates a new branch when given a branch name. |
| **Switch branches** | `git checkout` / `git switch` | Moves your working directory onto a different branch. |
| **Publish changes** | `git push` | Uploads local commits from your computer to a remote repository on GitHub. |
| **Retrieve remote changes** | `git pull` | Downloads and merges the latest commits from GitHub onto your local branch. |

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
* `mission-06-git-github/README.md`
* Branch `update-about` and Pull Request visible on GitHub

## 8. Commit details
Committed with message: `"Complete Git and GitHub collaboration mission"` and pushed to GitHub.
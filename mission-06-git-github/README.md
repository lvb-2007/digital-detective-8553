 — Git and GitHub

## 1. Task / objective
Explain the Git workflow, create and publish a branch, open a Pull Request,
and describe how branches and reviews support collaboration.

## 2. Work completed

### Task 6.1 — Basic Git workflow

| Git operation | What it does |
|---|---|
| Check status | Shows changed, staged and untracked files |
| Stage changes | Selects changes for the next commit |
| Commit changes | Saves staged changes in the repository history |
| View history | Shows earlier commits |

Staging selects which changes to include; committing records those staged
changes in history.

### Task 6.2 — Branch and README change
The `update-about` branch was created and published. It adds a “My Learning”
section to the root README.

### Task 6.3 — Pull Request
A Pull Request from `update-about` to `main` requests review of the root README
change. [PR #1](https://github.com/lvb-2007/digital-detective-8553.git1)
is open and has not been merged. I reviewed its diff: it changes only the
intended “My Learning” section in `README.md`.

A branch is an isolated line of work. A Pull Request asks for changes from a
branch to be reviewed before they are merged into another branch.

### Task 6.4 — Git command glossary

| Operation | Command | Explanation |
|---|---|---|
| Initialise a repository | `git init` | Starts Git tracking in a folder |
| Check status | `git status` | Shows changed, staged and untracked files |
| Stage changes | `git add <file>` | Selects changes for the next commit |
| Commit changes | `git commit -m "message"` | Records staged changes with a message |
| View history | `git log --oneline` | Lists commits in short form |
| Create/list branches | `git switch -c name` / `git branch` | Creates a branch / lists branches |
| Switch branches | `git switch name` | Moves to another branch |
| Publish changes | `git push` | Uploads local commits to GitHub |
| Retrieve changes | `git pull` | Fetches and integrates remote commits |

## 3. Commands / tools used
- `git status`, `git add`, `git commit`, `git log --oneline` — the basic
  workflow.
- `git switch -c update-about` and `git push -u origin update-about` — created
  and published the branch.
- GitHub — opened PR #1 and reviewed its one-file diff.
- VS Code — edited the mission and root README files.

## 4. My understanding
Git records changes, while GitHub hosts a repository for sharing and
collaboration. Staging and committing are separate so I can choose exactly
what enters each commit. Branches let me work separately, and Pull Requests
make proposed changes visible for review before merging.

## 5. Difficulties faced
I initially forgot the `-u` option when publishing a new branch, and the PR
status was not recorded in the README.

## 6. How I resolved them
I used `git push -u origin update-about` to set the upstream branch and checked
the GitHub Pull Request page to record its actual status.

## 7. Evidence / files
- The `update-about` branch and its Pull Request on GitHub.
- The root README's “My Learning” section.

## 8. Commit details
- Branch commit: `Add My learning section to README`
- Pull Request #1: open, not merged.
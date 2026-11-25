Mission 2 — Become comfortable with the Terminal

## 1. Task / objective
Practise basic Terminal operations, manage files inside a safe practice
folder, understand command flags and pipes, and learn what package managers
do.

## 2. Work completed

### Task 2.1 — Basic Terminal operations

| Operation | Command | What it does | What I observed |
|---|---|---|---|
| Current-directory display | `pwd` | Shows the current folder's full path | It ended at the assignment project folder; the account portion is redacted |
| Directory listing | `ls` | Lists files and folders | It showed the README and mission folders |
| Detailed listing | `ls -l` | Shows permissions, size and modification time | The permission string included `-rw-r--r--` |
| Change directory | `cd ..` | Moves to the parent folder | The path became one directory shorter |
| Create a directory | `mkdir terminal-practice` | Creates a folder | The new folder appeared in the listing |
| Create a file | `touch terminal-practice/notes.txt` | Creates an empty file | `notes.txt` appeared in the practice folder |
| Copy a file | `cp .../notes.txt .../notes-copy.txt` | Creates a second copy | Both names were present |
| Rename a file | `mv .../notes-copy.txt .../notes-renamed.txt` | Moves or renames a file | The renamed file appeared and the old name was gone |
| Display file contents | `cat terminal-practice/notes.txt` | Prints a text file | Nothing printed because the file was empty |

### Task 2.2 — File changes
The practice file contained:

```text
This is the first line
This is the second line
```

The `>` operator replaces a file's contents; `>>` appends text while keeping
what is already there. `cp` leaves the original in place, while `mv` moves or
renames the file.

### Task 2.3 — Flags and pipes
- `-l` requests a detailed listing.
- `-a` includes hidden entries.
- `-h` displays sizes in a human-readable form.
- `|` sends one command's output to another command. For example,
  `ls -l | head` shows only the first lines.

### Task 2.4 — Package managers
`brew --version` reported Homebrew 7.0.14. A package manager installs,
updates and removes software and can install required dependencies.

## 3. Commands / tools used
- `pwd`, `ls`, `ls -l`, `ls -lah`, `cd`, `mkdir`, `touch`, `cp`, `mv` and
  `cat` — inspected and managed files.
- `echo`, `>` and `>>` — replaced and appended file contents.
- `|` and `head` — passed output between commands and limited displayed lines.
- `brew --version` — checked the installed Homebrew version.
- Git — committed and published the mission work.

## 4. My understanding
The Terminal runs commands in the current directory, so `pwd` and `ls` help
confirm where I am and what files are present. Flags change how a command
behaves, and pipes pass output between commands. Copying preserves the
original, moving changes its location or name, and `>` differs from `>>` in
whether existing file contents are replaced or retained.

## 5. Difficulties faced
Homebrew's list and update information did not display as expected.

## 6. How I resolved them
I confirmed that Homebrew was installed with `brew --version`. No package
installation was needed for this mission.

## 7. Evidence / files
- This README and the files under `terminal-practice/`.
- The practice files include `notes.txt`, `notes-renamed.txt`, `practice.txt`
  and `practice-backup-renamed.txt`.
- Personal account and device names are redacted from command observations.

## 8. Commit details
- Commit message: `Complete Terminal and file management mission`
- The mission commit is present on GitHub.
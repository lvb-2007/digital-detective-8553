# Mission 3 — Understand the operating system

## 1. Task / objective
Explore system information, processes, storage, paths and file permissions,
then explain the responsibilities of an operating system.

## 2. Work completed

### Task 3.1 — System information

| Information | Command | Privacy-safe observation |
|---|---|---|
| Operating system | `uname -s` | Darwin (macOS) |
| Hardware architecture | `uname -m` | arm64 |
| Root-volume storage | `df -h /` | 926 GiB total, 17 GiB used, 798 GiB available (3% used) |

### Task 3.2 — Processes
A process is a running program or operating-system service. The operating
system assigns each process a PID so it can identify and manage it. In the
process list I observed `launchd` (PID 1) and `logd` (PID 324), both macOS
system processes.

### Task 3.3 — Paths and permissions
An absolute path starts at `/`; for privacy, the user-folder portion of my
project path is redacted: `/Users/[redacted]/Desktop/the-digital-detective-8553`.
A relative path such as `mission-03-operating-system/README.md` is interpreted
from the current project directory.

The README's permission string is `-rw-r--r--`. The first character (`-`)
means it is a regular file. The owner's `rw-` means read and write are
allowed, but execute is not. I did not change file permissions.

| Permission | Meaning | Example |
|---|---|---|
| `r` | Read the file's contents | Open a text file |
| `w` | Change the file | Edit a text file |
| `x` | Run a file or enter a directory | Run a script or `cd` into a folder |

### Task 3.4 — Operating-system responsibilities

| Responsibility | What it does | Example |
|---|---|---|
| Process management | Schedules and tracks running programs | Running a browser and an editor |
| Memory management | Allocates and reclaims RAM | Closing an application releases resources |
| Device management | Provides software access to hardware | Sending a document to a printer |
| File management | Organises and accesses files and folders | Saving a document on a drive |
| User interface | Lets people interact with the computer | Finder or Terminal |
| Security and permissions | Controls access to resources | Restricting access to a protected file |

## 3. Commands / tools used
- `uname -s` and `uname -m` — identified the OS and architecture without
  including the machine name.
- `df -h /` — checked root-volume storage.
- `ps -Ao pid,comm` — observed running processes and their PIDs.
- `pwd` and `ls -l` — checked the project location and file permissions.
- VS Code and Git — documented and versioned the work.

## 4. My understanding
macOS manages the computer's hardware and supplies services that applications
use. Processes are running programs or services, and PIDs let the OS track
them. Paths identify files either from the filesystem root or relative to the
current folder. Permission bits control reading, writing and executing; the
OS also manages memory, devices, files and security.

## 5. Difficulties faced
The initial notes included unfinished storage placeholders and identifying
device information.

## 6. How I resolved them
I replaced the placeholders with observed storage and process information and
used commands that did not expose the device name or account name.

## 7. Evidence / files
- This README contains the privacy-safe system, process, path and permission
  observations.

  

## 8. Commit details
- Commit message: `Document operating system and file management`
- Pushed to GitHub: YES
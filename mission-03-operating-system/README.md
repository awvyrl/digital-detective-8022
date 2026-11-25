# Mission 3 - Operating System, Processes, and Permissions

## 1. Task / objective
Explore the operating system environment, active user account, disk storage, running processes, file paths, and permissions using Terminal, and explain the core responsibilities of an operating system.

## 2. Work completed
* Inspected OS kernel details, user identity (redacted), available disk storage, and active system processes via Terminal.
* Identified running processes and explained the purpose of Process Identifiers (PIDs).
* Compared absolute and relative file paths and inspected owner file permissions (`r`, `w`, `x`) using `ls -l`.
* Documented the six core responsibilities of an operating system with real-world examples.

## 3. Commands / tools used
* `uname -srm` — Displays the operating system kernel name, version, and hardware architecture.
* `whoami` — Prints the username of the currently active account.
* `df -h /` — Displays total, used, and available storage space on the main disk volume in human-readable units.
* `ps aux | head -n 6` — Displays a snapshot of currently running processes and their PIDs.
* `ls -l` — Shows detailed file metadata, including read, write, and execute permission letters.

## 4. My understanding

### Task 3.1 - Explore Your Operating System

| Information Explored | What it tells you | Your Observation (Privacy-Safe) |
| :--- | :--- | :--- |
| **Operating system / system details (`uname -srm`)** | Identifies the OS kernel name, release version, and CPU architecture. | `Darwin 25.x.x arm64` (macOS running on Apple Silicon). |
| **Current account identity (`whoami`)** | Shows which user account owns the active Terminal session. | `[redacted]` (standard non-administrator user account). |
| **Available and used storage (`df -h /`)** | Shows total disk capacity, used storage, and free space available on the main drive. | Displayed total SSD capacity along with used and available space in GiB. |
| **System activity snapshot (`ps aux`)** | Shows active background daemons and user applications currently consuming CPU and memory. | Showed system processes (`launchd`) alongside active user apps. |

---

### Task 3.2 - Understand Processes
* **What is a process?** A process is an active instance of a program that is currently loaded into memory and being executed by the CPU.
* **What does the PID column represent?** PID stands for **Process Identifier**—a unique number assigned by the operating system to track, manage, or terminate each running process.
* **Two examples of running processes on my computer:**
  1. `zsh` (the interactive Terminal shell running my commands).
  2. `Visual Studio Code` / `Google Chrome` (open desktop applications).

---

### Task 3.3 - Understand Paths and Permissions
* **Absolute Path vs. Relative Path:**
  * An **absolute path** starts from the root directory (`/`) and gives the complete location of a file or folder regardless of where you currently are in Terminal.
    * *Example:* `/Users/[redacted]/Desktop/digital-detective-8022/mission-03-operating-system`
  * A **relative path** describes a location starting from your current working directory.
    * *Example:* `./mission-03-operating-system` (when inside `digital-detective-8022`) or `../mission-02-terminal` (moving to a sibling folder).
* **Owner Permissions Observation (`ls -l README.md`):**
  * The output begins with `-rw-r--r--`. The first three permission characters after the leading `-` (`rw-`) belong to the file's owner. This means the owner has **read (`r`)** and **write (`w`)** permissions, while **execute (`-`)** permission is disabled because `README.md` is a text document rather than a runnable script.

| Permission | Meaning | Example |
| :--- | :--- | :--- |
| **r - Read** | Allows a file's contents to be viewed or a directory's contents to be listed. | Opening `README.md` with `cat` or VS Code. |
| **w - Write** | Allows a file's contents to be modified or files inside a directory to be added/deleted. | Editing and saving changes in `README.md`. |
| **x - Execute** | Allows a file to be run as a program/script; on a directory, allows entering/traversing it with `cd`. | Running a Python/shell script or opening a folder. |

---

### Task 3.4 - Operating-System Responsibilities

| OS Responsibility | Your Explanation | Example |
| :--- | :--- | :--- |
| **Process management** | Decides which processes get CPU time, switches between tasks smoothly, and handles starting/stopping programs. | Running VS Code, a browser, and Terminal simultaneously without freezing. |
| **Memory management** | Allocates RAM to active programs when they open and reclaims that memory when they close. | Giving Chrome memory for open tabs while preventing apps from overwriting each other's data. |
| **Device management** | Communicates with hardware components and external peripherals using device drivers. | Recognizing a keyboard, trackpad, or wireless earbuds when connected. |
| **File management** | Organizes stored data into folders, files, and directory trees while tracking file sizes and locations. | Creating mission folders and saving `.md` and `.py` files on the SSD. |
| **User interface / shell** | Provides an interface for users to interact with the computer visually or through text commands. | macOS Finder (graphical UI) and the `zsh` Terminal (command-line shell). |
| **Security and permissions** | Enforces user authentication and access rules so unauthorized users or programs cannot modify protected files. | Requiring a password for admin actions and restricting write access via file permissions. |

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
* `mission-03-operating-system/README.md`

## 8. Commit details
Committed with message: `"Document operating system and file management"` and pushed to GitHub.
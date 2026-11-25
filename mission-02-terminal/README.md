# Mission 2 - Terminal and File Management

## 1. Task / objective
Practice essential command-line interface (CLI) navigation and file-management commands safely inside a practice folder, understand command flags and pipes, and explain the role of package managers.

## 2. Work completed
* Practiced core Terminal commands (`pwd`, `ls`, `ls -l`, `cd`, `mkdir`, `touch`, `cp`, `mv`, `cat`)[cite: 5].
* Created a safe `terminal-practice/` folder inside the repository and practiced creating, appending, copying, and renaming text files[cite: 5].
* Compared normal and flagged directory listings (`ls` vs. `ls -lah`) and tested command piping (`ls -l | head -n 5`)[cite: 6].
* Checked package manager availability (`brew --version`) and documented how package managers work[cite: 6].

## 3. Commands / tools used
* `pwd` — Prints the full path of the current working directory[cite: 5].
* `ls` / `ls -l` / `ls -lah` — Lists folder contents in standard, detailed, and hidden + human-readable formats[cite: 5, 6].
* `cd` — Changes the current working directory[cite: 5].
* `mkdir` — Creates a new directory[cite: 5].
* `touch` — Creates an empty file[cite: 5].
* `echo` with `>` and `>>` — Writes or appends text into a file[cite: 5].
* `cat` — Displays the contents of a file in Terminal[cite: 5].
* `cp` — Copies a file[cite: 5].
* `mv` — Moves or renames a file[cite: 5].
* `head -n 5` with `|` — Pipes command output to display only the first 5 lines[cite: 6].
* `brew --version` — Checks whether the Homebrew package manager is installed on macOS[cite: 6].

## 4. My understanding

### Task 2.1 - Basic Terminal Operations

| Operation / Command Name | What it does | What I observed |
| :--- | :--- | :--- |
| **Current-directory display (`pwd`)** | Displays the full path of the folder I am currently working in[cite: 5]. | Printed `/Users/[redacted]/.../digital-detective-8022`[cite: 5, 6]. |
| **Directory listing (`ls`)** | Lists visible files and folders in the current location[cite: 5]. | Showed `README.md`, `evidence`, and all `mission-00` to `mission-08` folders[cite: 3, 5]. |
| **Detailed listing (`ls -l`)** | Lists items with permissions, owner, file size, and last modified timestamp[cite: 5]. | Displayed detailed rows starting with `drwxr-xr-x` for folders and `-rw-r--r--` for files[cite: 5, 7]. |
| **Change directory (`cd`)** | Moves into another folder or up to the parent folder (`cd ..`)[cite: 5]. | Prompt location changed from `digital-detective-8022` to `terminal-practice` and back[cite: 5]. |
| **Create directory (`mkdir`)** | Creates a new empty folder[cite: 5]. | Created the `terminal-practice` folder inside my repository[cite: 5]. |
| **Create empty file (`touch`)** | Creates a new 0-byte empty file[cite: 5]. | Created `notes.txt` inside `terminal-practice`[cite: 5]. |
| **Copy file (`cp`)** | Creates a duplicate copy of a file with a new name[cite: 5]. | Both `notes.txt` and `notes_copy.txt` appeared in the directory[cite: 5]. |
| **Move / rename file (`mv`)** | Renames a file or moves it to a different path[cite: 5]. | `notes_copy.txt` was renamed to `backup_notes.txt`[cite: 5]. |
| **Display file contents (`cat`)** | Prints the text stored inside a file directly to the terminal screen[cite: 5]. | Displayed both lines of text saved inside `notes.txt`[cite: 5]. |

---

### Task 2.2 - Safe File Changes & Concept Questions
* **Difference between replacing a file's contents (`>`) and adding text to the end (`>>`):** Using a single `>` overwrites the entire file and erases whatever was inside before, whereas `>>` appends new text to the bottom without deleting existing lines[cite: 5].
* **Difference between copying a file (`cp`) and moving a file (`mv`):** Copying creates a second identical file while keeping the original intact; moving transfers the original file to a new name or folder without leaving a duplicate behind[cite: 5].
* **What information the current-directory display (`pwd`) provides:** It shows your exact path from the root directory down to your current folder so you always know where commands will execute[cite: 5].
* **Why a directory-listing operation (`ls`) is useful:** It lets you quickly verify what files and folders exist in your current location and confirm that new files or changes worked properly[cite: 5].

---

### Task 2.3 - Flags and Pipes
* **Normal listing (`ls`) vs. Flagged listing (`ls -lah`):** Running plain `ls` only shows visible file and folder names[cite: 5, 6]. Adding `-lah` combines three flags: `-l` displays permissions, ownership, and timestamps; `-a` reveals hidden files starting with a dot (such as `.git` and `.DS_Store`); and `-h` converts raw byte counts into human-readable units like `KB` or `MB`[cite: 6].
* **How pipes work (`ls -l | head -n 5`):** The pipe symbol (`|`) connects two commands by taking the standard output of the command on the left (`ls -l`) and feeding it directly as input into the command on the right (`head -n 5`), which filters the output to show only the first 5 lines[cite: 6].

---

### Task 2.4 - Package Managers
A package manager is a command-line tool (such as Homebrew on macOS) that automates installing, updating, configuring, and removing software packages[cite: 6]. It is useful because it saves time, automatically installs required dependencies, and keeps developer tools organized and updated safely from one place[cite: 6].

## 5. Difficulties faced
No major difficulties[cite: 12].

## 6. How I resolved them
Not applicable[cite: 12].

## 7. Evidence / files
* `mission-02-terminal/README.md`[cite: 3, 12]
* `terminal-practice/` (local practice directory used for safe file operations)[cite: 5]

## 8. Commit details
Committed with message: `"Complete Terminal and file management mission"` and pushed to GitHub[cite: 6, 12, 13].
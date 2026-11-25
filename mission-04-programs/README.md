# Mission 4 - How Programs Run

## 1. Task / objective
Create and run a basic Python script from Terminal and compare how compilers and interpreters translate and execute source code.

## 2. Work completed
* Created `hello.py` inside `mission-04-programs/` to print `"Hello from Python"`.
* Executed `hello.py` using `python3` in Terminal and verified the output.
* Completed a comparison table and summary explaining the differences between compilers and interpreters.

## 3. Commands / tools used
* **VS Code** — Used to write and save `hello.py` and `README.md`.
* `python3 mission-04-programs/hello.py` — Runs the Python script using the Python 3 interpreter.
* **Git (`git add`, `git commit`, `git push`)** — Used to stage, commit, and publish Mission 4 to GitHub.

## 4. My understanding

### Task 4.1 - Create and Run a Python Program
Created `hello.py` with `print("Hello from Python")` and ran `python3 mission-04-programs/hello.py` in Terminal. Terminal immediately displayed `Hello from Python`, confirming that Python executed the instruction directly without requiring a separate compilation step.

---

### Task 4.2 - Compare Compiler and Interpreter

| Point | Compiler | Interpreter |
| :--- | :--- | :--- |
| **When translation / execution happens** | Translates the entire source code file into machine code before the program runs. | Translates and executes source code line-by-line during runtime. |
| **Typical output** | Produces a standalone executable binary file (such as `.exe` or a macOS binary). | Produces direct program output on screen without generating a separate executable file. |
| **One example** | C / C++ (`gcc` or `clang`) | Python (`python3`) |
| **One advantage** | Compiled programs execute very fast once built because the CPU runs native machine code directly. | Easier to test, edit, and debug quickly because code runs immediately without waiting for a build step. |

**Difference between a compiler and an interpreter:**
A compiler translates an entire program into machine code ahead of time, creating a standalone executable file that runs quickly afterward. In contrast, an interpreter reads, translates, and executes source code one instruction at a time while the program is running. As shown in the table, compiled languages like C++ prioritize fast execution speed, whereas interpreted languages like Python make testing and debugging much faster and simpler.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
* `mission-04-programs/hello.py`
* `mission-04-programs/README.md`

## 8. Commit details
Committed with message: `"Compare compilers and interpreters"` and pushed to GitHub.
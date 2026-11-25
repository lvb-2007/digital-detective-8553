# Mission 4 — How programs run

## 1. Task / objective
Run a simple Python program and compare how compilers and interpreters
translate or execute programs.

## 2. Work completed
- Created hello.py, which prints "Hello from Python", and ran it with
  python3.
- Output seen: Hello from Python

### Task 4.2 — Compiler and interpreter comparison

| Point | Compiler | Interpreter |
|---|---|---|
| When translation/execution happens | Translates source code before the program runs | Executes the program through a runtime as it runs |
| Typical output | Translated code, often a native executable | Program output; a separate native executable is usually not produced |
| Example | A C compiler such as Clang | The Python interpreter |
| One advantage | The translated program can run efficiently without translating the source each time | Convenient to run and test source code directly |

A compiler translates source code into another form before execution, often
machine code that can run as an executable. An interpreter runs source code
through a runtime and reports the program's output as it executes. Python
programs are commonly run with the Python interpreter, so I can run this file
without creating a separate native executable.

## 3. Commands / tools used
- echo and >: created hello.py with one line of code.
- cat: displayed the file to check it.
- python3 hello.py: ran the program using the Python interpreter.
- VS Code: used to write this README.
- Git (status, add, commit, push): saved and uploaded the mission.

## 4. My understanding
The compiler/interpreter table compares when translation happens, the output,
an example and one advantage. The two approaches differ in how they translate
and execute programs; Python ran this file using its interpreter.

## 5. Difficulties faced
No major difficulties. 

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- mission-04-programs/hello.py
- mission-04-programs/README.md
- Sanitized run output is recorded in
  [evidence/verification.txt](../evidence/verification.txt).

## 8. Commit details
- Correction commit: `fix: repair program example and comparison`
- Pushed to GitHub: YES

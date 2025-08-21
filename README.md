# 0x16. C - Simple Shell




![shell](https://github.com/user-attachments/assets/0407a16d-8bd6-498b-a9e9-85052f854f67)

## Description
This project is an implementation of a simple UNIX command-line interpreter, developed as part of the **ALX Software Engineering Program**.  
The goal was to recreate a minimalist shell similar to `/bin/sh`, capable of executing basic commands and handling system calls.  

The project challenged us to deepen our understanding of:
- System programming in C
- Process creation and management
- File descriptors and system calls
- Environment handling
- Error handling
- Collaboration in team-based projects

This work was done as a **group project** by **[Tunde Lawal](https://github.com/your-github)**

---

## Learning Objectives
By completing this project, we gained the ability to:
- Explain how a UNIX shell works
- Understand the difference between a process ID (PID) and a parent process ID (PPID)
- Manipulate the environment of a running process
- Differentiate between functions and system calls
- Create and manage processes using `fork`, `execve`, and `wait`
- Use the `PATH` variable to locate executables
- Handle the `EOF` signal and implement basic built-ins (`exit`, `env`, etc.)

---

## Requirements
- Allowed editors: `vi`, `vim`, `emacs`
- Compiled on **Ubuntu 20.04 LTS** using:
  ```bash
  gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh

---

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

This work was done as a **group project** by **[Tunde Lawal](https://github.com/Lawaltunde/)**

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

## Compilation

```bash
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh

$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$

$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$

```
---

## List of allowed functions and system calls:
- access (man 2 access)
- chdir (man 2 chdir)
- close (man 2 close)
- closedir (man 3 closedir)
- execve (man 2 execve)
- exit (man 3 exit)
- _exit (man 2 _exit)
- fflush (man 3 fflush)
- fork (man 2 fork)
- free (man 3 free)
- getcwd (man 3 getcwd)
- getline (man 3 getline)
- getpid (man 2 getpid)
- isatty (man 3 isatty)
- kill (man 2 kill)
- malloc (man 3 malloc)
- open (man 2 open)
- opendir (man 3 opendir)
- perror (man 3 perror)
- read (man 2 read)
- readdir (man 3 readdir)
- signal (man 2 signal)
- stat (__xstat) (man 2 stat)
- lstat (__lxstat) (man 2 lstat)
- fstat (__fxstat) (man 2 fstat)
- strtok (man 3 strtok)
- wait (man 2 wait)
- waitpid (man 2 waitpid)
- wait3 (man 2 wait3)
- wait4 (man 2 wait4)
- write (man 2 write)

---
## Requirements
- Allowed editors: `vi`, `vim`, `emacs`
- Compiled on **Ubuntu 20.04 LTS** using:
  ```bash
  gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh

---

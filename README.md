# Linux Shell

A lightweight Unix-like command-line shell developed in C that executes Linux commands using system calls. The project demonstrates process creation, command execution, and process synchronization in a Linux environment.

## Project Structure

```text
myShell/
├── README.md
├── LICENSE
├── .gitignore
├── shell.c
└── screenshots/
```

## Features

* Execute Linux commands from the terminal
* Process creation using `fork()`
* Command execution using `execvp()`
* Parent-child process synchronization using `wait()`
* Command parsing and argument handling
* Interactive command-line interface

## Technologies Used

* C
* Linux System Programming
* GCC
* Linux Terminal

## Core Concepts

* Process Management
* System Calls
* Parent and Child Processes
* Command Parsing
* Process Synchronization

## Workflow

1. Accept command input from the user.
2. Parse the command and arguments.
3. Create a child process using `fork()`.
4. Execute the command using `execvp()`.
5. Wait for the child process to complete using `wait()`.
6. Display the shell prompt for the next command.

## Example

```bash
myshell> pwd
/home/user

myshell> ls
Documents Downloads

myshell> mkdir test

myshell> exit
```

## Build and Run

### Compile

```bash
gcc shell.c -o myshell
```

### Run

```bash
./myshell
```

## Learning Outcomes

* Understanding Linux process creation and management
* Working with system calls
* Executing commands using child processes
* Building a command-line interpreter
* Applying Operating System concepts in practice

## Current Status

### Implemented

* Command execution
* Process creation using `fork()`
* Command execution using `execvp()`
* Process synchronization using `wait()`

### Planned Enhancements

* Pipe support (`|`)
* Input/Output redirection
* Background process execution (`&`)
* Command history
* Auto-completion

## Author

Dithesh Gowda

# Linux Shell

A Unix-like command-line shell developed in C that supports command execution using Linux system calls. This project demonstrates process creation, command parsing, and operating system fundamentals.

## Features

* Execute Linux commands from the terminal
* Process creation using `fork()`
* Command execution using `execvp()`
* Parent-child process synchronization using `wait()`
* Basic command parsing and execution
* Lightweight and easy-to-understand implementation

## Technologies Used

* C Programming
* Linux System Programming
* GCC Compiler
* Linux Terminal

## Operating System Concepts Used

* Process Management
* System Calls
* Parent and Child Processes
* Command Interpretation
* Process Synchronization

## How It Works

1. The shell waits for user input.
2. The entered command is parsed into arguments.
3. A child process is created using `fork()`.
4. The child process executes the command using `execvp()`.
5. The parent process waits for the child process to finish using `wait()`.
6. The shell prompts the user for the next command.

## Example

```bash
myshell> pwd
/home/user

myshell> ls
file1.txt
file2.txt

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

* Understanding Linux process creation
* Working with system calls
* Implementing command execution
* Building a basic command-line interpreter
* Applying operating system concepts in a practical project

## Future Enhancements

* Pipe (`|`) support
* Input/Output redirection
* Background process execution (`&`)
* Command history
* Auto-completion

## Author

Dithesh Gowda

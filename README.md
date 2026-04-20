# minishell
Project: Build Your Own Mini Shell (Command Line Interpreter)

You’ll create a simplified version of a Linux shell like Bash.

What you’ll learn

This project hits both Linux and C fundamentals:

C programming concepts
Strings, arrays, pointers
Memory management (malloc, free)
Structs and parsing
Linux system programming
Process creation (fork)
Running programs (exec)
Waiting for processes (wait)
File descriptors & I/O redirection
Pipes (|)
Signals (Ctrl+C handling)

Core Features (build step-by-step)

Start simple and expand:

1. Basic command execution
Read user input
Parse command (ls, pwd, etc.)
Execute using fork() + execvp()

Example:

> ls -l
2. Built-in commands

Implement commands inside your shell:

cd
exit
maybe help
3. Arguments parsing

Support:

> grep hello file.txt
4. I/O Redirection
> ls > output.txt
> cat < input.txt

Learn:

open()
dup2()
5. Pipes
> ls | grep .c

This is where things get very Linux-heavy:

pipe()
multiple processes communicating
6. Background processes
> sleep 10 &

Learn:

non-blocking execution
process management
7. Signal handling (optional but powerful)
Handle Ctrl+C using signal() or sigaction()

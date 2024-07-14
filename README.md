# Unix Shell Command Line Interpreter
Creator: Avishek Choudhury

## Overview
In this project, I crafted a simple Unix shell in C++. This custom shell allows users to run commands, incorporating features like I/O redirection and piping, akin to common Unix shells such as bash and zsh.

## Video Walkthrough
https://github.com/user-attachments/assets/bf6fc1a1-09e8-4c33-bed0-e7b44b65c95e

## Tech Stack
C++

## Implementation
1. **Running a Single Command**: Used fork(), exec(), and wait() to execute user commands and awaited their completion before processing the next input.
2. **I/O Redirection**: Expanded the shell to support I/O redirection, enabling programs to utilize files for stdin and stdout. This feature involved manipulating file descriptors using the dup2() system call.
3. **Pipes**: Introduced support for piping multiple commands together. This feature empowers users to chain commands with pipes, offering capabilities similar to advanced Unix shells.
4. **Shell Builtins**: Implemented a crucial shell builtin: 'cd.' This feature allows users to change directories within the shell.
5. **Tab Completion**: Incorporated tab completion using the readline library. This feature simplifies command and filename input by providing auto-completion suggestions.

## Running the Program
1. **Download the Code or fork the repo**
   ```
   git clone https://github.com/avishek04/UnixShell-CommandLine.git
   ```
2. **Build the Program:**
   ```
   make
   ```
3. **Execute the Program:**
   ```
   ./program
   ```

## Test Commands
You can use the following test commands to explore the functionality of the Unix shell. In your terminal. 

- **Change Directory (`cd`):**
  - Use the `cd test_folder` command to navigate into the "test_folder" directory.
  - Use `cd ..` to move back up one directory.

- **List Contents (`ls`):**
  - Execute `ls` to display the list of contents in the current directory.

- **File Creation and Output (`echo`):**
  - Create a file named "someFile" and write the sentence "hello world" into it using the command:

    ```
    echo hello world > someFile
    ```

- **Display First Lines (`head`):**
  - Display the first 10 lines from a file called "someFile" using:

    ```
    head < someFile
    ```

- **Display Content and Filtering (`cat`, `grep`, `tail`):**
  - Use `cat file.txt` to display the contents of a file named "file.txt."

  - Filter the content to display the last 10 lines where the word "love" appears using:

    ```
    cat file.txt | grep love | tail
    ```

Feel free to explore the code and run the shell to experience its functionality.

Thanks for visiting.

Fell Free to connect on [LinkedIn](https://www.linkedin.com/in/avishekchoudhury/)

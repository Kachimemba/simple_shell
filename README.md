<<<<<<< HEAD
### Shell Description

This repository contains a simple shell implementation. The shell supports both interactive and non-interactive modes, offering a range of built-in commands for managing the environment and executing commands.

### Installation

To get started, follow these installation steps:

1. Clone this repository into your desired working directory:
   ```sh
   git clone <repository_url>
   cd <repository_directory>
   ```

2. Compile the source files using GCC with the following flags for optimal results:
   ```sh
   gcc -Wall -Wextra -Werror -pedantic -std=gnu89 *.c -o hsh
   ```

### Usage

Once compiled, the shell can be run in either interactive or non-interactive mode.

#### Interactive Mode

1. Run the compiled program:
   ```sh
   ./hsh
   ```

2. Wait for the shell prompt to appear.

3. Input commands and press Enter to execute them. Use the "exit" command or Ctrl-D to exit the shell.

#### Non-Interactive Mode

1. Use the following format to run the shell in non-interactive mode:
   ```sh
   echo "<command>" | ./hsh
   ```

2. Replace `<command>` with the desired command.

3. The shell will execute the provided command(s) and then exit.

### Included Built-In Commands

The shell includes the following built-in commands for managing operations:

| Command             | Definition                                                                                |
| ------------------- | ----------------------------------------------------------------------------------------- |
| exit [n]            | Exit the shell, with an optional exit status, n.                                          |
| env                 | Display the current environment variables.                                                |
| setenv [var][value] | Set an environment variable along with its value. If the variable exists, its value will be updated. |
| unsetenv [var]      | Remove a specified environment variable.                                                  |
| cd [dir]            | Change the current directory.                                                             |
| help [built-in]     | Display documentation for a specified built-in command.                                   |

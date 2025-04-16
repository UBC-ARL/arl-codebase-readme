# Terminal, Shell and Command-Line

Although strictly speaking, the word `terminal`, `shell`, and `command-line` refer to different concepts, for a quick-start guide, we will use them interchangeably.

## Run

- **Windows 10/11**: Press `Win`, type `terminal`, and hit `Enter`.
- **Mac**: Press `Command + Space`, type `terminal`, and hit `Enter`.

The black window that pops up is the terminal. It is a command-line interface (CLI) that allows you to interact with your computer using text commands instead of a graphical user interface (GUI). You can use it to run programs, manage files, and perform various tasks. Many software tools in programming are CLI only.

## Learning Material

[This tutorial](<(https://linuxcommand.org/lc3_learning_the_shell.php)>) from linuxcommand.org covers more than what you need for this codebase. Take some time and read through it. Although it is for Linux, a lot of frequently used commands are the same for Windows and Mac.

### Frequently Used Commands

- `ls`: List files and directories in the current directory.
  - `ls -a`: Show all files, including hidden files. (\*nix)
- `cd`: Change the current directory.
  - `cd ..`: Go up one directory.
  - `cd ~`: Go to the home directory.
  - `cd D://`: Go to the D drive. (Windows)
  - `cd /`: Go to the root directory. (\*nix)
- `pwd`: Print the current working directory.
- `mkdir`: Create a new directory.
- `rm`: Remove files or directories.
- `echo`: Display a line of text or a variable value.
- `which`: Show the full path of a command.
  - `get-command`: The PowerShell equivalent.

## Shell Script

### Windows

On Windows, you can save your commands in a script by creating a file with the `.ps1` extension.
To run the script, you can use the following command:

```powershell
powershell .\script.ps1
```

You may need to set the execution policy to allow running scripts. Please refer to [Microsoft's documentation](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-7.5) for more information.

Also, you can right-click on the script file and select "Run with PowerShell" to execute it.

### Linux/MacOS

On \*nix, you can save your commands in a script by creating a file with the `.sh` extension.

To run the script, you can use the following command:

```bash
sh ./script.sh
```
